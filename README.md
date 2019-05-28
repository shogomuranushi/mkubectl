# mkubectl
This is kubectl wrapper for multiple clusters.
This is just a simple tool to run kubectl on multiple clusters. Therefore, it is completely compatible.

# How to use
## 1. Install mkubectl.
```
```

## 2. Please create ~/.mkubectl.
```bash
touch ~/.mkubectl
```

## 3. Please write Kubernetes context to ~/.mkubectl

### EKS
```:~/.mkubectl
arn:aws:eks:us-west-2:123456789012:cluster/your-cluster-name1
arn:aws:eks:us-west-2:123456789012:cluster/your-cluster-name2
```

## 4. Execute mkubectl
```
mkubectl get node -o wide
mkubectl get pods --all-namespaces
```

# Roadmap
- Parallel execution for  high speed
- Simple registration of Context
