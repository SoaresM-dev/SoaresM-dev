## Murilo Soares

**Construo sistemas que funcionam sob restrição real.**

Estudante de Análise e Desenvolvimento de Sistemas. Vim do lado do negócio —
sites e campanhas de tráfego pago para clientes, onde a única métrica que
importava era conversão — e isso me deixou o hábito de olhar software pelo
resultado. Hoje eu sou desenvolvedor, e a pergunta continua sendo a mesma: isso
resolve o quê, e como eu sei que resolveu?

🔍 **Procuro estágio em desenvolvimento**, remoto ou híbrido.

### O que está aqui

| | |
|---|---|
| [**aiden**](https://github.com/SoaresM-dev/aiden) | Assistente de voz em português rodando **100% offline** numa máquina sem GPU, com 15,7 GB de RAM. Pipeline inteiro: wake word treinada localmente → faster-whisper → roteador com 27 skills → LLM via Ollama → Piper → HUD por WebSocket. **524 testes**, tempo até a primeira resposta de 14,8s para 8,5s. |
| [**painel-convertta**](https://github.com/SoaresM-dev/painel-convertta) | Ferramenta interna para acompanhar leads e custo por lead de campanhas. FastAPI + PostgreSQL + Alembic + JWT, front em React, `docker compose up` sobe tudo. **43 testes** rodando contra Postgres na CI. |
| [**sql-trafego-pago**](https://github.com/SoaresM-dev/sql-trafego-pago) | Modelagem em estrela e **dez consultas** que respondem as perguntas de uma reunião de cliente. Semente determinística e CI que confere a saída de cada consulta — sem `random()` em lugar nenhum. |
| [**portfolio**](https://github.com/SoaresM-dev/portfolio) | Página única em HTML, CSS e JavaScript puros. Sem framework, sem build. |

### Como eu trabalho

Três hábitos que os repositórios acima mostram melhor do que eu descrevo:

**Meço antes de otimizar.** A cascata de STT do Aiden existe porque uma bancada
de 25 áudios mostrou que o modelo pequeno errava demais e o grande era lento
demais em CPU — não porque pareceu uma boa ideia. Em `sql-trafego-pago` eu
registrei até uma previsão minha que o `EXPLAIN ANALYZE` desmentiu.

**O que se viola vira trava.** No Aiden a regra "padrão de ativação vem do log,
nunca da cabeça" foi quebrada quatro vezes, inclusive por mim horas depois de
escrevê-la. Virou teste. Garantia estrutural nunca falhou naquele projeto;
garantia documental falhou quatro vezes.

**Escopo travado.** O Painel Convertta tem três entidades, um painel e um
login, e para aí. A versão que fica pronta vale mais que a versão completa que
nunca sobe.

### Stack

`Python` `FastAPI` `SQLAlchemy` `Alembic` `pytest` `PostgreSQL` `SQL`
`JavaScript` `HTML` `CSS` `React` `Docker` `Git` `GitHub Actions` `C`

E, do lado do negócio: `Google Ads` `Meta Ads` `Analytics` `CRO`.

### Onde me achar

[Portfólio](https://soaresm-dev.github.io/portfolio/) ·
[LinkedIn](https://www.linkedin.com/in/murilo-soares-dev/) ·
soaresmurilor@gmail.com


<!--
**SoaresM-dev/SoaresM-dev** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
