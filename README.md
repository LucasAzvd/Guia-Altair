# Guia simples para uso da biblioteca Altair (Python)

## Instalação
Para execução dos arquivos precisa-se instalar o pandas e o Altair, de preferência com os datasets do vegas para funcionar os códigos  
`$ conda install -c conda-forge altair vega_datasets`  
`$ conda install pandas`

## Distribuição dos arquivos
Temos 2 arquivos  
1. `Tipos de gráficos.ipynb` - Onde estão tipos de gráficos simples    
2. `Personalizações.ipynb` - Algumas maneiras de melhorar os gráficos (zoom, tooltip e etc)   
    
## Resumo básico 
Após importar a biblioteca, os gráficos vão seguir o padrão:  
~~~pyhton
alt.Chart(SEUS DADOS).TIPO DE GRAFICO(PARAMETRO).encode(
    alt.X(COLUNA, type=TIPO, PARAMETROS), #OU x=COLUNA,
    alt.Y(COLUNA, type=TIPO, PARAMENTROS), #OU y=COLUNA
    color=PARAMETROS
)
~~~~
