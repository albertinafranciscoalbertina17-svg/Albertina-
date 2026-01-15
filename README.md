DOCTYPE html>
<html lang="pt">
<head>
<meta charset="UTF-8">
<title>Tabela HOME</title>
<style>
body {
    font-family: Arial, sans-serif;
    padding: 20px;
}
table {
    width: 100%;
    border-collapse: collapse;
}
th, td {
    border: 1px solid #000;
    padding: 10px;
    vertical-align: top;
}
th {
    background-color: #f0f0f0;
    text-align: center;
}
textarea {
    width: 100%;
    height: 80px;
}
button {
    margin-top: 5px;
}
</style>

<script>
function copyText(id) {
    let text = document.getElementById(id);
    text.select();
    document.execCommand("copy");
    alert("Código copiado!");
}
</script>
</head>

<body>

<table>
<tr>
    <th>HOME</th>
    <th>1º Trimestre</th>
    <th>2º Trimestre</th>
    <th>3º Trimestre</th>
    <th>Fim</th>
</tr>

<!-- T2 -->
<tr>
<th>T2</th>
<td>
    🔗 Enviar links visitados<br>
    <input type="text" placeholder="Cole aqui o link"><br><br>

    📎 Enviar ficheiro<br>
    <input type="file"><br><br>

    💻 Código<br>
    <textarea id="c1"></textarea>
    <button onclick="copyText('c1')">Copiar</button>
</td>
<td>O que é CSS?
é uma linguagem,usado para difinir a parência de estilo da pagina web.como titulo,texto,imagens,entre outros.</td>
<td></td>
<td></td>
</tr>

<!-- T3 -->
<tr>
<th>T3</th>
<td>
    📝 Fazer formulário pessoal<br>
    <input type="text" placeholder="Nome"><br>
    <input type="email" placeholder="Email"><br>
</td>
<td>A importância do CSS,é fundamental no desenvolvimento web,porque css transforma uma pagina simples em uma experência bonita.</td>
<td></td>
<td></td>
</tr>

<!-- T4 -->
<tr>
<th>T4</th>
<td>
    📊 Criar tabela<br>
    <textarea id="c2"></textarea>
    <button onclick="copyText('c2')">Copiar</button>
</td>
<td>Os tipos de CSS,inline,interno,externo,
inline,ajustes rápido,interno,pagina única,externo sites profissionais.</td>
<td></td>
<td></td>
</tr>

<!-- T5 -->
<tr>
<th>T5</th>
<td>
    🖼️ Criar página com imagem, áudio e vídeo<br><br>
    Imagem: <input type="file"><br><br>
    Áudio: <input type="file"><br><br>
    Vídeo: <input type="file">
</td>
<td></td>
<td></td>
<td></td>
</tr>

</table>

</body>
</html>