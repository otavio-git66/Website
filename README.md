# Sabor da Casa

> Site institucional de um restaurante brasileiro que combina comida afetiva, identidade visual acolhedora e uma experiência simples de navegação.

## Sobre o projeto

O **Sabor da Casa** é uma página web criada para representar um restaurante de bairro com uma presença digital elegante, clara e acessível. O projeto apresenta a essência do estabelecimento logo na primeira tela: uma proposta de cozinha brasileira feita com afeto, um prato em destaque e um convite direto para conhecer o menu ou reservar uma mesa.

A interface foi desenvolvida sem frameworks ou dependências de JavaScript, priorizando uma estrutura leve, fácil de entender e simples de manter. A combinação entre verde profundo, terracota, fundo claro e tipografia editorial reforça a sensação de acolhimento e proximidade associada ao restaurante.

## Objetivos

- Criar uma apresentação profissional para um restaurante fictício;
- Destacar a identidade, a proposta e os pratos da casa;
- Facilitar o acesso às informações de contato e reserva;
- Oferecer uma experiência agradável em computadores e dispositivos móveis;
- Manter o código organizado para facilitar futuras alterações.

## Principais recursos

### Apresentação do restaurante

A seção inicial apresenta o nome do restaurante, sua proposta de valor, uma imagem de prato e o horário de funcionamento. Os botões conduzem o visitante ao menu ou ao telefone de reserva.

### História e posicionamento

A seção “Nossa história” explica a relação do restaurante com receitas brasileiras, ingredientes da estação e experiências compartilhadas à mesa.

### Menu em destaque

Os pratos favoritos da casa são apresentados em cartões com:

- Fotografia do prato;
- Nome e descrição dos ingredientes;
- Preço em destaque;
- Imagens carregadas de forma otimizada com `loading="lazy"`.

### Contato e reservas

A área de contato reúne telefone, e-mail e endereço. Os links de telefone e e-mail são interativos, permitindo iniciar uma chamada ou abrir o aplicativo de mensagens do dispositivo.

### Responsividade

O layout se adapta a diferentes larguras de tela. Em dispositivos menores, a navegação é simplificada, os pratos passam para uma única coluna e os elementos da área de reserva são reorganizados para melhorar a leitura.

## Direção visual

O projeto utiliza uma identidade visual baseada em três ideias principais:

- **Acolhimento:** fundo claro, espaços generosos e textos próximos do visitante;
- **Naturalidade:** verde profundo e imagens de alimentos frescos;
- **Personalidade:** terracota para chamadas, preços e detalhes importantes.

As fontes utilizadas são `Playfair Display`, para títulos com caráter editorial, e `DM Sans`, para textos corridos e elementos de navegação. As imagens dos pratos são provenientes do Unsplash e podem ser substituídas por fotografias próprias do restaurante.

## Tecnologias utilizadas

- **HTML5:** estrutura semântica da página;
- **CSS3:** layout, cores, tipografia, animações de interação e responsividade;
- **CSS Grid e Flexbox:** organização das seções e dos cartões de pratos;
- **Google Fonts:** carregamento das famílias tipográficas;
- **Unsplash:** imagens ilustrativas dos pratos.

## Estrutura de arquivos

```text
.
├── index.html   # Estrutura, conteúdo e links da página
├── style.css    # Identidade visual, layout e regras responsivas
└── README.md    # Documentação do projeto
```

## Como executar

O site é estático e pode ser executado em qualquer computador com um navegador moderno. Não é necessário instalar banco de dados, Node.js ou outras dependências.

### Forma recomendada: Visual Studio Code e Live Server

O servidor local é a melhor opção para desenvolver e testar o projeto, pois simula o acesso de um site real e atualiza a página automaticamente após cada alteração.

1. Instale o [Visual Studio Code](https://code.visualstudio.com/) caso ainda não o tenha.
2. Abra o Visual Studio Code.
3. Acesse **File > Open Folder** e selecione a pasta do projeto.
4. Abra a aba **Extensions** usando `Ctrl + Shift + X`.
5. Pesquise por **Live Server**, escolha a extensão publicada por **Ritwick Dey** e clique em **Install**.
6. No explorador de arquivos do VS Code, clique com o botão direito em `index.html`.
7. Selecione **Open with Live Server**.
8. O navegador abrirá automaticamente um endereço semelhante a:

```text
http://127.0.0.1:5500/index.html
```

Depois disso, mantenha o Live Server aberto enquanto estiver editando. Ao salvar `index.html` ou `style.css` com `Ctrl + S`, atualize o navegador para visualizar as mudanças.

### Alternativa: abrir o arquivo diretamente

Para apenas visualizar o resultado, sem editar:

1. Abra a pasta do projeto no Explorador de Arquivos do Windows.
2. Clique duas vezes em `index.html`.
3. Escolha um navegador, como Google Chrome, Microsoft Edge ou Firefox.

O endereço aparecerá no formato `file:///.../index.html`. Essa opção funciona para este projeto, mas o Live Server é mais adequado durante o desenvolvimento.

### Alternativa: servidor local pelo PowerShell

Caso o Python esteja instalado no computador, também é possível iniciar um servidor sem instalar uma extensão:

1. Abra a pasta do projeto no Explorador de Arquivos.
2. Clique na barra de endereço, digite `powershell` e pressione `Enter`.
3. Execute:

```powershell
python -m http.server 8000
```

4. Abra no navegador o endereço:

```text
http://localhost:8000
```

5. Para encerrar o servidor, volte ao PowerShell e pressione `Ctrl + C`.

### Requisitos para o visual completo

As imagens dos pratos são carregadas do Unsplash e as fontes são carregadas do Google Fonts. Por isso, mantenha o computador conectado à internet para que todos os elementos visuais apareçam corretamente. Sem conexão, a estrutura e os estilos locais continuarão funcionando, mas as imagens e fontes externas poderão não carregar.

### Problemas comuns

- **A página aparece sem estilo:** confirme se `style.css` está na mesma pasta que `index.html`.
- **As imagens não aparecem:** verifique a conexão com a internet e recarregue a página com `Ctrl + F5`.
- **O Live Server não abre:** confirme se a extensão está instalada e se o arquivo aberto é exatamente `index.html`.
- **A porta já está em uso:** escolha outra porta no Live Server ou execute o comando Python com outro número, como `python -m http.server 8080`.

## Como personalizar

### Conteúdo

Edite o arquivo `index.html` para alterar:

- Nome e logotipo do restaurante;
- Textos de apresentação e história;
- Nome, descrição, foto e preço dos pratos;
- Telefone, e-mail e endereço;
- Horários de funcionamento;
- Links das redes sociais.

### Aparência

Edite o arquivo `style.css` para modificar:

- Cores principais, disponíveis nas variáveis dentro de `:root`;
- Tipografia e tamanhos de títulos;
- Espaçamentos entre seções;
- Bordas, sombras e formatos das imagens;
- Comportamento da página em telas menores.

### Imagens

Para trocar uma imagem, substitua o valor do atributo `src` e atualize o texto alternativo do atributo `alt`. O texto alternativo deve descrever a imagem para que o conteúdo continue compreensível para pessoas que utilizam leitores de tela.

## Acessibilidade e boas práticas

O projeto utiliza elementos semânticos como `header`, `nav`, `main`, `section`, `article` e `footer`, além de:

- Textos alternativos nas imagens;
- Rótulo descritivo na navegação principal;
- Hierarquia de títulos organizada;
- Links de contato acionáveis;
- Contraste visual entre textos e fundos;
- Layout utilizável em telas pequenas.

Em uma versão de produção, ainda seria recomendável validar o contraste com uma ferramenta específica, adicionar uma página ou modal real de reservas e hospedar as imagens em um serviço próprio para obter maior controle sobre desempenho e disponibilidade.

## Próximas evoluções

O projeto pode ser ampliado com:

- Menu completo dividido por categorias;
- Formulário de reserva com validação;
- Integração com WhatsApp ou sistema de reservas;
- Galeria de fotos do ambiente;
- Página de localização com mapa;
- Versões em outros idiomas;
- Área administrativa para atualizar pratos e preços;
- Otimização das imagens em formatos modernos, como WebP ou AVIF.

## Licença e créditos

Este projeto foi criado para fins educacionais e demonstrativos. O conteúdo textual e a identidade do restaurante são fictícios. As imagens e fontes externas seguem as condições de uso de seus respectivos serviços.

