# README

Create and configure a Kubernetes cluster on DigitalOcean and retrieve the configuration script to manage it via kubectl.

## How to run

```
$ git clone git@github.com:mcicolella/tf-digital-ocean-cluster.git
$ export TF_VAR_do_token=<your_digital_ocean_token>
$ export TF_VAR_do_cluster_name=<your_cluster_name>
$ cd tf-digital-ocean-cluster
$ terraform plan
$ terraform apply
$ chmod +x get_config.sh
$ ./get_config.sh
$ export KUBECONFIG=$(pwd)/config
```

##  Credits

Based on the original work by [ponderosa-io](https://github.com/ponderosa-io/tf-digital-ocean-cluster)
