# Terraform Pipeline com CI/CD

Este repositório contém a configuração de um pipeline para gerenciar infraestrutura com Terraform. O pipeline é configurado para ser executado em diferentes ambientes (dev, hml, prd), com etapas de validação (CI) e deploy.

---

## Estrutura de Diretórios

```plaintext
.
├── .github
│   └── workflows
│       └── terraform-pipeline.yml   # Configuração do pipeline no GitHub Actions
├── terraform
│   ├── main.tf                      # Código principal do Terraform
│   ├── variables.tf                 # Declaração de variáveis
│   ├── outputs.tf                   # Outputs do Terraform
│   ├── providers.tf                 # Configuração dos provedores
│   ├── backend.tf                   # Configuração do backend remoto
│   └── envs                         # Pasta com os arquivos de variáveis por ambiente
│       ├── dev.tfvars               # Variáveis específicas para o ambiente dev
│       ├── hml.tfvars               # Variáveis específicas para o ambiente hml
│       └── prd.tfvars               # Variáveis específicas para o ambiente prd
└── README.md                        # Documentação do projeto
