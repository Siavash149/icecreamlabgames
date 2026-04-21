---
layout: page
title: Support
eyebrow: Help Center
subtitle: Answers to common questions — or reach us directly
---

<div class="section">
<div style="display:grid;grid-template-columns:1.1fr 0.9fr;gap:5rem;align-items:start">

<div>
<div class="section-head" style="margin-bottom:2rem">
  <div class="eyebrow">FAQ</div>
  <h2 style="font-size:1.6rem">Common questions</h2>
</div>

<div class="faq-item">
  <div class="faq-q">Why can't I connect to the game server?</div>
  <div class="faq-a">Check your internet connection first. If you're on mobile data, try switching to Wi-Fi. Our servers can occasionally be under maintenance. Restarting the app usually resolves temporary connection issues.</div>
</div>

<div class="faq-item">
  <div class="faq-q">I lost my progress / account. Can it be recovered?</div>
  <div class="faq-a">If you were signed in with a Google account, your progress is linked to that account and should restore automatically on a new device. If you played as a guest, unfortunately guest data cannot be recovered after uninstalling. We recommend signing in with Google to keep your progress safe.</div>
</div>

<div class="faq-item">
  <div class="faq-q">How do I report a cheater or abusive player?</div>
  <div class="faq-a">Use the in-game report button next to the player's profile, or send us an email with the player's username and a description of the behavior. We review all reports and take action on confirmed violations.</div>
</div>

<div class="faq-item">
  <div class="faq-q">I made an in-app purchase but didn't receive the item.</div>
  <div class="faq-a">First, restart the app — purchases sometimes take a moment to sync. If the item still hasn't appeared after a few minutes, contact us with your order ID from Google Play. We'll resolve it promptly.</div>
</div>

<div class="faq-item">
  <div class="faq-q">How do I request a refund?</div>
  <div class="faq-a">Refunds for in-app purchases are processed through Google Play. Visit <a href="https://play.google.com/store/account/orderhistory" target="_blank" style="color:var(--pink-500)">play.google.com/store/account/orderhistory</a>, find your order, and request a refund through Google's system.</div>
</div>

<div class="faq-item">
  <div class="faq-q">The game crashes on my device. What should I do?</div>
  <div class="faq-a">Make sure you're on the latest version of the game. Try clearing the app cache (Settings → Apps → [Game] → Clear Cache) and restarting. If the problem continues, please contact us with your device model and Android version.</div>
</div>

<div class="faq-item">
  <div class="faq-q">How do I delete my account and data?</div>
  <div class="faq-a">Send us an email at support@icecreamlabgames.com with your username and the subject "Account Deletion Request". We'll process your request within 14 days and confirm by email.</div>
</div>

<div class="faq-item">
  <div class="faq-q">I have a suggestion for the game.</div>
  <div class="faq-a">We love hearing from players! Use the contact form or send us an email. We read every suggestion and many features in our games came directly from player feedback.</div>
</div>

</div>

<div style="position:sticky;top:80px">
  <div class="form-card">
    <div class="eyebrow" style="margin-bottom:0.75rem">Still need help?</div>
    <h3 style="font-size:1.2rem;margin-bottom:0.5rem">Contact support</h3>
    <p style="font-size:0.85rem;color:var(--muted);margin-bottom:1.75rem">We usually respond within 24–48 hours.</p>
    <form action="mailto:support@icecreamlabgames.com" method="GET">
      <div class="form-group">
        <label>Your name</label>
        <input type="text" name="name" placeholder="Your name" required>
      </div>
      <div class="form-group">
        <label>Email address</label>
        <input type="email" name="email" placeholder="you@email.com" required>
      </div>
      <div class="form-group">
        <label>Which game?</label>
        <select name="game">
          <option value="">Select a game…</option>
          {% for game in site.data.games %}
          <option>{{ game.name }}</option>
          {% endfor %}
          <option>Other / General</option>
        </select>
      </div>
      <div class="form-group">
        <label>Message</label>
        <textarea name="body" placeholder="Describe your issue…" required></textarea>
      </div>
      <button type="submit" class="btn btn-primary" style="width:100%;justify-content:center">Send message</button>
    </form>
    <p style="font-size:0.75rem;color:var(--muted);margin-top:1rem;text-align:center">
      Or email: <a href="mailto:support@icecreamlabgames.com" style="color:var(--pink-500)">support@icecreamlabgames.com</a>
    </p>
  </div>
</div>

</div>
</div>
