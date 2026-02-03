# Proposta de Condomínio de Laboratórios Multiusuários - Edital Nº 01/2026
### Campus Professor Alberto Carvalho | Universidade Federal de Sergipe (UFS)

Este documento detalha a infraestrutura tecnológica e científica proposta para o **Condomínio de Laboratórios Multiusuários**, visando atender seis grupos de pesquisa de diferentes áreas do conhecimento através de uma arquitetura centralizada em Nuvem (AWS) e microsserviços (Docker).

---

## 🏗️ 1. Infraestrutura Tecnológica Compartilhada

O "Condomínio" opera sobre uma infraestrutura unificada para reduzir custos e facilitar a manutenção, composta por:

* **Servidor em Nuvem:** Instância AWS EC2 (Ubuntu Linux) atuando como *host* central.
* **Orquestração:** Docker e Docker Compose para isolamento de serviços.
* **Serviços Ativos:**
    * 🌐 **Portal Web (Nginx):** Servidor HTTP para divulgação científica dos resultados.
    * 🗃️ **Servidor de Arquivos (Zipline):** Sistema para upload e compartilhamento seguro de ativos digitais (imagens, textos, dados brutos).
    * 🛢️ **Banco de Dados (PostgreSQL):** Persistência de dados unificada.
* **Rede e Segurança:**
    * Firewall (AWS Security Groups) restringindo acesso às portas 80 (HTTP), 443 (HTTPS) e 3000 (Aplicação).
    * Topologia de Rede (Arquivo `.imn` disponível neste repositório) simulando a conexão física e lógica do laboratório.

---

## 👥 2. Equipe de Gestão (Exigência Edital Item 4.2.f)

Conforme exigido pelo edital, a equipe técnica e administrativa é composta por:

| Função | Membro Responsável | Justificativa |
| :--- | :--- | :--- |
| **Coordenador Geral** | **Guilherme Menezes de Azevedo** | Responsável técnico pela infraestrutura AWS e Docker. |
| **Assistente de Atas** | **Adomak Silva Oliveira** | Gestào das Atas. |
| **Contador/Tesoureiro** | **Júlia Rocha Valverde** | Gestão financeira do projeto. |

---

## 🔬 3. Laboratórios Residentes (Grupos de Pesquisa)

Abaixo estão listados os grupos de pesquisa que compõem este condomínio.
> **Instrução para Avaliação:** Clique no link "Acesso ao Laboratório" para visualizar o ambiente virtual de cada pesquisador.

### 🏛️ 1. Figurações do Feminino: Florbela Et Alii
* **Pesquisador:** Adomak Silva Oliveira
* **Líder:** Adriana Sacramento de Oliveira
* **Área:** Lingüística, Letras e Artes
* **Foco:** Estudos sobre o corpo feminino e hibridismo na literatura latino-americana.
* **🔗 ACESSO AO LABORATÓRIO (DNS):** `http://ec2-54-87-198-4.compute-1.amazonaws.com`

### 🌍 2. GRUPE - Estudos Urbano-regionais, Política e Educação
* **Pesquisador:** Andre Felipe de Santana Conceicao
* **Líder:** Ana Rocha dos Santos
* **Área:** Geografia (Ciências Humanas)
* **Foco:** Desenvolvimento regional, estado neoliberal e desigualdades em Sergipe.
* **🔗 ACESSO AO LABORATÓRIO (DNS):** `http://ec2-44-193-202-252.compute-1.amazonaws.com`

### 🎨 3. Laboratório de Literatura e Visualidade
* **Pesquisador:** Guilherme Menezes de Azevedo
* **Líder:** Fabio Jose Santos de Oliveira
* **Área:** Letras (Lingüística, Letras e Artes)
* **Foco:** O Teatro de Ariano Suassuna e as relações entre texto e imagem.
* **🔗 ACESSO AO LABORATÓRIO (DNS):** `http://ec2-54-157-63-79.compute-1.amazonaws.com`

### 📚 4. Clínica da Atividade e Trabalho Docente (CATD)
* **Pesquisador:** Joao Antonio Sousa da Silva
* **Líder:** Isabela Rosalia Lima de Araujo
* **Área:** Educação (Ciências Humanas)
* **Foco:** Precarização docente, inclusão escolar e BNCC nas escolas públicas.
* **🔗 ACESSO AO LABORATÓRIO (DNS):** `http://ec2-100-31-110-182.compute-1.amazonaws.com`

### 📊 5. Gestão da Informação e Evidenciação Contábil (GIEC)
* **Pesquisador:** José Renato Araújo Santana Filho
* **Líder:** Juliano Almeida de Faria
* **Área:** Administração (Ciências Sociais Aplicadas)
* **Foco:** Auditoria, mercado acionário, educação financeira e marco legal do gás natural.
* **🔗 ACESSO AO LABORATÓRIO (DNS):** `http://ec2-34-235-136-209.compute-1.amazonaws.com`

### 🌿 6. Taxonomia e Ecologia de Liquens
* **Pesquisador:** Júlia Rocha Valverde
* **Líder:** Marcela Eugenia da Silva Caceres
* **Área:** Botânica (Ciências Biológicas)
* **Foco:** Biodiversidade, taxonomia de fungos liquenizados e biotecnologia na Mata Atlântica/Caatinga.
* **🔗 ACESSO AO LABORATÓRIO (DNS):** `http://ec2-52-23-165-115.compute-1.amazonaws.com`

---

## 💰 4. Resumo Orçamentário

* **Teto por Grupo:** R$ 50.000,00 (Respeitado)
* **Total da Proposta Integrada:** Abaixo de R$ 1.000.000,00 (Respeitado)
* **Itens Financiados:** Servidor de Aplicação, Licenças de Software, Estações de Trabalho para edição visual (Letras) e análise de dados (Contábeis/Geografia).

---
*Atualizado em: Janeiro/2026 - Edital UFS 01/2026*
