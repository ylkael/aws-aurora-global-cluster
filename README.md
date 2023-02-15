# AWS Aurora PostgreSQL DB replication with Global Cluster

### Replicating Aurora PostgreSQL Database to another regions via Global Cluster.  
Amazon Aurora global databases span multiple AWS Regions, enabling low latency global reads and providing fast recovery from the rare outage that might affect an entire AWS Region. An Aurora global database has a primary DB cluster in one Region, and up to five secondary DB clusters in different Regions.  

&nbsp;  


```yaml
aurora-global-cluster.yaml:  
```
Creating a Global Cluster and a primary Aurora DB cluster with 2 serverless instances in eu-west-2 in the Global Cluster.  

&nbsp;  


```yaml
aurora-global-cluster-secondary.yaml:  
``` 
Adding a secondary region for Aurora DB with creating a secondary cluster in the Global Cluster in another region. Also creating a KMS key for accessing encrypted storage in primary cluster.    

&nbsp;  