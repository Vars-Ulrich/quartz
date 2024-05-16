---
sticker: vault//Media/icons/aws-icons/Neptune.svg
---
# Overview 
- Fully-managed graph database
- A popular example of a graph dataset would be a social network
	- Users have friends
	- Posts hae comments
	- Comments have likes from users
	- Users share and like posts...
- Highly available
	- with replication across 3 AZ
	- with up to 15 read replicas
- Used to build and run applications with highly-connected datasets
	- Optimized for these complex and hard queries
- Can store up to billions of relations and query the graph with MILLISECONDS LATENCY
- Highly available with replication across multiple AZs
- Great for: 
	- knowledge graphs (Wikipedia or dare I say, OBSIDIAN!!!)
	- fraud detection
	- recommendation engines
	- social networking

## Neptune Streams
- Real-time ordered sequence of every change to your graph daa
- Changes are available immediately after writing
- **No duplicates, strict order**
- Writes are written to:
	- Your Neptune cluster
	- Your Neptune Stream
		- This stream data is accessible in an [[Hypertext Transfer Protocol|HTTP]] [[REST API]]
- Use cases
	- send notifications when certain changes are made
	- maintain graph data synchronized in another data store
		- [[Simple Storage Service|S3]]
		- [[OpenSearch Service|OpenSearch]]
		- [[ElastiCache]]
#### Exam Alerts 
#saa_exam_alerts 
- any time you see anything related to graph databases, think... :: [[Neptune]]
<!--SR:!2024-05-04,1,230-->
- 

###### Key words