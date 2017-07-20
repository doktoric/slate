--- 

title: Cloudbreak API 

language_tabs: 
   - shell 

toc_footers: 
   - <a href='#'>Sign Up for a Developer Key</a> 
   - <a href='https://github.com/lavkumarv'>Documentation Powered by lav</a> 

includes: 
   - errors 

search: true 

--- 

# Introduction 

Cloudbreak is a powerful left surf that breaks over a coral reef, a mile off southwest the island of Tavarua, Fiji.
Cloudbreak is a cloud agnostic Hadoop as a Service API. Abstracts the provisioning and ease management and monitoring of on-demand clusters.
SequenceIQ's Cloudbreak is a RESTful application development platform with the goal of helping developers to build solutions for deploying Hadoop YARN clusters in different environments.
Once it is deployed in your favourite servlet container it exposes a REST API allowing to span up Hadoop clusters of arbitary sizes and cloud providers. Provisioning Hadoop has never been easier.
Cloudbreak is built on the foundation of cloud providers API (Amazon AWS, Microsoft Azure, Google Cloud Platform, Openstack), Apache Ambari, Docker lightweight containers, Swarm and Consul.
For further product documentation follow the link: <a href="http://hortonworks.com/apache/cloudbreak/">http://hortonworks.com/apache/cloudbreak/</a> 

**Version:** 1.15.0-dev.199 

# /ACCOUNTPREFERENCES
## ***GET*** 

**Summary:** retrieve account preferences for admin user

**Description:** Account related preferences that could be managed by the account admins and different restrictions could be added to Cloudbreak resources.

### HTTP Request 
`***GET*** /accountpreferences` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** post account preferences of admin user

**Description:** Account related preferences that could be managed by the account admins and different restrictions could be added to Cloudbreak resources.

### HTTP Request 
`***POST*** /accountpreferences` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***PUT*** 

**Summary:** update account preferences of admin user

**Description:** Account related preferences that could be managed by the account admins and different restrictions could be added to Cloudbreak resources.

### HTTP Request 
`***PUT*** /accountpreferences` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /ACCOUNTPREFERENCES/ISPLATFORMSELECTIONDISABLED
## ***GET*** 

**Summary:** is platform selection disabled

**Description:** Account related preferences that could be managed by the account admins and different restrictions could be added to Cloudbreak resources.

### HTTP Request 
`***GET*** /accountpreferences/isplatformselectiondisabled` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /ACCOUNTPREFERENCES/VALIDATE
## ***GET*** 

**Summary:** validate account preferences of all stacks

**Description:** Account related preferences that could be managed by the account admins and different restrictions could be added to Cloudbreak resources.

### HTTP Request 
`***GET*** /accountpreferences/validate` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /BLUEPRINTS/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) blueprints

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***GET*** /blueprints/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create blueprint as public resource

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***POST*** /blueprints/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /BLUEPRINTS/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) blueprint by name

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***GET*** /blueprints/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private blueprint by name

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***DELETE*** /blueprints/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /BLUEPRINTS/USER
## ***GET*** 

**Summary:** retrieve private blueprints

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***GET*** /blueprints/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create blueprint as private resource

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***POST*** /blueprints/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /BLUEPRINTS/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private blueprint by name

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***GET*** /blueprints/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private blueprint by name

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***DELETE*** /blueprints/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /BLUEPRINTS/{ID}
## ***GET*** 

**Summary:** retrieve blueprint by id

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***GET*** /blueprints/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete blueprint by id

**Description:** Ambari Blueprints are a declarative definition of a Hadoop cluster. With a Blueprint, you specify a stack, the component layout and the configurations to materialize a Hadoop cluster instance. Hostgroups defined in blueprints can be associated to different templates, thus you can spin up a highly available cluster running on different instance types. This will give you the option to group your Hadoop services based on resource needs (e.g. high I/O, CPU or memory) and create an infrastructure which fits your workload best.

### HTTP Request 
`***DELETE*** /blueprints/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /CLUSTERTEMPLATES/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) cluster template

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***GET*** /clustertemplates/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create cluster template as public resource

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***POST*** /clustertemplates/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CLUSTERTEMPLATES/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) cluster template by name

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***GET*** /clustertemplates/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private cluster template by name

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***DELETE*** /clustertemplates/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /CLUSTERTEMPLATES/USER
## ***GET*** 

**Summary:** retrieve private cluster templates

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***GET*** /clustertemplates/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create cluster template as private resource

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***POST*** /clustertemplates/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CLUSTERTEMPLATES/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private cluster template by name

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***GET*** /clustertemplates/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private cluster template by name

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***DELETE*** /clustertemplates/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /CLUSTERTEMPLATES/{ID}
## ***GET*** 

**Summary:** retrieve cluster template by id

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***GET*** /clustertemplates/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete cluster template by id

**Description:** Cluster templates are stored cluster configurations, which configurations are reusable any time

### HTTP Request 
`***DELETE*** /clustertemplates/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /CONNECTORS
## ***GET*** 

**Summary:** retrive available platforms

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| extended | query |  | No | boolean |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/CONNECTORS/REGIONS
## ***GET*** 

**Summary:** retrive available regions

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/connectors/regions` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/CONNECTORS/VMTYPES
## ***GET*** 

**Summary:** retrive available vm types

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/connectors/vmtypes` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| extended | query |  | No | boolean |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/CUSTOM
## ***GET*** 

**Summary:** retrive special properties

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/custom` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/DISKTYPES
## ***GET*** 

**Summary:** retrive available disk types

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/disktypes` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/DISKTYPES/{TYPE}
## ***GET*** 

**Summary:** retrive disks by type

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/disktypes/{type}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| type | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/IMAGES
## ***GET*** 

**Summary:** retrive available images

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/images` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/IMAGES/{TYPE}
## ***GET*** 

**Summary:** retrive images by type

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/images/{type}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| type | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/OCHESTRATORS
## ***GET*** 

**Summary:** retrive available orchestrator types

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/ochestrators` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/OCHESTRATORS/{TYPE}
## ***GET*** 

**Summary:** retrive orchestrators by type

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/ochestrators/{type}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| type | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/REGIONS/AV/{TYPE}
## ***GET*** 

**Summary:** retrive availability zones by type

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/regions/av/{type}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| type | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/REGIONS/R/{TYPE}
## ***GET*** 

**Summary:** retrive regions by type

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/regions/r/{type}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| type | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/TAGSPECIFICATIONS
## ***GET*** 

**Summary:** retrive tag specifications

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/tagspecifications` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/VARIANTS
## ***GET*** 

**Summary:** retrive available platform variants

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/variants` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/VARIANTS/{TYPE}
## ***GET*** 

**Summary:** retrive a platform variant by type

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/variants/{type}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| type | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONNECTORS/VMTYPES/{TYPE}
## ***GET*** 

**Summary:** retrive vm types by type

**Description:** Each cloud provider has it's own specific resources like instance types and disk types. These endpoints are collecting them.

### HTTP Request 
`***GET*** /connectors/vmtypes/{type}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| type | path |  | Yes | string |
| extended | query |  | No | boolean |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONSTRAINTS/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) constraint templates

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***GET*** /constraints/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create constraint template as public resource

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***POST*** /constraints/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONSTRAINTS/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) constraint template by name

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***GET*** /constraints/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private constraint template by name

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***DELETE*** /constraints/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /CONSTRAINTS/USER
## ***GET*** 

**Summary:** retrieve private constraint templates

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***GET*** /constraints/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create constraint template as private resource

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***POST*** /constraints/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CONSTRAINTS/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private constraint template by name

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***GET*** /constraints/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private constraint template by name

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***DELETE*** /constraints/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /CONSTRAINTS/{ID}
## ***GET*** 

**Summary:** retrieve constraint template by id

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***GET*** /constraints/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete constraint template by id

**Description:** A constraint template tells Cloudbreak the resource constraints (cpu, memory, disk) of the Ambari containers that will be deployed to the cluster. A constraint template must be created onenvironments where there is no one-to-one mapping between containers and nodes, like Mesos.

### HTTP Request 
`***DELETE*** /constraints/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /CREDENTIALS/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) credentials

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***GET*** /credentials/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create credential as public resource

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***POST*** /credentials/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CREDENTIALS/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) credential by name

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***GET*** /credentials/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private credential by name

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***DELETE*** /credentials/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /CREDENTIALS/ACCOUNTINTERACTIVELOGIN
## ***POST*** 

**Summary:** interactive login

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***POST*** /credentials/accountinteractivelogin` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CREDENTIALS/USER
## ***GET*** 

**Summary:** retrieve private credentials

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***GET*** /credentials/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create credential as private resource

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***POST*** /credentials/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CREDENTIALS/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private credential by name

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***GET*** /credentials/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private credential by name

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***DELETE*** /credentials/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /CREDENTIALS/USERINTERACTIVELOGIN
## ***POST*** 

**Summary:** interactive login

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***POST*** /credentials/userinteractivelogin` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /CREDENTIALS/{ID}
## ***GET*** 

**Summary:** retrieve credential by id

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***GET*** /credentials/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete credential by id

**Description:** Cloudbreak is launching Hadoop clusters on the user's behalf - on different cloud providers. One key point is that Cloudbreak does not store your Cloud provider account details (such as username, password, keys, private SSL certificates, etc). We work around the concept that Identity and Access Management is fully controlled by you - the end user. The Cloudbreak deployer is purely acting on behalf of the end user - without having access to the user's account.

### HTTP Request 
`***DELETE*** /credentials/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /EVENTS
## ***GET*** 

**Summary:** retrieve events by timestamp (long)

**Description:** Events are used to track stack creation initiated by cloudbreak users. Events are generated by the backend when resources requested by the user become available or unavailable

### HTTP Request 
`***GET*** /events` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| since | query |  | No | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /EVENTS/{ID}
## ***GET*** 

**Summary:** retrieve events by stackid (long)

**Description:** Events are used to track stack creation initiated by cloudbreak users. Events are generated by the backend when resources requested by the user become available or unavailable

### HTTP Request 
`***GET*** /events/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| stackId | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /FLEXSUBSCRIPTIONS/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) Flex subscriptions

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***GET*** /flexsubscriptions/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create Flex subscription as public resource

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***POST*** /flexsubscriptions/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /FLEXSUBSCRIPTIONS/ACCOUNT/SETDEFAULT/{NAME}
## ***PUT*** 

**Summary:** sets the account default flag on the Flex subscription

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***PUT*** /flexsubscriptions/account/setdefault/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /FLEXSUBSCRIPTIONS/ACCOUNT/SETUSEDFORCONTROLLER/{NAME}
## ***PUT*** 

**Summary:** sets the account 'used for controller' flag on the Flex subscription

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***PUT*** /flexsubscriptions/account/setusedforcontroller/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /FLEXSUBSCRIPTIONS/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) Flex subscription by name

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***GET*** /flexsubscriptions/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private Flex subscription by name

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***DELETE*** /flexsubscriptions/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /FLEXSUBSCRIPTIONS/SETDEFAULT/{ID}
## ***PUT*** 

**Summary:** sets the account default flag on the Flex subscription

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***PUT*** /flexsubscriptions/setdefault/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /FLEXSUBSCRIPTIONS/SETUSEDFORCONTROLLER/{ID}
## ***PUT*** 

**Summary:** sets the account 'used for controller' flag on the Flex subscription

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***PUT*** /flexsubscriptions/setusedforcontroller/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /FLEXSUBSCRIPTIONS/USER
## ***GET*** 

**Summary:** retrieve private Flex subscriptions

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***GET*** /flexsubscriptions/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create Flex subscription as private resource

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***POST*** /flexsubscriptions/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /FLEXSUBSCRIPTIONS/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private Flex subscription by name

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***GET*** /flexsubscriptions/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private Flex subscription by name

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***DELETE*** /flexsubscriptions/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /FLEXSUBSCRIPTIONS/{ID}
## ***GET*** 

**Summary:** retrieve Flex subscription by id

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***GET*** /flexsubscriptions/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete Flex subscription by id

**Description:** Flex subscriptions could be configured.

### HTTP Request 
`***DELETE*** /flexsubscriptions/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /LDAP/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) LDAP configs

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***GET*** /ldap/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create LDAP config as public resource

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***POST*** /ldap/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /LDAP/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) LDAP config by name

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***GET*** /ldap/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private LDAP config by name

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***DELETE*** /ldap/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /LDAP/USER
## ***GET*** 

**Summary:** retrieve private LDAP configs

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***GET*** /ldap/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create LDAP config as private resource

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***POST*** /ldap/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /LDAP/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private LDAP config by name

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***GET*** /ldap/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private LDAP config by name

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***DELETE*** /ldap/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /LDAP/{ID}
## ***GET*** 

**Summary:** retrieve LDAP config by id

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***GET*** /ldap/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete LDAP config by id

**Description:** LDAP server integration enables the user to provide a central place to store usernames and passwords for the users of his/her clusters.

### HTTP Request 
`***DELETE*** /ldap/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /NETWORKS/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) networks

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***GET*** /networks/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create network as public resource

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***POST*** /networks/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /NETWORKS/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) network by name

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***GET*** /networks/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private network by name

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***DELETE*** /networks/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /NETWORKS/USER
## ***GET*** 

**Summary:** retrieve private networks

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***GET*** /networks/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create network as private resource

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***POST*** /networks/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /NETWORKS/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private network by name

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***GET*** /networks/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private network by name

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***DELETE*** /networks/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /NETWORKS/{ID}
## ***GET*** 

**Summary:** retrieve network by id

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***GET*** /networks/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete network by id

**Description:** Provider specific network settings could be configured by using Network resources.

### HTTP Request 
`***DELETE*** /networks/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /RDSCONFIGS/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) RDS configurations

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***GET*** /rdsconfigs/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create RDS configuration as public resource

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***POST*** /rdsconfigs/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /RDSCONFIGS/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) RDS configuration by name

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***GET*** /rdsconfigs/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private RDS configuration by name

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***DELETE*** /rdsconfigs/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /RDSCONFIGS/USER
## ***GET*** 

**Summary:** retrieve private RDS configurations

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***GET*** /rdsconfigs/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create RDS configuration as private resource

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***POST*** /rdsconfigs/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /RDSCONFIGS/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private RDS configuration by name

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***GET*** /rdsconfigs/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private RDS configuration by name

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***DELETE*** /rdsconfigs/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /RDSCONFIGS/{ID}
## ***GET*** 

**Summary:** retrieve RDS configuration by id

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***GET*** /rdsconfigs/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete RDS configuration by id

**Description:** An RDS Configuration describe a connection to an external Relational Database Service that can be used as the Hive Metastore.

### HTTP Request 
`***DELETE*** /rdsconfigs/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /RECIPES/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) recipes

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***GET*** /recipes/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create recipe as public resource

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***POST*** /recipes/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /RECIPES/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) recipe by name

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***GET*** /recipes/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private recipe by name

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***DELETE*** /recipes/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /RECIPES/USER
## ***GET*** 

**Summary:** retrieve private recipes

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***GET*** /recipes/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create recipe as private resource

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***POST*** /recipes/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /RECIPES/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private recipe by name

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***GET*** /recipes/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private recipe by name

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***DELETE*** /recipes/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /RECIPES/{ID}
## ***GET*** 

**Summary:** retrieve recipe by id

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***GET*** /recipes/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete recipe by id

**Description:** Recipes are basically script extensions to a cluster that run on a set of nodes before or after the Ambari cluster installation.

### HTTP Request 
`***DELETE*** /recipes/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SECURITYGROUPS/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) security groups

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***GET*** /securitygroups/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create security group as public resource

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***POST*** /securitygroups/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SECURITYGROUPS/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) security group by name

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***GET*** /securitygroups/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private security group by name

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***DELETE*** /securitygroups/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SECURITYGROUPS/USER
## ***GET*** 

**Summary:** retrieve private security groups

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***GET*** /securitygroups/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create security group as private resource

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***POST*** /securitygroups/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SECURITYGROUPS/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private security group by name

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***GET*** /securitygroups/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private security group by name

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***DELETE*** /securitygroups/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SECURITYGROUPS/{ID}
## ***GET*** 

**Summary:** retrieve security group by id

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***GET*** /securitygroups/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete security group by id

**Description:** Different inbound security rules(group) could be configured by using SecurityGroup resources and a group could be assigned to any Stack(cluster).

### HTTP Request 
`***DELETE*** /securitygroups/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SETTINGS/ALL
## ***GET*** 

**Summary:** retrive all available settings

**Description:** Collecting Cloudbreak specific resource settings.

### HTTP Request 
`***GET*** /settings/all` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SETTINGS/DATABASE
## ***GET*** 

**Summary:** retrive available Ambari database settings

**Description:** Collecting Cloudbreak specific resource settings.

### HTTP Request 
`***GET*** /settings/database` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SETTINGS/RECIPE
## ***GET*** 

**Summary:** retrive available recipe settings

**Description:** Collecting Cloudbreak specific resource settings.

### HTTP Request 
`***GET*** /settings/recipe` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SETTINGS/SSSD
## ***GET*** 

**Summary:** retrive available SSSD configuration settings

**Description:** Collecting Cloudbreak specific resource settings.

### HTTP Request 
`***GET*** /settings/sssd` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SMARTSENSESUBSCRIPTIONS
## ***GET*** 

**Summary:** retrieve default SmartSense subscription

**Description:** SmartSense subscriptions could be configured.

### HTTP Request 
`***GET*** /smartsensesubscriptions` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SMARTSENSESUBSCRIPTIONS/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) SmartSense subscriptions

**Description:** SmartSense subscriptions could be configured.

### HTTP Request 
`***GET*** /smartsensesubscriptions/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create SmartSense subscription as public resource

**Description:** SmartSense subscriptions could be configured.

### HTTP Request 
`***POST*** /smartsensesubscriptions/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SMARTSENSESUBSCRIPTIONS/ACCOUNT/{SUBSCRIPTIONID}
## ***DELETE*** 

**Summary:** delete public (owned) or private SmartSense subscription by subscription ID

**Description:** SmartSense subscriptions could be configured.

### HTTP Request 
`***DELETE*** /smartsensesubscriptions/account/{subscriptionId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| subscriptionId | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SMARTSENSESUBSCRIPTIONS/USER
## ***GET*** 

**Summary:** retrieve private SmartSense subscriptions

**Description:** SmartSense subscriptions could be configured.

### HTTP Request 
`***GET*** /smartsensesubscriptions/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create SmartSense subscription as private resource

**Description:** SmartSense subscriptions could be configured.

### HTTP Request 
`***POST*** /smartsensesubscriptions/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SMARTSENSESUBSCRIPTIONS/USER/{SUBSCRIPTIONID}
## ***DELETE*** 

**Summary:** delete private SmartSense subscription by subscription ID

**Description:** SmartSense subscriptions could be configured.

### HTTP Request 
`***DELETE*** /smartsensesubscriptions/user/{subscriptionId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| subscriptionId | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SMARTSENSESUBSCRIPTIONS/{ID}
## ***GET*** 

**Summary:** retrieve SmartSense subscription by id

**Description:** SmartSense subscriptions could be configured.

### HTTP Request 
`***GET*** /smartsensesubscriptions/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete SmartSense subscription by id

**Description:** SmartSense subscriptions could be configured.

### HTTP Request 
`***DELETE*** /smartsensesubscriptions/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SSSD/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) SSSD configs

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***GET*** /sssd/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create SSSD config as public resource

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***POST*** /sssd/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SSSD/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) SSSD config by name

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***GET*** /sssd/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private SSSD config by name

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***DELETE*** /sssd/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SSSD/USER
## ***GET*** 

**Summary:** retrieve private SSSD configs

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***GET*** /sssd/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create SSSD config as private resource

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***POST*** /sssd/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /SSSD/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private SSSD config by name

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***GET*** /sssd/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private SSSD config by name

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***DELETE*** /sssd/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SSSD/{ID}
## ***GET*** 

**Summary:** retrieve SSSD config by id

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***GET*** /sssd/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete SSSD config by id

**Description:** SSSD configs are defining external user database configuration for provisioned clusters.

### HTTP Request 
`***DELETE*** /sssd/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /STACKS/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) stacks

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***GET*** /stacks/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create stack as public resource

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***POST*** /stacks/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) stack by name

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***GET*** /stacks/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |
| entry | query |  | No | array |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private stack by name

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***DELETE*** /stacks/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |
| forced | query |  | No | boolean |
| deleteDependencies | query |  | No | boolean |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /STACKS/ACCOUNT/{NAME}/CLUSTER
## ***GET*** 

**Summary:** retrieve cluster by stack name (public)

**Description:** Clusters are materialised Hadoop services on a given infrastructure. They are built based on a Blueprint (running the components and services specified) and on a configured infrastructure Stack. Once a cluster is created and launched, it can be used the usual way as any Hadoop cluster. We suggest to start with the Cluster's Ambari UI for an overview of your cluster.

### HTTP Request 
`***GET*** /stacks/account/{name}/cluster` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/ALL
## ***GET*** 

**Summary:** retrieve all stacks

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***GET*** /stacks/all` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/AMBARI
## ***POST*** 

**Summary:** retrieve stack by ambari address

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***POST*** /stacks/ambari` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/PLATFORMVARIANTS
## ***GET*** 

**Summary:** retrieve available platform variants

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***GET*** /stacks/platformVariants` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/USER
## ***GET*** 

**Summary:** retrieve private stack

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***GET*** /stacks/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create stack as private resource

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***POST*** /stacks/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private stack by name

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***GET*** /stacks/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |
| entry | query |  | No | array |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private stack by name

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***DELETE*** /stacks/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |
| forced | query |  | No | boolean |
| deleteDependencies | query |  | No | boolean |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /STACKS/USER/{NAME}/CLUSTER
## ***GET*** 

**Summary:** retrieve cluster by stack name (private)

**Description:** Clusters are materialised Hadoop services on a given infrastructure. They are built based on a Blueprint (running the components and services specified) and on a configured infrastructure Stack. Once a cluster is created and launched, it can be used the usual way as any Hadoop cluster. We suggest to start with the Cluster's Ambari UI for an overview of your cluster.

### HTTP Request 
`***GET*** /stacks/user/{name}/cluster` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/VALIDATE
## ***POST*** 

**Summary:** validate stack

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***POST*** /stacks/validate` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /STACKS/{ID}
## ***GET*** 

**Summary:** retrieve stack by id

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***GET*** /stacks/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| entry | query |  | No | array |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***PUT*** 

**Summary:** update stack by id

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***PUT*** /stacks/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

## ***DELETE*** 

**Summary:** delete stack by id

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***DELETE*** /stacks/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| forced | query |  | No | boolean |
| deleteDependencies | query |  | No | boolean |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /STACKS/{ID}/CERTIFICATE
## ***GET*** 

**Summary:** retrieves the TLS certificate used by the gateway

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***GET*** /stacks/{id}/certificate` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/{ID}/CLUSTER
## ***GET*** 

**Summary:** retrieve cluster by stack id

**Description:** Clusters are materialised Hadoop services on a given infrastructure. They are built based on a Blueprint (running the components and services specified) and on a configured infrastructure Stack. Once a cluster is created and launched, it can be used the usual way as any Hadoop cluster. We suggest to start with the Cluster's Ambari UI for an overview of your cluster.

### HTTP Request 
`***GET*** /stacks/{id}/cluster` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create cluster for stack

**Description:** Clusters are materialised Hadoop services on a given infrastructure. They are built based on a Blueprint (running the components and services specified) and on a configured infrastructure Stack. Once a cluster is created and launched, it can be used the usual way as any Hadoop cluster. We suggest to start with the Cluster's Ambari UI for an overview of your cluster.

### HTTP Request 
`***POST*** /stacks/{id}/cluster` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***PUT*** 

**Summary:** update cluster by stack id

**Description:** Clusters are materialised Hadoop services on a given infrastructure. They are built based on a Blueprint (running the components and services specified) and on a configured infrastructure Stack. Once a cluster is created and launched, it can be used the usual way as any Hadoop cluster. We suggest to start with the Cluster's Ambari UI for an overview of your cluster.

### HTTP Request 
`***PUT*** /stacks/{id}/cluster` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

## ***DELETE*** 

**Summary:** delete cluster on a specific stack

**Description:** Clusters are materialised Hadoop services on a given infrastructure. They are built based on a Blueprint (running the components and services specified) and on a configured infrastructure Stack. Once a cluster is created and launched, it can be used the usual way as any Hadoop cluster. We suggest to start with the Cluster's Ambari UI for an overview of your cluster.

### HTTP Request 
`***DELETE*** /stacks/{id}/cluster` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /STACKS/{ID}/CLUSTER/CONFIG
## ***POST*** 

**Summary:** get cluster properties with blueprint outputs

**Description:** Clusters are materialised Hadoop services on a given infrastructure. They are built based on a Blueprint (running the components and services specified) and on a configured infrastructure Stack. Once a cluster is created and launched, it can be used the usual way as any Hadoop cluster. We suggest to start with the Cluster's Ambari UI for an overview of your cluster.

### HTTP Request 
`***POST*** /stacks/{id}/cluster/config` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/{ID}/CLUSTER/FAILUREREPORT
## ***POST*** 

**Summary:** failure report

**Description:** Endpoint to report the failed nodes in the given cluster. If recovery mode for the node's hostgroup is AUTO then autorecovery would be started. If recovery mode for the node's hostgroup is MANUAL, the nodes will be marked as unhealthy.

### HTTP Request 
`***POST*** /stacks/{id}/cluster/failurereport` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /STACKS/{ID}/CLUSTER/FULL
## ***GET*** 

**Summary:** retrieve cluster by stack id

**Description:** Clusters are materialised Hadoop services on a given infrastructure. They are built based on a Blueprint (running the components and services specified) and on a configured infrastructure Stack. Once a cluster is created and launched, it can be used the usual way as any Hadoop cluster. We suggest to start with the Cluster's Ambari UI for an overview of your cluster.

### HTTP Request 
`***GET*** /stacks/{id}/cluster/full` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/{ID}/CLUSTER/MANUALREPAIR
## ***POST*** 

**Summary:** repair the cluster

**Description:** Removing the failed nodes and starting new nodes to substitute them.

### HTTP Request 
`***POST*** /stacks/{id}/cluster/manualrepair` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /STACKS/{ID}/CLUSTER/UPGRADE
## ***POST*** 

**Summary:** upgrade the Ambari version

**Description:** Ambari is used to provision the Hadoop clusters.

### HTTP Request 
`***POST*** /stacks/{id}/cluster/upgrade` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /STACKS/{ID}/STATUS
## ***GET*** 

**Summary:** retrieve stack status by stack id

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***GET*** /stacks/{id}/status` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /STACKS/{STACKID}/{INSTANCEID}
## ***DELETE*** 

**Summary:** delete instance resource from stack

**Description:** Stacks are template instances - a running cloud infrastructure created based on a template. Stacks are always launched on behalf of a cloud user account. Stacks support a wide range of resources, allowing you to build a highly available, reliable, and scalable infrastructure for your application needs.

### HTTP Request 
`***DELETE*** /stacks/{stackId}/{instanceId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| stackId | path |  | Yes | long |
| instanceId | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /SUBSCRIPTIONS
## ***POST*** 

**Summary:** retrive subscribe identifier

**Description:** Accepting client subscriptions to notification events.

### HTTP Request 
`***POST*** /subscriptions` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /TEMPLATES/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) templates

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***GET*** /templates/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create template as public resource

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***POST*** /templates/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /TEMPLATES/ACCOUNT/{NAME}
## ***GET*** 

**Summary:** retrieve a public or private (owned) template by name

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***GET*** /templates/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete public (owned) or private template by name

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***DELETE*** /templates/account/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /TEMPLATES/USER
## ***GET*** 

**Summary:** retrieve private templates

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***GET*** /templates/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create template as private resource

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***POST*** /templates/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /TEMPLATES/USER/{NAME}
## ***GET*** 

**Summary:** retrieve a private template by name

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***GET*** /templates/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete private template by name

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***DELETE*** /templates/user/{name}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /TEMPLATES/{ID}
## ***GET*** 

**Summary:** retrieve template by id

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***GET*** /templates/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete template by id

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***DELETE*** /templates/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /TOPOLOGIES/ACCOUNT
## ***GET*** 

**Summary:** retrieve topoligies

**Description:** A topology gives system administrators an easy way to associate compute nodes with data centers and racks.

### HTTP Request 
`***GET*** /topologies/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***POST*** 

**Summary:** create topology as public resource

**Description:** A topology gives system administrators an easy way to associate compute nodes with data centers and racks.

### HTTP Request 
`***POST*** /topologies/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /TOPOLOGIES/ACCOUNT/{ID}
## ***GET*** 

**Summary:** retrieve topology by id

**Description:** A template gives developers and systems administrators an easy way to create and manage a collection of cloud infrastructure related resources, maintaining and updating them in an orderly and predictable fashion. Templates are cloud specific - and on top of the infrastructural setup they collect the information such as the used machine images, the datacenter location, instance types, and can capture and control region-specific infrastructure variations. We support heterogenous clusters - this one Hadoop cluster can be built by combining different templates.

### HTTP Request 
`***GET*** /topologies/account/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

## ***DELETE*** 

**Summary:** delete topology by id

**Description:** A topology gives system administrators an easy way to associate compute nodes with data centers and racks.

### HTTP Request 
`***DELETE*** /topologies/account/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |
| forced | query |  | No | boolean |

**Responses**

| Code | Description |
| ---- | ----------- |
| default | successful operation |

# /USAGES
## ***GET*** 

**Summary:** retrieve usages by filter parameters

**Description:** Cloudbreak gives you an up to date overview of cluster usage based on different filtering criteria (start/end date, users, providers, region, etc)

### HTTP Request 
`***GET*** /usages` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| since | query |  | No | long |
| filterenddate | query |  | No | long |
| user | query |  | No | string |
| account | query |  | No | string |
| cloud | query |  | No | string |
| zone | query |  | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /USAGES/ACCOUNT
## ***GET*** 

**Summary:** retrieve public and private (owned) usages by filter parameters

**Description:** Cloudbreak gives you an up to date overview of cluster usage based on different filtering criteria (start/end date, users, providers, region, etc)

### HTTP Request 
`***GET*** /usages/account` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| since | query |  | No | long |
| filterenddate | query |  | No | long |
| user | query |  | No | string |
| cloud | query |  | No | string |
| zone | query |  | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /USAGES/FLEX/DAILY
## ***GET*** 

**Summary:** retrieve Flex related daily usages

**Description:** Cloudbreak gives you an up to date overview of cluster usage based on different filtering criteria (start/end date, users, providers, region, etc)

### HTTP Request 
`***GET*** /usages/flex/daily` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /USAGES/FLEX/LATEST
## ***GET*** 

**Summary:** retrieve Flex related latest usages, usages for the given day

**Description:** Cloudbreak gives you an up to date overview of cluster usage based on different filtering criteria (start/end date, users, providers, region, etc)

### HTTP Request 
`***GET*** /usages/flex/latest` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /USAGES/USER
## ***GET*** 

**Summary:** retrieve private usages by filter parameters

**Description:** Cloudbreak gives you an up to date overview of cluster usage based on different filtering criteria (start/end date, users, providers, region, etc)

### HTTP Request 
`***GET*** /usages/user` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| since | query |  | No | long |
| filterenddate | query |  | No | long |
| cloud | query |  | No | string |
| zone | query |  | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /USERS/EVICT
## ***DELETE*** 

**Summary:** remove current user from cache

**Description:** Users can be invited under an account by the administrator, and all resources (e.g. resources, networks, blueprints, credentials, clusters) can be shared across account users

### HTTP Request 
`***DELETE*** /users/evict` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /USERS/{ID}
## ***PUT*** 

**Summary:** remove user from cache (by username)

**Description:** Users can be invited under an account by the administrator, and all resources (e.g. resources, networks, blueprints, credentials, clusters) can be shared across account users

### HTTP Request 
`***PUT*** /users/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | string |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /USERS/{ID}/RESOURCES
## ***GET*** 

**Summary:** check that account user has any resources

**Description:** Users can be invited under an account by the administrator, and all resources (e.g. resources, networks, blueprints, credentials, clusters) can be shared across account users

### HTTP Request 
`***GET*** /users/{id}/resources` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /UTIL/AMBARI-DATABASE
## ***POST*** 

**Summary:** tests a database connection parameters

**Description:** 

### HTTP Request 
`***POST*** /util/ambari-database` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /UTIL/LDAP
## ***POST*** 

**Summary:** tests an LDAP connection

**Description:** 

### HTTP Request 
`***POST*** /util/ldap` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /UTIL/LDAP/{ID}
## ***GET*** 

**Summary:** tests an already exists LDAP connection

**Description:** 

### HTTP Request 
`***GET*** /util/ldap/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /UTIL/RDS
## ***POST*** 

**Summary:** tests an RDS connection

**Description:** 

### HTTP Request 
`***POST*** /util/rds` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /UTIL/RDS-DATABASE
## ***POST*** 

**Summary:** create a database connection parameters

**Description:** 

### HTTP Request 
`***POST*** /util/rds-database` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body |  | No |  |
| target | query |  | No | array |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

# /UTIL/RDS/{ID}
## ***GET*** 

**Summary:** tests an already exists RDS connection

**Description:** 

### HTTP Request 
`***GET*** /util/rds/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | long |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | successful operation |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
