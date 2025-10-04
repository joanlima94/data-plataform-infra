# Repositório para Hospedagem de Aplicações de Dados
Este repositório tem como objetivo facilitar a implantação de um ambiente completo para processamento e visualização de dados, utilizando as seguintes ferramentas:
## Ferramentas Hospedadas
1. **Apache Kafka**
   Um sistema distribuído de streaming de eventos, responsável por coletar e transmitir mensagens com alta escalabilidade e baixa latência.
2. **Apache Druid**
   Um banco de dados analítico projetado para ingestão rápida, consultas OLAP em tempo real e histórico, ideal para grandes volumes de dados.
3. **Apache Superset**
   Uma plataforma de visualização e exploração de dados moderna e de código aberto, que possibilita criar dashboards e explorar dados de forma interativa.
4. **Grafana**
   Uma ferramenta avançada de monitoramento e visualização de métricas e logs, permitindo acompanhar o desempenho das aplicações e ambientes.

## Sobre o Repositório
Este repositório organiza os manifestos Kubernetes necessários para implantar as aplicações no cluster, garantindo um ambiente estável e integrado para as seguintes funcionalidades:

- Ingestão de dados (Apache Kafka).
- Processamento em tempo real e análises (Apache Druid).
- Visualização e dashboards (Apache Superset, Grafana).

Todos os recursos são estruturados em manifestos YAML e são projetados para serem implantados em um cluster Kubernetes.
## Estrutura do Repositório
- **`kafka/`**: Contém os manifestos para deploy do Apache Kafka, incluindo Zookeeper e configurações associadas.
- **`druid/`**: (A ser criado) Manifestos do Apache Druid para ingestão de dados e consultas analíticas.
- **`superset/`**: (A ser criado) Configurações para implantação do Apache Superset.
- **`grafana/`**: (A ser criado) Configurações do Grafana para monitoramento e visualização de métricas.

## Como usar este repositório
1. Instale e configure seu cluster Kubernetes.
2. Acesse o diretório correspondente à aplicação que deseja implantar.
3. Aplique os manifestos com o comando:
``` bash
   kubectl apply -f <pasta-da-aplicacao>/
```
1. Após a implantação, acesse a interface de cada ferramenta usando os serviços expostos.

## Próximos Passos
- Adicionar suporte para integração nativa entre as ferramentas (Kafka → Druid → Superset).
- Definir volumes persistentes e políticas de monitoramento melhoradas.
- Incluir instruções detalhadas para configurar ingestão de dados e dashboards personalizados.

## Contribuindo
Contribuições são bem-vindas! Se você deseja adicionar melhorias, corrigir problemas ou trazer novas ideias ao repositório, sinta-se à vontade para abrir um Pull Request.
Se precisar de ajustes ou de instruções adicionais, me avise! 😊
