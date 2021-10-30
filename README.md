# Tamama Cloud Deployer

1. This is the release repository of Tamama Cloud Deployer only for the binary artifacts.
2. The corresponding source is meant to remain closed on Gitlab.

## Get started (Linux x86_64)

### Download binary

Visit the [release page](https://github.com/tamama/tamama-cloud-deployer/releases) to determine the latest version.

For example: v0.1.0-alpha
```
[centos@ip-172-31-13-180 bin]$ pwd
/home/centos/bin
[centos@ip-172-31-13-180 bin]$
[centos@ip-172-31-13-180 bin]$ curl -kL https://github.com/tamama/tamama-cloud-deployer/releases/download/v0.1.0-alpha/tamama-cloud-deployer -O
...
[centos@ip-172-31-13-180 bin]$ chmod +x tamama-cloud-deployer
```

### Get hints.
```
[centos@ip-172-31-13-180 ~]$ tamama-cloud-deployer 
NAME:
   Tamama Cloud Deployer - Your convenient infrastructure provisioner.

USAGE:
   tamama-cloud-deployer [global options] command [command options] [arguments...]

DESCRIPTION:
   This application is capable of conveniently provisioning the infrastructure of your data-center.

AUTHOR:
   Tama MA <Tama.Ma@ibm.com>

COMMANDS:
   base     Provisions the base for this current node
   app      Runs the application - Tamama Cloud Deployer
   help, h  Shows a list of commands or help for one command

GLOBAL OPTIONS:
   --help, -h  show help (default: false)
[centos@ip-172-31-13-180 ~]$ 
```
### A naive approach of starting the application
```
[centos@ip-172-31-13-180 ~]$ tamama-cloud-deployer app
2021/10/30 18:43:26 Processing - application::component::grpcservice[0] - {Name:tamama-cloud-deployer Version:v1 Enabled:true Host:127.0.0.1 Port:12345}
2021/10/30 18:43:26 Starting gRPC service (tamama-cloud-deployer) at 127.0.0.1:12345 
```
Of course, the magic is what that follows...

Cheers.
