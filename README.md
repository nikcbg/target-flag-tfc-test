# target-flag-tfc-test

### Purpose of the repository
Test repository to configure a workspace in Terraform Cloud to use a specific target resource with `-target` flag.

### How to use the repo
- have terraform installed 
- create Terraform Cloud (TFC) organization and user
- create worlspace in TFC and connection it VCS provider where you terrafom code is stored 
- set an enviroment varibale in your workspace `TF_CLI_ARGS_plan=-target=aws_instance.myinstance` with the resource you want to target, see screenshot [here](https://github.com/nikcbg/target-flag-tfc-test/blob/master/target_flag.png)
- execute plan/apply and check if eevrything works as planned.
