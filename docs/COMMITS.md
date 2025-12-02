# 📝 Padrão para mensagem de commit

Nesta seção estão definidos os tipos de commits utilizados no projeto para manter clareza, organização e facilitar revisões.

> **Observação:** todas as mensagens de commit devem utilizar letras minúsculas para manter consistência e facilitar leitura. Coloque letras maiúsculas apenas se necessário para identificar alguma funcionalidade.

---

## Funcionalidade & Lógica

### `feat:`
**Nova funcionalidade ou mudanças relacionadas à gameplay.**
Exemplos: mecânicas, sistemas, interações, funcionalidades novas.

---

### `fix:`
**Correção de bug ou pequenos ajustes de comportamento.**
Inclui correções em gameplay, colisão, lógica, animações etc.

---

### `refactor:`
**Mudança estrutural de código sem alterar o comportamento final.**
Ex.: reorganizar código, mover funções, melhorar legibilidade.

---

### `opt:`
**Otimizações de desempenho.**
Ex.: reduzir alocações, melhorar loops, ajustar físicas pesadas.

---

### `ai:`
**Alterações no comportamento de NPCs, inimigos, navmesh ou decisões de IA.**

---

## Conteúdo / Arte / Áudio

### `asset:`
**Adição ou remoção de assets.**
Sprites, texturas, modelos, UI visual, animações, fontes, etc.

---

### `vfx:`
**Efeitos visuais.**
Partículas, shaders, pós-processamento, efeitos especiais.

---

### `audio:`
**Sons, música, mixagem e SFX.**

---

### `voice:`
**Diálogos gravados, narração, voice-over.**

---

## Level Design & Flow

### `level:`
**Alterações em fases ou mapas.**
Layout, colisões, encontros, spawn points, fluxo do level.

---

### `flow:`
**Alterações de fluxo do jogo.**
Cutscenes, narrativa, transições, sequenciamento de cenas.

---

## Balanceamento

### `balance:`
**Ajustes de estatísticas e dificuldade.**
Dano, vida, velocidade, economia, curva de progressão.

---

## Manutenção & Suporte

### `chore:`
**Tarefas de manutenção e infraestrutura**
(build, config, pipeline, dependências, organização de pastas)

---

### `docs:`
**Documentação**
README, wikis, tutoriais, comentários longos etc.

---

### `test:`
**Criação ou modificação de testes.**

---

### `style:`
**Formatação de código e lint.**
Sem alterar lógica: indentação, renomear variáveis, padrões de estilo.

---

## Estrutura da Mensagem de Commit
Padronização das mensagens de commit:
```
[tipo]: assunto

descrição (apenas se necessário)
```

---

## Exemplos de commit

- Exemplo 1
```
feat: adicionar dash ao personagem principal

- implementa sistema de dash com cooldown de 1.5s
- adiciona animação e efeito sonoro específicos para o dash
- permite cancelar ataques com dash para maior mobilidade
```

- Exemplo 2
```
fix: corrigir colisão errada entre projéteis e inimigos

- ajusta camada de colisão para evitar hits fantasmas
- corrige cálculo da altura mínima para detecção de impacto
```

- Exemplo 3
```
feat: adicionar sistema de inventário
```

- Exemplo 4
```
asset: atualizar ícones de inventário e status
```

- Exemplo 5
```
audio: atualizar BGM do Level 01 com versão estendida
```

- Exemplo 6
```
audio: adicionar efeitos de áudio para UI

- click com mouse
- hover com mouse
```

- Exemplo 7
```
level: ajustar layout da área de ponte no Level 03
```

- Exemplo 8
```
balance: reduzir velocidade de movimento do boss final
```

- Exemplo 9
```
chore: ajustar configurações de build e otimizar perfil IL2CPP
```

---

# Resumo Geral — Padronização de Commits

| Tipo        | Descrição curta |
|-------------|-----------------|
| **feat**    | Nova funcionalidade / gameplay |
| **fix**     | Correção de bug / ajustes |
| **refactor**| Reestruturação sem mudar comportamento |
| **opt**     | Otimizações de desempenho |
| **ai**      | IA: NPCs, navmesh, decisões |
| **asset**   | Adição/remoção de assets |
| **vfx**     | Efeitos visuais / partículas / shaders |
| **audio**   | Sons, músicas, SFX, mix |
| **voice**   | Diálogos gravados / voice-over |
| **level**   | Alterações de fases / mapas |
| **flow**    | Cutscenes, narrativa, transições |
| **balance** | Ajuste de stats / dificuldade |
| **chore**   | Manutenção, build, config, pipeline |
| **docs**    | Documentação |
| **test**    | Testes |
| **style**   | Formatação, lint |