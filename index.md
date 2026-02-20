<div class="bio-container">
  <div class="bio-image">
    <img src="assets/profile.jpg" alt="Foto de Michel França">
  </div>
  <div class="bio-text">
    <h1>Michel França</h1>
    <h2>Especialista em Dados & Business Intelligence</h2>
    <p>
      Profissional apaixonado por transformar dados brutos em insights de negócio que geram valor e direcionam decisões estratégicas. Com sólida experiência em SQL e Power BI, meu foco é construir soluções de dados eficientes, desde a engenharia e modelagem até a criação de dashboards interativos.
    </p>
    <p>
      Bem-vindo ao meu portfólio, um espaço onde compartilho projetos, guias de estudo e minha jornada de aprendizado contínuo no mundo dos dados.
    </p>
  </div>
</div>

[Sobre Mim no LinkedIn](https://www.linkedin.com/in/michel-fran%C3%A7a-346b24309/ )

/* Estilos da Biografia */
.bio-container {
  display: flex;
  align-items: center;
  gap: 30px;
  padding: 20px;
  border-bottom: 1px solid #e0e0e0;
  margin-bottom: 40px;
}
.bio-image img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
}
.bio-text h1 { margin-top: 0; margin-bottom: 5px; font-size: 2.5em; }
.bio-text h2 { margin-top: 0; margin-bottom: 20px; font-size: 1.2em; font-weight: 400; color: #555; }
.bio-text p { font-size: 1.1em; line-height: 1.6; }

/* Estilos dos Botões */
.button-container {
  display: flex;
  flex-direction: column;
  gap: 15px;
  margin-top: 40px;
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

