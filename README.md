# Matheus André Rodrigues Alves Lima

**Genômica comparativa e engenharia de pipelines.** Estudante de Análise e
Desenvolvimento de Sistemas (Senac-SP). Venho da engenharia de software e
trabalho em *comparative genomics*, *evolutionary biology* e bioinformática
aplicada a zoologia.

O que me interessa é a pergunta que ainda não tem resposta medida — e o
controle que decide se a resposta é real ou artefato.

---

## Trabalho

### 🦖 [archosauria-atavismo](https://github.com/patoangolano/archosauria-atavismo)
**As aves perderam o hardware do dente, não o software.**

Os genes de matriz de esmalte não foram deletados do genoma das aves. Estão lá,
como pseudogenes, num vão não anotado do **cromossomo Z**. Localizei ψ-`ENAM`,
ψ-`AMBN` e ψ-`AMELX` em *Gallus gallus* com coordenadas em `GRCg7b`, e repliquei
em quatro ordens de ave mais *Struthio* e *Chrysemys*.

O que sustenta o achado são os controles: *Alligator* e *Anolis*, que têm dente,
dão **zero** códons de parada internos nos mesmos alinhamentos. As aves dão 24 a
34. E dois candidatos que pareciam bons foram descartados pelo teste recíproco —
estão documentados com o motivo.

`comparative genomics` · `pseudogenes` · `DIAMOND blastx` · `synteny` · `NCBI Datasets API`

### 🐋 [bowhead-longevity-genomics](https://github.com/patoangolano/bowhead-longevity-genomics)
**Por que a baleia-da-groenlândia vive 200 anos — e por que não é um gene.**

Seis testes independentes eliminaram sequência, número de cópias e arquitetura
regulatória. O elefante resolve o paradoxo de Peto com ~20 retrogenes de `TP53`;
a baleia é o dobro do peso dele, vive quatro vezes mais, e tem **uma** cópia.
O domínio RRM da CIRBP é 100% invariante em nove espécies que cobrem de 20 a
211 anos de longevidade máxima.

Os controles validam o método antes da conclusão: proteínas de tradução aparecem
como as mais restritas do genoma (w = 0,041), receptores olfatórios como as mais
relaxadas (w = 0,329) — exatamente o esperado.

`dN/dS` · `orthology` · `MAFFT` · `IQ-TREE` · `de novo transcriptome` · `scipy`

### ⚙️ [bio-stack](https://github.com/patoangolano/bio-stack)
**A engenharia que roda por baixo.**

Servidores MCP próprios para os NIMs de biologia da NVIDIA — tratam o 202 +
`nvcf-reqid` do NVCF, validam sequência antes de gastar chamada, gravam
estruturas em disco e devolvem só o caminho (um mmCIF inteiro passa de 100 mil
tokens). Seis agentes especializados, hooks de proveniência que escrevem o
caderno de laboratório sozinhos, e **103 testes sem uma única chamada de rede**.

`MCP` · `Python` · `Nextflow` · `nf-core` · `Docker` · `WSL2` · `pytest` · `ruff`

---

## Como eu trabalho

Três regras que saíram de erros meus, e que estão documentadas nos repositórios
junto com os erros que as produziram:

1. **Nunca aceitar um resultado negativo sem exigir que o pipeline reencontre um
   positivo que você já conhece.** Um screen de duplicações deu "limpo" porque o
   mapa de símbolos cobria 56% do proteoma — não porque não havia duplicação.
2. **Ausência na anotação não é ausência no genoma.** Pseudogene degenerado some
   da consulta por símbolo sem ter saído do cromossomo.
3. **Um hit só vira achado depois do teste recíproco.** Sintenia correta e
   E-value bom não bastam: meu melhor candidato a ψ-`MMP20` acertava quatro
   outras MMPs antes da certa.

Resultado retirado fica no repositório com a correção ao lado. É o registro que
vale mais que o achado.

---

## Ferramentas

**Linguagens** Python · Bash · SQL · JavaScript
**Bioinformática** Biopython · DIAMOND · BLAST+ · MAFFT · IQ-TREE · samtools · bcftools · bedtools · seqkit · scanpy · pydeseq2 · Ensembl VEP
**Pipelines** Nextflow · nf-core · Snakemake · Docker · WSL2
**Dados & APIs** pandas · scipy · FastAPI · PostgreSQL · Redis · NCBI E-utilities · Ensembl REST · UniProt · STRING
**Reprodutibilidade** pytest · ruff · uv · proveniência estruturada (JSONL)

---

## Contato

📍 São Paulo, Brasil · aberto a remoto
💼 [LinkedIn](https://www.linkedin.com/in/matheus-andr%C3%A9-rodrigues-alves-lima-90464530a)
📧 matheusandrelima47@gmail.com

Procurando primeira posição em **bioinformática** — genômica comparativa,
engenharia de pipelines ômicos, ou biologia computacional aplicada a zoologia.
