# mkubectl
This is kubectl wrapper for multiple clusters.

This is just a simple tool to run kubectl on multiple clusters. Therefore, it is completely compatible.

# How to use
## 1. Install mkubectl.
```
$ curl https://raw.githubusercontent.com/shogomuranushi/mkubectl/master/mkubectl --output /usr/local/bin/mkubectl
$ chmod 755 /usr/local/bin/mkubectl
```

## 2. Create ~/.mkubectl.
```bash
$ touch ~/.mkubectl
```

## 3. Write Kubernetes context to ~/.mkubectl

### Example) EKS
```:~/.mkubectl
arn:aws:eks:us-west-2:123456789012:cluster/your-cluster-name1
arn:aws:eks:us-west-2:123456789012:cluster/your-cluster-name2
```

## 4. Execute mkubectl
```
$ mkubectl get node -o wide
$ mkubectl get pods --all-namespaces
```

# Roadmap
- Parallel execution for  high speed
- Simple registration of Context
