# Terraform Module for Kubernetes
Terraform module to set up Bitbucket self-hosted runner on a Kubernetes cluster 

## Usage
# Uncommit namespace, secret_name, job_name, container_name if not default values
```hcl
module "runner" {
  source              = "koklushkin/runner/bitbucket"
  #namespace           = "" #default namespace "bitbucket"
  #secret_name         = "" #default secret_name "runner-oauth-credentials"
  #job_name            = "" #default job_name "runner"
  #container_name      = "" #default container_name "runner"
  account_uuid        = "d8a764e1-7920-483d-a234-246cccf4b0ae"
  repository_uuid     = "cfa64585-b2d5-4fba-ae2d-5175cac8c257"
  runner_uuid         = "da2a786c-7637-52b0-add9-9986b5d4d4e3"
  oauth_client_id     = "AKq8S6pYkAJHERo3gFOOOd02IZJD7y7V"
  oauth_client_secret = "ATOAgtO8PDo0JPUYjy4bKLixfwwZJQi8fVvdNEbdzZEeEAmzKflYreZ1jsjvr-DC4Ddu38E45206"
}
```
