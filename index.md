<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Michel França - Hub de Conhecimento</title>
    <style>
        /* Estilos Gerais */
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 800px;
            margin: 40px auto;
            padding: 0 20px;
        }

        /* Estilos da Biografia */
        .bio-container {
            display: flex;
            align-items: center;
            gap: 30px;
            padding-bottom: 40px;
            border-bottom: 1px solid #e0e0e0;
            margin-bottom: 40px;
        }
        .bio-image img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
        }
        .bio-text h1 {
            margin-top: 0;
            margin-bottom: 5px;
            font-size: 2.5em;
        }
        .bio-text h2 {
            margin-top: 0;
            margin-bottom: 20px;
            font-size: 1.2em;
            font-weight: 400;
            color: #555;
        }
        .bio-text p {
            font-size: 1.1em;
        }

        /* Estilos dos Botões */
        .button-container {
            display: flex;
            flex-direction: column;
            gap: 15px;
            align-items: center;
        }
        .button-link {
            display: block;
            width: 80%;
            max-width: 400px;
            padding: 15px 20px;
            border: 1px solid #333;
            border-radius: 5px;
            text-align: center;
            text-decoration: none;
            color: #333;
            font-size: 1.1em;
            font-weight: bold;
            transition: all 0.2s ease-in-out;
        }
        .button-link:hover {
            background-color: #333;
            color: #fff;
        }

        /* Ajuste para telas pequenas */
        @media (max-width: 600px) {
            .bio-container {
                flex-direction: column;
                text-align: center;
            }
        }
    </style>
</head>
<body>

    <div class="bio-container">
      <div class="bio-image">
        <!-- Lembre-se de fazer o upload da sua foto para a pasta 'assets' com o nome 'profile.jpg' -->
        <img src="assets/profile.jpg" alt="Foto de Michel França">
      </div>
      <div class="bio-text">
        <h1>Michel França</h1>
        <h2>Especialista em Dados & Business Intelligence</h2>
        <p>
          Profissional apaixonado por transformar dados brutos em insights de negócio que geram valor e direcionam decisões estratégicas. Com sólida experiência em SQL e Power BI, meu foco é construir soluções de dados eficientes, desde a engenharia e modelagem até a criação de dashboards interativos.
        </p>
      </div>
    </div>

    <div class="button-container">
      <a href="trilhas.html" class="button-link">
        Trilhas de Conhecimento
      </a>
      <a href="projetos.html" class="button-link">
        Portfólio de Projetos
      </a>
      <a href="curriculo.html" class="button-link">
        Currículo
      </a>
      <a href="mailto:seu-email@provedor.com" class="button-link">
        Contato
      </a>
    </div>

</body>
</html>
