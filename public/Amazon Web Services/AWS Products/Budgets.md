---
icon: AiBudgets
aliases:
  - AWS Budgets
---

# Overview
AWS Budgets gives you the ability to set custom budgets that alert you when your costs or usage exceed (or are forecasted to exceed) your budgeted amount.

You can also use AWS Budgets to set reservation utilization or coverage targets and receive alerts when your utilization drops below the threshold you define. Reservation alerts are supported for [[Elastic Cloud Compute|EC2]], Amazon [[Relational Database Service|RDS]], Amazon [[Redshift]], Amazon [[ElastiCache]], and Amazon Elasticsearch (now deprecated, replaced with [[OpenSearch Service]]) reservations.

## Budget types (4)
- Cost budget
	- plan how much you want to spend on a service
- Usage budget
	- plan how much you want to use one or more services
- Reservation Budget
	- keep track of Reserved Instances 
	- two different ways
		- RI utlization budgets
			- see if RIs are unused or under-utlized
		- RI coverage budgets
			- how much of your instance usage is covered by a reservation
- Savings Plans budget
	- 