from PIL import Image
import requests
import matplotlib.pyplot as plt
from io import BytesIO
import time


def exb_img(url):
    dados = requests.get(url)
    imagem = Image.open(BytesIO(dados.content))
    plt.axis("off")
    plt.imshow(imagem)
    plt.show()

def negrito(texto):
    return "f\033[1m{texto}\033[0m"


xp = 0
chegou_no_castelo = False
falou_cm_rei = False
falou_cm_elara = False


def introducao():
    global chegou_no_castelo, falou_cm_rei, falou_cm_elara


    print(negrito("Você está caminhando até o Castelo."))
    time.sleep(1.5)

    exb_img("https://i.pinimg.com/1200x/6c/11/79/6c1179bb23a1860a4094a560a51dac41.jpg")
    time.sleep(3)

    print(negrito("""Após você chegar na frente do Castelo, um
guarda vai falar com você. """))
    time.sleep(2)

    print("Guarda do Castelo: Quem é você?")
    nome = input()

    print(f"""Guarda do Castelo: Ah, você é o {nome}, não é? Venha,
 o Rei está esperando por você.""")
    time.sleep(2)

    print(negrito("O Guarda leva você até a Pré-Entrada e diz:"))
    time.sleep(1.5)

    print("Guarda do Castelo: Você deve ir para a esquerda, seguir em frente e suba as escadas.")
    time.sleep(2)

    print("Guarda do Castelo: O Rei estará lá à sua espera. Vá.")
    time.sleep(2)

    print(negrito("O Guarda já foi embora, siga seu caminho:"))
    time.sleep(1.5)

    exb_img("https://i.pinimg.com/736x/b0/d6/9a/b0d69a6bd5fd78d12f662b0d053f2204.jpg")
    time.sleep(1.5)

    resposta1 = int(input("1: Seguir em Frente\n2: Ir para a Direta\n3: Ir para a Esquerda"))
    if resposta1 == 1:
        chegou_no_castelo = True
        print(negrito("Você caminha e encontra um campo, junto de outras casas."))
        time.sleep(1.5)

        exb_img("https://i.pinimg.com/736x/2e/c2/a0/2ec2a0b1392368efb5c9db3497f8101b.jpg")
        time.sleep(3)

        resposta1_1 = int(input("1: {negrito("Voltar")}\n2: Continuar"))
        if resposta1_1 == 2:
            print(negrito("""Você continua caminhando até as casas
e escuta alguns barulhos."""))
            time.sleep(1.5)

            exb_img("https://i.pinimg.com/736x/07/45/8b/07458bb305f7896a565038a9ce40663c.jpg")
            time.sleep(3)

            print(negrito("Pelo visto está tendo uma festa."))
            time.sleep(2)

            exb_img("https://i.pinimg.com/736x/2f/26/e7/2f26e7a8f46a71639c578e2cd3a5fac1.jpg")
            time.sleep(3)

            print("")
