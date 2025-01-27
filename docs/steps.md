# Steps

---

## Process steps in the Terraform-IAAC plug-in

### Run Terraform Command (AWS)

Use this step to execute rexx program

| Name                 | Type   | Description                                                                                                                  | Required |
|----------------------|--------|------------------------------------------------------------------------------------------------------------------------------|----------|
| Terraform File Path  | String | Full path of the .tf file that contains all configurations needed for a resource creation for any cloud service provider.    | Yes      |
| Source Value         | String | Full path of the terraform installation. Ex: /usr/local/bin/.                                                                | Yes      |
| AWS Role             | String | AWS Role to assume                                                                                                           | No       |
