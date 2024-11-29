# Dashboard de Controle Estatístico

## Introdução

É um dashboard para monitoramento em tempo real de controle estatístico.  
Este é um exemplo do framework interativo Python Dash desenvolvido por John Souza.

---

## Tecnologias Utilizadas

- [Dash](https://dash.plot.ly/): Servidor principal e componentes interativos.
- [Plotly Python](https://plot.ly/python/): Usado para criar gráficos interativos.
- [Dash DAQ](https://dash.plot.ly/dash-daq): Componentes técnicos estilizados para aplicações industriais.

---

## Requisitos

Recomendamos criar um ambiente virtual separado executando Python 3 para este aplicativo e instalar todas as dependências necessárias lá. Execute no Terminal/Prompt de Comando:

```bash
git clone https://github.com/plotly/dash-sample-apps.git
cd dash-sample-apps/apps/dash-manufacture-spc-dashboard/
python3 -m virtualenv venv
```

Em sistemas UNIX:

```bash
source venv/bin/activate
```

No Windows:

```bash
venv\Scripts\activate
```

Para instalar todos os pacotes necessários neste ambiente, simplesmente execute:

```bash
pip install -r requirements.txt
```

Todos os pacotes do `pip` serão instalados e o aplicativo estará pronto para ser executado.

---

## Como usar este aplicativo

Execute o aplicativo localmente com o comando:

```bash
python app.py
```

Abra o endereço [http://0.0.0.0:8050/](http://0.0.0.0:8050/) no navegador para acessar o dashboard em tempo real.

Clique no botão **Learn more** para saber mais sobre como o aplicativo funciona.

---

## O que este aplicativo demonstra

- Clique nos botões na coluna `Parameter` para visualizar detalhes da linha de tendência no painel inferior.
- Clique no botão `Start` para que as tendências sejam atualizadas a cada dois segundos, simulando medições em tempo real.

O Sparkline no painel superior e o gráfico de controle no painel inferior exibem o controle de processo de Shewhart usando dados simulados. Dados fora dos limites de controle são sinalizados como "Fora de Controle (Out of Control - OOC)" e acionam alertas instantaneamente para uma verificação detalhada.

Os operadores podem interromper a medição clicando no botão `Stop` e editar os parâmetros de especificação para a linha de processo selecionada (métricas) na aba de Especificações.

---

## Recursos e Referências

- [Controle estatístico de processo de Shewhart](https://en.wikipedia.org/wiki/Shewhart_individuals_control_chart)
- [Guia do Usuário Dash](https://dash.plot.ly/)
