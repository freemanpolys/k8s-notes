- Create repo folder : mkdir custom-repo
- Create custom charts in repo folder : helm create mychart
- Package charts in the repo folder : helm package mychart
- Generate the index.yaml file : helm repo index
- Update charts urls in index.yaml according to your web server path
- Push the code to the web server (exple : http://my-helm.com/repo
- Index must be available on : http://my-helm.com/repo/index.yaml
- Add the repo to helm : helm add repo dev http://my-helm.com/repo
- Install a release of the chart : helm install dev/mychart 

