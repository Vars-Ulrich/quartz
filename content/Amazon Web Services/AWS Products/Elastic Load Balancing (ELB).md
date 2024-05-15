---
sticker: vault//Media/icons/aws-icons/ElasticLoadBalancing.svg
aliases:
---
# Elastic Load Balancing (ELB)

- Load balancers are servers that forward internet traffic to multiple servers (EC2 Instances) downstream.
- Spread Load across multiple downstream instances
- Expose single point of access (DNS) to your application
- Do regular health checks to your instances
- Provide [[Secure Sockets Layer|SSL]] termination (https) for your websites
- High availability across zones
- its managed so AWS guarantees it will be working, take care of upgrades, maintenance, and high availability
	- This incurs higher cost than setting up your own load balancer, but the trade off is less personal effort towards setup, maintenance and integrations

## Types of LBs offered by AWS (3)
### Application load balancer
- HTTP/HTTPS only, which means it works at [[Open Systems Interconnection Model#Layer 7 - Application|layer 7]]
### Network load balancer
- Ultra-high performance
	- Keyword to look for  on the exam
- Gaming situations
- Millions of requests per second
- Allows for tcp, which means it works at [[Open Systems Interconnection Model#Layer 4 - Transport|Layer 4]]
- 
### Classic load balancer
- The exam will never ask you to choose this as it is being slowly retired
- Works at layers 4 and 7 

## Overview

#### Exam Alerts
#saa_exam_alerts 


##### Key words