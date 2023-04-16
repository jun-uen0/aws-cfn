# CloudFormation Templates

- [ ] You need to import SSL Certification to ACM
- [ ] You need to have pushed a Docker image to ECR
- [ ] Your machine has to have AWS CLI installed
- [ ] You need to define environment variables in './env/[dev,stg,prod]' ※ Make directory and files
- [ ] You need to define AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY in GitLab CI/CD Variables

※ If you don't use Document DB, you can skip launching '2.db.yml'<br>
※ If you don't use WAF, you can skip launching '5.waf.yml'

# Usage
1. Launch '1.base.yml'
2. Launch '2.db.yml' (optional)
3. Launch '3.nlb.yml'
4. Launch '4.ecs.yml'
5. Launch '5.waf.yml'

# Reference
How to build blue/green deployment with AWS Fargate and AWS CloudFormation<br>
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/blue-green.html#blue-green-resources