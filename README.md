# nodejs-express-on-aws-ec2

CI/CD from Github to an AWS EC2 instance via CodePipeline and CodeDeploy.
Used a node.js express app as an example for the demo.

### Install CodeDeploy Agent in EC2
    -- create a script or execute comands one by one
    #!/bin/bash
    sudo yum -y update
    sudo yum -y install ruby
    sudo yum -y install wget
    cd /home/ec2-user
    wget https://aws-codedeploy-us-east-1.s3.amazonaws.com/latest/install
    sudo chmod +x ./install
    sudo ./install auto

### Test CodeDeploy Agent in EC2
    sudo service codedeploy-agent status
    tail -100f /opt/codedeploy-agent/deployment-root/deployment-logs/codedeploy-agent-deployments.log
    -- delete it
    sudo yum erase codedeploy-agent


### See

- [Video Tutorial](https://www.youtube.com/watch?v=Buh3GjHPmjo)
- [CodeDeploy failures - too many individual instances failed deployment](https://www.youtube.com/watch?v=sXZVkOH6hrA)  