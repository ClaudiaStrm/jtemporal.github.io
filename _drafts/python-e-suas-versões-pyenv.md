---
title: 'Python and it''s versions: pyenv'
layout: post
date: 2017-12-29 10:00:00
img: "/pro_tip.png"
tags:
- english
- versions
- protip
- python
- pyenv
comments: true
subtitle: Learn how to install manage Python versions using pyenv

---
Uma das primeiras coisas que aprendemos sobre [Python](https://www.python.org/) é que existem mais de uma versão da mesma linguagem funcionando a todo vapor. Isso traz alguns problemas e a inevitável pergunta _"Qual versão eu devo usar?"_. A colinha de hoje mostra uma forma de instalar e manter o controle de várias versões do Python na sua máquina usando o [pyenv](https://github.com/pyenv/pyenv) 😉.

Entre outras coisas, as duas melhores features _pyenv_ na minha humilde opinião são:

1. instalar novas versões do Python facilmente;
2. escolher a versão global do Python.

![sombrancelhas gif](https://media.giphy.com/media/10lqVdCCc9812M/giphy.gif)

Pra começar você precisa instalar o pyenv, aqui eu vou mostrar um dos métodos de instalação, mas [lá no _readme_ do projeto tem outras](https://github.com/pyenv/pyenv#installation) (e também detalhes específicos de cada sistema operacional):

``` console
$ git clone https://github.com/pyenv/pyenv.git ~/.pyenv
$ echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
$ echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
$ exec "$SHELL"
```

Depois desse passo é bem facinho, as outras versões do Python estão a um _install_ de distância:

``` console
$ pyenv install 3.6.4
```

Se estiver em dúvida quais versões você pode instalar só usar a flag `-l` do _install_ que ele vai listar todas as disponíveis:

``` console
$ pyenv install -l
```

Massa né? Agora é só sair instalando versão adoidado 😂

***

Links

* [Você pode continuar a ler sobre o pyenv na Parte 2 desse texto](https://jtemporal.com/pyenv-parte2/).