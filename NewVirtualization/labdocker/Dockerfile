# Use uma Imagem Official do Python
FROM python:rc-slim

# Definindo a variavel de ambiente
ENV MESSAGE='Praesent vel viverra nisi. Mussum Ipsum, cacilds vidis litro abertis.'
ENV REDIS_HOST='127.0.0.1'

# Definindo o diretório onde a aplicação será armazenada
WORKDIR /app

# Copiar os arquivos da pasta local para dentro do container
COPY . /app

# Instalar as dependências de Python de acordo com o que foi desenvolvido na aplicação e que está declarado no arquivo requirements.txt.
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Garante que será iniciado a aplicação.
CMD ["python", "app.py"]