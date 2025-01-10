# help-ist-sigma-access

### Acesso remoto ao ambiente de referência

Os computadores dos labs da Alameda podem ser acedidos de forma remota com SSH (_Secure Shell_), no entanto, não diretamente: é preciso antes aceder a uma máquina com acesso aos PCs dos labs.

Para este efeito pode-se usar o [cluster da RNL](https://rnl.tecnico.ulisboa.pt/servicos/cluster/), a autenticação é feita com o IST ID e password do Fénix. A home de cada utilizador (directoria presente quando se faz login) consiste na sua área pessoal do AFS disponibilizada pela DSI. É necessário portanto que o serviço AFS esteja ativo no [selfservice da DSI](https://selfservice.dsi.tecnico.ulisboa.pt/).

```bash
ssh ist1XXXXXX@cluster.rnl.tecnico.ulisboa.pt
```

Depois de entrar na shell do cluster, é possível aceder aos computadores dos labs por SSH. O computador precisa de estar ligado e no ambiente Linux. O seguinte comando lista os computadores neste estado:

```bash
# Correr no cluster
sinfo -Nr
```

Qualquer um dos computadores listados pode ser usado:

```bash
# Correr no cluster após substituir X e Y
ssh labXpY
```
