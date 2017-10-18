# DataDog Agent packer

Build example:

```shell
packer build \
    -var 'ddagent_api_key=<your_dd_api_key>' \
    -var 'ami_id=<the_ecs_ami_base_from_devguide>' \
    -var 'aws_region=us-west-2' \
    packer-ddagent.json
```

You can select the AMI Base id from (ECS Optimized-AMI list)[http://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-optimized_AMI.html].
