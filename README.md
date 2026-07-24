<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
    <meta name="theme-color" content="#FAF7F5">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <title>Aura — Premium Wellbeing</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">

    <style>
        :root {
            --bg-main: #FAF7F5;
            --bg-card: #FFFFFF;
            --bg-secondary: #F3ECE7;
            --primary-pink: #E8A0BF;
            --primary-pink-light: #FDF0F5;
            --primary-pink-dark: #C97A9C;
            --blush-accent: #F4C2C2;
            --water-blue: #93C5FD;
            --water-blue-light: #EFF6FF;
            --text-primary: #2D2727;
            --text-secondary: #786F6F;
            --text-muted: #A39B9B;
            --border-color: #EFE8E3;
            --border-radius-s: 12px;
            --border-radius-m: 20px;
            --border-radius-l: 28px;
            --border-radius-full: 9999px;
            --shadow-card: 0 4px 20px rgba(0, 0, 0, 0.03);
            --shadow-floating: 0 12px 35px rgba(232, 160, 191, 0.25);
            --font-primary: 'Plus Jakarta Sans', 'Inter', -apple-system, sans-serif;
            --transition-fast: 0.2s cubic-bezier(0.4, 0, 0.2, 1);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; -webkit-tap-highlight-color: transparent; user-select: none; }
        body { background-color: var(--bg-main); color: var(--text-primary); font-family: var(--font-primary); min-height: 100vh; padding-bottom: 90px; }
        h1, h2, h3 { font-weight: 600; letter-spacing: -0.02em; }
        p { color: var(--text-secondary); font-size: 0.95rem; line-height: 1.5; }

        /* Header Bar */
        .top-bar { display: flex; justify-content: space-between; align-items: center; padding: 16px 24px; background: rgba(250, 247, 245, 0.9); backdrop-filter: blur(12px); position: sticky; top: 0; z-index: 50; }
        .greeting-subtitle { font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; color: var(--text-muted); font-weight: 600; }
        .greeting-title { font-size: 1.3rem; color: var(--text-primary); }
        .highlight-name { color: var(--primary-pink-dark); }
        .avatar-container { width: 40px; height: 40px; border-radius: var(--border-radius-full); background: linear-gradient(135deg, var(--primary-pink), var(--blush-accent)); display: flex; align-items: center; justify-content: center; color: white; font-weight: 700; box-shadow: var(--shadow-card); cursor: pointer; }

        /* Viewport Layout */
        .viewport { padding: 12px 20px 30px; max-width: 600px; margin: 0 auto; }
        .view-screen { animation: fadeInSlide 0.35s cubic-bezier(0.16, 1, 0.3, 1) forwards; }
        @keyframes fadeInSlide { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }

        /* UI Components */
        .card { background: var(--bg-card); border-radius: var(--border-radius-m); padding: 20px; margin-bottom: 16px; box-shadow: var(--shadow-card); border: 1px solid var(--border-color); }
        .card-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 12px; }
        .card-title { font-size: 1.05rem; display: flex; align-items: center; gap: 8px; color: var(--text-primary); }
        
        .progress-ring-card { display: flex; align-items: center; gap: 20px; }
        .ring-container { position: relative; width: 80px; height: 80px; }
        .ring-container svg { transform: rotate(-90deg); }
        .ring-text { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); font-weight: 700; font-size: 1rem; }

        .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
        .stat-box { background: var(--bg-main); padding: 12px; border-radius: var(--border-radius-s); text-align: center; }
        .stat-val { font-size: 1.2rem; font-weight: 700; color: var(--text-primary); }
        .stat-lbl { font-size: 0.75rem; color: var(--text-muted); }

        .check-item { display: flex; align-items: center; justify-content: space-between; padding: 12px; background: var(--bg-main); border-radius: var(--border-radius-s); margin-bottom: 8px; cursor: pointer; transition: var(--transition-fast); }
        .check-item.completed { background: var(--primary-pink-light); }
        .check-item.completed .check-txt { text-decoration: line-through; color: var(--text-muted); }
        .checkbox { width: 20px; height: 20px; border-radius: 6px; border: 2px solid var(--border-color); background: white; display: flex; align-items: center; justify-content: center; }
        .check-item.completed .checkbox { background: var(--primary-pink); border-color: var(--primary-pink); color: white; }

        .btn-primary { width: 100%; background: linear-gradient(135deg, var(--primary-pink), var(--primary-pink-dark)); color: white; border: none; padding: 14px; border-radius: var(--border-radius-m); font-weight: 600; font-size: 0.95rem; box-shadow: var(--shadow-floating); cursor: pointer; margin-top: 8px; }
        .btn-primary:active { transform: scale(0.98); }

        /* Water Animation */
        .water-bottle { height: 160px; width: 90px; border: 3px solid var(--water-blue); border-radius: 20px; margin: 15px auto; position: relative; overflow: hidden; background: #FFF; }
        .water-fill { position: absolute; bottom: 0; width: 100%; background: linear-gradient(180deg, #A5F3FC, var(--water-blue)); transition: height 0.5s ease; }

        /* Navigation */
        .bottom-nav { position: fixed; bottom: 0; left: 0; right: 0; height: 70px; background: rgba(255, 255, 255, 0.95); backdrop-filter: blur(16px); border-top: 1px solid var(--border-color); display: flex; justify-content: space-around; align-items: center; z-index: 100; }
        .nav-item { background: none; border: none; display: flex; flex-direction: column; align-items: center; gap: 4px; color: var(--text-muted); font-size: 0.7rem; font-weight: 500; cursor: pointer; width: 20%; }
        .nav-item svg { width: 22px; height: 22px; stroke: var(--text-muted); fill: none; stroke-width: 2; stroke-linecap: round; stroke-linejoin: round; }
        .nav-item.active { color: var(--primary-pink-dark); font-weight: 700; }
        .nav-item.active svg { stroke: var(--primary-pink-dark); }

        /* Subtabs */
        .subtabs { display: flex; gap: 8px; overflow-x: auto; padding-bottom: 8px; margin-bottom: 12px; }
        .subtab-btn { background: var(--bg-card); border: 1px solid var(--border-color); padding: 8px 16px; border-radius: var(--border-radius-full); font-size: 0.8rem; white-space: nowrap; cursor: pointer; }
        .subtab-btn.active { background: var(--text-primary); color: white; border-color: var(--text-primary); }

        /* Toast */
        .toast { position: fixed; top: 20px; left: 50%; transform: translateX(-50%); background: var(--text-primary); color: white; padding: 10px 20px; border-radius: var(--border-radius-full); font-size: 0.85rem; z-index: 200; display: none; }
    </style>
</head>
<body>

    <header class="top-bar">
        <div>
            <span class="greeting-subtitle" id="current-date">Sexta, 24 de Julho</span>
            <h1 class="greeting-title">Aura <span class="highlight-name">Wellness</span> ✨</h1>
        </div>
        <div class="avatar-container" onclick="app.nav('perfil')">A</div>
    </header>

    <main id="app-viewport" class="viewport"></main>
    <div id="toast" class="toast"></div>

    <nav class="bottom-nav">
        <button class="nav-item active" onclick="app.nav('dashboard')">
            <svg viewBox="0 0 24 24"><path d="m3 9 9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg>
            <span>Início</span>
        </button>
        <button class="nav-item" onclick="app.nav('alimentacao')">
            <svg viewBox="0 0 24 24"><path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"/><path d="M13.73 21a2 2 0 0 1-3.46 0"/></svg>
            <span>Nutrição</span>
        </button>
        <button class="nav-item" onclick="app.nav('treinos')">
            <svg viewBox="0 0 24 24"><path d="m6.5 6.5 11 11"/><path d="m21 21-1-1"/><path d="m3 3 1 1"/><path d="m18 22 4-4"/><path d="m2 6 4-4"/></svg>
            <span>Treinos</span>
        </button>
        <button class="nav-item" onclick="app.nav('agua')">
            <svg viewBox="0 0 24 24"><path d="M12 2.69l5.66 5.66a8 8 0 1 1-11.31 0z"/></svg>
            <span>Água</span>
        </button>
        <button class="nav-item" onclick="app.nav('perfil')">
            <svg viewBox="0 0 24 24"><path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2"/><circle cx="12" cy="7" r="4"/></svg>
            <span>Perfil</span>
        </button>
    </nav>

    <script>
        // Data Store & App Engine
        const DB = {
            user: { name: 'Usuária', age: 27, height: '1.52m', weight: 60, targetWeight: 50 },
            water: { current: 750, target: 2000 },
            checklist: [
                { id: 1, text: 'Treino de Glúteos completo', done: false },
                { id: 2, text: 'Beber 2L de água', done: false },
                { id: 3, text: 'Dormir às 22h', done: false },
                { id: 4, text: 'Marmita saudável no almoço', done: true }
            ]
        };

        const app = {
            init() {
                this.loadDB();
                this.nav('dashboard');
                document.getElementById('current-date').innerText = new Date().toLocaleDateString('pt-BR', { weekday: 'short', day: 'numeric', month: 'short' });
            },

            loadDB() {
                const saved = localStorage.getItem('aura_db');
                if (saved) Object.assign(DB, JSON.parse(saved));
            },

            saveDB() {
                localStorage.setItem('aura_db', JSON.stringify(DB));
            },

            toast(msg) {
                const t = document.getElementById('toast');
                t.innerText = msg;
                t.style.display = 'block';
                setTimeout(() => t.style.display = 'none', 2000);
            },

            nav(screen) {
                document.querySelectorAll('.nav-item').forEach(el => el.classList.remove('active'));
                const btnMap = { dashboard: 0, alimentacao: 1, treinos: 2, agua: 3, perfil: 4 };
                if (btnMap[screen] !== undefined) document.querySelectorAll('.nav-item')[btnMap[screen]].classList.add('active');

                const vp = document.getElementById('app-viewport');
                vp.innerHTML = `<div class="view-screen">${this.screens[screen]()}</div>`;
            },

            toggleCheck(id) {
                const item = DB.checklist.find(i => i.id === id);
                if (item) {
                    item.done = !item.done;
                    this.saveDB();
                    this.nav('dashboard');
                }
            },

            addWater(amount) {
                DB.water.current = Math.min(DB.water.target, DB.water.current + amount);
                this.saveDB();
                this.toast(`+${amount}ml registrados! 💧`);
                this.nav('agua');
            },

            screens: {
                dashboard() {
                    const doneCount = DB.checklist.filter(i => i.done).length;
                    const pct = Math.round((doneCount / DB.checklist.length) * 100);
                    return `
                        <div class="card progress-ring-card">
                            <div class="ring-container">
                                <svg width="80" height="80">
                                    <circle cx="40" cy="40" r="32" stroke="#EFE8E3" stroke-width="8" fill="none"/>
                                    <circle cx="40" cy="40" r="32" stroke="#E8A0BF" stroke-width="8" fill="none" stroke-dasharray="201" stroke-dashoffset="${201 - (201 * pct) / 100}" stroke-linecap="round"/>
                                </svg>
                                <div class="ring-text">${pct}%</div>
                            </div>
                            <div>
                                <h3>Progresso Diário</h3>
                                <p style="font-size:0.85rem">${doneCount} de ${DB.checklist.length} metas concluídas hoje.</p>
                            </div>
                        </div>

                        <div class="card">
                            <div class="card-header"><h3 class="card-title">Checklist Hoje</h3></div>
                            ${DB.checklist.map(i => `
                                <div class="check-item ${i.done ? 'completed' : ''}" onclick="app.toggleCheck(${i.id})">
                                    <span class="check-txt">${i.text}</span>
                                    <div class="checkbox">${i.done ? '✓' : ''}</div>
                                </div>
                            `).join('')}
                        </div>

                        <div class="grid-2">
                            <div class="card stat-box" onclick="app.nav('agua')">
                                <div class="stat-lbl">Hidratação</div>
                                <div class="stat-val">${DB.water.current} / ${DB.water.target} ml</div>
                            </div>
                            <div class="card stat-box" onclick="app.nav('perfil')">
                                <div class="stat-lbl">Meta de Peso</div>
                                <div class="stat-val">${DB.user.weight}kg ➔ ${DB.user.targetWeight}kg</div>
                            </div>
                        </div>
                    `;
                },

                alimentacao() {
                    return `
                        <div class="subtabs">
                            <button class="subtab-btn active">Pré-Treino</button>
                            <button class="subtab-btn">Café</button>
                            <button class="subtab-btn">Almoço</button>
                            <button class="subtab-btn">Lanche</button>
                            <button class="subtab-btn">Jantar</button>
                        </div>
                        <div class="card">
                            <div class="card-header"><h3 class="card-title">🥑 Café da Manhã</h3></div>
                            <p><strong>Opção 1:</strong> 2 ovos mexidos + 2 fatias de pão integral + café preto sem açúcar.</p>
                            <br>
                            <p><strong>Opção 2:</strong> Banana amassada com canela e pão integral com requeijão light.</p>
                        </div>
                        <div class="card">
                            <div class="card-header"><h3 class="card-title">💡 Dica da Nutri</h3></div>
                            <p>Mantenha as proteínas bem fracionadas ao longo do dia para preservar sua massa magra durante o déficit calórico.</p>
                        </div>
                    `;
                },

                treinos() {
                    return `
                        <div class="card">
                            <div class="card-header"><h3 class="card-title">🏋️‍♀️ Treino A — Glúteo & Posterior</h3></div>
                            <p style="font-size:0.8rem; margin-bottom:12px">Segunda-Feira • Foco em Força e Carga</p>
                            <div class="check-item"><span class="check-txt">Elevação Pélvica (4x 8–12)</span></div>
                            <div class="check-item"><span class="check-txt">Agachamento Búlgaro (3x 10–12)</span></div>
                            <div class="check-item"><span class="check-txt">Bom Dia / Good Morning (4x 10–12)</span></div>
                            <div class="check-item"><span class="check-txt">Cadeira Flexora (4x 12–15)</span></div>
                            <div class="check-item"><span class="check-txt">Glúteo na Polia (3x 12–15)</span></div>
                            <button class="btn-primary" onclick="app.toast('Treino concluído com sucesso! 🔥')">Finalizar Treino</button>
                        </div>
                    `;
                },

                agua() {
                    const pct = Math.round((DB.water.current / DB.water.target) * 100);
                    return `
                        <div class="card" style="text-align:center">
                            <h3>Meta Diária de Água</h3>
                            <p>${DB.water.current}ml acumulados (${pct}%)</p>
                            
                            <div class="water-bottle">
                                <div class="water-fill" style="height: ${pct}%"></div>
                            </div>

                            <div class="grid-2">
                                <button class="btn-primary" style="background:var(--water-blue)" onclick="app.addWater(250)">+250 ml</button>
                                <button class="btn-primary" style="background:var(--water-blue)" onclick="app.addWater(500)">+500 ml</button>
                            </div>
                        </div>
                    `;
                },

                perfil() {
                    return `
                        <div class="card">
                            <h3>Seu Perfil Aura</h3>
                            <br>
                            <div class="check-item"><span class="check-txt">Idade: ${DB.user.age} anos</span></div>
                            <div class="check-item"><span class="check-txt">Altura: ${DB.user.height}</span></div>
                            <div class="check-item"><span class="check-txt">Peso Atual: ${DB.user.weight} kg</span></div>
                            <div class="check-item"><span class="check-txt">Objetivo final: ${DB.user.targetWeight} kg</span></div>
                        </div>
                        <div class="card">
                            <h3>Metas Principais</h3>
                            <p style="margin-top:8px">• Definir Glúteos & Costas<br>• Déficit Calórico Controlado<br>• Rotina de Treino 5x na Semana</p>
                        </div>
                    `;
                }
            }
        };

        window.onload = () => app.init();
    </script>
</body>
</html>
