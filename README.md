# Clean-Runner
Não pegue coins
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>Evite as Moedas</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&family=Nunito:wght@600;800&display=swap');

  :root {
    --bg: #0f0f1a;
    --accent: #ff3b5c;
    --gold: #ffd700;
    --lane: #2a2a40;
    --green: #00e676;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; user-select: none; -webkit-tap-highlight-color: transparent; }

  body {
    background: var(--bg);
    color: #fff;
    font-family: 'Nunito', sans-serif;
    overflow: hidden;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .screen {
    display: none;
    width: 100%;
    max-width: 480px;
    height: 100%;
    flex-direction: column;
    position: relative;
    background: linear-gradient(180deg, #1a1a2e 0%, #0f0f1a 100%);
  }
  .screen.active { display: flex; }

  /* ===== LOGIN ===== */
  #loginScreen {
    padding: 40px 28px;
    justify-content: center;
    gap: 18px;
  }
  .logo {
    font-family: 'Press Start 2P', cursive;
    font-size: 22px;
    text-align: center;
    color: var(--gold);
    text-shadow: 0 0 20px rgba(255,215,0,0.5);
    margin-bottom: 10px;
    line-height: 1.4;
  }
  .logo span { color: var(--accent); display: block; font-size: 14px; margin-top: 6px; }
  input, select {
    width: 100%;
    padding: 14px 16px;
    border: 2px solid #333;
    border-radius: 12px;
    background: #1e1e30;
    color: #fff;
    font-size: 16px;
    font-family: inherit;
    outline: none;
    transition: border 0.2s;
  }
  input:focus, select:focus { border-color: var(--accent); }
  .btn {
    width: 100%;
    padding: 16px;
    border: none;
    border-radius: 14px;
    font-size: 17px;
    font-weight: 800;
    cursor: pointer;
    font-family: inherit;
    transition: transform 0.15s, box-shadow 0.15s;
  }
  .btn:active { transform: scale(0.96); }
  .btn-primary {
    background: linear-gradient(135deg, #ff3b5c, #ff6b8a);
    color: #fff;
    box-shadow: 0 6px 20px rgba(255,59,92,0.4);
  }
  .btn-secondary {
    background: #2a2a40;
    color: #fff;
  }

  /* ===== MAIN MENU ===== */
  #menuScreen { padding-top: 20px; }
  .top-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 12px 20px;
  }
  .icon-btn {
    width: 48px; height: 48px;
    border-radius: 50%;
    background: #2a2a40;
    border: none;
    color: #fff;
    font-size: 22px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: background 0.2s;
  }
  .icon-btn:active { background: #3a3a55; }
  .player-name {
    font-weight: 800;
    font-size: 18px;
    text-align: center;
  }
  .character-area {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 16px;
  }
  .character {
    width: 120px;
    height: 160px;
    position: relative;
  }
  .char-body {
    width: 70px;
    height: 90px;
    background: linear-gradient(180deg, #4fc3f7, #0288d1);
    border-radius: 20px 20px 12px 12px;
    position: absolute;
    left: 25px;
    top: 40px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.4);
  }
  .char-head {
    width: 56px;
    height: 56px;
    background: #ffcc80;
    border-radius: 50%;
    position: absolute;
    left: 32px;
    top: 0;
    border: 3px solid #ffb74d;
  }
  .char-eye {
    width: 10px; height: 10px;
    background: #333;
    border-radius: 50%;
    position: absolute;
    top: 22px;
  }
  .char-eye.l { left: 12px; }
  .char-eye.r { right: 12px; }
  .char-leg {
    width: 22px; height: 40px;
    background: #1565c0;
    border-radius: 0 0 8px 8px;
    position: absolute;
    bottom: 0;
  }
  .char-leg.l { left: 28px; }
  .char-leg.r { right: 28px; }
  .char-arm {
    width: 16px; height: 50px;
    background: #4fc3f7;
    border-radius: 8px;
    position: absolute;
    top: 50px;
  }
  .char-
... 
