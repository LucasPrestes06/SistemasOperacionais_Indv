# 📘 Aula 07 – Computação em Nuvem e Sistemas Operacionais

## Introdução

A computação em nuvem revolucionou a forma como aplicações são desenvolvidas e disponibilizadas, permitindo que recursos computacionais sejam utilizados através da internet sem a necessidade de infraestrutura física própria. Nesta atividade foi desenvolvida uma aplicação utilizando Node.js e Express.js capaz de exibir informações do sistema operacional em execução. Posteriormente, a aplicação foi publicada na plataforma Render para comparação entre um ambiente local e um ambiente em nuvem.

---

# 🛠️ 1. Ferramentas Utilizadas

Durante o desenvolvimento do projeto foram utilizadas as seguintes tecnologias:

- Node.js para execução do JavaScript no servidor;
- Express.js para criação da aplicação web;
- Visual Studio Code como ambiente de desenvolvimento;
- Git e GitHub para versionamento do código;
- Render para hospedagem da aplicação em nuvem.

---

# 💻 2. Desenvolvimento da Aplicação

O projeto teve como objetivo apresentar informações do sistema operacional através de uma página web gerada dinamicamente pelo servidor.

As informações exibidas foram:

- Nome do host (Hostname);
- Plataforma do sistema operacional;
- Arquitetura;
- Quantidade de CPUs;
- Memória total disponível;
- Memória livre;
- Tempo de atividade do sistema (Uptime).

Para obter esses dados foi utilizado o módulo nativo **os** do Node.js, responsável por fornecer informações do ambiente onde a aplicação está sendo executada.

## Etapas de criação

1. Criação da pasta do projeto;
2. Inicialização do ambiente Node.js;
3. Instalação das dependências necessárias;
4. Implementação do arquivo principal da aplicação;
5. Testes locais para validação do funcionamento.

## Instalação das dependências

```bash
npm install express
npm install cors
```

## Execução local

```bash
node index.js
```

Após iniciar o servidor, a aplicação ficou disponível no endereço:

```text
http://localhost:3000
```

[Inserir imagem da execução local]

---

# ☁️ 3. Publicação da Aplicação no Render

Após a validação local, o projeto foi enviado para um repositório GitHub e posteriormente publicado na plataforma Render.

## Procedimento realizado

1. Criação do repositório no GitHub;
2. Envio dos arquivos do projeto;
3. Criação de uma conta na plataforma Render;
4. Criação de um novo Web Service;
5. Vinculação do repositório GitHub;
6. Configuração do comando de inicialização;
7. Execução do deploy.

## Comando de inicialização

```bash
node index.js
```

**Repositório GitHub:**  
https://github.com/TheOffsteel/SOProject.git

**Aplicação publicada:**  
https://soproject.onrender.com/

[Inserir imagem do painel do Render]

[Inserir imagem da aplicação hospedada]

---

# 🔍 4. Comparação entre Ambiente Local e Ambiente em Nuvem

## Ambiente Local

| Informação | Valor |
|------------|--------|
| Hostname | DESKTOP-PGKEFBF |
| Plataforma | win32 |
| Arquitetura | x64 |
| CPUs | 4 |
| Memória Total | 8092 MB |
| Memória Livre | 1145 MB |
| Uptime | 377 minutos |

## Ambiente Cloud (Render)

| Informação | Valor |
|------------|--------|
| Hostname | srv-d8efca9o3t8c73fdolp0-hibernate-8664bb95fd-jpg24 |
| Plataforma | linux |
| Arquitetura | x64 |
| CPUs | 8 |
| Memória Total | 31387 MB |
| Memória Livre | 16228 MB |
| Uptime | 7312 minutos |

## Análise Comparativa

Os resultados demonstram claramente a diferença entre os dois ambientes.

Enquanto a execução local ocorreu em um computador com sistema operacional Windows, a execução em nuvem ocorreu em um servidor Linux administrado pelo Render.

Também foi possível observar diferenças significativas nos recursos disponíveis. O servidor hospedado na nuvem apresentou maior quantidade de memória RAM e maior número de CPUs, evidenciando que a aplicação passou a utilizar recursos fornecidos pela infraestrutura do provedor.

Outra diferença observada foi o hostname. No ambiente local, o nome do host corresponde ao computador do usuário. Já no ambiente cloud, o hostname é gerado automaticamente pela infraestrutura utilizada pelo serviço de hospedagem.

O tempo de atividade também foi superior no ambiente cloud, demonstrando que os servidores permanecem ativos continuamente para garantir disponibilidade dos serviços.

---

# ⚙️ 5. Relação da Aplicação com Conceitos de Sistemas Operacionais

## Processos

Ao executar o comando `node index.js`, o sistema operacional cria um processo responsável pela execução da aplicação. Esse processo permanece em funcionamento aguardando solicitações dos usuários.

## Gerenciamento de Memória

As informações de memória total e memória livre exibidas pela aplicação demonstram como o sistema operacional administra os recursos disponíveis para os programas em execução.

## Utilização de CPU

A aplicação consulta a quantidade de núcleos de processamento disponíveis no sistema. Esses recursos são utilizados pelo sistema operacional para executar processos e atender requisições simultâneas.

## Sistema Operacional Hospedeiro

O projeto demonstrou que uma mesma aplicação pode ser executada em diferentes sistemas operacionais. Localmente ela foi executada sobre Windows, enquanto na nuvem foi executada sobre Linux.

## Virtualização

A infraestrutura utilizada pelo Render é baseada em tecnologias de virtualização e isolamento de ambientes. Isso permite que diversas aplicações compartilhem os mesmos servidores físicos sem interferir umas nas outras.

## Computação em Nuvem

A hospedagem da aplicação no Render representa um exemplo prático de computação em nuvem, onde recursos computacionais são disponibilizados através da internet de forma escalável e sob demanda.

Além disso, o serviço utilizado pode ser classificado como um modelo **PaaS (Platform as a Service)**, pois o desenvolvedor se preocupa apenas com a aplicação enquanto a plataforma gerencia toda a infraestrutura necessária.

---

# 🧾 6. Considerações Finais

A realização desta atividade possibilitou compreender na prática a integração entre Sistemas Operacionais e Computação em Nuvem.

Através da construção da aplicação foi possível acessar informações do ambiente de execução e observar como os recursos do sistema operacional são disponibilizados para os programas. Já a publicação no Render permitiu visualizar as diferenças existentes entre um ambiente local e um ambiente hospedado em nuvem.

Os resultados obtidos demonstraram conceitos importantes como gerenciamento de recursos, processos, virtualização, abstração de hardware e utilização de infraestrutura sob demanda, evidenciando a importância da computação em nuvem no desenvolvimento moderno de aplicações.
