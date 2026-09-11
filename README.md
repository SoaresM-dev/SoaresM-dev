## Murilo Soares

**I build systems that work under real constraints.** · *[Em português abaixo ↓](#murilo-soares-1)*

3+ years building web applications for real clients, currently studying Systems
Analysis and Development. I came from the business side — websites and paid-traffic
campaigns where conversion was the only metric — and it left me with the habit of
judging software by its result. The question hasn't changed: what does this solve,
and how do I know it did?

🔍 **Open to junior and internship roles** — remote (UTC−3, overlaps US Eastern) or hybrid.

🌎 English: advanced — I read documentation and hold technical conversations without a translator.

| | |
|---|---|
| [**aiden**](https://github.com/SoaresM-dev/aiden) | Portuguese voice assistant running **100% offline** on a GPU-less machine with 15.7 GB of RAM. Whole pipeline: locally trained wake word → faster-whisper → 27-skill intent router → LLM through Ollama → Piper → WebSocket HUD. **531 tests**, time to first answer from 14.8s to 8.5s. |
| [**painel-convertta**](https://github.com/SoaresM-dev/painel-convertta) | Internal tool tracking leads and cost per lead across campaigns. FastAPI + PostgreSQL + Alembic + JWT, React front end, `docker compose up` brings it all up. **120 tests** against Postgres in CI, and [live with a demo account](https://painel-convertta-web.onrender.com). |
| [**sql-trafego-pago**](https://github.com/SoaresM-dev/sql-trafego-pago) | Star schema and **ten queries** answering the questions of a real client meeting. Deterministic seed and CI that checks every query's output — no `random()` anywhere. |
| [**consulta-cnpj**](https://github.com/SoaresM-dev/consulta-cnpj) | **Node and TypeScript** API for public company records, with caching, rate limiting and selective retry. **35 tests**, and none of them touch the network. |
| [**estruturas-c**](https://github.com/SoaresM-dev/estruturas-c) | Dynamic array, doubly linked list and circular queue in **strict C11**. **23 tests**, Valgrind clean, `gcc` and `clang` with `-Werror`, and a bench measuring O(1) against O(n). |
| [**portfolio**](https://github.com/SoaresM-dev/portfolio) | Single page in plain HTML, CSS and JavaScript. No framework, no build step. |

---

## Murilo Soares

**Construo sistemas que funcionam sob restrição real.**

3+ anos construindo aplicações web para clientes reais, hoje estudante de Análise e
Desenvolvimento de Sistemas. Vim do lado do negócio — sites e campanhas de tráfego
pago para clientes, onde a única métrica que importava era conversão — e isso me
deixou o hábito de olhar software pelo resultado. Hoje eu sou desenvolvedor, e a
pergunta continua sendo a mesma: isso resolve o quê, e como eu sei que resolveu?

🔍 **Procuro estágio ou vaga júnior em desenvolvimento**, remoto ou híbrido.

🌎 Inglês avançado — leio documentação e converso sem tradutor no caminho.

### O que está aqui

| | |
|---|---|
| [**aiden**](https://github.com/SoaresM-dev/aiden) | Assistente de voz em português rodando **100% offline** numa máquina sem GPU, com 15,7 GB de RAM. Pipeline inteiro: wake word treinada localmente → faster-whisper → roteador com 27 skills → LLM via Ollama → Piper → HUD por WebSocket. **531 testes**, tempo até a primeira resposta de 14,8s para 8,5s. |
| [**painel-convertta**](https://github.com/SoaresM-dev/painel-convertta) | Ferramenta interna para acompanhar leads e custo por lead de campanhas. FastAPI + PostgreSQL + Alembic + JWT, front em React, `docker compose up` sobe tudo. **120 testes** rodando contra Postgres na CI, e [no ar com conta demo](https://painel-convertta-web.onrender.com). |
| [**sql-trafego-pago**](https://github.com/SoaresM-dev/sql-trafego-pago) | Modelagem em estrela e **dez consultas** que respondem as perguntas de uma reunião de cliente. Semente determinística e CI que confere a saída de cada consulta — sem `random()` em lugar nenhum. |
| [**consulta-cnpj**](https://github.com/SoaresM-dev/consulta-cnpj) | API em **Node e TypeScript** que consulta dados públicos de empresas, com cache, limite de uso e repetição seletiva — repete no que é falha passageira, desiste no que não vai melhorar. **35 testes**, e nenhum toca a rede. |
| [**estruturas-c**](https://github.com/SoaresM-dev/estruturas-c) | Vetor dinâmico, lista duplamente encadeada e fila circular em **C11 estrito**. **23 testes**, Valgrind sem vazamento, `gcc` e `clang` com `-Werror`, e uma bancada que mede O(1) contra O(n). |
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
`Node.js` `TypeScript` `JavaScript` `HTML` `CSS` `React` `Vite`
`Docker` `Git` `GitHub Actions` `C`

E, do lado do negócio: `Google Ads` `Meta Ads` `Analytics` `CRO`.

### Onde me achar

[Portfólio](https://soaresm-dev.github.io/portfolio/) ·
[LinkedIn](https://www.linkedin.com/in/murilo-soares-dev/) ·
soaresmurilor@gmail.com
