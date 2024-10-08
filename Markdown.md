<p>Claro, aqui estão algumas das tags mais comuns do Markdown:</p><ol><li><strong>Títulos:</strong> <code>#</code> para títulos de diferentes níveis (<code>#</code> para título de nível 1, <code>##</code> para título de nível 2, e assim por diante).</li><li><strong>Negrito:</strong> <code>**texto**</code> ou <code>__texto__</code>.</li><li><strong>Itálico:</strong> <code>*texto*</code> ou <code>_texto_</code>.</li><li><strong>Riscado:</strong> <code>~~texto~~</code>.</li><li><strong>Lista não ordenada:</strong> <code>*</code>, <code>-</code>, ou <code>+</code> no início de uma linha para criar itens de lista.</li><li><strong>Lista ordenada:</strong> Números seguidos por um ponto (ex: <code>1.</code>, <code>2.</code>, etc.).</li><li><strong>Links:</strong> <code>[texto do link](URL)</code>.</li><li><strong>Imagens:</strong> <code>![texto alternativo](URL da imagem)</code>.</li><li><strong>Citações:</strong> <code>&gt; texto</code> para citações.</li><li><strong>Código inline:</strong> `código`.</li><li><strong>Bloco de código:</strong> Coloque 3 acentos graves (`) antes e depois do bloco de código, ou indente com 4 espaços.</li><li><strong>Linhas horizontais:</strong> Três ou mais traços (<code>---</code> ou <code>***</code> ou <code>___</code>).</li><li><strong>Tabelas:</strong> Use barras verticais (<code>|</code>) para separar as células e hífens (<code>-</code>) para separar os cabeçalhos do restante da tabela.</li><li><strong>Destaque de sintaxe:</strong> Coloque o nome da linguagem após os três acentos graves para destacar a sintaxe do código (ex: ```python).</li></ol>

<p>Claro, aqui estão mais algumas tags e funcionalidades do Markdown:</p><ol start="15"><li><strong>Links âncora:</strong> <code>[texto](URL#ancora)</code>, onde "ancora" é o identificador de uma seção específica do documento.</li><li><strong>Listas de tarefas:</strong> <code>- [ ]</code> para tarefas não concluídas e <code>- [x]</code> para tarefas concluídas.</li><li><strong>Notas de rodapé:</strong> <code>[texto][1]</code> e, em outro lugar do documento, <code>[1]: URL</code> para adicionar notas de rodapé.</li><li><strong>Texto suprimido:</strong> <code>^(texto)</code>.</li><li><strong>Texto subscrito:</strong> <code>~texto~</code>.</li><li><strong>Texto destacado:</strong> <code>==texto==</code>.</li><li><strong>Citação de múltiplas linhas:</strong> Use <code>&gt;</code> no início de cada linha da citação.</li><li><strong>Títulos com identificadores:</strong> <code># Título {#identificador}</code>.</li><li><strong>Adicionando classes CSS:</strong> <code>{: .classe}</code> para adicionar uma classe CSS a um elemento Markdown.</li><li><strong>Escape de caracteres:</strong> Use <code>\</code> para escapar caracteres especiais que têm significados em Markdown, como asteriscos ou underscores.</li><li><strong>Inserir HTML:</strong> Embora não seja recomendado, você pode inserir HTML diretamente em documentos Markdown para funcionalidades mais avançadas.</li></ol><p>Essas são apenas algumas das muitas funcionalidades do Markdown. Ele é bastante flexível e pode ser estendido de várias maneiras para atender às necessidades específicas de formatação de texto.</p>


Para mudar a cor da fonte em um arquivo Markdown (.md), você pode usar HTML embutido, já que o Markdown padrão não suporta diretamente a alteração de cores de texto. Aqui está um exemplo de como fazer isso:

```markdown
<p style="color:red;">Este texto será vermelho.</p>
```

Você também pode usar outras cores substituindo “red” pelo nome da cor desejada ou pelo código hexadecimal da cor, como “#FF5733” para um tom de laranja.

### Exemplo com código hexadecimal:

```markdown
<p style="color:#FF5733;">Este texto será laranja.</p>
```

### Exemplo com nome de cor:

```markdown
<p style="color:blue;">Este texto será azul.</p>
```

<p style="color:red;">Este texto será vermelho.</p>
