<!-- Seção de Apresentação das Trilhas -->
<div class="trilhas-intro">
  <h2>Trilhas de Conhecimento</h2>
  <p>
    Acredito que o conhecimento deve ser estruturado e prático. Criei estas trilhas como guias detalhados, cobrindo desde os fundamentos até o nível de especialista, para organizar meus estudos e compartilhar a jornada com a comunidade.
  </p>
</div>

<!-- Container dos Cards das Trilhas -->
<div class="cards-container">
  <!-- Card de SQL -->
  <a href="sql.html" class="card">
    <h3>🚀 SQL: A Linguagem dos Dados</h3>
    <p>O guia definitivo para extrair, manipular e otimizar dados. Essencial para qualquer profissional que queira construir uma base sólida em análise de dados.</p>
  </a>

  <!-- Card de Power BI -->
  <a href="powerbi.html" class="card">
    <h3>📊 Power BI: Da Análise à Ação</h3>
    <p>Construa dashboards que contam histórias e geram insights. Um roadmap focado na preparação para a certificação oficial da Microsoft (PL-300).</p>
  </a>

  <!-- Card de Inglês -->
  <a href="ingles.html" class="card">
    <h3>🌐 Inglês: Fluência Profissional</h3>
    <p>O roadmap completo para a fluência, do nível intermediário à maestria (B1 ao C2), com foco na comunicação para o ambiente de trabalho global.</p>
  </a>
</div>

<!-- Estilos para a Seção de Trilhas e Cards -->
<style>
  .trilhas-intro {
    text-align: center;
    margin-top: 40px;
    margin-bottom: 40px;
  }
  .trilhas-intro h2 {
    font-size: 2em;
    margin-bottom: 10px;
  }
  .trilhas-intro p {
    font-size: 1.1em;
    color: #555;
    max-width: 700px;
    margin-left: auto;
    margin-right: auto;
  }

  .cards-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); /* Layout responsivo */
    gap: 20px; /* Espaço entre os cards */
    margin-bottom: 40px;
  }
  .card {
    display: block;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 25px;
    text-decoration: none;
    color: inherit;
    transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
  }
  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  }
  .card h3 {
    margin-top: 0;
    font-size: 1.4em;
  }
  .card p {
    font-size: 1em;
    line-height: 1.5;
  }
</style>
