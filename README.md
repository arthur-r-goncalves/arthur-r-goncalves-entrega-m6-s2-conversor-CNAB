# Conversor de CNAB

## 1. Resumo

Essa aplicação foi concebida para ler e interpretar um arquivo com código CNAB, trazendo um retorno visual para que torne a leitura e entendimento mais simples.

---

## 2. Passos de instalação

Para testar a aplicação você terá que seguir os seguintes passos:

1. Fazer o clone do repositório;
   
2. Iniciar o ambiente virtual (Venv);

   ```bash
   python -m venv venv
   ```
   
3. Em seguida, rode o seguinte comando no terminal para instalar as dependências:

   ```bash
   pip install -r requirements.txt
   ```

4. Agora, rode os seguintes comandos para gerar as tabelas do banco de dados:

   ```bash
   python manage.py makemigrations
   ```

   ```bash
   python manage.py migrate
   ```

5. Uma vez instaladas, inicie a aplicação com o seguinte comando:

   ```bash
   python manage.py runserver
   ```

---

## 3. Como utilizar a aplicação

1. No seu navegador vá para a rota `localhost:8000/api/transactions/`
   
2. Na aba de “Envie seu arquivo” selecione o arquivo de texto (.txt) desejado para que possa ser interpretado, nesse repositório você encontrará um arquivo exemplo para teste.
   
3. Após realizar o envio o resultado das transações aparecerá na aba “Resultados” juntamente com o saldo final.

---

## 4. Tecnologias e Bibliotecas

- Python;
- Django Rest Framework;
