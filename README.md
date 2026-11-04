<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:2b2300&height=170&section=header&text=Victor%20Huggo&fontSize=44&fontColor=FFD700&animation=fadeIn&fontAlignY=38&desc=Back-end%20%7C%20C%23%20%7C%20.NET%20%7C%20APIs%20REST&descAlignY=60&descSize=16&descColor=c9d1d9"/>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=FFD700&center=true&vCenter=true&width=720&lines=Desenvolvedor+Back-end+em+forma%C3%A7%C3%A3o;C%23+%C2%B7+.NET+%C2%B7+APIs+REST+%C2%B7+SQL;Kafka+%C2%B7+Flink+%C2%B7+CDC+%C2%B7+Dados+em+tempo+real;Analista+de+TI+%7C+Ci%C3%AAncia+da+Computa%C3%A7%C3%A3o;Gotham+n%C3%A3o+dorme.+Eu+compilo." alt="Typing SVG" />
</div>
<br/>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0d1117?style=for-the-badge&logo=linkedin&logoColor=FFD700)](https://www.linkedin.com/in/victor-huggo-2993a4280)
[![E-mail](https://img.shields.io/badge/E--mail-0d1117?style=for-the-badge&logo=gmail&logoColor=FFD700)](mailto:huggoV226@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-0d1117?style=for-the-badge&logo=github&logoColor=FFD700)](https://github.com/ictor226)
[![Americana/SP](https://img.shields.io/badge/Americana%2FSP-0d1117?style=for-the-badge&logo=googlemaps&logoColor=FFD700)](https://github.com/ictor226)

</div>

---

## 🦇 Sobre mim

Sou **Técnico em Tecnologia da Informação** e estudante de **Bacharelado em Ciência da Computação** na Universidade Anhembi Morumbi, com foco em construir minha carreira como **Desenvolvedor Back-end C#/.NET**.

Tenho interesse em desenvolvimento de APIs REST, regras de negócio, integração com bancos de dados e construção de aplicações bem estruturadas. Venho aprimorando meus conhecimentos em **C#, .NET, ASP.NET Core, SQL e MySQL** por meio dos estudos acadêmicos, cursos e projetos práticos publicados no GitHub.

Minha experiência profissional em ambientes corporativos me proporcionou uma visão prática sobre sistemas, infraestrutura, resolução de problemas e necessidades dos usuários. O contato com o ERP **TOTVS Protheus** também contribuiu para ampliar minha compreensão sobre processos empresariais e regras de negócio.

Busco evoluir continuamente como desenvolvedor, aprofundando meus conhecimentos em arquitetura de software, boas práticas de programação, APIs e bancos de dados. Quero transformar essa evolução em soluções eficientes, seguras e de fácil manutenção.

**Objetivo profissional:** conquistar uma oportunidade como **Desenvolvedor Back-end Júnior C#/.NET ou Estagiário em Desenvolvimento de Software**, contribuindo com a equipe, adquirindo experiência em projetos reais e crescendo profissionalmente na área de desenvolvimento.

---

## Stack

<div align="center">

**Back-end e linguagens**

<img src="https://skillicons.dev/icons?i=cs,dotnet,php,mysql,js&theme=dark" />

**Front-end de apoio**

<img src="https://skillicons.dev/icons?i=html,css,bootstrap&theme=dark" />

**Ferramentas**

<img src="https://skillicons.dev/icons?i=git,github,vscode,visualstudio,linux&theme=dark" />

**Estudando agora**

<img src="https://skillicons.dev/icons?i=docker,aws,postgres&theme=dark" />
<img src="https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white" />
<img src="https://img.shields.io/badge/Flink-E6526F?style=for-the-badge&logo=apacheflink&logoColor=white" />
<img src="https://img.shields.io/badge/Confluent-0d1117?style=for-the-badge&logo=confluent&logoColor=FFD700" />
</div>

---

## Estatísticas

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=ictor226&show_icons=true&hide_border=true&count_private=true&bg_color=0d1117&title_color=FFD700&icon_color=FFD700&text_color=c9d1d9&title=Estat%C3%ADsticas+do+GitHub" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ictor226&layout=compact&langs_count=6&hide_border=true&bg_color=0d1117&title_color=FFD700&text_color=c9d1d9&title=Linguagens+mais+usadas" />

<img src="https://streak-stats.demolab.com?user=ictor226&hide_border=true&background=0d1117&ring=FFD700&fire=FFD700&currStreakLabel=FFD700&sideLabels=FFD700&currStreakNum=c9d1d9&sideNums=c9d1d9&dates=8b949e&stroke=30363d" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=ictor226&bg_color=0d1117&color=FFD700&line=FFD700&point=ffffff&area=true&area_color=FFD700&hide_border=true&title_color=FFD700" />

</div>

---

## Projetos

### [pipeline-tempo-real](https://github.com/ictor226/pipeline-tempo-real) `Kafka` `Confluent Cloud` `Debezium` `Flink SQL` `Iceberg` `Avro`
Pipeline de dados em tempo real, desenvolvido no bootcamp **IBM Confluent: Dados em tempo real para agentes de IA (DIO)**. Caso de uso de pagamentos: **Postgres (Neon) → CDC com Debezium → tópicos Avro + Schema Registry → Flink SQL → tabelas Apache Iceberg (Tableflow)**.
- **Ingestão:** CDC com Kafka Connect + Debezium capturando INSERT, UPDATE e DELETE (`REPLICA IDENTITY FULL`), com a chave primária como chave Kafka para preservar a ordem
- **Contrato de dados:** schemas Avro no Schema Registry com compatibilidade BACKWARD, testes de evolução e tags PII/PCI por campo
- **Processamento:** Flink SQL com watermark, regra de fraude via `MATCH_RECOGNIZE` (3 transações do mesmo cartão em 60 s) e enriquecimento por join com contas
- **Segurança e operação:** service accounts com menor privilégio e ACLs por prefixo, métricas pela Metrics API, análise de custo e `setup.sh`/`teardown.sh` para subir e derrubar tudo
- **Lakehouse:** saída do Flink materializada em Iceberg e consultada com `pyiceberg`
- A camada de IA (embeddings e agentes) ainda não foi implementada e está nos próximos passos

### [API_em_Csharp](https://github.com/ictor226/API_em_Csharp) `C#` `.NET 8`
API RESTful completa com todas as operações **CRUD** (Create, Read, Update, Delete), desenvolvida com foco em boas práticas e organização do código.

### [CGV_CONPETITION](https://github.com/ictor226/CGV_CONPETITION) `PHP` `C#` `MySQL` `JavaScript`
Projeto Integrador do curso técnico do Senac: e-commerce de peças automotivas esportivas, simulando parceria com uma preparadora de veículos.
- **Loja:** vitrine de produtos, carrinho, cadastro e login de usuários, finalização de pedidos e painel institucional
- **Administração:** sistema desktop em C# (Windows Forms) para gerenciar usuários e produtos direto no banco MySQL

### [atv.avaliativa03](https://github.com/ictor226/atv.avaliativa03) `C#` `MySQL`
Aplicação com cadastro de lanches, validação de dados e consulta ao banco MySQL.

### [calculadora](https://github.com/ictor226/calculadora) · [área de login](https://github.com/ictor226/-rea-de-login) `HTML` `CSS` `JavaScript`
Projetos de front-end dos meus primeiros estudos em desenvolvimento web.
