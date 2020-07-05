# kubectl-isolate

Kubectl plugin to isolate a Pod from the Kubernetes Service.

Inspired from

- https://twitter.com/danielepolencic/status/1275786970610843648
- https://www.reddit.com/r/kubernetes/comments/gt3uvg/how_to_quarantine_pods/

## Install

Download `kubectl-isolate` file to the directory in your PATH and set it executable.

```
curl -Lo ~/bin/kubectl-isolate https://raw.githubusercontent.com/yteraoka/kubectl-isolate/master/kubectl-isolate
chmod +x ~/bin/kubectl-isolate
```

## Usage

```
kubectl isolate <service_name> <pod_name>
```

If you have [fzf](https://github.com/junegunn/fzf) or [peco](https://github.com/peco/peco) then you can type just `kubectl isolate` to select Service and Pod interactively.
