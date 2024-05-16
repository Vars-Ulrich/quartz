---
sticker: vault//Media/icons/aws-icons/RDS.svg
---
# RDS (Relational Database Service)
https://aws.amazon.com/rds/features/multi-az/


multi-az configuration

enhanced database availability

Amazon RDS Multi-AZ deployments provide enhanced availability and durability for RDS database (DB) instances, making them a natural fit for production database workloads. When you provision a Multi-AZ DB Instance, Amazon RDS automatically creates a primary DB Instance and synchronously replicates the data to a standby instance in a different Availability Zone (AZ). In case of an infrastructure failure, Amazon RDS performs an automatic failover to the standby so that you can resume database operations as soon as the failover is complete.

read replica configuration

main purpose is scalability

replicates asynchronously

can be single AZ, Cross-AZ, or Cross Region 