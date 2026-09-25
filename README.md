# Matheus André Rodrigues Alves Lima

**Desenvolvedor Python · Backend, automação e IA aplicada · Bioinformática.**
Estudante de Análise e Desenvolvimento de Sistemas (Senac-SP). Construo APIs,
automações e agentes de IA, e uso essa engenharia em genômica comparativa e
biologia computacional.

O que me interessa é a pergunta que ainda não tem resposta medida - e o
controle que decide se a resposta é real ou artefato. Vale para um genoma e
vale para código gerado por IA.

> *Python developer (backend, automation, applied AI/LLM agents) and
> bioinformatics. Open to internship, junior and trainee roles - remote or São Paulo.*

---

## Engenharia de software e IA

### [bio-stack](https://github.com/patoangolano/bio-stack)
**A engenharia que roda por baixo das análises.**

Servidores MCP próprios para os NIMs de biologia da NVIDIA - tratam o 202 +
`nvcf-reqid` do NVCF, validam sequência antes de gastar chamada, gravam
estruturas em disco e devolvem só o caminho (um mmCIF inteiro passa de 100 mil
tokens). Seis agentes especializados, hooks de proveniência que escrevem o
caderno de laboratório sozinhos, e **103 testes sem uma única chamada de rede**.

`MCP` · `Claude Code` · `agentes de IA` · `Python` · `Nextflow` · `pytest` · `ruff`

### [bot-disparos-multicanal](https://github.com/patoangolano/bot-disparos-multicanal)
**Campanhas por e-mail, WhatsApp e SMS com fila, limite de taxa e opt-out.**

Segmentação por grupos e categorias, templates com variáveis, deduplicação,
logs e reprocessamento de falhas. Um webhook (Twilio) recebe as respostas dos
contatos; scripts de linha de comando criam grupos, importam contatos e
disparam campanhas.

`Python` · `SQLite` · `Twilio` · `SMTP` · `webhooks` · `CLI`

### [chatbot-whatsapp-ia](https://github.com/patoangolano/chatbot-whatsapp-ia)
**Atendimento no WhatsApp com IA generativa, pronto para subir em VPS.**

Fluxo no n8n integrado à Evolution API e ao Google Gemini, com Docker Compose,
Nginx, scripts de instalação, backup e deploy, e validação de token no webhook.

`n8n` · `Evolution API` · `Gemini` · `Docker` · `Nginx` · `Postgres` · `Redis`

---

## Pesquisa em bioinformática

### [archosauria-atavismo](https://github.com/patoangolano/archosauria-atavismo)
**As aves perderam o hardware do dente, não o software.**

Os genes de matriz de esmalte não foram deletados do genoma das aves. Estão lá,
como pseudogenes, num vão não anotado do **cromossomo Z**. Localizei ψ-`ENAM`,
ψ-`AMBN` e ψ-`AMELX` em *Gallus gallus* com coordenadas em `GRCg7b`, e repliquei
em quatro ordens de ave mais *Struthio* e *Chrysemys*.

O que sustenta o achado são os controles: *Alligator* e *Anolis*, que têm dente,
dão **zero** códons de parada internos nos mesmos alinhamentos. As aves dão 24 a
34. E dois candidatos que pareciam bons foram descartados pelo teste recíproco -
estão documentados com o motivo.

`comparative genomics` · `pseudogenes` · `DIAMOND blastx` · `synteny` · `NCBI Datasets API`

### [bowhead-longevity-genomics](https://github.com/patoangolano/bowhead-longevity-genomics)
**Por que a baleia-da-groenlândia vive 200 anos - e por que não é um gene.**

Seis testes independentes eliminaram sequência, número de cópias e arquitetura
regulatória. O elefante resolve o paradoxo de Peto com ~20 retrogenes de `TP53`;
a baleia é o dobro do peso dele, vive quatro vezes mais, e tem **uma** cópia.
O domínio RRM da CIRBP é 100% invariante em nove espécies que cobrem de 20 a
211 anos de longevidade máxima.

Os controles validam o método antes da conclusão: proteínas de tradução aparecem
como as mais restritas do genoma (ω = 0,041), receptores olfatórios como as mais
relaxadas (ω = 0,329) - exatamente o esperado.

`dN/dS` · `orthology` · `MAFFT` · `IQ-TREE` · `de novo transcriptome` · `scipy`

---

## Como eu trabalho

Três regras que saíram de erros meus, e que estão documentadas nos repositórios
junto com os erros que as produziram:

1. **Nunca aceitar um resultado negativo sem exigir que o pipeline reencontre um
   positivo que você já conhece.** Um screen de duplicações deu "limpo" porque o
   mapa de símbolos cobria 56% do proteoma - não porque não havia duplicação.
2. **Ausência na anotação não é ausência no genoma.** Pseudogene degenerado some
   da consulta por símbolo sem ter saído do cromossomo.
3. **Um hit só vira achado depois do teste recíproco.** Sintenia correta e
   E-value bom não bastam: meu melhor candidato a ψ-`MMP20` acertava quatro
   outras MMPs antes da certa.

Uso IA (Claude Code, agentes, MCP) todos os dias para desenvolver - e aplico
essas mesmas regras ao código que ela gera: teste antes de confiar, e resultado
retirado fica no repositório com a correção ao lado.

---

## Ferramentas

**Linguagens** Python · SQL · Bash · JavaScript
**Backend e dados** FastAPI · PostgreSQL · Redis · SQLite · APIs REST · JWT · webhooks · pandas
**IA e automação** Claude Code · servidores MCP · agentes · Google Gemini API · n8n · Evolution API · Prefect
**DevOps** Docker · GitHub Actions · Linux (VPS) · Caddy/Nginx · Git
**Bioinformática** Biopython · DIAMOND · BLAST+ · MAFFT · IQ-TREE · samtools · bcftools · bedtools · Ensembl VEP · Nextflow · Snakemake
**Qualidade** pytest · ruff · uv · proveniência estruturada (JSONL)

---

## Contato

São Paulo, Brasil · aberto a remoto, híbrido ou presencial na Grande SP
[LinkedIn](https://www.linkedin.com/in/matheusarlima) · limatheus458@gmail.com

Procurando estágio, vaga júnior ou trainee em **desenvolvimento Python / IA
aplicada / dados** - com atenção especial a saúde, genômica e biologia
computacional.
