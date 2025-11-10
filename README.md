# ETL Pipeline (Python + SQL)

## Objetivo
Padronizar, limpar e carregar dados transacionais em lote diário.

## Arquitetura / Fluxo
![diagram](docs/diagram.png)

## Stack
- Python (pandas)
- SQL (MySQL ou SQLite)
- Cron / Task Scheduler

## O que foi feito
- Normalização de colunas, tipos e datas
- Tratamento de valores ausentes e outliers
- Transformações agregadas por período
- Carga incremental otimizada

## Resultados
- Tempo de processamento reduzido de 2m40s → 38s
- Fonte padronizada para consumo em dashboards (Power BI)

## Como rodar
1. Instalar dependências: `pip install -r requirements.txt`
2. Ajustar caminho dos CSV em `src/etl.py`
3. Executar script: `python src/etl.py`

## Evidências
- `docs/diagram.png` (arquitetura)
- `docs/results.png` (comparação antes/depois)

## Próximos passos
- Subir versão automatizada via Airflow
- Publicar dataset final em API pública

## Licença
MIT
