<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

# API de Consulta de CEPs utilizando Laravel

Este projeto implementa uma API em Laravel para consultar informações de CEPs utilizando a API pública do ViaCEP. A API permite consultar múltiplos CEPs simultaneamente e retorna os dados em um formato específico em JSON.

## Pré-requisitos

- PHP >= 7.4
- Composer instalado globalmente
- Laravel >= 9.x
- Acesso à internet para consultar a API do ViaCEP

## Instalação

1. **Clone o repositório**

   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
##Instale as dependências do projeto

bash
Copiar código
cd nome-do-repositorio
composer install
Configure o ambiente

Renomeie o arquivo .env.example para .env e configure as variáveis de ambiente, especialmente a conexão com o banco de dados, se necessário.
bash
Copiar código
cp .env.example .env
php artisan key:generate
Uso
Executando o servidor de desenvolvimento
Para iniciar o servidor de desenvolvimento do Laravel:

bash
Copiar código
php artisan serve
A API estará acessível em http://localhost:8000.

Consultando CEPs
Faça uma requisição GET para a rota /search/local/CEP-1,CEP-2,... para consultar informações de múltiplos CEPs separados por vírgula. Por exemplo:

sql
Copiar código
GET http://localhost:8000/search/local/01001000,17560-246
A API retornará um JSON com os dados de cada CEP consultado no formato especificado.


##Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request com melhorias.
