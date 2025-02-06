# Hands On - Apache Superset

## 1. Iniciar ambiente python do projeto

```shell
python -m venv .venv 
.venv/bin/activate
python -m pip install --upgrade pip
```

## 2. Instalar superset (dashboard)

```shell
pip install apache-superset
```

## 3. Criar variável de ambiente

```shell
export SUPERSET_SECRET_KEY=1234567890
export FLASK_APP=superset
```

## 4. Iniciar base de dados

```shell
superset db upgrade
```

## 5. Criar usuário admin

```shell
superset fab create-admin
```

## 6. Carregar exemplos

```shell
superset load_examples
```

## 7. Criar papéis e permissões iniciais

```shell
superset init
```

## 8. Iniciar servidor web local do Superset

```shell
superset run -p 8088 --with-threads --reload --debugger
```

## Referências

[Documentação](https://superset.apache.org/docs/intro)