# Star WARs — A Game

Jogo de estratégia para desktop inspirado nas regras de WAR/Risk e ambientado no universo de Star Wars.

## Sobre

O projeto foi desenvolvido em Java como trabalho acadêmico de engenharia de software. O jogador disputa sistemas planetários, distribui tropas, realiza ataques, recebe cartas e tenta cumprir um objetivo. O código também inclui um adversário controlado por inteligência artificial.

## Arquitetura

O repositório foi dividido em projetos Eclipse para separar responsabilidades:

- `Main/`: composição dos componentes e ponto de entrada.
- `StarWar/`: interface gráfica, telas, apresentadores, imagens e sons.
- `StarWar.Entities/`: entidades e regras centrais do jogo.
- `StarWar.UseCases/`: criação da partida, distribuição, ataque, movimentação e inteligência artificial.
- `StarWar.Boundaries/`: portas de entrada e saída dos casos de uso.
- `StarWar.DTOs/`: objetos de transferência de dados.
- `Data/` e `DataInterfaces/`: repositórios e seus contratos.
- `Tests/`: testes das regras e dos repositórios.

Essa organização aproxima o projeto de uma arquitetura em camadas, com as regras do jogo separadas da interface e da persistência em memória.

## Como executar

O ambiente original é o Eclipse. Importe os projetos Java existentes na raiz, ajuste as dependências entre eles e execute:

```text
Main/src/Program.java
```

A interface utiliza Java Swing. Os recursos visuais e de áudio devem permanecer nos caminhos originais. A reprodução de MP3 depende do arquivo `StarWar/jl1.0.1.jar`.

## Estado do projeto

Projeto acadêmico legado. Não há configuração Maven ou Gradle que reconstrua automaticamente o espaço de trabalho com todos os módulos. A execução em versões atuais do Java pode exigir ajustes de classpath e compatibilidade.

Star Wars e seus elementos são marcas e criações de seus respectivos titulares. Este repositório tem finalidade educacional e não comercial.

