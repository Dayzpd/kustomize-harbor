# Harbor
Repo for managing the configuration of harbor across my homelab clusters.

Initially I was using [Pulp as a container registry for my homelab](https://github.com/Dayzpd/kustomize-pulp). While Pulp is a very interesting project, it's also quite ambitious. The docs are not always clear and pull through caches seemingly stop working at random. Given that my primary need for a local container registry is caching, I've decided to use Harbor instead. 

Overall, Harbor is a lot easier to get working and the builtin Web UI is also quite nice. While Pulp is more extensible and supports other types of package repos, I only need a container registry. Pulp also didn't have a Web UI. Most configuration had to be done either via its CLI or through the Rest API (b/c the CLI often didn't support some of the newer features).

TLDR if you need a local self-hosted container registry to act as a pull through cache, use Harbor instead of Pulp for the time being.