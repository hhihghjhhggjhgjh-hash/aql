<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>عقل — AQL</title>
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800;900&display=swap" rel="stylesheet">
<style>
  :root {
    --black: #080808;
    --gold: #c9a84c;
    --gold-dim: rgba(201,168,76,0.15);
    --gold-border: rgba(201,168,76,0.3);
    --white: #f0ece4;
    --muted: rgba(240,236,228,0.45);
  }
  * { margin: 0; padding: 0; box-sizing: border-box; }
  html, body {
    min-height: 100vh;
    background: var(--black);
    font-family: 'Tajawal', sans-serif;
    color: var(--white);
    overflow-x: hidden;
  }
  body::before {
    content: '';
    position: fixed;
    inset: 0;
    background: radial-gradient(ellipse 60% 40% at 50% 0%, rgba(201,168,76,0.08) 0%, transparent 70%);
    pointer-events: none;
    z-index: 0;
  }
  .container {
    position: relative;
    z-index: 1;
    max-width: 480px;
    margin: 0 auto;
    padding: 56px 24px 80px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .crow-ring {
    width: 96px; height: 96px;
    border-radius: 50%;
    border: 1.5px solid rgba(201,168,76,0.3);
    display: flex;
    align-items: center;
    justify-content: center;
    background: radial-gradient(circle, rgba(201,168,76,0.07) 0%, transparent 70%);
    margin-bottom: 20px;
  }
  .crow-ring img {
    width: 60px; height: 60px;
    object-fit: contain;
    filter: brightness(10);
  }
  .channel-name {
    font-size: 38px;
    font-weight: 900;
    letter-spacing: 10px;
    color: #c9a84c;
    margin-bottom: 6px;
  }
  .channel-sub {
    font-size: 13px;
    color: rgba(240,236,228,0.45);
    letter-spacing: 3px;
    margin-bottom: 12px;
  }
  .divider {
    width: 40px; height: 1px;
    background: linear-gradient(90deg, transparent, #c9a84c, transparent);
    margin-bottom: 20px;
  }
  .bio {
    font-size: 14px;
    color: rgba(240,236,228,0.45);
    text-align:
    
