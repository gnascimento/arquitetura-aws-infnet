# Sobre este projeto

Este é um projeto apresentado para entrega final da disciplina de Arquitetura de Soluções na Amazon AWS

## Instruções

Primeiramente crie e dê permissões para utilizar a key pair para a instância EC2 da atividade 1:
```bash
$ aws ec2 create-key-pair --key-name GabeKeyPair --query 'KeyMaterial' --output text > GabeKeyPair.pem
$ chmod 400 GabeKeyPair.pem
````


Para executar a atividade 1:

```bash
aws cloudformation create-stack --stack-name Atividade1 --template-body file://atividade1.yaml
````

Para executar a atividade 2:

```bash
aws cloudformation create-stack --stack-name Atividade2 --template-body file://atividade2.yaml
````
