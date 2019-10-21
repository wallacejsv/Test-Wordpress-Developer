# Test-WordPress-Developer
Teste Desenvolvedor WordPress - SETTA

Com esse desafio iremos testar sua capacidade em resolver problemas com WordPress.

# Siga os passos a seguir

- Utulize o plugin ACF ( Advanced Custom Fields )

# LEIA: 
Iremos criar um sistema real que disponibiliza trilhas para os usuários.
Cada trilha terá módulos. Nos módulos terão atividades.
Essas atividades podem ser, textos, fotos, video e galerias. Fique a vontade e use a criatividade.

# IMPORTANTE:
Ao clicar no módulo dentro da trilha, terá que abrir um modal ( pode ser do bootstrap ). O modal conterá todas as atividades preenchidas no módulo clicado. Utilize Ajax para buscar as atividades do módulo e listar dentro do modal.
Dentro do modal crie os botoes Anterior e Proximo. Faça a paginação de atividade para atividade, também utilizando Ajax.

### Vamos começar!

1 - Crie os seguintes CPT's ( Custom post type ) com os campos personalizados abaixo:
  - CPT Atividades
    - Campos personalizados: 
      - Subtítulo Atividade 
      - Galeria do plugin ACF ( Advanced Custom Fields )
  - CPT Módulos
    - Campos personalizados: 
      - Atividades ( Utilizar o ACF para pegar os posts do CPT Atividades criado anteriormente. Pode selecionar mais de uma atividade. )
      - Imagem Destaque (url da imagem)
      - Tempo do módulo (string)
  - CPT Trilhas
     - Campos personalizados: 
      - Módulos ( Utilizar o ACF para pegar os posts do CPT Módulos. Pode selecionar mais de um módulo. )
      - Categoria Trilha ( Categoria Default de Posts - Alma, Mente, Prazer, Profissional, Relações, Saúde )
      - Nome Creator ( string )
      
2 - Preencha no mínimo 5 atividades no CPT atividade
3 - Preencha no mínimo 5 módulos no CPT Modulos. Lembre-se que dentro do CPT módulo você precisará selecionar algumas atividades.
4 - Crie uma trilha e selecione no minimo 5 modulos nela.
      
5 - Com todos os CPT's e ACF's criados, cria o single do CPT trilhas
  - /trilhas/post-trilha-exemplo
  - Dentro de cada single trilha, você terá que listar os módulos relacionados nessa trilha em forma de card. Layout abaixo:
  
  ![image](https://user-images.githubusercontent.com/6198834/67249685-e645e200-f43e-11e9-88a5-43cd9b7116a2.png)
  
  - Liste pelo menos 5 Módulos usando display flex no css
