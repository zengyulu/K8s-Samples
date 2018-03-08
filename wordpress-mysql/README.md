##########################################################################
##			 License - Apache 2.0	 			##
##			 Copyright 2018 Siemens AG			## 
##########################################################################	


Wordpress MySQL Sample for K8s

Pre-Requisite: 

One node must be preconfigured within K8s cluster for AWS as cloud provider. Node should contain following labels:
 failure-domain.beta.kubernetes.io/region: #REGION
 failure-domain.beta.kubernetes.io/zone: #AZ

Provisoning one EBS volume with at least 3GiB so that PV can be created and PVC can be bound.Modify both PV files.

wordpress service will create one ELB in the same AWS region so ensure that node has corresponding permission / role assigned.

Tested with Rancher v1.6.14 + K8s 1.7


