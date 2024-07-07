# AWS

### IAM
    1. Role -> Create Role -> AWS service -> EC2 -> Policy: AmazonEC2RoleForAWSCodeDeploy
    2. Role -> Create Role -> AWS service -> CodeDeploy -> Service or usecase: CodeDeploy -> RadioBox: CodeDeploy

### EC2
    change IAM to the EC2

### CodeDeploy
    Developer Tools -> CodeDeploy -> Applications
    New Application -> node-git-to-aws-app -> Deployment group name: node-git-to-aws-group
    Service role: codeDeploy-role (created in IAM.2)

    Disable Load Balancing

### CodePipeline
    Deploy -> Application name: node-git-to-aws-app -> Deployment group: node-git-to-aws-group



### See

- [Video Tutorial](https://www.youtube.com/watch?v=Buh3GjHPmjo)
- [CodeDeploy failures - too many individual instances failed deployment](https://www.youtube.com/watch?v=sXZVkOH6hrA)  