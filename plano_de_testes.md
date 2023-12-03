# Roteiro de Testes

Aplicação: Uninventário

Versão: 1.0

Data: 12-11-2023

Autor: Luisa Franco


## Cenário 1: Cadastrar uma nova máquina

### Dado que
o usuário está na página de cadastro de máquinas

### E
o usuário preenche os campos obrigatórios
- nome: "Máquina 1"
- modelo: "Dell Latitude E6540"
- processador: "Intel Core i5-5200U"
- memória RAM: "8 GB"
- armazenamento: "500 GB"
- laboratório: "Laboratório 20"

### Quando
o usuário clica no botão "Salvar"

### Então
a máquina deve ser cadastrada com sucesso


## Cenário 2: Alterar os dados de uma máquina

### Dado que
o usuário está na página de detalhes de uma máquina

### E
a máquina está cadastrada com os seguintes dados
- nome: "Máquina 1"
- modelo: "Dell Latitude E6540"
- processador: "Intel Core i5-5200U"
- memória RAM: "8 GB"
- armazenamento: "500 GB"
- laboratório: "Laboratório 20"

### E
o usuário altera os seguintes dados da máquina
- nome: "Máquina 2"
- modelo: "Dell Latitude E7440"
- processador: "Intel Core i7-5500U"
- memória RAM: "16 GB"
- armazenamento: "1 TB"
- laboratório: "Laboratório 45"

### Quando
o usuário clica no botão "Salvar alterações"

### Então
os dados da máquina devem ser alterados com sucesso

### E
os dados da máquina devem ser os seguintes
- nome: "Máquina 2"
- modelo: "Dell Latitude E7440"
- processador: "Intel Core i7-5500U"
- memória RAM: "16 GB"
- armazenamento: "1 TB"
- laboratório: "Laboratório 45"


## Cenário 3: Excluir uma máquina

### Dado que
o usuário está na página de detalhes de uma máquina

### E
a máquina está cadastrada com os seguintes dados
- nome: "Máquina 2"
- modelo: "Dell Latitude E7440"
- processador: "Intel Core i7-5500U"
- memória RAM: "16 GB"
- armazenamento: "1 TB"
- laboratório: "Laboratório 45"

### Quando
o usuário clica no botão "Excluir"

### Então
a máquina deve ser excluída com sucesso

### E
a máquina não deve mais ser exibida na lista de máquinas

