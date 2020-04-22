# NVIDIA Hack

This was 'forked', sort-of, by using Helm to install the NVIDIA gpu-operator Helm chart.

```bash
helm repo add nvidia https://nvidia.github.io/gpu-operator
helm repo update
helm install --devel nvidia/gpu-operator --wait --generate-name
```

Then grabbing the tarball from the Helm cache and saving it to the root of this repo as:

```
gpu-operator-1.1.0.tgz
```

Then I untarred this and used the sources.
I did this because it was difficult for me to figure out how to produce this v1.1.0 tarball from the original [source](https://github.com/NVIDIA/gpu-operator).
	 
