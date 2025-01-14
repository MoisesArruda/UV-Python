# Primeiros passos com o UV

## Por que usar o uv

O uv é um pacote desenvolvido em Rust que proporciona uma instalação rápida e eficiente de bibliotecas, superando a performance do pip em muitos casos.

Possuí também um controle de versões Python similar ao pyenv, controle de dependências, além,é claro, da possíbilidade de criar ambientes virtuais.

Acesse a [Documentação oficial.](https://github.com/astral-sh/uv)

## Como Instalar o UV
```
pip install uv
```

Ou instalando utilizando curl no macOS ou Linux e PowerShell no Windows

## Iniciar um novo projeto
Para iniciar um novo projeto com o modelo do uv
```
uv init novo_projeto
```
Após criar um novo diretório, navegue até ele: 
```
cd novo_projeto
```

## Criar ambiente virtual
```
uv venv
```

## Importante!
Se enfrentar o seguinte erro:  \
**"No global/local python version has been set yet. Please set the global/local version by typing"**

Siga uma das soluções abaixo:

1. Excluir o arquivo *.python-version* e tentar novamente.

2. Entrar no arquivo *.python-version* e incluir a versão completa da versão que está utilizando, no meu exemplo ele trouxe apenas *3.10*, tive de complementar como *3.10.10* para funcionar.\
![Exemplo de arquivo python-version corrigido](https://github.com/MoisesArruda/UV-Python/blob/main/imgs/python-version.png)


## Ative o ambiente virtual
1. Windows
```bash
.venv\Scripts\activate
```
2. macOS/Linux
```bash
source .venv/bin/activate
```

## Instale as bibliotecas que deseja utilizar.

```bash
uv add langflow
```