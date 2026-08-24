# 🚕 Urban Routes — Automação de Testes com POM

Projeto de **automação de testes da aplicação Urban Routes**, desenvolvido em Python utilizando **Selenium WebDriver, Pytest e o padrão Page Object Model (POM)**.

O repositório registra a evolução prática da automação, desde a criação da classe de página até a combinação de métodos e o uso de `setup_class()` e `teardown_class()` para gerenciamento do navegador.

## 🎯 Objetivo

O projeto tem como objetivo praticar a automação de cenários funcionais da Urban Routes, utilizando uma estrutura baseada em POM para separar as ações realizadas na interface dos arquivos responsáveis pelos testes.

## 🛠️ Tecnologias

- **Python**
- **Selenium 4.25.0**
- **Pytest 8.3.3**
- **Page Object Model (POM)**
- **Google Chrome / ChromeDriver**
- **Git e GitHub**

As versões de Selenium e Pytest utilizadas no projeto estão registradas no `requirements.txt`.

## 🧪 O que foi praticado

### 1. Criação do Page Object

Foi criada a classe `UrbanRoutesPage` para centralizar elementos e ações da página Urban Routes, incluindo preenchimento de endereços e interação com opções de transporte.

### 2. Criação de testes utilizando POM

Os testes utilizam a classe de página para executar ações e validar resultados com `assert`.

Entre os cenários desenvolvidos estão:

- Seleção da opção **Personal** e validação da opção **Bicicleta**.
- Seleção de **Carsharing**, reserva e escolha de **Camping**, com validação do veículo **Audi A3 Sedã**.
- Validação de informações relacionadas à duração do trajeto.

Esses cenários estão organizados nas etapas de criação e evolução dos testes do repositório.

### 3. Combinação de métodos

O projeto também pratica a combinação de diferentes métodos do Page Object para representar fluxos completos de interação com a aplicação.

### 4. Setup e teardown

Na etapa mais recente, o projeto utiliza `setup_class()` para inicializar o navegador uma vez para a classe de testes e `teardown_class()` para encerrá-lo ao final da execução.

## 📁 Estrutura do projeto

```text
projeto-urban-routes-POM/
│
├── 3. Criação de arquivo POM/
│   ├── urban_routes_main_page.py
│   └── run_urban_routes_main_page.py
│
├── 4. Criação de arquivo de teste usando POM/
│   ├── Tarefa1/
│   ├── Tarefa2/
│   └── Tarefa3/
│
├── 5. Combinar métodos em POM/
│   ├── test_camping.py
│   └── urban_routes_main_page.py
│
├── 6. Métodos Setup_class() e teardown_class()/
│   ├── test_personal_scooter_and_duration.py
│   ├── test_setup_teardown_urban_routes.py
│   └── urban_routes_main_page.py
│
├── requirements.txt
└── README.md
```

A estrutura acima corresponde aos arquivos atualmente presentes no repositório.

## ▶️ Como executar

### 1. Criar o ambiente virtual

```bash
python -m venv .venv
```

### 2. Ativar o ambiente virtual

**macOS/Linux:**

```bash
source .venv/bin/activate
```

**Windows:**

```bash
.venv\Scripts\activate
```

### 3. Instalar as dependências

```bash
pip install -r requirements.txt
```

### 4. Executar os testes

```bash
pytest
```

> **Observação:** os testes dependem do ambiente da aplicação Urban Routes e do navegador Chrome. As URLs utilizadas nos arquivos de teste são ambientes de execução disponibilizados para o projeto.

## 📚 Aprendizados de QA Automation

Este projeto demonstra a aplicação prática de conceitos importantes para automação de testes:

- Localização e interação com elementos web
- Criação e reutilização de métodos
- Page Object Model
- Organização de testes automatizados
- Validação com `assert`
- Uso de `setup_class()` e `teardown_class()`
- Gerenciamento do WebDriver
- Estruturação de um projeto de automação com Python e Pytest

## 👩‍💻 Sobre o projeto

Este projeto faz parte da minha formação prática em **Quality Assurance e Test Automation**, com foco no desenvolvimento de habilidades em automação de testes utilizando **Python, Selenium, Pytest e Page Object Model**.
