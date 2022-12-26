# What is NoSQL
**Misconception**: "No" means SQL is not used in the database

**Correct definition**: "No" means "Not only SQL"
There are four categories:
- [[#Document stores]]
- [[#Graph database]]
- [[#Key-value stores]]
- [[#Wide-column data stores]]


# Document stores
- Like SQL database but without schemas and normalization 
- Collection of the things that I want to save
	- JSON only?
- Suit for dynamic data
- Easy to add or remove fileds from entities 
- Entities can have different fields
	- Easy to make a mess with the data
- Faster and more scalable than SQL DB
	- Because it runs on multiple servers

### Popular Database 
| DB Name | Provider |
| - | - |
| CosmosDB | Azure |
| DynamoDB | AWS? |
| Firebase | Google - GCP? |
| MongoDB | Independent |


# Graph database
- Common use case: people you may know
	- can be use for facebook friend recommendation
	- For example, friend of friends
- Each entity is a node, and each node relation is called edge
- Each edge connected a node with another 
- Takes only a few seconds to get all the nodes in a graph for a big data set

### Popular database
| Name | Provider |
| - | - |
| CosmosDB | Azure |
| ArangoDB | |

# Key-value stores
- Store collections os Key-Value pairs
- Can be:
	- Numeric value
	- Complex objects with subobjects
- Use cases
	- Catching
	- Session data

### Popular database 
| Name | Provider |
| - | - |
| Redis | OpenSource? Azure also has it |
| CosmosDB | Azure |
| Memcached | |

# Wide-column data stores
- Similar to Key-Value store
- Instead of having a single value, a single key have access to multiple columns
- Value can be dynamic 
- Schemeless SQL DB or Document DB inside a Key-Value store
- Use cases
	- Time series data (cpu)
	- Financial data marketing 
	- IoT data
	- Graph data

### Popular database
| Name | Provider |
| - | - |
| Cassandra | AWS? |
| HBase | |
| BigTable | |
| CosmosDB | |


