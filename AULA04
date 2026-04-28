Faça uma função para validar senha forte.

def senha_forte(senha):
    return len(senha) > 8

Problemas:

Critério extremamente simplista
Não define o que é “forte”
Não considera segurança real
Não documentado
Não reutilizável

Faça um código que seja uma calculadora.

PROMPT: Você é um desenvolvedor Python experiente em segurança.
Estou criando um sistema de cadastro de usuários e preciso validar senhas fortes.
A função deve:

Ter pelo menos 8 caracteres
Conter maiúscula, minúscula, número e símbolo
Ser clara e reutilizável
Retorne o código e uma breve explicação.

import re

def validar_senha(senha):
    if len(senha) < 8:
        return False
    if not re.search(r"[A-Z]", senha):
        return False
    if not re.search(r"[a-z]", senha):
        return False
    if not re.search(r"[0-9]", senha):
        return False
    if not re.search(r"[!@#$%^&*]", senha):
        return False
    return True

