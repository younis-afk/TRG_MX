# TRG_MX
https://github.com/username/my-webs
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>TRG_MX - Contact</title>
  <style>
    body{
      font-family: system-ui, -apple-system, "Segoe UI", Roboto, "Noto Sans", "Helvetica Neue", Arial;
      background:#f7fafc;
      color:#111827;
      display:flex;
      min-height:100vh;
      align-items:center;
      justify-content:center;
      padding:20px;
    }
    .card{
      background:white;
      border-radius:12px;
      box-shadow: 0 6px 18px rgba(15,23,42,0.08);
      max-width:420px;
      width:100%;
      padding:20px;
    }
    h1{ margin:0 0 10px 0; font-size:20px; }
    .meta{ color:#6b7280; margin-bottom:14px; font-size:14px; }
    label{ display:block; margin-top:10px; font-size:13px; color:#374151; }
    input[type="text"], input[type="email"], input[type="tel"], textarea{
      width:100%;
      padding:10px 12px;
      margin-top:6px;
      border:1px solid #e5e7eb;
      border-radius:8px;
      font-size:14px;
      box-sizing:border-box;
    }
    button{
      margin-top:14px;
      width:100%;
      padding:10px 12px;
      border-radius:8px;
      border:0;
      background:#111827;
      color:white;
      font-weight:600;
      cursor:pointer;
    }
    .small{ font-size:13px; color:#6b7280; margin-top:8px; text-align:center; }
  </style>
</head>
<body>
  <div class="card" role="main">
    <h1>TRG_MX — Contact Form</h1>
    <div class="meta">This code works directly on mobile — name, phone, and email are pre-filled.</div>

    <form id="contactForm" onsubmit="return handleSubmit(event);">
      <label for="name">Name</label>
      <input id="name" name="name" type="text" value="TRG_MX" required>

      <label for="phone">Phone Number</label>
      <input id="phone" name="phone" type="tel" value="+919596661366" required>

      <label for="email">Email</label>
      <input id="email" name="email" type="email" value="younislone259@gmail.com" required>

      <label for="message">Message (optional)</label>
      <textarea id="message" name="message" rows="4" placeholder="Write your message here..."></textarea>

      <button type="submit">Send</button>
    </form>

    <div class="small">The form is handled locally — no server required.</div>
  </div>

  <script>
    function handleSubmit(e){
      e.preventDefault();
      const name = document.getElementById('name').value;
      const phone = document.getElementById('phone').value;
      const email = document.getElementById('email').value;
      const message = document.getElementById('message').value;
      alert(
        "Details:\n\n" +
        "Name: " + name + "\n" +
        "Phone: " + phone + "\n" +
        "Email: " + email + "\n\n" +
        "Message: " + (message || "(No message)")
      );
      return false;
    }
  </script>
</body>
</html>
