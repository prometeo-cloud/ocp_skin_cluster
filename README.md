# ocp_skin_cluster

## Description:

Skin a OpenShift cluster with a custom logo and a new login-page

_Note: Still work in progress_

## Behaviour:

**Feature:** Skin a OpenShift Cluster
- **Given** a OpenShift cluster is installed and accessible
- **When** The installation is done and you want to apply a new skin
- **Then** Ensure directory exists
- **Then** Find all files which we will copy
- **Then** Copy all files to directory onto servers
- **Then** Modify yaml - Add extra CSS to master-config.yml
- **Then** Modify yaml - Add new login template
- **Then** restart master api on first master
- **Then** Waiting for service to be up on first master

## Configuration:

Expecing a logo.css and login-template.html inside the files ansible directory

## Usage:

How to invoke the role from a playbook:

```yaml
- name: Install RH IDM
  include_role:
    name: ocp_skin_cluster
```
