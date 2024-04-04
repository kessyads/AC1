# AC1Grupo de 3 integrantes

Arquivos:

index.html (estático)
paciente.html (estático)
classes.js (classe paciente classe medicamento)
main.js
style.css
===============================
Classe Paciente:
===============================
Propriedades:

- id: int
- nome: String
- medicamentosPrescritos: array<Medicamento>

Construtor:

+ Paciente(id: int, nome: String)

Métodos:

+ get id(): int
+ inserirMedicamentoPrescrito(medicamento: Medicamento)
+ removerMedicamentoPrescritoByCodigo(codigo: int): void
+ getMedicamentoPrescrito(codigo: int): Medicamento
+ imprimir(): String // apenas dados do paciente
+ imprimirCompleto(): String // paciente e medicamentos

===============================
Classe Medicamento:
===============================

Propriedades:

- codigo: int
- nome: String
- tipo: String

Construtor:

+ Medicamento(codigo: int, nome: String, tipo: String)

Métodos:

+ get codigo(): int
+ imprimir(): String // dados do medicamento

===============================
Classe Main:
===============================

Propriedades:

- pacientes: array<Paciente>

Construtor:

+ Main()

Métodos:

+ addPaciente(paciente): void // adiciona paciente no array pacientes
+ addMedicamentoPaciente(idPaciente, codigoMedicamento, nome, tipo): void // adiciona medicamento para paciente específico
+ transferirMedicamento(idPacienteOrigem, idPacienteDestino, codigoMedicamento): void // transfere um medicamento de um paciente para outro
+ mostrarTodosOsPacientes(): void // chama imprimirCompleto de cada paciente

Rodando o Teste:

Main main = new Main();
main.addPaciente(new Paciente(1, "Maria"));
main.addMedicamentoPaciente(1, 1, "Paracetamol", "Analgésico");
main.addMedicamentoPaciente(1, 2, "Amoxicilina", "Antibiótico");
main.mostrarTodosOsPacientes();
main.addPaciente(new Paciente(2, "João"));
main.transferirMedicamento(1, 2, 1);
main.mostrarTodosOsPacientes();
=================================================================
Página Index.html

faz referências aos arquivos JS para rodar no console
ter CSS
A página deve ter:
Cabeçalho
título do Sistema
subtítulo
Menu
"Home" e "Pacientes"
Corpo
Img referente ao Sistema
Descrição do Sistema
Lista de pacientes (2 pacientes) e seus medicamentos (Hardcode)
Rodapé
Página "Paciente.html" (Cadastrar Pacientes)

Cabeçalho
título do Sistema
subtítulo
Menu
"Home" e "Pacientes"
Corpo
formulário com:
data
id
nome
Endereco
Número
Estado
Cidade
Rodapé
====================================================

Notas para funcionalidades rodando com o "Teste":

cadastrar Paciente (1.5)
cadastrar Medicamento para paciente (1.5)
mostrar todos pacientes (1.0)
transferir medicamento (2.0)

index.html (estrurura e visual) 2.0
paciente.html (estrurura, visual e elementos corretos do Form) (2.0)

