# Minicurso: Apache Superset

## Sobre

O Apache Superset é uma plataforma de visualização de dados open-source que facilita a criação e compartilhamento de painéis interativos. Este minicurso introduz as principais funcionalidades do Superset, mostrando como ele pode ser usado para transformar dados brutos em informações visuais significativas, ideal para empresas e projetos acadêmicos.

## Instalação

Siga o tutorial de instalação para configurar o Apache Superset no seu ambiente.

### Pré-requisitos

1. **Docker & Docker-Compose**:
    ```bash
    sudo snap install docker
    sudo apt install docker-compose
    ```
2. **Git**:
    ```bash
    sudo apt install git
    ```

### Clonar o Repositório

Clone o repositório do Apache Superset:
```bash
git clone https://github.com/apache/superset.git
cd superset
```

### Conectar a Fonte de Dados

Adicione as bibliotecas necessárias aos requisitos locais. Exemplo para Google BigQuery:
```bash
echo "sqlalchemy-bigquery" | sudo tee -a ./docker/requirements-local.txt
```

### Iniciar o Superset

Para ambiente de desenvolvimento:
```bash
docker-compose up
```

Para ambiente de produção:
```bash
docker-compose -f docker-compose-non-dev.yml pull
docker-compose -f docker-compose-non-dev.yml up -d
```

## Acessar o Superset

Acesse a interface web em [http://localhost:8088/](http://localhost:8088/)

Login inicial:
- **Usuário:** admin
- **Senha:** admin

## Slides

<div style="position: relative; width: 100%; height: 0; padding-top: 56.2500%;
 padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
 border-radius: 8px; will-change: transform;">
  <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
    src="https:&#x2F;&#x2F;www.canva.com&#x2F;design&#x2F;DAGKdloojxU&#x2F;ZobH5xG6B9qBvXPAjP7CYw&#x2F;view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
  </iframe>
</div>
<a href="https:&#x2F;&#x2F;www.canva.com&#x2F;design&#x2F;DAGKdloojxU&#x2F;ZobH5xG6B9qBvXPAjP7CYw&#x2F;view?utm_content=DAGKdloojxU&amp;utm_campaign=designshare&amp;utm_medium=embeds&amp;utm_source=link" target="_blank" rel="noopener"></a> 

## Referências

- [Artigo do Medium sobre instalação do Apache Superset com Docker](https://medium.com/yavar/apache-superset-docker-installation-9e4cc58224fd)
- [Documentação Oficial do Superset](https://superset.apache.org/docs/installation/installing-superset-using-docker-compose/)
