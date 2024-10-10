
# Protoss AI for StarCraft II



Este projeto é uma IA desenvolvida em **Python** para jogar **StarCraft II** utilizando a raça **Protoss**. A IA foi projetada para vencer um oponente Terran no nível de dificuldade "Hard" usando estratégias otimizadas para expandir a economia e criar forças ofensivas eficazes com **Stalkers** e **Voidrays**.

## Estratégia

A IA implementa as seguintes táticas:

- **Trabalhadores:** Maximiza a produção de trabalhadores até atingir 50 unidades para otimizar a coleta de recursos.
- **Construção:** Prioriza a construção de **Pylons**, **Assimilators**, **Gateways** e **Stargates** de maneira eficiente para garantir o desenvolvimento contínuo das forças.
- **Unidades Ofensivas:** Foca na criação de unidades de ataque, como **Stalkers** e **Voidrays**, que são mobilizadas para atacar o inimigo assim que um número suficiente for treinado.
- **Expansão:** Expande a base automaticamente ao longo da partida, garantindo mais recursos para sustentar a produção.

## Execução do Código

O projeto pode ser executado no mapa **AbyssalReefLE** contra um bot controlado pela IA do jogo. O código abaixo mostra o exemplo de execução da partida:

```python
run_game(maps.get("AbyssalReefLE"), [
    Bot(Race.Protoss, BotAP()),
    Computer(Race.Terran, Difficulty.Hard)
    ], realtime=False)
```

- **AbyssalReefLE**: O mapa da partida.
- **Protoss (Bot)**: A raça controlada pela IA.
- **Terran (Computer)**: O adversário, com dificuldade configurada para "Hard".

## Dependências

Para rodar o projeto, você precisará do **sc2** e **numpy**

## Instalação

1. Clone o repositório:

    ```bash
    git clone https://github.com/jotamath/aiprotoss.git
    cd aiprotoss
    ```

2. Instale as dependências:

    ```bash
    pip install -r requirements.txt
    ```

3. Certifique-se de que o **StarCraft II** está instalado e o caminho de instalação está configurado corretamente.
