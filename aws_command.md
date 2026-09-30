aws ec2 run-instances \
    --image-id ami-0e5497a77ef21b5ac \
    --count 1 \
    --instance-type t3.micro \
    --key-name MyKpCli \
    --security-group-ids sg-07fb004ea65241355 \
    --subnet-id subnet-014a863e399856589 \
