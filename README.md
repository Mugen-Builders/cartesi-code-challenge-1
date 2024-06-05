# Cartesi Rollups Code Challenge

## Descrição

Este desafio de código é parte da masterclass da @cartesiproject no Brasil, realizada no Inteli. O objetivo deste desafio é encontrar o guess correto que faz a aplicação transitar para o estado RED no código fornecido. Além disso, os alunos devem documentar todo o processo em um README e compartilhar um vídeo no Twitter.

## Instruções do Desafio

1.  *Encontrar o guess correto*:
    
    -   Utilize o código fornecido para identificar o valor correto que deve ser adivinhado (guess) para mudar o estado da aplicação para RED. Logo após leia o estado atual que indica RED.
2.  *Documentar o processo*:
    
    -   Crie um README documentando cada passo que você tomou para encontrar o guess correto. Inclua como você utilizou as funções notice, report e inspect durante o processo.
3.  *Postagem no Twitter|X*:
    
    -   Faça uma postagem no Twitter|X com um vídeo demonstrando a resolução do desafio. Use o template de mensagem fornecido abaixo e sinta-se à vontade para comentar sobre a experiência da masterclass.

## Dicas

-   Você pode utilizar o nonodo para testar mais rapidamente. O endereço a ser utilizado no Cartesi Send é: 0x70ac08179605AF2D9e75782b8DEcDD3c22aA4D0C
-   Em modo de produção, você pode utilizar o endereço padrão: 0xab7528bb862fb57e8a2bcd567a2e929a0be56a5e

## Template de Mensagem
```text
Estou participando da @cartesiproject masterclass, brazil, que está acontecendo no Inteli. 
Aqui está um vídeo demonstrando a resolução do code challenge apresentado no dia 2. Acesse o link [hyperlink], para o README onde eu explico como resolvi esse desafio.
```

## Estrutura do Repositório

-   main.py: O código principal do desafio.
-   README.md: Documentação do processo de resolução do desafio.
-   requirements.txt: Dependências necessárias para rodar o código.

## Passo a Passo

### 1. Configuração do Ambiente

1.  Clone o repositório:
    
```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

### 2. Rodando o Código

```bash
cd challenge
cartesi build
cartesi run
```

### 3. Interaja com o dApp:

```bash
cartesi send generic \                                                    ─╯
    --dapp=<endereço-do-dapp> \
    --chain-id=31337 \
    --rpc-url=http://127.0.0.1:8545 \
    --mnemonic-passphrase='test test test test test test test test test test test junk' \
    --input='<seu-input-aqui>'
```

Envie quantas inputs achar necessário para encontrar o guess!

### 4. Encontrando o Guess

Utilize a função check_guess para testar diferentes valores até encontrar o valor correto que muda o estado para RED, logo após,leia esse estado. Documente o processo no README.

### 5. Postagem no Twitter

Grave um vídeo demonstrando o processo e poste no Twitter|X utilizando o template fornecido.

## Observações Finais

Certifique-se de seguir todas as instruções e documentar claramente cada passo no README. Boa sorte!
