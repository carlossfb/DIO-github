# DIO-github
Bootcamp GFT Java #5 - projeto GIT (inicializando repositório e configurações)

## Aqui vai um pequeno Tutorial:

Criação de chave SSH para acesso facilitado as alterações do GitHub sem necessitar de autenticação via navegador: <br>
- **Primeiro passo** - Abra o GitBash e digite o seguinte código: 
~~~ 
ssh-keygen -t ed25519 -C seuemail@gmail.com; 
~~~
- **Segundo passo** - Serão geradas duas chaves em um local especificado no seu bash *id_ed25519 e id_ed25519.pub*, navegue até lá e abra a chave pública (.pub) usando 
~~~
cat id_ed25519.pub
~~~
Assim irá conseguir visualizar o conteúdo e copiar para seu GitHub na opção settings do seu perfil; <br><br>

- **Terceiro passo** - Agora só confirmar que seu bash continua na pasta .ssh e inicializar o agente que administrará suas chaves usando o cod: 
~~~
eval $(ssh-agent -) id_ed25519
~~~
- **Finalizando** - Execute no mesmo bash o cod 
~~~
ssh-add *id_ed25519*
~~~

### Preparando para versionar com Git

1. Git init -> Inicializar um repositório local // em caso de o repositório já ter sido criado -> **Git remote add origin "link do repositório"**
2. Git add * -> Setar todos os arquivos do diretório para serem visiveis ao git para commit
3. Git status -> verificar estado dos arquivos e se estão OK para envio
4. Git commit -m "mensagem" -> identificação do commit
5. git push origin master -> concretizando envio

### Clonando repositório para trabalhar de forma local
1. git clone "link do repositório" -> só autenticar e seguir os mesmos processos para atualizar os arquivos


*PS: Typora pode ser uma boa opção para anotações em arquivos md*
