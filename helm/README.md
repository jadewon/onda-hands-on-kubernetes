## [Helm](https://docs.aws.amazon.com/AmazonECR/latest/userguide/push-oci-artifact.html)

```sh
$ helm install nginx ./handson --set image.tag=stable --dry-run
$ helm install webserver ./handson --set host=web.nginx.info --dry-run

$ helm upgrade nginx ./handson --reuse-values --set replicaCount=2 --dry-run

$ helm upgrade webserver ./handson \
  --reuse-values \
  --set image.repository=handson \
  --set image.tag=v0.0.1 \
  --set image.pullPolicy=Never \
  --set targetPort=3000 \
  --set health='\' \
  --dry-run
```
