# Projeto Final NExT
## Extração de Imagens em Documentos

### Equipe
* Alecsander Cruz
* Lara Dantas
* Caio Oliveira
* Wellington Lima
* Iago Aquino


## Desafio
### Criar uma API que seja capaz de:
- Realizar o processamento de um documento do tipo XLSX, extrair as imagens desse documento e armazená-las em uma base de dados e/ou sistema de arquivos.
- Recuperar a lista de todos os documentos processados, considerando a paginação de dados para evitar lentidão na consulta e na recuperação das informações.
- Recuperar um documento específico através de um identificador do documento, que foi gerado dinamicamente na hora do seu processamento.
- Recuperar uma imagem extraída através de um identificador da imagem, que foi gerado quando extraído do documento.
- Remover da lista de documentos processados, um documento específico e todas as suas imagens através do identificador do documento.


# Configurações iniciais do projeto
## applications.properties

### AWS S3
* Necessário ter um usuário IAM (Identity and Access Management) para que a API funcione da maneira desejada.
  - EndpointUrl
  - Access Key
  - Secret Key
  - Bucket Name
    
![Configurações AWS S3](.github/assets/images/aws-s3-configurations.png)
  
### MySQL
- Url
- Username
- Password

![Configurações MySQL](.github/assets/images/mysql-configurations.png)

### Spring File size
* É necessário definir um tamanho de arquivo que seja adequado para o projeto! O tamanho padrão de arquivo aceitado pelo Spring Boot é pequeno, tornando necessária essa configuração extra.

![Configurações Spring Servlet](.github/assets/images/spring-filesize-configurations.png)
