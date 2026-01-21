
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Minha Página</title>

    <!-- CSS INTERNO -->
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #eef2f3;
            padding: 20px;
        }

        h1 {
            text-align: center;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: #fff;
            margin-bottom: 30px;
        }

        th, td {
            border: 1px solid #333;
            padding: 12px;
            vertical-align: top;
        }

        th {
            background-color: #ddd;
        }

        .home {
            background-color: #cce5ff;
            font-weight: bold;
            text-align: center;
        }

        input, button {
            padding: 6px;
            margin-top: 5px;
        }

        .externo {
            background-color: lightyellow;
            padding: 10px;
        }
    </style>

    <!-- CSS EXTERNO (simulado no mesmo arquivo) -->
    <link rel="stylesheet" href="#">
</head>
<body>

<h1>Bem-vindo à minha página</h1>

<table>
    <tr>
        <th>Home</th>
        <th>Primeiro Trimestre</th>
        <th>Segundo Trimestre</th>
        <th>Terceiro / Fim</th>
    </tr>

    <tr>
        <!-- HOME -->
        <td class="home">
            HOME<br><br>
            T2<br>
            T3<br>
            T4<br>
            T5
        </td>

        <!-- PRIMEIRO TRIMESTRE -->
        <td>
            <strong>T1 – Enviar link do Git</strong><br>
            <input type="text" id="gitLink" placeholder="Cole o link do GitHub">
            <button onclick="enviarGit()">Enviar</button>
            <p id="resultadoGit"></p>

            <hr>

            <strong>T2 – Formulário Pessoal</strong><br>
            <form>
                Nome:<br>
                <input type="text"><br>
                Email:<br>
                <input type="email"><br>
                Idade:<br>
                <input type="number"><br>
                <button type="submit">Enviar</button>
            </form>

            <hr>

            <strong>T3 – Tabela</strong>
            <table>
                <tr>
                    <th>Nome</th>
                    <th>Curso</th>
                </tr>
                <tr>
                    <td>Ana</td>
                    <td>Informática</td>
                </tr>
                <tr>
                    <td>João</td>
                    <td>Web</td>
                </tr>
            </table>

            <hr>

            <strong>T4 – Imagem, Vídeo e Áudio</strong><br>
            <input type="file" accept="image/*"><br><br>
            <input type="file" accept="video/*"><br><br>
            <input type="file" accept="audio/*">
        </td>

        <!-- SEGUNDO TRIMESTRE -->
        <td>
            <strong>T1 – O que é CSS</strong>
            <p>
                CSS (Cascading Style Sheets) é uma linguagem usada para estilizar páginas HTML,
                definindo cores, tamanhos, fontes e layout.
            </p>

            <strong>T2 – Importância do CSS</strong>
            <p>
                O CSS separa o conteúdo do design, deixando o site mais bonito,
                organizado e fácil de manter.
            </p>

            <strong>T3 – Tipos de CSS</strong>
            <ul>
                <li>CSS Inline</li>
                <li>CSS Interno</li>
                <li>CSS Externo</li>
            </ul>

            <strong>T4 – Página com tipos de CSS</strong>

            <!-- CSS INLINE -->
            <p style="color: red;">
                Este texto usa CSS INLINE.
            </p>

            <!-- CSS INTERNO -->
            <p>
                Este texto usa CSS INTERNO.
            </p>

            <!-- CSS EXTERNO -->
            <p class="externo">
                Este texto representa CSS EXTERNO (fundo definido).
            </p>
        </td>

        <!-- TERCEIRO / FIM -->
        <td>
            Fim do Trimestre
        </td>
    </tr>
</table>

<script>
    function enviarGit() {
        const link = document.getElementById("gitLink").value;
        document.getElementById("resultadoGit").innerHTML =
            "Link enviado: <a href='" + link + "' target='_blank'>" + link + "</a>";
    }
</script>
