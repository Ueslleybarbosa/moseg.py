# Intuito do Código

O código fornecido implementa uma interface de terminal em Python usando a biblioteca `curses` para demonstrar os modelos de segurança Bell-LaPadula e Biba. Esses modelos são usados para controlar o acesso a informações sensíveis em sistemas de segurança.

## Modelos de Segurança

### Bell-LaPadula

O modelo Bell-LaPadula é focado na **confidencialidade** das informações. Ele define duas regras principais:
1. **Regra de Leitura (No Read Up):** Um usuário só pode ler informações de um nível igual ou inferior ao seu.
2. **Regra de Escrita (No Write Down):** Um usuário só pode escrever informações de um nível igual ou superior ao seu.

### Biba

O modelo Biba é focado na **integridade** das informações. Ele define duas regras principais:
1. **Regra de Leitura (No Read Down):** Um usuário só pode ler informações de um nível igual ou superior ao seu.
2. **Regra de Escrita (No Write Up):** Um usuário só pode escrever informações de um nível igual ou inferior ao seu.

## Funcionamento do Código

O código cria uma interface de terminal interativa que permite aos usuários escolher um usuário, um recurso e uma ação (leitura ou escrita). Com base nessas escolhas, o programa verifica se a ação é permitida de acordo com os modelos de segurança Bell-LaPadula e Biba.

### Passos do Programa

1. **Inicialização da Interface:**
   - O programa inicializa a interface de terminal usando a biblioteca `curses` e define algumas cores para a interface.

2. **Descrição dos Modelos de Segurança:**
   - O programa exibe uma descrição dos modelos de segurança Bell-LaPadula e Biba e espera que o usuário pressione uma tecla para continuar.

3. **Escolha do Usuário:**
   - O usuário pode escolher entre Alice (Diretor), Bob (RH) e Charlie (Funcionário) usando as setas para cima/baixo e pressionando Enter.

4. **Escolha do Recurso:**
   - O usuário pode escolher entre Funcionario, RH e Diretor.

5. **Escolha da Ação:**
   - O usuário pode escolher entre Leitura e Escrita.

6. **Verificação de Permissões:**
   - O programa verifica se a ação é permitida de acordo com os modelos de segurança e exibe o resultado na tela.

7. **Informações Adicionais:**
   - O programa exibe informações adicionais sobre os modelos de segurança Bell-LaPadula e Biba.

## Conclusão

Este código é uma ferramenta educacional que permite aos usuários aprender sobre os modelos de segurança Bell-LaPadula e Biba de forma interativa. Ele demonstra como esses modelos podem ser usados para controlar o acesso a informações sensíveis em um sistema de segurança.
