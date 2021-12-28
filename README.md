# Desafio Ignite - Princípios do SOLID

Desafio do Ignite, trilha de Nodejs, focado em fixar os princípios do SOLID, atribuindo as funções corretas para Model, Controllers, Use cases e Repositories.

Para completar o desafio é necessário que a API passe pelos seguintes testes

### Teste do model
 ##### User model
    ✓ should be able to create an user with all props 

### Testes do repositório
 ##### UsersRepository
    ✓ should be able to create new users 
    ✓ should be able to list all users 
    ✓ should be able to find user by ID 
    ✓ should be able to find user by e-mail address 
    ✓ should be able to turn an user as admin 

### Testes do useCases  
 ##### ListAllUsersUseCase
    ✓ should be able to list all users 
    ✓ should not be able to a non admin user get list of all users 
    ✓ should not be able to a non existing user get list of all users 

 ##### TurnUserAdminUseCase
    ✓ should be able to turn an user as admin 
    ✓ should not be able to turn a non existing user as admin 

 ##### CreateUserUseCase
    ✓ should be able to create new users 
    ✓ should not be able to create new users when email is already taken 

 ##### ShowUserProfileUseCase
    ✓ should be able to get user profile by ID 
    ✓ should not be able to show profile of a non existing user 

### Testes das rotas
 ##### [POST] /users
    ✓ should be able to create new users 
    ✓ should not be able to create new users when email is already taken 
 ##### [PATCH] /users/:user_id/admin
    ✓ should be able to turn an user as admin 
    ✓ should not be able to turn a non existing user as admin 
 ##### [GET] /users/:user_id
    ✓ should be able to get user profile by ID 
    ✓ should not be able to show profile of a non existing user 
 ##### [GET] /users
    ✓ should be able to list all users 
    ✓ should not be able to a non admin user get list of all users 
    ✓ should not be able to a non admin user get list of all users 
    ✓ should not be able to a non existing user get list of all users

## Executar

- Para testar esta API basta fazer o clone do repositório `git clone`
- Executar o comando `yarn` para instalar todas as dependências
- E depois `yarn dev` para iniciar o servidor

![Página do Swagger com as rotas da aplicação](/assets/swagger.png)

## Documentação

- Para acessar a documentação basta executar o comando `yarn dev`
- E acessar o endereço `http://localhost:3333/api-docs`

## Créditos

🚀 **[Rocketseat](https://www.rocketseat.com.br)**