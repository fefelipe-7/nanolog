# internal.md
> guia de taxonomia do nanolog. define como cada tipo de nota deve ser nomeada e onde deve viver.
> criado em: 02-02-2026 | última revisão: 25-02-2026

---

## regras gerais

- datas sempre no formato dd-mm-aaaa
- nomes de arquivo em letras minúsculas, sem acentos
- o caminho da pasta já carrega o contexto da área — o nome do arquivo deve ser o mais limpo possível
- notas que perdem relevância ativa vão para `08. arquivo` sem serem deletadas

---

## estrutura de pastas

```
00. inbox
01. diário
02. devaneios
03. ideias
04. memórias
05. sonhos
06. notas de amor
07. biblioteca
08. arquivo
09. mente
    ├── aprendizados
    │   ├── tecnologia
    │   │   ├── programacao
    │   │   ├── sistemas
    │   │   └── ia
    │   ├── psicologia
    │   │   ├── cognitiva
    │   │   └── comportamental
    │   ├── financas
    │   │   ├── pessoal
    │   │   └── investimentos
    │   ├── saude
    │   │   ├── fisica
    │   │   └── mental
    │   ├── filosofia
    │   ├── comunicacao
    │   ├── relacoes
    │   └── criatividade
    ├── habilidades
    ├── projetos
    ├── modelos
    └── revisoes
```

---

## taxonomia por pasta

### 00. inbox
zona de captura rápida. nada precisa estar polido aqui.

```
_index: {tipo} + {data} + {status}
exemplo: "inbox 02-02-2026 rascunho.md"
status: rascunho, pendente, processado
```

---

### 01. diário
registro diário. um arquivo por dia.

```
_index: {dia da semana} + {data}
exemplo: "segunda 02-02-2026.md"
```

---

### 02. devaneios
pensamentos livres, reflexões sem destino definido, fluxo de consciência.
> distinção com ideias: devaneio não tem intenção de aplicação. é o pensamento em si, não o que fazer com ele.

```
_index: {tipo} + {data} + { - titulo curto}
exemplo: "devaneio 02-02-2026 - o que e amar.md"
```

---

### 03. ideias
pensamentos com potencial de virar algo — um projeto, uma ação, uma decisão.
> distinção com devaneios: ideia tem um objeto de relação claro e uma intenção de uso.

```
_index: {tipo} + {(objeto de relacao)} + {data}
exemplo: "ideia (presente) 02-02-2026.md"
```

---

### 04. memórias
registros de experiências vividas que você quer preservar.

```
_index: {tipo} + {(objeto de memoria)} + {data}
exemplo: "memoria (familia) 02-02-2026.md"
```

---

### 05. sonhos
registro de sonhos ao acordar.

```
_index: {tipo} + {data}
exemplo: "sonho 02-02-2026.md"
```

---

### 06. notas de amor
notas direcionadas, com índice sequencial.

```
_index: {tipo} + {index - } + {titulo curto}
exemplo: "nota 01 - dificil aceitar essas coisas.md"
```

---

### 07. biblioteca
notas que referenciam ou descrevem conteúdos externos — vídeos, pdfs, imagens, áudios.
o arquivo binário pode ser hospedado no próprio repositório ou linkado externamente.

```
_index: {tipo de arquivo} + {(tipo de nota atrelada)} + {data}
exemplo: "video (devaneio) 02-02-2026.md"
formatos aceitos: mp3, mp4, wav, pdf, txt, docx, png, jpg
```

---

### 08. arquivo
destino de notas que saíram do fluxo ativo. nunca delete — arquive.

```
_index: {"arquivo - "} + {nome original do arquivo}
exemplo: "arquivo - inbox 02-02-2026 rascunho.md"
```

---

### 09. mente / aprendizados
síntese de conhecimento adquirido. o caminho da subpasta define a área — o nome do arquivo é limpo.

```
_index: {tipo} + {data} + { - titulo curto}
exemplo (dentro de aprendizados/psicologia/cognitiva/): "aprendizado 02-02-2026 - vies de confirmacao.md"
```

---

### 09. mente / habilidades
habilidades que você está desenvolvendo ativamente.

```
_index: {tipo} + {(habilidade)} + {status}
exemplo: "habilidade (leitura rapida) em andamento.md"
status: planejada, em andamento, consolidada
```

---

### 09. mente / projetos
onde conhecimento vira ação. cada nota de projeto contém: estado atual, próximo passo, e links para aprendizados e habilidades relacionados.

```
_index: {tipo} + {(nome do projeto)} + {status}
exemplo: "projeto (nanolog) em andamento.md"
status: planejado, em andamento, pausado, concluido
```

---

### 09. mente / modelos
frameworks e padrões que emergem da sua experiência e do que você aprende. como você toma decisões, como você pensa sobre certos problemas.

```
_index: {tipo} + {data} + { - titulo curto}
exemplo: "modelo 02-02-2026 - como eu tomo decisoes.md"
```

---

### 09. mente / revisões
fechamento de ciclo. sem revisão, o sistema vira arquivo morto.

```
_index: {tipo de revisao} + {data}
exemplo: "revisao semanal 02-02-2026.md"
tipos: semanal, mensal, trimestral
```