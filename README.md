# Monitoramento de Sistema

Este programa monitora e exibe informações do sistema em tempo real, incluindo sistema operacional, arquitetura, modelo do processador, tempo de atividade e uso de memória RAM. Ele também salva os logs das informações em um arquivo.

## Requisitos

Node.js instalado (versão 16 ou superior recomendada)

## Instalação

- Clone este repositório:

`git clone https://github.com/GabrielBurack/System-Monitor.git`

- Acesse a pasta do projeto:

`cd seu-repositorio`

## Uso

Execute o script com o comando:

`node monitor.js`

O programa exibe as informações do sistema no console e atualiza os logs a cada segundo.

## Funcionalidades

- Exibe:

  - Sistema operacional

  - Arquitetura do sistema

  - Modelo do processador

  - Tempo de atividade formatado (dias:horas:minutos:segundos)

  - Uso de memória RAM total e percentual

- Salva logs no diretório /log/log.txt

- Atualiza os dados a cada 1 segundo

## Estrutura do Código

-**getSystemInfo()**: Coleta as informações do sistema.

-**printLog()**: Exibe os dados no console.

-**saveLog()**: Salva as informações no arquivo log.txt.

-**setInterval()**: Atualiza e armazena os dados a cada segundo.

## Exemplo de Saída no Console

```
DETALHES DO SISTEMA
Sistema Operacional: Linux
Modelo do Processador: Intel(R) Core(TM) i7-10750H CPU @ 2.60GHz
Tempo de Atividade do Sistema: 5:12:34:21
Uso de Memória RAM: 5.42 GB / 16.00 GB (34 %)
```

## Observações

O programa cria um diretório /log na raiz do sistema para armazenar os logs.

Para evitar erros de permissão, execute o script com permissões adequadas ou modifique o caminho do diretório de logs.
