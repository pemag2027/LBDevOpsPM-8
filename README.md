# LBDevOpsPM-8
L8

## ECS Nginx Demo
​
## Popis
Tento projekt nasazuje nginx aplikaci na AWS ECS pomocí Terraform a GitHub Actions.
​
### Architektura
- AWS ECS Fargate cluster
- Application Load Balancer
- VPC s public subnety
- CloudWatch logging
​
### Nasazení
1. Fork tento repository
2. Nastavte GitHub Secrets:
   - `AWS_ACCESS_KEY_ID`
   - `AWS_SECRET_ACCESS_KEY`
3. Vytvořte S3 bucket pro Terraform state
4. Upravte backend konfiguraci v `main.tf`
5. Push do main branch spustí nasazení
​
### Použití
Po úspěšném nasazení bude aplikace dostupná na URL z GitHub Actions výstupu.
​
### Čištění
```bash
terraform destroy -auto-approve
