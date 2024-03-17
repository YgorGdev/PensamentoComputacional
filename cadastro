class Pessoa:
    def __init__(self, nome, cpf, telefone, endereco):
        self.nome = nome
        self.cpf = cpf
        self.telefone = telefone
        self.endereco = endereco

class Paciente(Pessoa):
    def __init__(self, nome, cpf, telefone, endereco):
        super().__init__(nome, cpf, telefone, endereco)

class Psicologo(Pessoa):
    def __init__(self, nome, crp, telefone, endereco):
        super().__init__(nome, crp, telefone, endereco)

def cadastrar_paciente():
    nome = input("Digite o nome do paciente: ")
    cpf = input("Digite o CPF do paciente: ")
    telefone = input("Digite o telefone do paciente: ")
    endereco = input("Digite o endereço do paciente: ")
    paciente = Paciente(nome, cpf, telefone, endereco)
    print("Paciente cadastrado com sucesso!")
    return paciente

def cadastrar_psicologo():
    nome = input("Digite o nome do psicólogo: ")
    crp = input("Digite o CRP do psicólogo: ")
    telefone = input("Digite o telefone do psicólogo: ")
    endereco = input("Digite o endereço do psicólogo: ")
    psicologo = Psicologo(nome, crp, telefone, endereco)
    print("Psicólogo cadastrado com sucesso!")
    return psicologo

def menu_principal():
    print("\n=== Menu ===")
    print("1. Cadastrar Paciente")
    print("2. Cadastrar Psicólogo")
    print("3. Sair")
    opcao = input("Escolha uma opção: ")

    if opcao == "1":
        paciente = cadastrar_paciente()
        menu_principal()
    elif opcao == "2":
        psicologo = cadastrar_psicologo()
        menu_principal()
    elif opcao == "3":
        print("Saindo...")
    else:
        print("Opção inválida! Tente novamente.")
        menu_principal()

menu_principal()
