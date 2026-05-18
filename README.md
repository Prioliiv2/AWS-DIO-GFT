# Laboratório AWS: Infraestrutura com EC2, VPC e Security Groups

## 📋 Descrição do Projeto
Este repositório contém a documentação e os aprendizados adquiridos durante o laboratório prático de computação em nuvem na AWS. 
O objetivo principal foi entender o fluxo de criação, gerenciamento e encerramento de recursos essenciais de infraestrutura como serviço (IaaS).

O projeto cobriu desde a base da rede (VPC e Subnets) até a segurança (Security Groups) e a implantação de poder computacional (Instâncias EC2).

---

## 🛠️ Recursos AWS Utilizados

*   **VPC (Virtual Private Cloud):** Criação de uma rede lógica isolada para provisionar os recursos.
*   **Subnet:** Segmentação da VPC em sub-redes para organização dos componentes.
*   **Security Groups:** Configuração de regras de firewall a nível de instância para controlar o tráfego de entrada e saída.
*   **EC2 (Elastic Compute Cloud):** Criação, conexão e encerramento de uma máquina virtual executando [Insira o SO, ex: Amazon Linux 2 / Ubuntu].

---

## 🚀 Passo a Passo Realizado

### 1. Arquitetura de Rede e Segurança
*   Criação da VPC com o bloco CIDR `[Ex: 10.0.0.0/16]`.
*   Configuração de uma Subnet `[Ex: Pública - 10.0.1.0/24]`.
*   Criação de um **Security Group** liberando as seguintes portas:
    *   Porta `22` (SSH) para conexões de administração remota.
    *   [Opcional] Porta `80` (HTTP) para tráfego web.

### 2. Provisionamento da Instância EC2
*   Seleção da AMI (Amazon Machine Image) e do tipo de instância `[Ex: t2.micro (Sustentável no nível gratuito)]`.
*   Associação do par de chaves (Key Pair) para acesso seguro.
*   Vinculação da instância à VPC, Subnet e Security Group criados anteriormente.

### 3. Validação e Encerramento
*   Conexão bem-sucedida na instância
*   **Encerramento (Termination):** Exclusão da instância EC2 para evitar custos desnecessários e limpeza dos recursos associados.

---

Aqui estão os registros visuais do processo:

#### Instância EC2 Ativa e Executando
<img width="1359" height="764" alt="image" src="https://github.com/user-attachments/assets/5c99daa1-481c-4920-a690-80c50f968ea2" /><br>

<img width="802" height="716" alt="image" src="https://github.com/user-attachments/assets/6bab701b-558a-4623-94de-d330f1d44ba1" />


#### Configuração do Security Group (Regras de Entrada)

<img width="1364" height="439" alt="image" src="https://github.com/user-attachments/assets/2b6a19dc-09dc-4abe-a197-b8d7e7037c21" />

#### Encerramento com Sucesso da Instância
<img width="1366" height="565" alt="image" src="https://github.com/user-attachments/assets/96874beb-f442-419d-92d5-e90e7694a84f" />



## 💡 Aprendizados e Conclusão
Durante este laboratório, foi possível fixar conceitos fundamentais sobre como a AWS organiza a rede e a segurança antes mesmo de colocar um servidor no ar. 
Entendi a importância do **Security Group** como primeira barreira de defesa e a necessidade de documentar e encerrar recursos (`Terminate`) para manter uma boa governança de custos em Cloud.

<img width="1218" height="859" alt="image" src="https://github.com/user-attachments/assets/b02a3444-5a5f-4e17-b681-f80179839fed" />

