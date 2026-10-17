```html
<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Escudo Banco | Segurança Digital</title>
  <style>
    :root {
      --navy: #071a33;
      --blue: #1268ed;
      --cyan: #27d5de;
      --ink: #17243b;
      --muted: #5d6b80;
      --pale: #f4f8ff;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      color: var(--ink);
      background: #fff;
    }

    .container {
      width: min(1120px, calc(100% - 40px));
      margin: auto;
    }

    header {
      background: var(--navy);
      color: white;
    }

    nav {
      height: 80px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      color: white;
      text-decoration: none;
      font-size: 20px;
      font-weight: bold;
    }

    .logo span { color: var(--cyan); }

    nav a {
      color: #c7d5ed;
      text-decoration: none;
      margin-left: 20px;
      font-size: 14px;
    }

    .button {
      display: inline-block;
      padding: 13px 20px;
      border-radius: 8px;
      background: var(--blue);
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    .hero {
      padding: 90px 0;
      color: white;
      background: radial-gradient(circle at right top, #0f579c, #071a33 60%);
    }

    .hero-content {
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 60px;
      align-items: center;
    }

    .tag {
      display: inline-block;
      margin-bottom: 18px;
      padding: 7px 12px;
      border: 1px solid #42dce8;
      border-radius: 30px;
      color: #8af7fb;
      font-size: 12px;
      font-weight: bold;
      text-transform: uppercase;
    }

    h1 {
      margin: 0;
      font-size: clamp(40px, 5vw, 70px);
      line-height: 1.05;
    }

    .hero p {
      max-width: 560px;
      color: #c6d8f1;
      line-height: 1.7;
      font-size: 18px;
    }

    .security-box {
      padding: 30px;
      border: 1px solid #70e6ef55;
      border-radius: 18px;
      background: #ffffff12;
    }

    .security-box small {
      color: #baf8fb;
      text-transform: uppercase;
      font-weight: bold;
    }

    .score {
      margin: 20px 0;
      font-size: 62px;
      font-weight: bold;
    }

    .bar {
      height: 10px;
      border-radius: 20px;
      overflow: hidden;
      background: #ffffff33;
    }

    .bar div {
      width: 94%;
      height: 100%;
      background: linear-gradient(90deg, var(--cyan), #64efa9);
    }

    .status {
      margin-top: 20px;
      color: #dce8fb;
      font-size: 14px;
    }

    .status strong { color: #6bf2a6; }

    section.features {
      padding: 80px 0;
      background: var(--pale);
    }

    .eyebrow {
      color: var(--blue);
      font-size: 12px;
      font-weight: bold;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    h2 {
      max-width: 650px;
      margin: 12px 0 40px;
      font-size: 42px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 18px;
    }

    .card {
      padding: 28px;
      border: 1px solid #dce7fa;
      border-radius: 14px;
      background: white;
    }

    .icon {
      width: 50px;
      height: 50px;
      display: grid;
      place-items: center;
      margin-bottom: 20px;
      border-radius: 12px;
      background: #e9f2ff;
      color: var(--blue);
      font-size: 24px;
    }

    .card h3 { margin: 0 0 12px; }

    .card p {
      margin: 0;
      color: var(--muted);
      line-height: 1.6;
    }

    .tips {
      padding: 80px 0;
    }

    .tips-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 70px;
    }

    .tips p {
      color: var(--muted);
      line-height: 1.7;
    }

    ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }

    li {
      position: relative;
      margin-bottom: 14px;
      padding: 18px 20px 18px 50px;
      border: 1px solid #dde6f2;
      border-radius: 10px;
      font-weight: bold;
    }

    li::before {
      content: "✓";
      position: absolute;
      left: 18px;
      color: #0aa67a;
      font-size: 20px;
    }

    .cta {
      padding: 65px 0;
      text-align: center;
      background: var(--blue);
      color: white;
    }

    .cta h2 {
      max-width: none;
      margin-bottom: 15px;
    }

    .cta p {
      margin: 0 auto 25px;
      max-width: 550px;
      color: #dce9ff;
      line-height: 1.6;
    }

    .cta .button {
      background: white;
      color: var(--navy);
    }

    footer {
      padding: 28px 0;
      color: #9db2d3;
      background: #06152b;
      font-size: 14px;
    }

    @media (max-width: 760px) {
      nav div { display: none; }

      .hero-content,
      .tips-grid,
      .cards {
        grid-template-columns: 1fr;
      }

      .hero-content { gap: 40px; }
      h2 { font-size: 32px; }
    }
  </style>
</head>
<body>

  <header>
    <nav class="container">
      <a href="#" class="logo"><span>◈</span> ESCUDO BANCO</a>
      <div>
        <a href="#protecao">Proteção</a>
        <a href="#dicas">Dicas de segurança</a>
        <a href="#ajuda">Ajuda</a>
      </div>
      <a class="button" href="#ajuda">Reportar fraude</a>
    </nav>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-content">
        <div>
          <span class="tag">Proteção digital 24 horas</span>
          <h1>Seu dinheiro merece uma defesa inteligente.</h1>
          <p>
            Monitoramento contínuo, alertas em tempo real e tecnologia avançada
            para proteger cada acesso e transação da sua conta.
            A proteção cibernética contra invasões de hackers é um dos pilares mais fundamentais para garantir a segurança da informação, a privacidade individual e a estabilidade das instituições na era digital.

O Impacto das Invasões de Hackers

A ação de cibercriminosos vai muito além do comprometimento técnico de sistemas; ela causa danos diretos e profundos à sociedade:

* **Violação da Privacidade:** A invasão de sistemas expõe dados pessoais sensíveis, como documentos, informações financeiras e históricos médicos, deixando indivíduos vulneráveis a fraudes, extorsões e roubo de identidade.
* **Prejuízos Econômicos:** Empresas e órgãos públicos enfrentam paralisações operacionais, perdas financeiras massivas e custos elevados para recuperação de infraestruturas afetadas por sequestro de dados (*ransomware*).
* **Ameaça à Segurança Nacional:** Ataques a infraestruturas críticas — como redes elétricas, sistemas de abastecimento de água, hospitais e redes bancárias — colocam a segurança pública e vidas humanas em risco direto.
* **Quebra de Confiança:** O vazamento ilícito de informações corrói a confiança entre clientes, empresas e governos, prejudicando o desenvolvimento econômico e a inovação tecnológica.

**Diferença Entre Hacker Ético e Cibercriminoso**

É fundamental diferenciar a invasão maliciosa do trabalho realizado por profissionais de segurança:

* **Cibercriminosos (Black Hats):** Acessam sistemas sem autorização com o objetivo de roubar dados, extorquir vítimas, causar destruição ou obter vantagem financeira ilícita.
* **Hackers Éticos (White Hats):** Atuam com autorização prévia para identificar vulnerabilidades e falhas de segurança, ajudando a fortalecer as defesas de uma organização antes que sejam exploradas maliciosamente.

**Promovendo a Cultura de Segurança**

Combater invasões cibernéticas exige um esforço contínuo que combina conscientização, políticas públicas rigorosas e investimento em tecnologia. Práticas essenciais para mitigar esses riscos incluem:

* **Uso de Autenticação Forte:** Implementação obrigatória de verificação em duas etapas (2FA) e senhas complexas e exclusivas.
* **Atualização Contínua:** Manutenção de softwares, firmware e sistemas operacionais sempre atualizados para corrigir brechas de segurança conhecidas.
* **Educação e Conscientização:** Treinamento constante contra técnicas de engenharia social, como *phishing*, que visam enganar usuários para obter credenciais de acesso.
* **Criptografia e Encurtamento de Superfície de Ataque:** Proteção de dados em trânsito e em repouso, limitando o acesso a informações apenas a pessoal estritamente autorizado.

A segurança cibernética não é um estado estático, mas um compromisso ativo e diário para preservar a integridade do ambiente digital.
          </p>
          <a class="button" href="#protecao">Conheça a proteção</a>
        </div>

        <div class="security-box">
          <small>Nível de proteção da conta</small>
          <div class="score">94</div>
          <div class="bar"><div></div></div>
          <p class="status"><strong>● Proteção ativa</strong><br>Atualizado agora</p>
        </div>
      </div>
    </section>

    <section class="features" id="protecao">
      <div class="container">
        <span class="eyebrow">Segurança que trabalha por você</span>
        <h2>Camadas de defesa para sua vida financeira.</h2>

        <div class="cards">
          <article class="card">
            <div class="icon">◈</div>
            <h3>Detecção de fraudes</h3>
            <p>Identificamos padrões suspeitos para bloquear movimentações incomuns antes que causem prejuízo.</p>
          </article>

          <article class="card">
            <div class="icon">⌁</div>
            <h3>Alertas instantâneos</h3>
            <p>Receba notificações sempre que houver um novo acesso, pagamento ou alteração na sua conta.</p>
          </article>

          <article class="card">
            <div class="icon">▣</div>
            <h3>Acesso protegido</h3>
            <p>Autenticação em duas etapas e criptografia protegem seus dados em cada conexão.</p>
          </article>
        </div>
      </div>
    </section>

    <section class="tips" id="dicas">
      <div class="container tips-grid">
        <div>
          <span class="eyebrow">Sua segurança começa com você</span>
          <h2>Golpistas evoluem. Seus hábitos também devem evoluir.</h2>
          <p>
            Nunca compartilhe senhas, códigos de confirmação ou dados do cartão.
            Bancos não pedem essas informações por ligação ou mensagem.
          </p>
        </div>

        <ul>
          <li>Confira o endereço do site antes de acessar sua conta.</li>
          <li>Desconfie de links e ofertas urgentes recebidas por mensagem.</li>
          <li>Use senhas exclusivas e ative a verificação em duas etapas.</li>
          <li>Em caso de dúvida, use apenas os canais oficiais do banco.</li>
        </ul>
      </div>
    </section>

    <section class="cta" id="ajuda">
      <div class="container">
        <h2>Percebeu algo fora do normal?</h2>
        <p>Bloqueie sua conta e entre em contato com a central de segurança imediatamente.</p>
        <a class="button" href="tel:08000000000">Ligar para 0800 000 0000</a>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      © 2026 Escudo Banco — Segurança em primeiro lugar.
    </div>
  </footer>

</body>
</html>
```
