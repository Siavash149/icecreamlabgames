---
layout: page
title: Contact Us
eyebrow: Say hello
subtitle: Partnerships, press, or general inquiries
---

<div class="section">
<div style="display:grid;grid-template-columns:1fr 1fr;gap:5rem;align-items:start">

<div>
  <h2 style="font-size:1.5rem;margin-bottom:1rem">Let's talk</h2>
  <p style="color:var(--muted);margin-bottom:2.5rem;font-size:0.95rem">
    Whether you're a player needing help, a publisher exploring collaboration, or a developer interested in working with us — we'd love to hear from you.
  </p>

  <div style="display:flex;flex-direction:column;gap:1.5rem">
    <div style="display:flex;gap:1rem;align-items:flex-start">
      <div style="width:40px;height:40px;border-radius:10px;background:var(--pink-200);display:flex;align-items:center;justify-content:center;font-size:1.1rem;flex-shrink:0">✉</div>
      <div>
        <div style="font-size:0.8rem;font-weight:600;color:var(--muted);margin-bottom:2px">General inquiries</div>
        <a href="mailto:{{ site.data.settings.contact_email }}" style="color:var(--text);font-size:0.95rem">{{ site.data.settings.contact_email }}</a>
      </div>
    </div>
    <div style="display:flex;gap:1rem;align-items:flex-start">
      <div style="width:40px;height:40px;border-radius:10px;background:var(--pink-200);display:flex;align-items:center;justify-content:center;font-size:1.1rem;flex-shrink:0">🎮</div>
      <div>
        <div style="font-size:0.8rem;font-weight:600;color:var(--muted);margin-bottom:2px">Player support</div>
        <a href="/support/" style="color:var(--text);font-size:0.95rem">Visit our Support page</a>
      </div>
    </div>
    <div style="display:flex;gap:1rem;align-items:flex-start">
      <div style="width:40px;height:40px;border-radius:10px;background:var(--pink-200);display:flex;align-items:center;justify-content:center;font-size:1.1rem;flex-shrink:0">▶</div>
      <div>
        <div style="font-size:0.8rem;font-weight:600;color:var(--muted);margin-bottom:2px">Our games on</div>
        <a href="{{ site.data.settings.play_store_url }}" target="_blank" style="color:var(--text);font-size:0.95rem">Google Play ↗</a>
      </div>
    </div>
  </div>

  <div style="margin-top:3rem;padding:1.5rem;background:var(--pink-100);border-radius:var(--r);border:1px solid var(--border)">
    <div style="font-family:'Playfair Display',serif;font-size:1rem;font-weight:600;margin-bottom:0.5rem">Response time</div>
    <p style="font-size:0.85rem;color:var(--muted);margin:0">We're a small team. We read every message and respond within <strong>1–3 business days</strong>.</p>
  </div>
</div>

<div>
  <div class="form-card">
    <form action="mailto:{{ site.data.settings.contact_email }}" method="GET">
      <div class="form-row">
        <div class="form-group">
          <label>Name</label>
          <input type="text" name="name" placeholder="Your name" required>
        </div>
        <div class="form-group">
          <label>Email</label>
          <input type="email" name="email" placeholder="you@email.com" required>
        </div>
      </div>
      <div class="form-group">
        <label>Subject</label>
        <select name="subject">
          <option value="">Select topic…</option>
          <option>Partnership / Publishing</option>
          <option>Press / Media inquiry</option>
          <option>Business inquiry</option>
          <option>Join the team</option>
          <option>Player support</option>
          <option>Other</option>
        </select>
      </div>
      <div class="form-group">
        <label>Message</label>
        <textarea name="body" placeholder="Tell us what's on your mind…" style="min-height:140px" required></textarea>
      </div>
      <button type="submit" class="btn btn-primary" style="width:100%;justify-content:center">Send message</button>
    </form>
  </div>
</div>

</div>
</div>
