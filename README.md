# Python-animais
class AnimalEstimacao:
    def _init_(self):
        self.nome = ""
        self.raca = ""
        self.idade = ""
        self.nome_responsavel = ""
        self.telefone_responsavel = ""

    def cadastrar_animal(self):
        self.nome = input("Digite o nome do animal: ")
        self.raca = input("Digite a raça do animal: ")
        self.idade = input("Digite a idade do animal: ")
        self.nome_responsavel = input("Digite o nome do responsável: ")
        self.telefone_responsavel = input("Digite o telefone do responsável: ")

    def retornar_cadastro(self):
        return f"Nome: {self.nome}\nRaça: {self.raca}\nIdade: {self.idade}\nResponsável: {self.nome_responsavel}\nTelefone: {self.telefone_responsavel}"

# Exemplo de uso:
animal = AnimalEstimacao()
animal.cadastrar_animal()
cadastro = animal.retornar_cadastro()
print("\nCadastro do animal de estimação:")
print(cadastro)
