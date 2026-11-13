# SyntropicMind V19 integrada

Extraia o ZIP inteiro e abra `SyntropicMind_V19_atualizado.html` no navegador. `index.html` contém a mesma página e é o arquivo inicial para hospedagem. As pastas `ensaios`, `angiosim`, `assets` e `downloads` precisam acompanhar a página para que todos os acessos funcionem.

A página principal preserva a V19: textos, sequência das seções, identidade visual e animações. As únicas atualizações editoriais informam a disponibilidade do AngioSim e dos quatro ensaios, inclusive nas perguntas frequentes e na descrição para buscadores. O cartão do AngioSim agora abre o simulador; o cartão dos ensaios abre a biblioteca.

## Editar os textos diretamente

1. Faça uma cópia de segurança antes de editar.
2. Abra `SyntropicMind_V19_atualizado.html` em um editor de código ou texto simples.
3. Busque uma frase existente e altere apenas o conteúdo entre as tags, preservando elementos como `<p>`, `<h1>` e `<br>`.
4. Salve em UTF-8 e atualize o navegador para conferir o resultado.
5. Se publicar, copie a versão final para `index.html`, mantendo os dois arquivos iguais.

Os textos dos conceitos Atenção, Autonomia e Responsabilidade também estão no bloco `const modes` do JavaScript. Preserve aspas, vírgulas e chaves. Os ensaios ficam em `ensaios/<nome-do-ensaio>/index.html`; a biblioteca fica em `ensaios/index.html`. A coletânea Word é um download separado: editar o HTML não atualiza o Word automaticamente.

## Prévia local verificada

A verificação no navegador integrado utiliza HTTP local. Dentro desta pasta, execute:

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Abra http://127.0.0.1:8765/ no navegador. A abertura direta de arquivos não é permitida pelo navegador integrado de testes; as páginas usam links relativos e não exigem uma aplicação de servidor.

A fonte Manrope e a fotografia do autor dependem de conexão. O AngioSim mantém seus dados e scripts originais, inclusive o requisito de WebGL2 e suas limitações educacionais. O site publicado e os arquivos originais não foram alterados.
