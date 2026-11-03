# Carteira de Investimentos (CP2)

## Descrição do projeto
Sistema em C que simula uma carteira de investimentos com múltiplos ativos. O tema é **inclusão financeira** (ODS 8.10 da ONU): aproximar do mercado quem ainda está fora dele, oferecendo uma ferramenta simples para acompanhar o patrimônio e o desempenho dos investimentos. Os dados são salvos em arquivo texto e recarregados a cada execução.

## Público-alvo
Pessoas iniciantes no mercado financeiro que desejam organizar e acompanhar seus primeiros investimentos.

## Funcionalidades
- Cadastrar ativo (nome, categoria, quantidade, preço de compra e preço atual)
- Listar todos os ativos da carteira
- Calcular o valor total atual da carteira
- Calcular a rentabilidade geral (valor investido x valor atual, em R$ e %)
- Salvar e recarregar os dados automaticamente de `data/carteira.txt`

## Tecnologias utilizadas
- Linguagem C (padrão C99)
- Compilador GCC
- `struct`, vetores, funções modulares e manipulação de arquivos (`fopen`, `fprintf`, `fscanf`, `fclose`)

## Requisitos mínimos
- GCC instalado (MinGW no Windows, ou `build-essential` no Linux)
- Terminal/prompt de comando
- Qualquer computador capaz de executar o GCC

## Estrutura de pastas
```
meu-projeto-c/
├── src/       main.c, funcoes.c, modulo.c
├── include/   funcoes.h, modulo.h
├── data/      carteira.txt
└── README.md
```

## Instruções para execução
Na **raiz do projeto** (a pasta `meu-projeto-c`):
```bash
gcc -Wall -Wextra -Iinclude src/main.c src/funcoes.c src/modulo.c -o programa
./programa          # Linux/macOS
programa.exe        # Windows
```
> Execute sempre a partir da raiz, pois o programa lê o arquivo `data/carteira.txt` por caminho relativo.

Formato do arquivo (um ativo por linha, campos separados por `;`):
```
nome;categoria;quantidade;precoCompra;precoAtual
```

## Desenvolvedores
| Nome | RGM |
|------|-----|
| Ryan Belizário Alves | 48120545 |
| Gustavo Carvalho | 48542504 |
| Leticia Schnabl | 46760709 |
| Stheffany Matos | 47260467 |
| Rafael Vargas | 47594985 |
| Matheus Massato | 48301930 |
