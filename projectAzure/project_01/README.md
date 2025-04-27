# 📦 E-Commerce na Cloud com Streamlit, Azure e SQL Server

Este projeto é uma aplicação web desenvolvida com **Streamlit** para cadastro e listagem de produtos em um ambiente de **e-commerce**, utilizando **Azure Blob Storage** para armazenar imagens e **Azure SQL Server** para armazenar os dados dos produtos.

## 🚀 Funcionalidades

- 📥 Upload de imagem do produto para o Azure Blob Storage
- 📝 Cadastro de nome, descrição e preço do produto
- 💾 Armazenamento das informações no banco de dados SQL Server
- 🖼️ Exibição dos produtos cadastrados com suas imagens
- 🧾 Backup local dos dados em um arquivo JSON

## 🧰 Tecnologias Utilizadas

- [Streamlit](https://streamlit.io/) — Interface web
- [Azure Blob Storage](https://azure.microsoft.com/en-us/services/storage/blobs/) — Armazenamento de imagens
- [Azure SQL Server](https://azure.microsoft.com/en-us/products/azure-sql/) — Banco de dados relacional
- [Python](https://www.python.org/)
- [pymssql](http://pymssql.org/en/stable/) — Conector SQL Server
- [dotenv](https://pypi.org/project/python-dotenv/) — Gerenciamento de variáveis de ambiente

## 📦 Instalação

1. Clone este repositório:
   
 ```bash
 git clone https://github.com/seu-usuario/seu-repositorio.git
 cd seu-repositorio
 ```

2. Crie e ative um ambiente virtual:

  ```python -m venv venv
  source venv/bin/activate  # no Windows: venv\Scripts\activate
```

3. Instale as dependências:
```
  pip install -r requirements.txt
  ```


4. Configure o arquivo .env com suas credenciais do Azure e SQL Server:


5. Execute a aplicação:
```
  streamlit run main.py
```


## 📋 Notas

- Certifique-se de que o container do Azure Blob e a tabela do SQL Server já existam.
- Imagens são renomeadas com UUID para garantir unicidade.
- Dados também são salvos em <code>produtos.json</code> como backup local.