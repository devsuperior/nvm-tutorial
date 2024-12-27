# Instalar NodeJS com NVM

## Introdução

A melhor forma de gerenciar instalações do NodeJS em seu sistema é por meio do NVM no terminal Linux ou Mac. 

Se você usa Windows, instale o Ubuntu com WLS para usar o terminal Linux integrado com seu Windows. Aqui está o passo a passo: https://learn.microsoft.com/pt-br/windows/wsl/install

## Explicação sobre as versões do NodeJS

Você sempre deve usar em seus projetos versões LTS (Long Term Support).

As versões do NodeJS são organizadas em *version branches* (ramos de versões). Cada *version branch* possui um Codenome e uma última versão LTS estável. 

Alguns exemplos:
- O *version branch* das versões 18.x.x tem o codnome `Hydrogen`, e na data em que eu faço este tutorial, a última versão LTS estável é a v18.20.5.
- O *version branch* das versões 22.x.x tem o codnome `Jod`, e na data em que eu faço este tutorial, a última versão LTS estável é a v22.12.0.

As versões do NodeJS podem ser consultadas em: https://nodejs.org/en/about/previous-releases

## Instalar o NVM no Ubuntu
```
sudo apt-get update
```

```
sudo apt install curl
```

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

Após os passos, **reinicie o terminal**.

## Comandos importantes do NVM

### Listar versões disponíveis e conferir qual está em uso
```
nvm ls
```

### Instalar uma versão

**Exemplo: instalar última versão LTS de um version branch usando o Codenome**
```
nvm install Jod
```

**Exemplo: instalar versão usando número exato**
```
nvm install v22.12.0
```

### Usar uma versão do NodeJS
```
nvm use v22.12.0
```

### Desinstalar uma versão
```
nvm uninstall v22.12.0
```

