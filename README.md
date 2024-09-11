# Sistema de Gerenciamento de Reservas de Hotel

Este projeto é um sistema de gerenciamento de reservas de hotel que permite gerenciar hóspedes, quartos e reservas. O sistema foi desenvolvido para facilitar o controle e a organização das informações relacionadas às reservas de um hotel.

## Estrutura do Banco de Dados

O banco de dados é composto pelas seguintes tabelas:

### Tabela Hospedes
Armazena informações sobre os hóspedes.
- **id_hospede** (INT, PK): Identificador único do hóspede.
- **nome** (VARCHAR): Nome do hóspede.
- **telefone** (VARCHAR): Telefone de contato do hóspede.
- **email** (VARCHAR): Endereço de e-mail do hóspede.

### Tabela Quartos
Armazena informações sobre os quartos disponíveis no hotel.
- **id_quarto** (INT, PK): Identificador único do quarto.
- **numero** (INT): Número do quarto.
- **tipo** (VARCHAR): Tipo de quarto (e.g., Individual, Duplo, Suíte).
- **preco** (DECIMAL): Preço por noite do quarto.

### Tabela Reservas
Armazena informações sobre as reservas feitas pelos hóspedes.
- **id_reserva** (INT, PK): Identificador único da reserva.
- **id_hospede** (INT, FK): Identificador do hóspede (referência à tabela Hospedes).
- **id_quarto** (INT, FK): Identificador do quarto (referência à tabela Quartos).
- **data_checkin** (DATE): Data de check-in.
- **data_checkout** (DATE): Data de check-out.

## Instruções de Uso

1. **Configuração do Banco de Dados**
   - Execute os comandos SQL fornecidos para criar as tabelas no seu banco de dados.

2. **Inserir Dados**
   - Use os comandos SQL fornecidos para inserir dados nas tabelas.

3. **Consultar Dados**
   - Realize consultas SQL para obter informações sobre hóspedes, quartos e reservas.

4. **Atualizar Dados**
   - Use comandos SQL para atualizar informações de hóspedes e quartos.

5. **Excluir Dados**
   - Utilize comandos SQL para excluir reservas e hóspedes.

## Contribuição

Se você deseja contribuir para o projeto, por favor, faça um fork do repositório e envie um pull request com suas alterações.

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
