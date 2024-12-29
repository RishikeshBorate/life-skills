# Scaling 
In the context of software development, scalability is an application’s ability to handle workload variation while adding or removing users with minimal costs. So, a scalable solution is expected to remain stable and maintain its performance after a steep workload increase, whether expected or spontaneous. Examples of increased workload are:
- Many users accessing the system simultaneously
- Expansion in storage capacity requirements
- Increased number of transactions being processed

There are two ways of scaling 
- Vertical Scaling
- Horizontal Scaling


## Vertical Scaling (Scale Up):

Vertical scaling involves adding more resources to a single server or instance, typically by upgrading its hardware components. This approach focuses on increasing the capacity of an individual server to handle more load.

### Key characteristics of vertical scaling:

- Adding Resources: Resources such as CPU, memory, storage, and network bandwidth are increased by upgrading components within the existing server. For example, adding more RAM, replacing the CPU with a faster one, or expanding storage capacity.
- Single Point of Failure: Since a single server handles all the workload, there is a higher risk of a single point of failure. If the server experiences a hardware failure, it can lead to downtime.
- Simplicity: Vertical scaling is often simpler to implement because it involves making changes to a single server. There is no need to manage and distribute the load across multiple instances.
- Limited Scalability: There is a limit to how much a single server can be scaled vertically. Eventually, hardware constraints may restrict further upgrades.


## Horizontal Scaling (Scale Out):
Horizontal scaling involves adding more instances or servers to distribute the workload, rather than upgrading individual components. This approach focuses on increasing capacity by distributing the load across multiple machines.

### Key characteristics of horizontal scaling:

- Adding Instances: More servers or instances are added to the system to share the workload. Each instance is capable of handling a portion of the overall traffic.
- Improved Redundancy and Availability: Horizontal scaling provides better redundancy and availability since the failure of one instance does not necessarily lead to downtime. Traffic can be redirected to healthy instances.
- Load Balancing: Load balancers are used to distribute incoming requests across multiple instances, ensuring even distribution of the workload.
- Better Scalability: Horizontal scaling can provide better scalability as new instances can be added as needed, allowing for more flexible capacity expansion (elasticity).
- Complexity: Managing multiple instances, load balancers, and distributing the workload can introduce increased complexity compared to vertical scaling.



#### The choice between vertical and horizontal scaling depends on factors such as: 
- Nature of the application
- Scalability requirements
- Budget considerations
- The desired level of redundancy and availability.

 Communication between multiple machines over the network is another very important consideration that we will study more about in the following sections.

## References:

### Articles: 
- DigitalOcean: Horizontal scaling vs vertical scaling: Choosing your strategy - https://www.digitalocean.com/resources/articles/horizontal-scaling-vs-vertical-scaling 
- What is software scalability, and why should your company take it seriously? - https://itrexgroup.com/blog/what-is-software-scalability/ 

### YouTube
- Vertical and Horizontal scaling | System design - https://youtu.be/uVXuZNttOzY?feature=shared 


