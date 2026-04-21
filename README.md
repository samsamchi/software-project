# Projetos de Software

Este é um projeto desenvolvido em **Python**, utilizando a biblioteca **Tkinter** para a interface gráfica. O sistema implementa 10 funcionalidades requisitadas pela disciplina, aplicando conceitos de **Programação Orientada a Objetos (POO)** e **Design Patterns**.

Os padrões de projeto utilizados foram:

* Singleton
* Strategy
* Template Method

O arquivo `sas_ds.py` contém a versão do sistema com os padrões de projeto aplicados.

---

# Aplicação dos Padrões de Projeto

## Singleton

* A classe `SAS` possui um atributo de classe `_instance`, responsável por armazenar a única instância da classe.
* O método `__new__` é sobrescrito para garantir que apenas uma instância seja criada.

## Strategy

* Existem três estratégias:

  * `SalvarNota`
  * `SalvarPagamento`
  * `SalvarFolhaPagamento`
* Cada estratégia implementa o método `salvar`, responsável por tratar e persistir um tipo específico de dado.
* A classe `SAS` utiliza o método `set_estrategia` para definir qual estratégia será usada em tempo de execução.

## Template Method

* A classe `GerenciadorArquivo` define métodos base para manipulação de arquivos:

  * `manipular_arquivo`
  * `salvar_arquivo`
* Esses métodos fornecem uma estrutura comum, enquanto o comportamento específico depende da estratégia utilizada.

---

# Pré-requisitos

* Python 3.x.x
* Biblioteca Tkinter

---

# Instruções para Executar

## 1. Clonar o repositório

```bash
git clone https://github.com/samsamchi/software-project.git
```

## 2. Acessar o diretório do projeto

```bash
cd software-project
```

## 3. Verificar se o Tkinter está instalado

```bash
python -m tkinter
```

## 4. Instalar o Tkinter (caso necessário)

```bash
python -m pip install tk
```

---

# Execução do Projeto

## Versão padrão

```bash
python3 sas.py
```

## Versão com Design Patterns

```bash
python3 sas_ds.py
```

---

# Observações

* Certifique-se de executar os comandos dentro da pasta do projeto.
* Caso o projeto utilize caminhos específicos no código, ajuste-os conforme o seu ambiente.
