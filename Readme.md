# Novo repositório

Aprendendo a usar GIT com tutorial da [Udemy](https://www.udemy.com/git-e-github-para-iniciantes/).

Para usar com o Sublime Text no Windows, é necessário adicioná-lo às variáveis de ambiente, mais informações [neste link](https://scotch.io/tutorials/open-sublime-text-from-the-command-line-using-subl-exe-windows).

Para usar o GIT dentro do Sublime, esse [tutorial ajuda](https://scotch.io/tutorials/using-git-inside-of-sublime-text-to-improve-workflow)

Para adicionar atalho PUSH em tags dentro do sublime, precisa-se adicionar o código abaixo em um novo arquivo com a extensão **.sublime-commands** salvo na pasta `User` dentro de `Preferences > Browse Packages`

```
[
    { 
        "caption": "Git: Push Tags", 
        "command": "git_custom", 
        "args": {
            "cmd": "push origin --tags",
            "output": "panel",
            "async": true
        }
    } 
]
```

Mais informações [aqui](https://sublimegit.readthedocs.io/en/latest//customizations.html) e [aqui](https://github.com/SublimeGit/SublimeGit/issues/68#issuecomment-36945176).