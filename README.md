# Doces da Vovó

## Sobre o projeto

A Tech Solutions foi contrata pela confeitaria Doces da Vovó, para criar um site institucional, com o objetivo de se conectar mais com seus clientes
trazendo uma exibição de seus produtos, uma maior facilidade para fazer pedidos e até mesmo entrar em contato para dúvidas e sugestões.

## Tecnologias utilizadas

- **Front-end:** HTML, CSS e JavaScript
- **Back-end:** PHP e SQL
- **Banco de dados:**phpMyAdmin
- **Ferramentas:**XAMPP

## Execução do Projeto

1. Instalação do XAMPP
   
- Acesse o site oficial: https://www.apachefriends.org/
- Baixe e instale a versão compatível com seu sistema operacional.
- Após instalar, abra o XAMPP Control Panel e inicie os serviços Apache e MySQL.
  
2. Criar o Banco de Dados e a Tabela de Contato
   
2.1 Acesse o phpMyAdmin:
http://localhost/phpmyadmin/

2.2 Crie o banco de dados:
CREATE DATABASE doces_da_vovo;

2.3 Selecione o banco de dados e execute o seguinte SQL para criar a tabela de contato:
CREATE TABLE contato (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL,
    mensagem TEXT NOT NULL
);

3. Preparar o Projeto
3.1 Copie a pasta do projeto para o diretório:
C:\xampp\htdocs\doces-da-vovo

3.2 No navegador, acesse o projeto:
http://localhost/doces-da-vovo

## Recomendações de Segurança

- **Sanitizar os campos:** Fazer o uso do htmlspecialchars() para converter caracteres inválidos ou do filter_var() para remover.
- **Validação de e-mail:** Tambem pode-se usar o filter_var() para uma validação de e-mails.
- **Tamanho máximo de mensagem:** Atravez do strlen() e possivel saber o tamanho da mensagem e limitar seu tamanho.
- **Prevenção de Injeção SQL:** Usar declarações preparadas como prepare(), bind_param(), execute() para que a consulta com o banco de dados seja segura.
