# aussie-holiday-api

sudo yum install -y apache-maven
sudo yum install -y postgresql



# curl -o https://data.gov.au/data/dataset/b1bc6077-dadd-4f61-9f8c-002ab2cdff10/resource/33673aca-0857-42e5-b8f0-9981b4755686/download/australian-public-holidays-combined-2021-2024.csv

# psql -h holiday-db.nnnn.eu-north-1.rds.amazonaws.com -p 5432



CREATE TABLE holiday_info 

(id varchar(3), 
date varchar(8), 
holiday_name varchar, 
information varchar,
additional_information varchar,
jurisdiction varchar(3)
);


\COPY holiday_info FROM /home/ssm-user/data.csv DELIMITER ',' CSV HEADER;

