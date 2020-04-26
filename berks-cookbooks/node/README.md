# Node Cookbook

This cookbook downloads node, npm, pm2 and Nginx. Which are needed to run an app. In addition the cookbook provisions the setup of Nginx so you don't need to manually configure it.

## List of what installs
- NodeJs
- Nginx
- pm2 and npm

## Prerequisites
- Chef
### What is Chef?
- Chef is a configuration management tool which allows you to provision files for installation.
- It allows you to be infrastructure agnostic.
- Chef allows for machines to be setup on physical machines, in the cloud and virtual machines.

## Clone
```
git clone git@github.com:atahar123/NodeCookbookStarterCode.git
```

## Commands
### Test locally
Running my unit test:
```
chef exec rspec
```

Running Integration tests and closing VM:
```
kitchen test
```

### Test in AWS
Running Integration tests in AWS
```
KITCHEN_YAML=yml_file_name.yml kitchen test
```
