
May 22, 2022
I could no get it to work with localhost! I had to hardcode my cluster domain to get the docker to work on ECS
I had to place it in my webpack.client.config file like all of my current applications



All build/push commands worked with addition of 'sudo' for root priviledge
The exception is the login where i had to add in the alternative format.



sudo docker login -u AWS -p $(aws ecr get-login-password --region us-west-2) 095538846514.dkr.ecr.us-west-2.amazonaws.com


