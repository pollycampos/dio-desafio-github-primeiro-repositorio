# GIT



## O que é e sua importância

O Git é um sistema que ajuda a criar e monitorar diferentes versões do nosso código, dentro da nossa máquina.

O Git Bash é um terminal extendido para otimizar o uso do Git.

**Benefícios:** Um dos maiores benefícios do uso do git é o controle de versão, pois a partir da criptografia que ele gera podemos saber se houve ou não alteração no arquivo.



## Objetos Fundamentais do Git

- **Blobs - ** são as "bolhas" que contém os metadados do objeto;

- **Tree -** são as "árvores", armazena os blobs e também contém metadados. É ela quem monta toda a estrutura de localização do arquivo. Pode apontar para blobs ou para tree;

- **Commits -** são as unidades estruturais e apontam para autor, mensagem, tree e parente.

  

## Comandos Básicos

:dart: **Alguns comandos são diferentes para linux e windows**

- dir - lista todos os diretórios (no linux o comando é ls);
- cd/ - permite navegar entre as pastas;
- cd .. - retroceder um nível na navegação;
- cls - limpar a tela de navegação (no linux o comando é clear ou o atalho control+l);
- mkdir + nome da pasta - cria pasta;
- echo - cria arquivo;
- del - deletar arquivo;
- rmdir - remove diretório com tudo que tem dentro;
- tecla tab - completa textos já digitados.

:dart: **Os comandos do git sempre iniciam com "git"**

- git status - mostra o status do arquivo;
- git add . - envia todos os arquivos para a "stage";
- git commit -m "descrição da alteração" - commita os arquivos;
- git push origin main - envia o repositório para a nuvem.





# GITHUB

## **O que é e sua importância**

É uma plataforma on line que permite a criação e hospedagem de repositórios. Além disso é possível colaborar com a criação de códigos abertos de software, interagir com outros códigos e seguir outros programadores.

**Benefícios -** além de armazenar os arquivos na nuvem, funciona como uma rede social de programadores permitindo a exposição das suas criações (é a vitrine do seu trabalho), a possibilidade de interação com outros códigos, entre outras. 



## Comandos Básicos



- Criar repositório público: cria novo > adiciona o nome > marca a opção public > adiciona descrição > **se quiser** marca a opção Add README;
- Clonar repositório para Desktop: clica no repositório > code > copia o link > abre o git bash here na pasta que deseja baixar o repositório > digita git clone + link copiado;
- Empurrar arquivo para repositório: git commit -m "incluir descrição da alteração" (para commitar) > git status (para verificar) > git push origin main (para empurrar para o repositório) > git status (para verificar se foi corretamente).

:dart: **Conflitos e como resolvê-los -** Como o github permite alterações nos seus códigos quando eles são públicos, existe a possibilidade de aparecer um conflito quando você tenta empurrar para o repositório um arquivo que estava trabalhando na sua máquina. Isso geralmente acontece quando a alteração feita no repositório e a que você fez na sua máquina ocorreram na mesma linha. Quando você tentar empurrar o arquivo vai aparecer um erro e é necessário resolvê-lo para conseguir empurrar o arquivo para o repositório.

**e como fazer isso?** integrando o arquivo local antes de empurrar para o respositório: git pull origin main (para trazer do repositório o código com alteração) > git status (para verificar o status) > git add * (para enviar os arquivos para a stage) > git commit -m "o que fazer com o conflito" (para commitar resolvendo o conflito) > git push origin master (para enviar o arquivo sem o conflito para o repositório).