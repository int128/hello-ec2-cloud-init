# hello-ec2-cloud-init

This is Hello World of Amazon EC2 with cloud-init.


## Getting Started

```sh
brew install terraform
brew cask install session-manager-plugin
```

```sh
# provision the resources
terraform init
terraform apply
```

This example will launch an instance running a background service.

```console
% aws ssm start-session --target i-0935e9832a6391309 --region us-west-2

$ tail -f /tmp/helloworld.log
Thu May 28 11:29:08 UTC 2020
Thu May 28 11:29:09 UTC 2020
Thu May 28 11:29:10 UTC 2020
...
```
