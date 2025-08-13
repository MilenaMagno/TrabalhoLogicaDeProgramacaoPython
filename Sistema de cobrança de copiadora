print('Bem-vindo à copiadora da Milena Magno.')
def escolha_servico ():
    #Pergunta o servico desejado e retorna o valor por página

    DIG = 1.10
    ICO = 1.00
    IPB = 0.40
    FOT = 0.20
    while True:
        serv = input('Qual o servico desejado?\n'
                     'DIG - Digitacão\n'
                     'ICO - Impressão colorida\n'
                     'IPB - Impressão preto e branco\n'
                     'FOT - Fotocópia\n'
                     '>>')
        if serv == 'DIG':
            return DIG
        elif serv == 'ICO':
            return ICO
        elif serv == 'IPB':
            return IPB
        elif serv == 'FOT':
            return FOT
        else:
             print('Servico inválido. Tente novamente...')
             continue


def num_pagina ():
    #Pergunta o número de páginas e retorna o resultado já com desconto aplicado
    while True:
        try:
            pag = int(input('Por favor, digite o número de páginas: '))
            if pag >= 20000:
                print('Não aceitamos esse número de páginas de uma vez. Tente novamente...')
                continue
            elif pag >= 2000:
                return pag * 0.75
            elif pag >= 200:
                return pag * 0.80
            elif pag >= 20:
                return pag * 0.85
            else:
                return pag
        except ValueError:
            print('Oops! Número inválido. Tente novamente... ')
        except:
            print('Oops! Ocorreu um erro. Tente novamente...')



def servico_extra ():
    #Pergunta se quer adicional e retorna o valor de um adicional apenas
    adicional = int(input('Deseja adicionar algum servico extra?\n'
                          '1 - Encadernacão simples - R$ 15\n'
                          '2 - Encadernacão de capa dura - R$ 40\n'
                          '0 - Não desejo mais nada\n'
                          '>>'))
    x = 15
    y = 40
    z = 0
    while True:
        if adicional == 1:
            return x
        elif adicional == 2:
            return y
        elif adicional == 0:
            return z
        else:
            print('Opcao inválida. Tente novamente...')
            continue
#Programa principal
servico = escolha_servico()
n_pagina = num_pagina()
extra = servico_extra()
#Calcular servicos e valores e imprimir na tela
total = servico * n_pagina + extra
print(f'Total: R$ {total:.2f} (servico: {servico:.2f} X paginas: {n_pagina} + {extra:.2f}).') 
