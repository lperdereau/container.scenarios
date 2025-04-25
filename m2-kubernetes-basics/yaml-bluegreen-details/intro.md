- We want to author YAML manifests for the "color" app

  (use image `jpetazzo/color` or `ghcr.io/jpetazzo/color`)

- That app serves web requests on port 80

- We want to deploy two instances of that app (`blue` and `green`)

- We want to expose the app with a service named `front`, such that:

  90% of the requests are sent to `blue`, and 10% to `green`

---

## End goal

- We want to be able to do something like:
  ```bash
  kubectl apply -f blue-green-demo.yaml
  ```

- Then connect to the `front` service and see responses from `blue` and `green`

- Then measure e.g. on 100 requests how many go to `blue` and `green`

  (we want a 90/10 traffic split)
