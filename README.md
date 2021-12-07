# ansible-helm
An example role to automate the deployment of an application on Kubernetes using Helm.

```site.yml``` performs the following tasks:
  * ensures that the latest versions of the helm repositories are installed locally
  * runs ```helm template``` on the charts in the repositories to generate K8S yaml with a given set of values
  * applies the yaml to the current OpenShift cluster in a given namespace
