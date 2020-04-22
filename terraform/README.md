# Gitlab CI template / Terraform

# Example

```
stages:
  - tflint
  - check_provider_version
  - check_terraform_version

include:
  - project: 'gitlab-ci-templates/terraform'
    file: '/tflint.gitlab-ci.yml'
  - project: 'gitlab-ci-templates/terraform'
    file: '/tfupdate.gitlab-ci.yml'
```
