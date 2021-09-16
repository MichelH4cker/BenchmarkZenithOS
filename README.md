# BenchmarkZenithOS
Este repositório contém os arquivos de Benchmark feito no sistema operacional Zenith, além de possuir um guia de como conduzir os próprios testes em diferentes sistemas.

## Environment and tools
- Sysbench
- Systemd-analyze
- Free command

## Steps to run and Debug
A primeira coisa a fazer é instalar todas as ferramentas citadas acima.

### Sysbench

#### CPU

Para analisar a performance da **CPU**, digite no terminal:
```zsh
    sysbench --test=cpu run
```
Informações e parâmetros adicionais para o teste da CPU: `sysbench --test=cpu help`.

#### Memória

Para analisar a performance da **memória**, digite no terminal:
```zsh
    sysbench --test=memory run
```
Informações e parâmetros adicionais para o teste da memória: `sysbench --test=memory help`.

### Free command
Para analisar o quanto de memória o sistema já usou e quanto está disponível, digite:
```zsh
    free -h
```

### Systemd-analyze
Determinar estatísticas de desempenho e inicialização do sistema, bem como informações de estado do sistema e do gerenciador de serviço.

Para analisar o tempo gasto no *kernel* antes que o *userspace* seja atingido, digite:
```zsh
    systemd-analyze
```
