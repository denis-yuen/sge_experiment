This recipe allows one to create an SGE environment that still functions even if the hostname is variable
i.e. the container is started with 
   
    docker run --rm -t -v `pwd`/datastore:/mnt/datastore  -i sge_experiment
   
as opposed to 

    docker run -h master --rm -t -v `pwd`/datastore:/mnt/datastore  -i sge_experiment
