# 📁 Estrutura de pastas do projeto

> **Observação:** Qualquer pasta pode ter subpastas dependendo da quantidade de arquivos e da lógica adotada pela equipe.

```
res://
├── autoload/
├── docs/
├── entities/
├── levels/
├── shared/
├── systems/
└── ui/
```

---

## Explicação detalhada

```
autoload/  
	- sistemas globais carregados automaticamente (singletons)
	- dados persistentes e gerenciadores centrais
	- exemplos: GameState.gd, AudioManager.gd, Settings.gd

docs/  
	- documentação interna do repositório
	- arquivos como BRANCHES.md, COMMITS.md, FOLDERS.md e WORKFLOW.md

entities/  
	- objetos completos do jogo (player, inimigos, NPCs, itens, cartas, botões, etc.)
	- cada entidade possui sua cena, script e assets específicos agrupados
	- exemplo:
		entities/card/
			card.tscn
			card.gd
			sprites/

levels/  
	- fases e ambientes jogáveis
	- cenas principais de cada fase e suas subpartes (salas, chunks, props do level)

shared/  
	- recursos reutilizáveis em múltiplas partes do jogo
	- sprites gerais, texturas, shaders, materiais, fonts, áudios comuns, vfx compartilhados
	- exemplo:
		shared/shaders/
		shared/sprites/
		shared/audio/

systems/  
	- sistemas independentes que não são entidades nem UI
	- lógica modular: save system, diálogo, inventário, combate, quests, pathfinding, etc.
	- cada sistema agrupa scripts e arquivos relacionados

ui/  
	- interfaces do jogo e elementos de apresentação
	- HUD, menus, popups, pause, inventário visual, diálogos
	- também inclui telas de apresentação:
		- tela da logo do estúdio (splash)
		- tela inicial (start screen)
		- tela de loadings
```