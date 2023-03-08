# App

GymPass style app.

## RFs (Requisitos funcionais)

- O usuário pode fazer cheking.

  - O requisito funcional é a funcionalidade em se, o que o usuário vai poder fazer dentro da nossa aplicação.

  - [ ] Deve ser possível se cadastrar;
  - [ ] Deve ser possível se autenticar;
  - [ ] Deve ser possível obter o perfil de um usuário logado;
  - [ ] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
  - [ ] Deve ser possível o usuário obter seu histórico de check-ins;
  - [ ] Deve ser possível o usuário buscar academias próximas;
  - [ ] Deve ser possível o usuário buscar academias pelo nome;
  - [ ] Deve ser possível o usuário realizar check-in em uma academia;
  - [ ] Deve ser possível validar o check-in de um usuário;
  - [ ] Deve ser possível cadastrar uma academia;

## RNs (Regras de negócios)

- O usuário só pode fazer cheking se estiver a menos de 10km da localização da academia.

  - Determina quando é, ao que condições que são necessárias para aplicar cada regra de negócio. A regra de negócio sempre vai esta associada ao requisito funcional, ao seja, nunca vai haver uma regra de negócio que não esteja ligada ao um requisito funcional.

  - [ ] O usuário não deve poder se cadastrar com um e-mail duplicado;
  - [ ] O usuário não pode fazer 2 check-ins no mesmo dia;
  - [ ] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
  - [ ] O check-in só pode ser validado até 20 minutos após ser criado;
  - [ ] O check-in só pode ser validado por administradores;
  - [ ] A academia só pode ser cadastrada por administradores;

## RNFs (Requisitos não-funcionais)

- São aqueles requisitos que não partem do cliente, ao seja, o cliente não vai ter controle sobre os requisitos não funcionais.
São requisitos muito mas técnico do que a nível de funcionalidades.

  - Qual banco de dados que vou utilizar, qual a estratégia que vou utilizar, se tem cache, se tem paginação, etc.
  - Coisas que só o desenvolvedor vai intender.

  - [ ] A senha do usuário precisa estar criptografada;
  - [ ] Os dados da aplicação precisam estar persistidos em um banco PostgreSQL;
  - [ ] Todas listas de dados precisam estar paginadas com 20 itens por página;
  - [ ] O usuário deve ser identificado por um JWT (JSON Web Token);