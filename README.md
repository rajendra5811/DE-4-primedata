### primedata architechure  
<img width="831" height="558" alt="image" src="https://github.com/user-attachments/assets/6bbbf132-1771-4b18-b9b6-dd8ec1693ffd" />

dataset from kaggle
https://www.kaggle.com/datasets/shivamb/amazon-prime-movies-and-tv-shows
##step-1
create data factory and storage account
upload dataset to github and https will be source format in linking service in copy activity ( extract data from github link by copy activity)
gen2 storage account will be sink where prime data in bronze container in storage account.
## step-2
create data bricks , commpute resources and setup connect to adls ( azure datalake storage) through registerion application with access storage account.
data transformation applied like data format changes .....etc
This transformed data placed in silver container 
## step=3
to connect synapse and get data from silver container into sql database.
create schema and external location in gold container.
integration of power bi
