nome_aluno = input("Digite o nome do aluno: ")
codigo_disc = input("Digite o código da disciplina: ")
print("Digite as notas (entre 0 e 10)")


p1 = float(input("P1: "))
while p1 < 0 or p1 > 10:
    print("Nota inválida! Digite um valor entre 0 e 10.")
    p1 = float(input("P1: ")) 


p2 = float(input("P2: "))
while p2 < 0 or p2 > 10:
    print("Nota inválida! Digite um valor entre 0 e 10.")
    p2 = float(input("P2: "))


pd = float(input("PD: "))
while pd < 0 or pd > 10:
    print("Nota inválida! Digite um valor entre 0 e 10.")
    pd = float(input("PD: "))


pp1 = float(input("Pp1: "))
while pp1 < 0 or pp1 > 10:
    print("Nota inválida! Digite um valor entre 0 e 10.")
    pp1 = float(input("Pp1: ")) 


pp2 = float(input("Pp2: "))
while pp2 < 0 or pp2 > 10:
    print("Nota inválida! Digite um valor entre 0 e 10.")
    pp2 = float(input("Pp2: "))


pp3 = float(input("Pp3: "))
while pp3 < 0 or pp3 > 10:
    print("Nota inválida! Digite um valor entre 0 e 10.")
    pp3 = float(input("Pp3: "))


media = (p1 + p2 + pd + pp1 + pp2 + pp3) / 6


print("\n--- RESULTADO ---")
print("Aluno: ", nome_aluno)
print("Disciplina: ", codigo_disc)
print("Média Final: ", round(media, 2))

if media >= 6.0:
    print("Situação: Aluno Aprovado")
elif media >= 4.0:
    print("Situação: Aluno em Recuperação")
else: 
    print("Situação: Aluno Reprovado")
