[santuary copy.html](https://github.com/user-attachments/files/25220513/santuary.copy.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SANTUARIO – Private Circle</title>

  <!-- Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;600&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">

  <style>
    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: #f7f7f7;
      color: #1a1a1a;
    }

    .wrapper {
      max-width: 480px;
      margin: 0 auto;
      padding: 3rem 1.5rem 4rem;
    }

    .logo {
      font-family: 'Playfair Display', serif;
      font-size: 2.2rem;
      letter-spacing: 0.25em;
      text-align: center;
      margin-bottom: 2rem;
    }

    .title {
      font-size: 1.6rem;
      text-align: center;
      margin-bottom: 1.2rem;
    }

    .description {
      font-size: 0.95rem;
      line-height: 1.7;
      text-align: center;
      color: #555;
      margin-bottom: 2rem;
    }

    ul {
      padding-left: 1.2rem;
      margin-bottom: 2rem;
      color: #555;
      font-size: 0.9rem;
    }

    ul li { margin-bottom: 0.6rem; }

    .note {
      font-size: 0.75rem;
      color: #777;
      text-align: center;
      margin-bottom: 2rem;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    input {
      padding: 0.9rem;
      font-size: 0.9rem;
      border: 1px solid #ddd;
      border-radius: 6px;
      font-family: inherit;
    }

    .row {
      display: flex;
      gap: 0.8rem;
    }

    .row input { flex: 1; }

    button {
      margin-top: 1.5rem;
      padding: 1rem;
      background: #000;
      color: #fff;
      border: none;
      border-radius: 999px;
      font-size: 0.85rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      cursor: pointer;
    }

    #confirmation {
      text-align: center;
      margin-top: 3rem;
      font-size: 1.1rem;
      letter-spacing: 0.05em;
    }

    footer {
      text-align: center;
      font-size: 0.65rem;
      letter-spacing: 0.2em;
      margin-top: 3rem;
      color: #999;
    }
  </style>
</head>

<body>

  <div class="wrapper">
    <div class="logo">SANTUARIO</div>

    <div class="title">Apply for Santuario's private circle.</div>

    <div class="description">
      Members of our private circle will be the first to receive:
    </div>

    <ul>
      <li>Early access to upcoming gatherings.</li>
      <li>Limited invitations & curated experiences.</li>
      <li>Access to private and invite-only events.</li>
    </ul>

    <div class="note">
      By signing up you consent to receive communications from Santuario.
    </div>

    <!-- FORM -->
    <form
      id="privateForm"
      action="https://docs.google.com/forms/d/e/1FAIpQLSd34aC83ii4R4KAPWt_uHXAs-GOezFUjTDSEDuBe8FcKIteRg/formResponse"
      method="POST"
      target="hidden_iframe"
      onsubmit="handleSubmit(event)"
    >

      <input type="email" name="entry.1683057520" placeholder="Your email address" required />

      <div class="row">
        <input type="text" name="entry.1961090126" placeholder="First name" />
        <input type="text" name="entry.1084424661" placeholder="Last name" />
      </div>

      <input type="tel" name="entry.1028863654" placeholder="Mobile number" />
      <input type="text" name="entry.148267164" placeholder="Instagram" />
      <input type="text" name="entry.783334638" placeholder="LinkedIn (optional)" />

      <button type="submit">APPLY</button>
    </form>

    <!-- CONFIRMATION -->
    <div id="confirmation" style="display:none;">
      You’ll hear from us.
    </div>

    <footer>
      INVITE ONLY · MUSIC FIRST · SANTUARIO
    </footer>
  </div>

  <!-- HIDDEN IFRAME -->
  <iframe name="hidden_iframe" style="display:none;"></iframe>

  <script>
    function handleSubmit(event) {
      document.getElementById("privateForm").style.display = "none";
      document.getElementById("confirmation").style.display = "block";
    }
  </script>

</body>
</html>
