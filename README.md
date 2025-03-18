# dify-k8s
    
    The entire yaml depends on the docker-compose.yaml file.
    All configuration items are retained, such as uploading files to OSS, switching vector databases, etc.
    Currently, YAML will do PVC storage. If it is not needed, please handle it yourself.


    If you use a local database, then you need to have a storageClass.
    
# Currently supported dify versions: V1.1.0

#### upgrade

 - Modify the dify-k8s.yaml file
 - kubectl apply -f dify-k8s.yaml
 - kubectl rollout restart statefulset/deployment <name> -n dify