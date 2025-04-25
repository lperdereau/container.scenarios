Create a Deployment named `blue` using the `jpetazzo/color` image.

<details>
    <summary>Hint</summary>
    <br/>

    ```plain
    kubectl create deployment -h
    ```{{exec}}
</details>

<br>
<details>
    <summary>Solution</summary>
    <br>

    ```plain
    kubectl create deployment blue --image=jpetazzo/color
    ```{{exec}}
</details>
<br>

Create a Service named `front` using ClusterIP, serving the `blue` Deployment.

<details>
    <summary>Hint</summary>
    <br>

    ```plain
    kubectl expose deployment -h
    ```{{exec}}
</details>

<br>
<details>
    <summary>Solution</summary>
    <br>

    ```plain
    kubectl expose deployment blue --name=front --port=80 --target-port=80 --type=ClusterIP
    ```{{exec}}
</details>
