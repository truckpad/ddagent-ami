# Amazon ECS - AMI packer with default DataDog Agent service

Build example:

```shell
packer build \
    -var 'ddagent_api_key=<your_dd_api_key>' \
    -var 'ami_id=<the_ecs_ami_base_from_devguide>' \
    -var 'aws_region=us-west-2' \
    packer-ddagent.json
```

You can select the AMI Base Id from [ECS Optimized-AMI list](http://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-optimized_AMI.html). Just select the AMI Base from the AWS-Region your infrastructure are in.
