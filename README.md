# M9-AWSCLI-COMMANDS

## Repository dedicated to showcasing proficiency with aws cli

### Command History:

```bash
2020  aws
 2021  aws --version
 2022  cat ~/.aws/credentials
 2023  cat ~/.aws/config 
 2024  aws ec2 describe-security-groups
 2025  aws ec2 describe-security-groups --no-cli-pager 
 2026  aws ec2 create-security-group --group-name my-sg --description "My SG" --vpc-id vpc-09d7ffddc09d64406
 2027  cd ..
 2028  ls
 2029  mkdir awscli
 2030  cd awscli/
 2031  ls
 2032  vim aws_command.md
 2033  aws ec2 describe-security-groups --no-cli-pager 
 2034  vim aws_command.md
 2035  aws ec2 authorize-security-group-ingress --group-id sg-07fb004ea65241355 --protocol tcp --port 22 --cidr 174.55.206.199/32 
 2036  aws ec2 describe-security-groups --group-ids sg-07fb004ea65241355
 2037  vim aws_command.md
 2038  aws ec2 create-key-pair --key-name MyKpCli --query 'KeyMaterial' --output text > mykpcli.pem
 2039  ls
 2040  vim aws_command.md
 2041  aws ec2 describe-subnets 
 2042  vim aws_command.md
 2043  cat aws_command.md 
 2044  aws ec2 run-instances
 2045  cat aws_command.md 
 2046  vim aws_command.md 
 2047  cat aws_command.md 
 2048  aws ec2 run-instances     --image-id ami-0e5497a77ef21b5ac     --count 1     --instance-type t3.micro     --key-name MyKpCli     --security-group-ids sg-07fb004ea65241355     --subnet-id subnet-014a863e399856589
 2049  aws ec2 describe-instances
 2050  ssh -i mykpcli.pem ubuntu@3.15.198.214
 2051  chmod 400 mykpcli.pem 
 2052  ssh -i mykpcli.pem ubuntu@3.15.198.214
 2053  aws ec2 describe-instances --filters "Name=instance-type,Values=t3.micro" --query "Reservations[].Instances[].InstanceID"
 2054  aws ec2 describe-instances --filters "Name=instance-type,Values=t3.micro" --query "Reservations[].Instances[].InstanceId"
 2055  aws ec2 describe-instances --filters "Name=instance-type,Values=t3.micro" --query "Reservations[].Instances[].InstanceId" --query "Reservations[].Instances[].KeyName"
 2056  aws ec2 describe-instances --filters "Name=instance-type,Values=t3.micro" --query "Reservations[].Instances[].KeyName"
 2057  aws iam create-group --group-name MyGroupCli
 2058  aws iam add-user-to-group --user-name MyUserCli --group-name MyGroupCli
 2059  aws iam create-user --user-name MyUserCli
 2060  aws iam add-user-to-group --user-name MyUserCli --group-name MyGroupCli
 2061  aws iam get-group --group-name MyGroupCli 
 2066  aws iam list-policies --query 'Policies[?PolicyName==`AmazonEC2FullAccess`].Arn' --output text
 2067  aws iam attach-group-policy --group-name MyGroupCli --policy-arn arn:aws:iam::aws:policy/AmazonEC2FullAccess
 2068  aws iam list-attached-group-policies --group-name MyGroupCli 
 2074  aws iam create-login-profile --user-name MyUserCli --password Mypassword! --password-reset-required 
 2075  aws iam get-user
 2076  aws iam get-group --group-name MyGroupCli
 2077  vim changePwdPolicy.json
 2078  aws iam create-policy --policy-name changePwd --policy-document file://changePwdPolicy.json 
 2079  aws iam attach-group-policy --group-name MyGroupCli --policy-arn arn:aws:iam::516633646044:policy/changePwd
 2080  aws iam create-access-key --user-name MyUserCli
 2084  export AWS_ACCESS_KEY_ID=REDACTED
 2085  aws ec2 describe-instances
 2086  export AWS_SECRET_ACCESS_KEY=REDACTED 
 2087  aws ec2 describe-instances
 2088  aws iam create-user --user-name test
 2090  cat aws_command.md 
```


