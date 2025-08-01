---
show_subscribe: false	

title: Markdown 文档
tags: 
    - Markdown
    - 文档
---


## 总览

几乎所有 [Markdown](https://www.markdown.xyz/cheat-sheet/) 应用程序都支持 John Gruber 原始设计文档中列出的 Markdown 基本语法。但是，Markdown 处理程序之间存在着细微的变化和差异，我们都会尽可能标记出来。

## 标题（Headings）

<p>要创建标题，请在单词或短语前面添加井号 (<code class="language-plaintext highlighter-rouge">#</code>) 。井号的数量代表了标题的级别。例如，添加三个井号即创建一个三级标题 (<code class="language-plaintext highlighter-rouge">&lt;h3&gt;</code>) (例如：<code class="language-plaintext highlighter-rouge">### My Header</code>)。</p>

<p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code class="highlighter-rouge"># Heading level 1</code></td>
      <td><code class="highlighter-rouge">&lt;h1&gt;Heading level 1&lt;/h1&gt;</code></td>
      <td><h1 class="no-anchor" data-toc-skip="" id="heading-level-1">Heading level 1</h1></td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">## Heading level 2</code></td>
      <td><code class="highlighter-rouge">&lt;h2&gt;Heading level 2&lt;/h2&gt;</code></td>
      <td><h2 class="no-anchor" data-toc-skip="" id="heading-level-2">Heading level 2</h2></td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">### Heading level 3</code></td>
      <td><code class="highlighter-rouge">&lt;h3&gt;Heading level 3&lt;/h3&gt;</code></td>
      <td><h3 class="no-anchor" data-toc-skip="" id="heading-level-3">Heading level 3</h3></td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">#### Heading level 4</code></td>
      <td><code class="highlighter-rouge">&lt;h4&gt;Heading level  4&lt;/h4&gt;</code></td>
      <td><h4 class="no-anchor" id="heading-level-4">Heading level 4</h4></td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">##### Heading level 5</code></td>
      <td><code class="highlighter-rouge">&lt;h5&gt;Heading level 5&lt;/h5&gt;</code></td>
      <td><h5 class="no-anchor" id="heading-level-5">Heading level 5</h5></td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">###### Heading level 6</code></td>
      <td><code class="highlighter-rouge">&lt;h6&gt;Heading level 6&lt;/h6&gt;</code></td>
      <td><h6 class="no-anchor">Heading level 6</h6></td>
    </tr>
  </tbody>
</table>

</p>

<h3 id="可选语法">可选语法<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%8F%AF%E9%80%89%E8%AF%AD%E6%B3%95" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>还可以在文本下方添加任意数量的 <code class="language-plaintext highlighter-rouge">==</code> 号来标识一级标题，或者 <code class="language-plaintext highlighter-rouge">--</code> 号来标识二级标题。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code class="highlighter-rouge">Heading level 1<br>===============</code></td>
      <td><code class="highlighter-rouge">&lt;h1&gt;Heading level 1&lt;/h1&gt;</code></td>
      <td><h1 class="no-anchor" data-toc-skip="" id="heading-level-1-1">Heading level 1</h1></td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">Heading level 2<br>---------------</code></td>
      <td><code class="highlighter-rouge">&lt;h2&gt;Heading level 2&lt;/h2&gt;</code></td>
      <td><h2 class="no-anchor" data-toc-skip="" id="heading-level-2-1">Heading level 2</h2></td>
    </tr>
  </tbody>
</table>

<h3 id="标题heading用法的最佳实践">标题（Heading）用法的最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E6%A0%87%E9%A2%98heading%E7%94%A8%E6%B3%95%E7%9A%84%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>当井号（<code class="language-plaintext highlighter-rouge">#</code>）和标题文本之间没有空格时，各 Markdown 应用程序的处理方式是不一样的。为了兼容考虑，请在井号和标题文本之间添加一个空格。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          # Here's a Heading<br><br>
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          #Here's a Heading
        </code>
      </td>
    </tr>
  </tbody>
</table>

<p>You should also put blank lines before and after a heading for compatibility.</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; Do this</th>
      <th>❌&nbsp; Don't do this</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
        Try to put a blank line before...<br><br>

        # Heading<br><br>

        ...and after a heading.
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
        Without blank lines, this might not look right.<br>
        # Heading<br>
        Don't do this!
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h2 id="paragraphs">段落（Paragraphs）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#paragraphs" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>要创建段落，请使用空白行将一行或多行文本进行分隔。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          I really like using Markdown.<br><br>

          I think I'll use it to format all of my documents from now on.
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">&lt;p&gt;I really like using Markdown.&lt;/p&gt;<br><br>

        &lt;p&gt;I think I'll use it to format all of my documents from now on.&lt;/p&gt;</code>
      </td>
      <td>
        <p>I really like using Markdown.</p>

        <p>I think I'll use it to format all of my documents from now on.</p>
      </td>
    </tr>
  </tbody>
</table>

<h3 id="段落paragraph用法的最佳实践">段落（Paragraph）用法的最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E6%AE%B5%E8%90%BDparagraph%E7%94%A8%E6%B3%95%E7%9A%84%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>除非 <a href="https://www.markdown.xyz/basic-syntax/#paragraphs">段落在列表中</a>，否则不要用空格（spaces）或制表符（ tabs）缩进段落。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          Don't put tabs or spaces in front of your paragraphs.<br><br>

          Keep lines left-aligned like this.<br><br>
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
        &nbsp;&nbsp;&nbsp;&nbsp;This can result in unexpected
        formatting problems.<br><br>

        &nbsp;&nbsp;Don't add tabs or spaces in front of paragraphs.
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h2 id="line-breaks">换行（Line Breaks）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#line-breaks" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>在一行的末尾添加两个或多个空格，然后按回车键（return），即可创建一个换行（line break）或新行 (<code class="language-plaintext highlighter-rouge">&lt;br&gt;</code>)。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          This is the first line. &nbsp;<br>
          And this is the second line.
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">&lt;p&gt;This is the first line.&lt;br&gt;<br>

        And this is the second line.&lt;/p&gt;</code>
      </td>
      <td>
        <p>This is the first line.<br>   
        And this is the second line.</p>
      </td>
    </tr>
  </tbody>
</table>

<h3 id="换行line-break用法的最佳实践">换行（Line Break）用法的最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E6%8D%A2%E8%A1%8Cline-break%E7%94%A8%E6%B3%95%E7%9A%84%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>几乎每个 Markdown 应用程序都支持两个或多个空格进行换行 (称为 “结尾空格（trailing whitespace）”) 的方式，但这是有争议的，因为很难在编辑器中直接看到空格，并且很多人在每个句子后面都会有意或无意地添加两个空格。由于这个原因，你可能需要使用除结尾空格以外的其它方式来进行换行。如果你所使用的 Markdown 应用程序 <a href="https://www.markdown.xyz/basic-syntax/#html">支持 HTML</a> 的话，你可以使用 HTML 的 <code class="language-plaintext highlighter-rouge">&lt;br&gt;</code> 标签来实现换行。</p>

<p>为了兼容性，请在行尾添加“结尾空格”或 HTML 的 <code class="language-plaintext highlighter-rouge">&lt;br&gt;</code> 标签来实现换行。</p>

<p>还有两种其他方式我并不推荐使用。CommonMark 和其它几种轻量级标记语言支持在行尾添加反斜杠 (<code class="language-plaintext highlighter-rouge">\</code>) 的方式实现换行，但是并非所有 Markdown 应用程序都支持此种方式，因此从兼容性的角度来看，不推荐使用。并且至少有两种轻量级标记语言支持无须在行尾添加任何内容，只须键入回车键（ return）即可实现换行。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          First line with two spaces after. &nbsp;<br>
          And the next line.<br><br>

          First line with the HTML tag after.&lt;br&gt;<br>
          And the next line.<br><br>
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
        First line with a backslash after.\<br>
        And the next line.<br><br>

        First line with nothing after.<br>
        And the next line.<br><br>
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h2 id="emphasis">强调（Emphasis）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#emphasis" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>通过将文本设置为粗体或斜体来强调其重要性。</p>

<h3 id="bold">粗体（Bold）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#bold" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>要加粗文本，请在单词或短语的前后各添加两个星号（asterisks）或下划线（underscores）。如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个星号（asterisks）。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code class="highlighter-rouge">I just love **bold text**.</code></td>
      <td><code class="highlighter-rouge">I just love &lt;strong&gt;bold text&lt;/strong&gt;.</code></td>
      <td>I just love <strong>bold text</strong>.</td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">I just love __bold text__.</code></td>
      <td><code class="highlighter-rouge">I just love &lt;strong&gt;bold text&lt;/strong&gt;.</code></td>
      <td>I just love <strong>bold text</strong>.</td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">Love**is**bold</code></td> <td><code class="highlighter-rouge">Love&lt;strong&gt;is&lt;/strong&gt;bold</code></td>
      <td>Love<strong>is</strong>bold</td>
    </tr>
  </tbody>
</table>

<h4 id="粗体bold用法最佳实践">粗体（Bold）用法最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E7%B2%97%E4%BD%93bold%E7%94%A8%E6%B3%95%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>Markdown 应用程序在如何处理单词或短语中间的下划线上并不一致。为兼容考虑，在单词或短语中间部分加粗的话，请使用星号（asterisks）。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          Love**is**bold
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          Love__is__bold
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h3 id="italic">斜体（Italic）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#italic" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>要用斜体显示文本，请在单词或短语前后添加一个星号（asterisk）或下划线（underscore）。要斜体突出单词的中间部分，请在字母前后各添加一个星号，中间不要带空格。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code class="highlighter-rouge">Italicized text is the *cat's meow*.</code></td>
      <td><code class="highlighter-rouge">Italicized text is the &lt;em&gt;cat's meow&lt;/em&gt;.</code></td>
      <td>Italicized text is the <em>cat’s meow</em>.</td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">Italicized text is the _cat's meow_.</code></td>
      <td><code class="highlighter-rouge">Italicized text is the &lt;em&gt;cat's meow&lt;/em&gt;.</code></td>
      <td>Italicized text is the <em>cat’s meow</em>.</td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">A*cat*meow</code></td>
      <td><code class="highlighter-rouge">A&lt;em&gt;cat&lt;/em&gt;meow</code></td>
      <td>A<em>cat</em>meow</td>
    </tr>
  </tbody>
</table>

<h4 id="斜体italic用法的最佳实践">斜体（Italic）用法的最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E6%96%9C%E4%BD%93italic%E7%94%A8%E6%B3%95%E7%9A%84%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>Markdown 的众多应用程序在如何处理单词中间的下划线上意见不一致。为了兼容起见，请用星号标注单词中间的斜体来表示着重。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          A*cat*meow
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          A_cat_meow
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h3 id="粗体bold和斜体italic">粗体（Bold）和斜体（Italic）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E7%B2%97%E4%BD%93bold%E5%92%8C%E6%96%9C%E4%BD%93italic" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>要同时用粗体和斜体突出显示文本，请在单词或短语的前后各添加三个星号或下划线。要加粗并用斜体显示单词或短语的中间部分，请在要突出显示的部分前后各添加三个星号，中间不要带空格。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code class="highlighter-rouge">This text is ***really important***.</code></td>
      <td><code class="highlighter-rouge">This text is &lt;strong&gt;&lt;em&gt;really important&lt;/em&gt;&lt;/strong&gt;.</code></td>
      <td>This text is <strong><em>really important</em></strong>.</td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">This text is ___really important___.</code></td>
      <td><code class="highlighter-rouge">This text is &lt;strong&gt;&lt;em&gt;really important&lt;/em&gt;&lt;/strong&gt;.</code></td>
      <td>This text is <strong><em>really important</em></strong>.</td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">This text is __*really important*__.</code></td>
      <td><code class="highlighter-rouge">This text is &lt;strong&gt;&lt;em&gt;really important&lt;/em&gt;&lt;/strong&gt;.</code></td>
      <td>This text is <strong><em>really important</em></strong>.</td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">This text is **_really important_**.</code></td>
      <td><code class="highlighter-rouge">This text is &lt;strong&gt;&lt;em&gt;really important&lt;/em&gt;&lt;/strong&gt;.</code></td>
      <td>This text is <strong><em>really important</em></strong>.</td>
    </tr>
    <tr>
      <td><code class="highlighter-rouge">This is really***very***important text.</code></td>
      <td><code class="highlighter-rouge">This is really&lt;strong&gt;&lt;em&gt;very&lt;/em&gt;&lt;/strong&gt;important text.</code></td>
      <td>This is really<strong><em>very</em></strong>important text.</td>
    </tr>
  </tbody>
</table>

<h4 id="粗体bold和斜体italic用法的最佳实践">粗体（Bold）和斜体（Italic）用法的最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E7%B2%97%E4%BD%93bold%E5%92%8C%E6%96%9C%E4%BD%93italic%E7%94%A8%E6%B3%95%E7%9A%84%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>Markdown 应用程序在处理单词或短语中间添加的下划线上并不一致。为了实现兼容性，请使用星号将单词或短语的中间部分加粗并以斜体显示，以示重要。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          This is really***very***important text.
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          This is really___very___important text.
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h2 id="blockquotes">块引用（Blockquotes）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#blockquotes" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>要创建块引用，请在段落前添加一个 <code class="language-plaintext highlighter-rouge">&gt;</code> 符号。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>&gt; Dorothy followed her through many of the beautiful rooms in her castle.
</code></pre></div></div>

<p>渲染效果如下所示：</p>

<blockquote>
  <p>Dorothy followed her through many of the beautiful rooms in her castle.</p>
</blockquote>

<h3 id="多个段落的块引用blockquotes">多个段落的块引用（Blockquotes）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%A4%9A%E4%B8%AA%E6%AE%B5%E8%90%BD%E7%9A%84%E5%9D%97%E5%BC%95%E7%94%A8blockquotes" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>块引用可以包含多个段落。为段落之间的空白行各添加一个 <code class="language-plaintext highlighter-rouge">&gt;</code> 符号。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>&gt; Dorothy followed her through many of the beautiful rooms in her castle.
&gt;
&gt; The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
</code></pre></div></div>

<p>渲染效果如下：</p>

<blockquote>
  <p>Dorothy followed her through many of the beautiful rooms in her castle.</p>

  <p>The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.</p>
</blockquote>

<h3 id="嵌套块引用nested-blockquotes">嵌套块引用（Nested Blockquotes）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%B5%8C%E5%A5%97%E5%9D%97%E5%BC%95%E7%94%A8nested-blockquotes" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>块引用可以嵌套。在要嵌套的段落前添加一个 <code class="language-plaintext highlighter-rouge">&gt;&gt;</code> 符号。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>&gt; Dorothy followed her through many of the beautiful rooms in her castle.
&gt;
&gt;&gt; The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
</code></pre></div></div>

<p>渲染效果如下：</p>

<blockquote>
  <p>Dorothy followed her through many of the beautiful rooms in her castle.</p>

  <blockquote>
    <p>The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.</p>
  </blockquote>
</blockquote>

<h3 id="带有其它元素的块引用blockquotes-with-other-elements">带有其它元素的块引用（Blockquotes with Other Elements）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%B8%A6%E6%9C%89%E5%85%B6%E5%AE%83%E5%85%83%E7%B4%A0%E7%9A%84%E5%9D%97%E5%BC%95%E7%94%A8blockquotes-with-other-elements" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>块引用可以包含其他 Markdown 格式的元素。并非所有元素都可以使用，你需要进行实验以查看哪些元素有效。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>&gt; #### The quarterly results look great!
&gt;
&gt; - Revenue was off the chart.
&gt; - Profits were higher than ever.
&gt;
&gt;  *Everything* is going according to **plan**.
</code></pre></div></div>

<p>渲染效果如下：</p>

<blockquote>
  <h4 class="no-anchor" id="the-quarterly-results-look-great">The quarterly results look great!</h4>

  <ul>
    <li>Revenue was off the chart.</li>
    <li>Profits were higher than ever.</li>
  </ul>

  <p><em>Everything</em> is going according to <strong>plan</strong>.</p>
</blockquote>

<h3 id="blockquotes-best-practices">Blockquotes Best Practices<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#blockquotes-best-practices" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>For compatibility, put blank lines before and after blockquotes.</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; Do this</th>
      <th>❌&nbsp; Don't do this</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
        Try to put a blank line before...<br><br>

        &gt; This is a blockquote<br><br>

        ...and after a blockquote.
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
        Without blank lines, this might not look right.<br>
        &gt; This is a blockquote<br>
        Don't do this!
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h2 id="lists">列表（Lists）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#lists" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>你可以将多个条目组织成有序或无序列表。</p>

<h3 id="ordered-lists">有序列表（Ordered Lists）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#ordered-lists" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>Rendered Output</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td>
      <code class="highlighter-rouge">
        1. First item<br>
        2. Second item<br>
        3. Third item<br>
        4. Fourth item
      </code>
    </td>
    <td>
      <code class="highlighter-rouge">
        &lt;ol&gt;<br>
          &nbsp;&nbsp;&lt;li&gt;First item&lt;/li&gt;<br>
          &nbsp;&nbsp;&lt;li&gt;Second item&lt;/li&gt;<br>
          &nbsp;&nbsp;&lt;li&gt;Third item&lt;/li&gt;<br>
          &nbsp;&nbsp;&lt;li&gt;Fourth item&lt;/li&gt;<br>
        &lt;/ol&gt;
      </code>
    </td>
    <td>
      <ol>
        <li>First item</li>
        <li>Second item</li>
        <li>Third item</li>
        <li>Fourth item</li>
      </ol>
    </td>
    </tr>
    <tr>
      <td>
        <code class="highlighter-rouge">
          1. First item<br>
          2. Second item<br>
          3. Third item<br>
          4. Fourth item
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          &lt;ol&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;First item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Second item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Third item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ol&gt;
        </code>
      </td>
      <td>
        <ol>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td>
        <code class="highlighter-rouge">
          5. First item<br>
          6. Second item<br>
          7. Third item<br>
          8. Fourth item
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          &lt;ol&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;First item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Second item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Third item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ol&gt;
        </code>
      </td>
      <td>
        <ol>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td>
        <code class="highlighter-rouge">
          9. First item<br>
          10. Second item<br>
          11. Third item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;1. Indented item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;2. Indented item<br>
          12. Fourth item
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          &lt;ol&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;First item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Second item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Third item<br>
              &nbsp;&nbsp;&nbsp;&nbsp;&lt;ol&gt;<br>
                &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;li&gt;Indented item&lt;/li&gt;<br>
                &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;li&gt;Indented item&lt;/li&gt;<br>
              &nbsp;&nbsp;&nbsp;&nbsp;&lt;/ol&gt;<br>
            &nbsp;&nbsp;&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ol&gt;
        </code>
      </td>
      <td>
        <ol>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item
            <ol>
              <li>Indented item</li>
              <li>Indented item</li>
            </ol>
          </li>
          <li>Fourth item</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>

<h4 id="有序列表ordered-list用法的最佳实践">有序列表（Ordered List）用法的最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E6%9C%89%E5%BA%8F%E5%88%97%E8%A1%A8ordered-list%E7%94%A8%E6%B3%95%E7%9A%84%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>CommonMark 和其它几种轻量级标记语言可以让你使用括号（<code class="language-plaintext highlighter-rouge">)</code>）作为分隔符（例如 <code class="language-plaintext highlighter-rouge">1) First item</code>），但并非所有的 Markdown 应用程序都支持此种用法，因此，从兼容的角度来看，此用法不推荐。为了兼容起见，请只使用英文句点作为分隔符。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          1. First item<br>
          2. Second item
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          1) First item<br>
          2) Second item
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h3 id="unordered-lists">无序列表（Unordered Lists）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#unordered-lists" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>要创建无序列表，请在每个列表项前面添加破折号 (<code class="language-plaintext highlighter-rouge">-</code>)、星号 (<code class="language-plaintext highlighter-rouge">*</code>) 或加号 (<code class="language-plaintext highlighter-rouge">+</code>) 。缩进一个或多个列表项可创建嵌套列表。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          - First item<br>
          - Second item<br>
          - Third item<br>
          - Fourth item
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          &lt;ul&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;First item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Second item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Third item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
        </code>
      </td>
      <td>
        <ul>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <code class="highlighter-rouge">
          * First item<br>
          * Second item<br>
          * Third item<br>
          * Fourth item
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          &lt;ul&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;First item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Second item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Third item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
        </code>
      </td>
      <td>
        <ul>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <code class="highlighter-rouge">
          + First item<br>
          + Second item<br>
          + Third item<br>
          + Fourth item
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          &lt;ul&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;First item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Second item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Third item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
        </code>
      </td>
      <td>
        <ul>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item</li>
          <li>Fourth item</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <code class="highlighter-rouge">
          - First item<br>
          - Second item<br>
          - Third item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;- Indented item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;- Indented item<br>
          - Fourth item
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          &lt;ul&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;First item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Second item&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Third item<br>
              &nbsp;&nbsp;&nbsp;&nbsp;&lt;ul&gt;<br>
                &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;li&gt;Indented item&lt;/li&gt;<br>
                &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;li&gt;Indented item&lt;/li&gt;<br>
              &nbsp;&nbsp;&nbsp;&nbsp;&lt;/ul&gt;<br>
            &nbsp;&nbsp;&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
        </code>
      </td>
      <td>
        <ul>
          <li>First item</li>
          <li>Second item</li>
          <li>Third item
            <ul>
              <li>Indented item</li>
              <li>Indented item</li>
            </ul>
          </li>
          <li>Fourth item</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

<h4 id="以数字开头的无序列表项">以数字开头的无序列表项<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E4%BB%A5%E6%95%B0%E5%AD%97%E5%BC%80%E5%A4%B4%E7%9A%84%E6%97%A0%E5%BA%8F%E5%88%97%E8%A1%A8%E9%A1%B9" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>如果你需要以数字开头并且紧跟一个英文句号（也就是 <code class="language-plaintext highlighter-rouge">.</code>）的无序列表项，则可以使使用反斜线（<code class="language-plaintext highlighter-rouge">\</code>）来 <a href="https://www.markdown.xyz/basic-syntax/#escaping-characters">转义</a> 这个英文句号。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>Rendered Output</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          - 1968\. A great year!<br>
          - I think 1969 was second best.
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          &lt;ul&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;1968. A great year!&lt;/li&gt;<br>
            &nbsp;&nbsp;&lt;li&gt;I think 1969 was second best.&lt;/li&gt;<br>
          &lt;/ul&gt;
        </code>
      </td>
      <td>
        <ul>
          <li>1968. A great year!</li>
          <li>I think 1969 was second best.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

<h4 id="无序列表unordered-list用法的最佳实践">无序列表（Unordered List）用法的最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E6%97%A0%E5%BA%8F%E5%88%97%E8%A1%A8unordered-list%E7%94%A8%E6%B3%95%E7%9A%84%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>Markdown 应用程序在如何处理同一列表中混用不同分隔符上并不一致。为了兼容起见，请不要在同一个列表中混用不同的分隔符，最好选定一种分隔符并一直用下去。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
          - First item<br>
          - Second item<br>
          - Third item<br>
          - Fourth item
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
          + First item<br>
          * Second item<br>
          - Third item<br>
          + Fourth item
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h3 id="在列表中添加列表项">在列表中添加列表项<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%9C%A8%E5%88%97%E8%A1%A8%E4%B8%AD%E6%B7%BB%E5%8A%A0%E5%88%97%E8%A1%A8%E9%A1%B9" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：</p>

<div class="alert alert-success">
  <i class="fas fa-lightbulb"></i> <strong>Tip:</strong> If things don't appear the way you expect, double check that you've indented the elements in the list four spaces or one tab.
</div>

<h4 id="段落paragraphs">段落（Paragraphs）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E6%AE%B5%E8%90%BDparagraphs" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.

* And here's the third list item.
</code></pre></div></div>

<p>渲染效果如下：</p>

<ul>
  <li>This is the first list item.</li>
  <li>
    <p>Here’s the second list item.</p>

    <p>I need to add another paragraph below the second list item.</p>
  </li>
  <li>And here’s the third list item.</li>
</ul>

<h4 id="引用块blockquotes">引用块（Blockquotes）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%BC%95%E7%94%A8%E5%9D%97blockquotes" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>* This is the first list item.
* Here's the second list item.

    &gt; A blockquote would look great below the second list item.

* And here's the third list item.
</code></pre></div></div>

<p>渲染效果如下：</p>

<ul>
  <li>This is the first list item.</li>
  <li>
    <p>Here’s the second list item.</p>

    <blockquote>
      <p>A blockquote would look great below the second list item.</p>
    </blockquote>
  </li>
  <li>And here’s the third list item.</li>
</ul>

<h4 id="code-blocks-1">代码块（Code Blocks）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#code-blocks-1" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p><a href="https://www.markdown.xyz/basic-syntax/#code-blocks">代码块（Code blocks）</a> 通常采用四个空格或一个制表符缩进。当它们被放在列表中时，请将它们缩进八个空格或两个制表符。</p>

<div class="language-text highlighter-rouge"><div class="highlight"><pre class="highlight"><code>1. Open the file.
2. Find the following code block on line 21:

        &lt;html&gt;
          &lt;head&gt;
            &lt;title&gt;Test&lt;/title&gt;
          &lt;/head&gt;

3. Update the title to match the name of your website.
</code></pre></div></div>

<p>渲染效果如下：</p>

<ol>
  <li>Open the file.</li>
  <li>
    <p>Find the following code block on line 21:</p>

    <div class="language-text highlighter-rouge"><div class="highlight"><pre class="highlight"><code> &lt;html&gt;
   &lt;head&gt;
     &lt;title&gt;Test&lt;/title&gt;
   &lt;/head&gt;
</code></pre></div>    </div>
  </li>
  <li>Update the title to match the name of your website.</li>
</ol>

<h4 id="图片images">图片（Images）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%9B%BE%E7%89%87images" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](assets/images/tux.png)

3. Close the file.
</code></pre></div></div>

<p>渲染效果如下：</p>

<ol>
  <li>Open the file containing the Linux mascot.</li>
  <li>
    <p>Marvel at its beauty.</p>

    <p><img src="./Markdown 基本语法 _ Markdown指南中文版_files/tux.png" alt="Tux, the Linux mascot"></p>
  </li>
  <li>Close the file.</li>
</ol>

<h4 id="列表lists">列表（Lists）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%88%97%E8%A1%A8lists" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>你可以将无序列表嵌套在有序列表中，反之亦然。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item
</code></pre></div></div>

<p>渲染效果如下：</p>

<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ul>
      <li>Indented item</li>
      <li>Indented item</li>
    </ul>
  </li>
  <li>Fourth item</li>
</ol>

<h2 id="code">代码<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#code" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>要将单词或短语表示为代码，请将其包裹在反引号 (<code class="language-plaintext highlighter-rouge">`</code>) 中。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code class="highlighter-rouge">At the command prompt, type `nano`.</code></td>
      <td><code class="highlighter-rouge">At the command prompt, type &lt;code&gt;nano&lt;/code&gt;. </code></td>
      <td>At the command prompt, type <code class="highlighter-rouge">nano</code>.</td>
    </tr>
  </tbody>
</table>

<h3 id="转义反引号">转义反引号<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E8%BD%AC%E4%B9%89%E5%8F%8D%E5%BC%95%E5%8F%B7" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(<code>``</code>)中。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染效果</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>``Use `code` in your Markdown file.``</code></td>
      <td><code class="highlighter-rouge">&lt;code&gt;Use `code` in your Markdown file.&lt;/code&gt;</code></td>
      <td><code>Use `code` in your Markdown file.</code></td>
    </tr>
  </tbody>
</table>

<h3 id="代码块code-blocks">代码块（Code Blocks）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E4%BB%A3%E7%A0%81%E5%9D%97code-blocks" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。</p>

<div class="language-text highlighter-rouge"><div class="highlight"><pre class="highlight"><code>    &lt;html&gt;
      &lt;head&gt;
      &lt;/head&gt;
    &lt;/html&gt;
</code></pre></div></div>

<p>渲染效果如下：</p>

<div class="language-text highlighter-rouge"><div class="highlight"><pre class="highlight"><code>&lt;html&gt;
  &lt;head&gt;
  &lt;/head&gt;
&lt;/html&gt;
</code></pre></div></div>

<div class="alert alert-info">
  <i class="fas fa-info-circle"></i> <strong>注意：</strong> 要创建不用缩进的代码块，请使用 <a href="https://www.markdown.xyz/extended-syntax/#fenced-code-blocks">围栏式代码块（fenced code blocks）</a>.
</div>

<h2 id="horizontal-rules">分隔线（Horizontal Rules）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#horizontal-rules" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>要创建分隔线，请在单独一行上使用三个或多个星号 (<code class="language-plaintext highlighter-rouge">***</code>)、破折号 (<code class="language-plaintext highlighter-rouge">---</code>) 或下划线 (<code class="language-plaintext highlighter-rouge">___</code>) ，并且不能包含其他内容。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>***

---

_________________
</code></pre></div></div>

<p>以上三个分隔线的渲染效果看起来都一样：</p>

<hr>

<h3 id="分隔线horizontal-rule用法最佳实践">分隔线（Horizontal Rule）用法最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%88%86%E9%9A%94%E7%BA%BFhorizontal-rule%E7%94%A8%E6%B3%95%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>为了兼容性，请在分隔线的前后均添加空白行。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
        Try to put a blank line before...<br><br>

        ---<br><br>

        ...and after a horizontal rule.
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
        Without blank lines, this would be a heading.<br>
        ---<br>
        Don't do this!
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h2 id="links">链接（Links）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#links" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>要创建链接，请将链接文本括在方括号（例如 <code class="language-plaintext highlighter-rouge">[Duck Duck Go]</code>）中，后面紧跟着括在圆括号中的 URL（例如 <code class="language-plaintext highlighter-rouge">(https://duckduckgo.com)</code> ）。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>My favorite search engine is [Duck Duck Go](https://duckduckgo.com).
</code></pre></div></div>

<p>渲染效果如下：</p>

<p>My favorite search engine is <a href="https://duckduckgo.com/">Duck Duck Go</a>.</p>

<div class="alert alert-info">
  <i class="fas fa-info-circle"></i> <strong>Note:</strong> To link to an element on the same page, see <a href="https://www.markdown.xyz/extended-syntax/#linking-to-heading-ids">linking to heading IDs</a>.
</div>

<h3 id="添加标题">添加标题<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E6%B7%BB%E5%8A%A0%E6%A0%87%E9%A2%98" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>你可以选择为链接添加标题（即 title 属性）。当用户将鼠标悬停在链接上时，将显示一个提示。要添加标题，请将其放在 URL 后面。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").
</code></pre></div></div>

<p>渲染效果如下：</p>

<p>My favorite search engine is <a href="https://duckduckgo.com/" title="The best search engine for privacy">Duck Duck Go</a>.</p>

<h3 id="网址和电子邮件地址">网址和电子邮件地址<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E7%BD%91%E5%9D%80%E5%92%8C%E7%94%B5%E5%AD%90%E9%82%AE%E4%BB%B6%E5%9C%B0%E5%9D%80" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>要将 URL 或电子邮件地址快速转换为链接，请将其括在尖括号中。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>&lt;https://www.markdownguide.org&gt;
&lt;fake@example.com&gt;
</code></pre></div></div>

<p>渲染效果如下：</p>

<p><a href="https://www.markdownguide.org/">https://www.markdownguide.org</a><br>
<a href="mailto:fake@example.com">fake@example.com</a></p>

<h3 id="格式化链接">格式化链接<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E6%A0%BC%E5%BC%8F%E5%8C%96%E9%93%BE%E6%8E%A5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>如需 <a href="https://www.markdown.xyz/basic-syntax/#emphasis">强调（emphasize）</a> 某个链接, 请在方括号前及圆括号后添加星号。要将链接表示为 <a href="https://www.markdown.xyz/basic-syntax/#code">代码（code）</a> ，请在方括号内添加反引号。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).
</code></pre></div></div>

<p>渲染效果如下：</p>

<p>I love supporting the <strong><a href="https://eff.org/">EFF</a></strong>.<br>
This is the <em><a href="https://www.markdownguide.org/">Markdown Guide</a></em>.<br>
See the section on <a href="https://www.markdown.xyz/basic-syntax/#code"><code class="language-plaintext highlighter-rouge">code</code></a>.</p>

<h3 id="引用式链接">引用式链接<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%BC%95%E7%94%A8%E5%BC%8F%E9%93%BE%E6%8E%A5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>引用式（Reference-style）链接是一种特殊类型的链接，它使得 URL 在 Markdown 中更易于显示和阅读。引用式链接由两部分组成：一部分被放置在正文文本中；另一部分被放置在文档中的其它地方，以便于阅读。</p>

<h4 id="引用式链接第一部分的格式">引用式链接第一部分的格式<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%BC%95%E7%94%A8%E5%BC%8F%E9%93%BE%E6%8E%A5%E7%AC%AC%E4%B8%80%E9%83%A8%E5%88%86%E7%9A%84%E6%A0%BC%E5%BC%8F" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>引用式链接的第一部分的格式由两组方括号组成。第一组方括号内放的是显示为链接的文本，第二组方括号内放的是一个标签，该标签用于指向您存放在文档中其它位置的链接。</p>

<p>尽管不是必须的，但你可以在第一组和第二组方括号之间添加一个空格。第二组方括号中的标签不区分大小写，并且可以包含字母、数字、空格或标点符号。</p>

<p>以下示例中，链接的第一部分是等效的：</p>

<ul>
  <li><code class="language-plaintext highlighter-rouge">[hobbit-hole][1]</code></li>
  <li><code class="language-plaintext highlighter-rouge">[hobbit-hole] [1]</code></li>
</ul>

<h4 id="引用式链接第二部分的格式">引用式链接第二部分的格式<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%BC%95%E7%94%A8%E5%BC%8F%E9%93%BE%E6%8E%A5%E7%AC%AC%E4%BA%8C%E9%83%A8%E5%88%86%E7%9A%84%E6%A0%BC%E5%BC%8F" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>引用式链接的第二部分可以包含以下属性：</p>

<ol>
  <li>放在方括号内的标签，以及紧跟在方括号后面的一个冒号和至少一个空格（例如 <code class="language-plaintext highlighter-rouge">[label]: </code>）。</li>
  <li>链接的 URL，可以选择将其括在尖括号内。</li>
  <li>链接的标题（可有可无），可以将其括在双引号、单引号或括号内。</li>
</ol>

<p>以下示例中，链接的第二部分是等效的：</p>

<ul>
  <li><code class="language-plaintext highlighter-rouge">[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle</code></li>
  <li><code class="language-plaintext highlighter-rouge">[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"</code></li>
  <li><code class="language-plaintext highlighter-rouge">[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'</code></li>
  <li><code class="language-plaintext highlighter-rouge">[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)</code></li>
  <li><code class="language-plaintext highlighter-rouge">[1]: &lt;https://en.wikipedia.org/wiki/Hobbit#Lifestyle&gt; "Hobbit lifestyles"</code></li>
  <li><code class="language-plaintext highlighter-rouge">[1]: &lt;https://en.wikipedia.org/wiki/Hobbit#Lifestyle&gt; 'Hobbit lifestyles'</code></li>
  <li><code class="language-plaintext highlighter-rouge">[1]: &lt;https://en.wikipedia.org/wiki/Hobbit#Lifestyle&gt; (Hobbit lifestyles)</code></li>
</ul>

<p>可以将链接的第二部分放在 Markdown 文档中的任何位置。有些人将它们放在被引用的段落的后面，有些人将它们放在文档的末尾（类似尾注或脚注）。</p>

<h4 id="将两部分组合在一起使用的示例">将两部分组合在一起使用的示例<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%B0%86%E4%B8%A4%E9%83%A8%E5%88%86%E7%BB%84%E5%90%88%E5%9C%A8%E4%B8%80%E8%B5%B7%E4%BD%BF%E7%94%A8%E7%9A%84%E7%A4%BA%E4%BE%8B" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h4>

<p>假设你将一个 URL 作为一个 <a href="https://www.markdown.xyz/basic-syntax/#links">标准 URL 链接</a> 添加到段落中，在 Markdown 中如下所示：</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.
</code></pre></div></div>

<p>Though it may point to interesting additional information, the URL as displayed really doesn’t add much to the existing raw text other than making it harder to read. To fix that, you could format the URL like this instead:</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole][1], and that means comfort.

[1]: &lt;https://en.wikipedia.org/wiki/Hobbit#Lifestyle&gt; "Hobbit lifestyles"
</code></pre></div></div>

<p>在上述两个实例中，渲染后的输出是相同的：</p>

<blockquote>
  <p>In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to  eat: it was a <a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle" title="Hobbit lifestyles">hobbit-hole</a>, and that means comfort.</p>
</blockquote>

<p>该链接的 HTML 为：</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>&lt;a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle" title="Hobbit lifestyles"&gt;hobbit-hole&lt;/a&gt;
</code></pre></div></div>

<h3 id="链接link的最佳使用实践">链接（Link）的最佳使用实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E9%93%BE%E6%8E%A5link%E7%9A%84%E6%9C%80%E4%BD%B3%E4%BD%BF%E7%94%A8%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>不同的 Markdown 应用程序在处理 URL 中间的空格方面是不一样的。为了兼容起见，请尽量使用 <code class="language-plaintext highlighter-rouge">%20</code> （空格的编码形式）来代替空格。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>✅&nbsp; 这样做</th>
      <th>❌&nbsp; 不要这样做</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code class="highlighter-rouge">
        [link](https://www.example.com/my%20great%20page)
        </code>
      </td>
      <td>
        <code class="highlighter-rouge">
        [link](https://www.example.com/my great page)
        </code>
      </td>
    </tr>
  </tbody>
</table>

<h2 id="images">图片（Images）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#images" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>要添加图片，首先请添加感叹号（<code class="language-plaintext highlighter-rouge">!</code>），然后紧跟着是方括号，方括号中可添加替代文本（alt text，即图片显示失败后显示此文本），最后跟着圆括号，圆括号中添加图片资源的路径或 URL。你可以选择在圆括号中的 URL 之后添加标题（即 title 属性）。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>![The San Juan Mountains are beautiful!](assets/images/san-juan-mountains.jpg "San Juan Mountains")
</code></pre></div></div>

<p>渲染效果如下：</p>

<p><img src="./Markdown 基本语法 _ Markdown指南中文版_files/san-juan-mountains.jpg" class="img-fluid" title="San Juan Mountains" alt="The San Juan Mountains are beautiful!" loading="lazy" sizes="100vw"></p>

<h3 id="带链接的图片">带链接的图片<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%B8%A6%E9%93%BE%E6%8E%A5%E7%9A%84%E5%9B%BE%E7%89%87" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>要为图片添加链接，请先为图片的 Markdown 标记添加一个方括号，然后紧跟着一个圆括号，并在圆括号中添加链接地址。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>[![An old rock in the desert](assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)
</code></pre></div></div>

<p>渲染效果如下：</p>

<div>
  <a href="https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv" class="no-underline">
  
<img src="./Markdown 基本语法 _ Markdown指南中文版_files/shiprock.jpg" class="img-fluid" title="Shiprock, New Mexico by Beau Rogers" alt="An old rock in the desert" loading="lazy" sizes="100vw">

  </a>
</div>

<h2 id="escaping-characters">转义字符（Escaping Characters）<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#escaping-characters" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>要显示原本用于格式化 Markdown 文档的字符，请在字符前面添加反斜杠字符 (<code class="language-plaintext highlighter-rouge">\</code>) 。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>\* 如果没有开头的反斜杠字符的话，这一行将显示为无序列表。
</code></pre></div></div>

<p>渲染效果如下：</p>

<p>* 如果没有开头的反斜杠字符的话，这一行将显示为无序列表。</p>

<h3 id="可做转义的英文字符">可做转义的（英文）字符<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#%E5%8F%AF%E5%81%9A%E8%BD%AC%E4%B9%89%E7%9A%84%E8%8B%B1%E6%96%87%E5%AD%97%E7%AC%A6" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>以下列出的字符都可以通过使用反斜杠字符从而达到转义目的。</p>

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>字符</th>
      <th>名称</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>\</td>
      <td>反斜杠（backslash）</td>
    </tr>
    <tr>
      <td>`</td>
      <td>backtick (另请参见 <a href="https://www.markdown.xyz/basic-syntax/#escaping-backticks">在代码中转义反引号</a>)</td>
    </tr>
    <tr>
      <td>*</td>
      <td>星号（asterisk）</td>
    </tr>
    <tr>
      <td>_</td>
      <td>下划线（underscore）</td>
    </tr>
    <tr>
      <td>{ }</td>
      <td>花括号（curly braces）</td>
    </tr>
    <tr>
      <td>[ ]</td>
      <td>方括号（brackets）</td>
    </tr>
    <tr>
      <td>&lt; &gt;</td>
      <td>angle brackets</td>
    </tr>
    <tr>
      <td>( )</td>
      <td>圆括号或括号（parentheses）</td>
    </tr>
    <tr>
      <td>#</td>
      <td>井号（pound sign）</td>
    </tr>
    <tr>
      <td>+</td>
      <td>加号（plus sign）</td>
    </tr>
    <tr>
      <td>-</td>
      <td>减号（minus sign） (也叫连字符 hyphen)</td>
    </tr>
    <tr>
      <td>.</td>
      <td>句点（dot）</td>
    </tr>
    <tr>
      <td>!</td>
      <td>感叹号（exclamation mark）</td>
    </tr>
    <tr>
      <td>|</td>
      <td>管道符（pipe） (另请参见 <a href="https://www.markdown.xyz/extended-syntax/#escaping-pipe-characters-in-tables">在表格中转义管道符</a>)</td>
    </tr>
  </tbody>
</table>

<h2 id="html">HTML 标签<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#html" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>

<p>大多 Markdown 应用程序允许你在 Markdown 格式文本中添加 HTML 标签。如果你喜欢某些 HTML 标签胜于 Markdown 语法的话，这将何有帮助。例如，某些人发现通过 HTML 标签添加图像更加容易。当你需要更改元素的属性时（例如为文本指定颜色或更改图像的宽度），使用 HTML 标签更方便些。</p>

<p>如需使用 HTML，请将 HTML 标签添加到 Markdown 格式文本中即可。</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>This **word** is bold. This &lt;em&gt;word&lt;/em&gt; is italic.
</code></pre></div></div>

<p>渲染效果如下：</p>

<p>This <strong>word</strong> is bold. This <em>word</em> is italic.</p>

<h3 id="html-用法最佳实践">HTML 用法最佳实践<a class="anchorjs-link " aria-label="Anchor" data-anchorjs-icon="" href="https://www.markdown.xyz/basic-syntax/#html-%E7%94%A8%E6%B3%95%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>

<p>出于安全原因，并非所有 Markdown 应用程序都支持在 Markdown 文档中添加 HTML。如有疑问，请查看 Markdown 应用程序的文档。某些应用程序只支持 HTML 标签的子集。</p>

<p>对于 HTML 的块级元素 <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code>、<code class="language-plaintext highlighter-rouge">&lt;table&gt;</code>、<code class="language-plaintext highlighter-rouge">&lt;pre&gt;</code> 和 <code class="language-plaintext highlighter-rouge">&lt;p&gt;</code>，请在其前后使用空行（blank lines）与其它内容进行分隔。尽量不要使用制表符（tabs）或空格（spaces）对 HTML 标签做缩进，否则将影响格式。</p>

<p>在 HTML 块级标签内不能使用 Markdown 语法。例如 <code class="language-plaintext highlighter-rouge">&lt;p&gt;italic and **bold**&lt;/p&gt;</code> 将不起作用。</p>
