How to use
```
resource "aws_instance" "xyz" {
  ...
  .....
  iam_instance_profile = "iam_instance_profile_m_${var.role_purpose}"
```

```
module "iam_role_for_ec2_to_cloud_watch" {
  source = "source = "https://github.com/kenych/terraform_module_iam_role.git""
  assume_role_policy = ...
  aws_iam_role_policy = ....
  role_purpose = "${var.role_purpose}"
}
```
