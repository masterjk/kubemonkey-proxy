
# kubemonkey-proxy
Serves as the Kubernetes-Minecraft proxy plugin (based in GO).

## Technical Architecture

Internally, this proxy script uses `kubectl get pod --watch` and poll for pods getting started, or being terminated.  It then relays this information to Minecraft (via KubeMonkey-Plugin).
