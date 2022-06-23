# SAE24

CREATE USER 'toto'@'%' IDENTIFIED BY 'toto';

FLUSH PRIVILEGES;

GRANT ALL PRIVILEGES ON *.* TO 'toto'@'%'
->     WITH GRANT OPTION;

USE datamining;

SELECT * FROM sensors_data;

to use the data_base.
