# k8s notes from course

kubectl create deployment --image=bioconductor/bioc-redis-manager:devel biock8s --dry-run=client -o yaml > manager-definition.yaml

kubectl run custom-nginx --image=nginx --port 8080 --dry-run=client -o yaml

kubectl expose pod redis --port=6379 --name redis-service --dry-run=client -o yaml

kubectl expose pod redis --port=6379 --name redis-service

## This will create a pod and a service!
kubectl run httpd --image=httpd:alpine --port=80 --expose




## General command type

    kubectl [command] [TYPE] [NAME] -o <output_format>

        -o jsonOutput a JSON formatted API object.

        -o namePrint only the resource name and nothing else.

        -o wideOutput in the plain-text format with any additional information.

        -o yamlOutput a YAML formatted API object.

