# These are my spark notes

# Write to a target database 
Spark will create a connection to each partition 

# Controlling concurrency

You can alter the number of concurrent writes using SELECT /** COALESCE(n) */ or SELECT /** REPARTITION(n) */
Coalesce is a narrow transformation and the spark wouldnt shuffle your data across the cluster

Repartition is a wide transformation and spark would transfer data across cluster to evenly distribute the data across the cluster
