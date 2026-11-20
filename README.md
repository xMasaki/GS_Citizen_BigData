# FIAP GS 2026.2 — CitizenTech

## Integrantes
- Lucas Masaki Nagahama | RM553084

## Resumo
**AcessaCidade** é uma plataforma web para o cidadão registrar barreiras de acessibilidade nas calçadas (buracos, pisos quebrados, rampas irregulares, obstáculos), com triagem automática inicial da foto.


## Pipeline de Dados do MVP CitizenTech

Componente Dados do AcessaCidade : pipeline **ELT** orquestrado
que coleta denúncias de problemas de acessibilidade em calçadas, trata-as em camadas **raw → bronze → silver → gold**
num warehouse **DuckDB** e publica indicadores para o app (`GET /api/indicadores/analiticos`) e para o BI.
