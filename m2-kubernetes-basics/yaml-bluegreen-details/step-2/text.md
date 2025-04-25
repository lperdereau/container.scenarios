- Create the `green` Deployment

- Export YAML manifests from Kubernetes cluster for all components

  (`blue` and `green` Deployments, `front` Service)

  following the structure:

  ```plain
  + colors/
  |_ blue.deployment.yaml
  |_ green.deployment.yaml
  |_ front.service.yaml
  ```

<br>
<details>
    <summary>Hint</summary>
    <br>

    ```plain
    kubectl get -o yaml
    ```{{exec}}
</details>

<br>
<details>
    <summary>Solution</summary>
    <br>

    ```plain
    mkdir colors
    kubectl get deployment blue -o yaml > colors/blue.deployment.yaml
    kubectl get deployment green -o yaml > colors/green.deployment.yaml
    kubectl get service front -o yaml > colors/front.service.yaml
    ```{{exec}}
</details>
<br>
