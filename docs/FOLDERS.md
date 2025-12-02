# 📁 Estrutura de pastas do projeto

> **Observação:** Qualquer pasta pode ter subpastas dependendo da quantidade de arquivos e da lógica adotada pela equipe.

---

## **assets/** — *Tudo relacionado à arte bruta do projeto (arquivos importados)*

```
assets/
    animations/         - animações criadas na Godot (.anim, .tres)

    audio/              - sons do jogo
        bgm/            - trilhas musicais e músicas de fundo
        sfx/            - efeitos sonoros

    fonts/              - fontes utilizadas no jogo

    sprites/            - imagens de sprites 2D
        characters/     - sprites de player, npcs e inimigos
        effects/        - sprites para efeitos
        ui/             - ícones, botões e elementos de interface

    textures/           - texturas para uso geral, abstratas ou repetíveis

    vfx/                - recursos específicos para efeitos visuais
        particles/      - sistemas de partículas (materiais, configs)
        shaders/        - shaders de efeitos
        textures/       - texturas usadas em shaders/efeitos
```

---

## **resources/** — *Prefabs e dados reutilizáveis (equivalente aos “prefabs” da Unity)*

```
resources/
    characters/         - “prefabs” de personagens (com animação, estados, scripts)
                            Ex: PlayerBase.tscn, Enemy1.tscn, Enemy2.tscn

    data/               - dados específicos ou de balanceamento
                            Ex: EnemyStats.tres, DifficultyConfig.tres

    interactables/      - objetos interativos
    
    items/              - itens do jogo
                            Ex: Carta.tscn

    props/              - objetos de decoração ou utilidade simples

    templates/          - “prefabs base” usados como modelos para novos objetos

    ui/                 - componentes reutilizáveis de UI
                            Ex: BotaoAnimado.tscn
```

---

## **scenes/** — *Cenas jogáveis do projeto*

```
scenes/
    levels/             - fases/cenários jogáveis
                            Ex: Level01.tscn, Level02.tscn, subscenes

    main/               - cenas principais do jogo
                            Ex: Menu.tscn, MainGame.tscn, SplashScreen.tscn

    ui/                 - cenas de interface (HUD, menus, popups)
                            Ex: PauseMenu.tscn, SettingsMenu.tscn, HUD.tscn
```

---

## **scripts/** — *Toda lógica de programação do projeto*

```
scripts/
    autoload/           - scripts carregados globalmente (singletons)
    
    characters/         - scripts relacionados a personagens

    core/               - sistemas essenciais, independentes de cena

    gameplay/           - lógica específica das mecânicas

    ui/                 - scripts exclusivos da interface

    utils/              - scripts reutilizáveis, helpers, funções genéricas
```