# 🔄 Fluxo de trabalho

## Fluxo de trabalho para programadores

Use branches como:
```
feat/dialogue-system
feat/save-system
fix/ai-stuck-on-corners
meta/opt-navmesh-performance
```

### Fluxo
1. Pull para atualizar repositório local
2. Criar a branch  
3. Desenvolver a feature / Corrigir bug
4. Fazer commit
5. Abrir PR para `dev`  
6. Outro dev revisa e faz merge para `dev`
7. Quando precisar fazer uma *versão final* (demo, ou build de versão), abrir/aceitar PR de `dev` para `main` 

---

## Fluxo de trabalho para artistas

Use branches como:
```
art/props-forest
art/enemy-textures
art/vfx-portal
art/ui-icons
```

### Fluxo
1. Pull para atualizar repositório local
2. Criar a branch  
3. Adicionar ou atualizar assets  
4. Testar localmente em cena sandbox  
5. Fazer commit
6. Abrir PR para `dev` (nunca para main)  
7. Devs revisam e fazem merge  

Artistas utilizam **cenas de teste/playground** e **prefabs próprios**.

---

## Fluxo de trabalho para game designers

Use branches como:
```
gd/level01-blockout
gd/level01-polish
gd/cutscene01
gd/flow-adjustment
```

### Fluxo
1. Pull para atualizar repositório local
2. Criar a branch  
3. Fazer ajustes no level, fluxo ou cutscenes 
4. Fazer commit 
5. Abrir PR para `dev`  
6. Devs revisam conflitos potenciais  
7. Quando for fazer uma versão mais "final" (demo, ou algo assim), aceitar PR de `dev` para `main`   

---

## Fluxo de trabalho para sound designers

Use branches como:
```
audio/footsteps
audio/ui-clicks
audio/item-pickup
audio/trailer-music
audio/monster-screech
```

### Fluxo
1. Pull para atualizar repositório local
2. Criar a branch  
3. Adicionar assets de áudio  
4. Atualizar eventos FMOD  
5. Fazer commit
6. Abrir PR para `dev`  
7. Devs revisam e fazem merge  

---

# Resumo geral de branches

| Papel             | Prefixo de branch | Pull Request para |
|-------------------|-------------------|-------------------|
| Programador       | `feat/...`        | `dev`             |
| Artista           | `art/...`         | `dev`             |
| Game Designer     | `gd/...`          | `dev`             |
| Sound Designer    | `audio/...`       | `dev`             |

- Somente **devs** e **GD** podem aprovar merges  
- Somente **devs** podem mergear em `main`, mas **GD** precisa aprovar também 
- `main` = versão estável  
- `dev` = integração das tarefas  