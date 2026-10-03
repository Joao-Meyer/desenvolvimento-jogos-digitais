# GDD Simplificado — "Coleta Sob Perseguição"

*Este é o documento de design (GDD) do projeto que vamos construir ao longo de todo o curso.

## 1. Visão geral

| Campo | Descrição |
|---|---|
| **Título** | Coleta Sob Perseguição |
| **Gênero** | Ação / coleta, single-player |
| **Plataforma** | Computador (PC) |
| **Visão de câmera** | Terceira pessoa (fixa) |
| **Engine** | Godot Engine |

## 2. Premissa

O jogador controla um personagem em um cenário 3D e precisa coletar todos os itens espalhados pelo mapa. Enquanto isso, um inimigo patrulha o cenário e, ao avistar o jogador, passa a persegui-lo. Se o inimigo alcançar o jogador, o jogo termina em derrota. Se o jogador coletar todos os itens antes disso, o jogo termina em vitória.

## 3. Elementos do jogo

- **Personagem jogável**: move-se pelo cenário sob controle do jogador (teclado).
- **Itens coletáveis**: objetos espalhados pelo cenário. Cada um coletado soma pontos.
- **Inimigo**: tem dois comportamentos — *patrulha* (movimento entre pontos fixos, quando não vê o jogador) e *perseguição* (vai direto na direção do jogador, quando o avista).
- **Cenário**: ambiente 3D estático que contém o personagem, os itens e o inimigo. Pode ter obstáculos.

## 4. Regras e progressão

- **Pontuação**: aumenta a cada item coletado.
- **Dificuldade crescente**: a velocidade do inimigo aumenta com o tempo de partida — quanto mais tempo o jogador leva, mais perigoso o inimigo fica.
- **Condição de vitória**: coletar todos os itens do cenário.
- **Condição de derrota**: ser alcançado pelo inimigo.
- **Missão bônus**: coletar todos os itens em menos de X segundos (valor exato a ser definido durante o desenvolvimento).
- **Ranking**: comparação simples dos resultados (pontuação e/ou tempo) entre os jogadores.

## 5. Áudio (visão geral)

- Trilha sonora ambiente, tocando durante a partida.
- Efeito sonoro ao coletar um item.
- Efeito sonoro quando o inimigo detecta o jogador.

## 6. Telas do jogo

- Tela de vitória.
- Tela de derrota.
- Indicação visível da pontuação atual durante a partida (HUD).

