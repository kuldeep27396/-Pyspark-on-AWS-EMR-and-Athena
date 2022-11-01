# PySparkAPI
>A currency exchange rate project

This project is to populate the exchange rates of various currency keeping
**SGD** as base currency.

As of now we are using [Openexchangerates]
use this link to get acces to the API (https://openexchangerates.org/signup/free)

If you want to execute the code on your local system, you will have to Install and Configure AWS CLI. Kindly follow the below links for assistance
Installation-  https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
Configuration- https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html

##### Command to run for manual load:
```bash
python main.py --run_ts "1999-01-09" --config '{"app_id" : "xyz","s3_out_location":"s3://prod-bucket/temp_dir/","s3_error_out_location":"s3://prod-bucket/error_temp_dir/"}'
```
```
##### Docker Installation:
#Update the packages on your instance
sudo yum update -y

#Install Docker
sudo yum install docker -y

#Start the Docker Service
sudo service docker start

<!-- Add the ec2-user to the docker group so you can execute Docker commands without using sudo. -->
sudo usermod -a -G docker ec2-user

Relogin post this
```

```
##### Docker Commands:
```bash
docker build -t mudra . -f Dockerfile     
docker run -dit mudra                     
docker exec -it 46b6bd22cf86 /bin/bash 
```

##### Note:

If you  are not passing the `--run_ts` config then it will take the  
current datetime.


