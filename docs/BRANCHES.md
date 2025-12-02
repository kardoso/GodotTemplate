# 🔀 Estrutura de branches

Esta é a estrutura de branches que deve ser usada sempre que você iniciar uma nova funcionalidade, correção ou alteração no projeto.

Cada tarefa (grande ou pequena) deve começar em uma branch própria, criada exclusivamente para aquele trabalho.

Criar branches separadas é essencial para manter o repositório organizado e confiável. Isso garante:
- alterações isoladas e fáceis de revisar;
- menos conflitos entre membros da equipe;
- segurança para desenvolver sem quebrar o projeto;
- histórico limpo e compreensível;
- possibilidade de descartar ou recomeçar uma tarefa sem riscos;
- fluxo de trabalho previsível e altamente colaborativo.

Em resumo:
- Nunca trabalhe direto em dev ou main.
- Nunca reutilize branches antigas para iniciar trabalhos novos.
- Sempre faça pull e crie uma branch nova antes de começar qualquer mudança.

A seguir, estão os nomes/prefixos que devem ser utilizados em branches novas, estrutura padrão que toda a equipe deve seguir.

```
main/          - protegida; apenas versões 100% estáveis (build final, demo, entrega de jam)
dev/           - protegida; integração das tarefas; onde tudo se junta antes de subir para main

feat/...       - branches curtas para novas funcionalidades
fix/...        - branches para correções ou ajustes de bugs
meta/...       - branches que acomodam tarefas de manutenção (refactor, opt, test, style, chore)

art/...        - branches curtas para assets (sprites, modelos, efeitos, ...)

gd/...         - branches para ajustes de cena, fluxo e level design

audio/...      - branches de áudio (SFX, BGM, mix, ...)

docs/...       - branches para alterações na documentação do repositório
```

Veja como fazer commits com mensagens padronizadas: **[docs/COMMITS.md](../docs/COMMITS.md)**

Veja o workflow que deve ser seguido: **[docs/WORKFLOW.md](../docs/WORKFLOW.md)**

> **Observação:** utilize sempre letras minúsculas para manter consistência e facilitar leitura.

> Branches ajudam a termos organização clara, isolamento de tarefas e facilidade de revisão.

---

# Proteção de Branches e Permissões

## main (protegida)
- Push direto proibido  
- Merge somente via Pull Request
- Deve passar nos *testes*
- Apenas devs e game designer podem aprovar merge  

---

## dev (protegida com regras mais flexíveis)
- Push direto proibido  
- Merge somente via Pull Request  
- 1 aprovação é suficiente  
- Não pode aprovar o próprio PR  
- Usada como integração contínua das tarefas

---

## Permissões de Merge
- **Devs:** podem fazer merge em `dev` e `main`  
- **Game Designers:** pode aprovar e realizar merge para `dev` 
- **Artistas e Músico:** não fazem merge (apenas PR para `dev`)  