# logx
Custom log plugin for Kubernetes

## Design
Plugin is under development. Below options will be supported in initial version.
### Usage
``` 
kubectl logx <pod> -c <container> -n <namespace> <options>
```
### Options
``` 
list                list available logs
                         
show                print selected logs
  -f, --file        log file location in container 
  -t, --tail        tail the specified logs
  -l, --log-level   log level (trace|debug|info|warn|error|fatal|panic)
  -s, --selector    filter based on label
  -p, --previous    print the logs for the previous instance of the container
  --limit-bytes     max bytes of logs to return, defaults to no limit
  --prefix          prefix each log line with the log source (pod/container/service)

```
