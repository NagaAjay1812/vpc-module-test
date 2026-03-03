# 🧪 vpc-module-test (Testing a VPC Module)

This repository is a test project used to validate VPC provisioning using Terraform.

It helps practice:
- Provider setup
- Module calling (or direct VPC resource usage)
- Outputs verification
- Safe iteration while learning

---

## 📂 Folder Structure (Actual)

```
vpc-module-test/
├── .gitignore
├── .terraform.lock.hcl
├── README.md
├── outputs.tf
├── provider.tf
└── vpc.tf
```

---

## 🧩 What This Repo Does

- `provider.tf` configures AWS provider/region
- `vpc.tf` contains the VPC/module calling logic
- `outputs.tf` prints useful IDs (VPC, subnets, etc.)
- `.terraform.lock.hcl` locks provider versions for consistency

---

## 🚀 How to Run

```bash
terraform init
terraform plan
terraform apply
```

Destroy:

```bash
terraform destroy
```

---

## 🎯 Why This Repo Matters

This repo is useful as a sandbox for testing VPC changes safely before applying the same pattern in bigger projects.

It’s also a clean example of how Terraform projects are typically organized:
- provider config separated
- infra code isolated
- outputs clearly exposed