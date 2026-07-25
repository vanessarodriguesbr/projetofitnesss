<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
    <meta name="theme-color" content="#FDF0F5">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <title>Projeto fitness da Van</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">

    <style>
        :root {
            /* Fundo com mais rosa suave */
            --bg-main: #FAF0F4;
            --bg-card: #FFFFFF;
            --bg-secondary: #F7E4EC;
            --primary-pink: #E8A0BF;
            --primary-pink-light: #FCE8F0;
            --primary-pink-dark: #C97A9C;
            --blush-accent: #F4C2C2;
            --water-blue: #93C5FD;
            --water-blue-light: #EFF6FF;
            --text-primary: #2D2727;
            --text-secondary: #786F6F;
            --text-muted: #A39B9B;
            --border-color: #F0D5E1;
            --border-radius-s: 12px;
            --border-radius-m: 20px;
            --border-radius-l: 28px;
            --border-radius-full: 9999px;
            --shadow-card: 0 4px 20px rgba(232, 160, 191, 0.12);
            --shadow-floating: 0 12px 35px rgba(232, 160, 191, 0.3);
            --font-primary: 'Plus Jakarta Sans', 'Inter', -apple-system, sans-serif;
            --transition-fast: 0.2s cubic-bezier(0.4, 0, 0.2, 1);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; -webkit-tap-highlight-color: transparent; user-select: none; }
        body { background-color: var(--bg-main); color: var(--text-primary); font-family: var(--font-primary); min-height: 100vh; padding-bottom: 90px; }
        h1, h2, h3 { font-weight: 600; letter-spacing: -0.02em; }
        p { color: var(--text-secondary); font-size: 0.95rem; line-height: 1.5; }

        /* Header Bar */
        .top-bar { display: flex; justify-content: space-between; align-items: center; padding: 16px 24px; background: rgba(250, 240, 244, 0.92); backdrop-filter: blur(12px); position: sticky; top: 0; z-index: 50; border-bottom: 1px solid var(--border-color); }
        .greeting-subtitle { font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; color: var(--primary-pink-dark); font-weight: 700; }
        .greeting-title { font-size: 1.25rem; color: var(--text-primary); }
        .highlight-name { color: var(--primary-pink-dark); }
        .avatar-container { width: 42px; height: 42px; border-radius: var(--border-radius-full); background: linear-gradient(135deg, var(--primary-pink), var(--primary-pink-dark)); display: flex; align-items: center; justify-content: center; color: white; font-weight: 700; font-size: 1.1rem; box-shadow: var(--shadow-card); cursor: pointer; border: 2px solid #FFF; }

        /* Viewport Layout */
        .viewport { padding: 12px 20px 30px; max-width: 600px; margin: 0 auto; }
        .view-screen { animation: fadeInSlide 0.35s cubic-bezier(0.16, 1, 0.3, 1) forwards; }
        @keyframes fadeInSlide { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }

        /* UI Components */
        .card { background: var(--bg-card); border-radius: var(--border-radius-m); padding: 20px; margin-bottom: 16px; box-shadow: var(--shadow-card); border: 1px solid var(--border-color); }
        .card-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 12px; }
        .card-title { font-size: 1.05rem; display: flex; align-items: center; gap: 8px; color: var(--text-primary); }
        
        .progress-ring-card { display: flex; align-items: center; gap: 20px; background: linear-gradient(135deg, #FFFFFF, #FDF0F5); }
        .ring-container { position: relative; width: 80px; height: 80px; flex-shrink: 0; }
        .ring-container svg { transform: rotate(-90deg); }
        .ring-text { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); font-weight: 700; font-size: 1rem; color: var(--primary-pink-dark); }

        .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
        .stat-box { background: var(--primary-pink-light); padding: 12px; border-radius: var(--border-radius-s); text-align: center; border: 1px solid var(--border-color); cursor: pointer; }
        .stat-val { font-size: 1.15rem; font-weight: 700; color: var(--primary-pink-dark); }
        .stat-lbl { font-size: 0.75rem; color: var(--text-secondary); font-weight: 600; }

        .check-item { display: flex; align-items: center; justify-content: space-between; padding: 12px 14px; background: var(--bg-main); border-radius: var(--border-radius-s); margin-bottom: 8px; cursor: pointer; transition: var(--transition-fast); border: 1px solid transparent; }
        .check-item:hover { border-color: var(--primary-pink); }
        .check-item.completed { background: var(--primary-pink-light); }
        .check-item.completed .check-txt { text-decoration: line-through; color: var(--text-muted); }
        .checkbox { width: 22px; height: 22px; border-radius: 6px; border: 2px solid var(--primary-pink); background: white; display: flex; align-items: center; justify-content: center; font-size: 0.8rem; font-weight: bold; }
        .check-item.completed .checkbox { background: var(--primary-pink); color: white; }

        .btn-primary { width: 100%; background: linear-gradient(135deg, var(--primary-pink), var(--primary-pink-dark)); color: white; border: none; padding: 14px; border-radius: var(--border-radius-m); font-weight: 600; font-size: 0.95rem; box-shadow: var(--shadow-floating); cursor: pointer; margin-top: 8px; }
        .btn-primary:active { transform: scale(0.98); }

        /* Select / Dropdown para Treinos */
        .select-custom { width: 100%; padding: 12px; border-radius: var(--border-radius-s); border: 1px solid var(--border-color); background: white; font-family: inherit; font-size: 0.95rem; font-weight: 600; color: var(--text-primary); margin-bottom: 16px; outline: none; cursor: pointer; box-shadow: var(--shadow-card); }

        /* Calendário Horizonal */
        .calendar-bar { display: flex; gap: 8px; overflow-x: auto; padding-bottom: 8px; margin-bottom: 16px; scrollbar-width: none; }
        .day-card { flex: 0 0 auto; width: 55px; padding: 10px 0; text-align: center; background: white; border-radius: var(--border-radius-s); border: 1px solid var(--border-color); cursor: pointer; }
        .day-card.active { background: var(--primary-pink); color: white; border-color: var(--primary-pink); }
        .day-card.active .day-num, .day-card.active .day-name { color: white; }
        .day-name { font-size: 0.7rem; text-transform: uppercase; color: var(--text-muted); font-weight: 600; }
        .day-num { font-size: 1.1rem; font-weight: 700; color: var(--text-primary); margin-top: 2px; }

        /* Water Animation */
        .water-bottle { height: 160px; width: 90px; border: 3px solid var(--water-blue); border-radius: 20px; margin: 15px auto; position: relative; overflow: hidden; background: #FFF; }
        .water-fill { position: absolute; bottom: 0; width: 100%; background: linear-gradient(180deg, #A5F3FC, var(--water-blue)); transition: height 0.5s ease; }

        /* Navigation */
        .bottom-nav { position: fixed; bottom: 0; left: 0; right: 0; height: 72px; background: rgba(255, 255, 255, 0.95); backdrop-filter: blur(16px); border-top: 1px solid var(--border-color); display: flex; justify-content: space-around; align-items: center; z-index: 100; }
        .nav-item { background: none; border: none; display: flex; flex-direction: column; align-items: center; gap: 4px; color: var(--text-muted); font-size: 0.7rem; font-weight: 600; cursor: pointer; width: 20%; }
        .nav-item svg { width: 22px; height: 22px; stroke: var(--text-muted); fill: none; stroke-width: 2; stroke-linecap: round; stroke-linejoin: round; }
        .nav-item.active { color: var(--primary-pink-dark); }
        .nav-item.active svg { stroke: var(--primary-pink-dark); }

        /* Subtabs para Nutrição */
        .subtabs { display: flex; gap: 8px; overflow-x: auto; padding-bottom: 8px; margin-bottom: 16px; scrollbar-width: none; }
        .subtab-btn { background: white; border: 1px solid var(--border-color); padding: 8px 16px; border-radius: var(--border-radius-full); font-size: 0.8rem; font-weight: 600; color: var(--text-secondary); white-space: nowrap; cursor: pointer; }
        .subtab-btn.active { background: var(--primary-pink-dark); color: white; border-color: var(--primary-pink-dark); }

        /* Toast */
        .toast { position: fixed; top: 20px; left: 50%; transform: translateX(-50%); background: var(--text-primary); color: white; padding: 10px 20px; border-radius: var(--border-radius-full); font-size: 0.85rem; z-index: 200; display: none; box-shadow: var(--shadow-floating); }
    </style>
</head>
<body>

    <header class="top-bar">
        <div>
            <span class="greeting-subtitle">Projeto fitness da Van</span>
            <h1 class="greeting-title" id="current-date-title">Carregando...</h1>
        </div>
        <div class="avatar-container" onclick="app.nav('perfil')">V</div>
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
        const DB = {
            user: { name: 'Vanessa', age: 27, height: '1.52m', weight: 60, targetWeight: 50 },
            water: { current: 750, target: 2000 },
            selectedDayOffset: 0,
            selectedNutriTab: 'pretreino',
            selectedWorkoutDay: 'segunda',
            workoutProgress: {},
            checklistState: {}
        };

        const workoutsData = {
            segunda: {
                title: "Glúteo Máximo & Posterior",
                desc: "Foco em Força e Carga • 55–65 min",
                items: [
                    "Elevação Pélvica (Barra/Máq) - 4x8–12 (2s topo)",
                    "Agachamento Búlgaro - 3x10–12",
                    "Bom Dia / Good Morning - 4x10–12",
                    "Cadeira Flexora - 4x12–15",
                    "Glúteo Caneleira/Polia - 3x12–15"
                ]
            },
            terca: {
                title: "Costas • Bíceps • Ombros",
                desc: "Definição do Tronco + Cardio",
                items: [
                    "Puxada Alta Aberta - 4x10–12",
                    "Remada Baixa Triângulo - 3x12",
                    "Desenvolvimento Halteres - 3x12",
                    "Elevação Lateral - 4x12–15",
                    "Rosca Bíceps - 4x12–15",
                    "Cardio: 25–30 min"
                ]
            },
            quarta: {
                title: "Quadríceps & Glúteo Médio",
                desc: "Foco em Pernas e Lateral do Glúteo",
                items: [
                    "Agachamento Halter (Goblet) - 4x10–12",
                    "Leg Press 45° - 3x10–12",
                    "Cadeira Extensora - 3x12–15",
                    "Cadeira Abdutora - 4x15–20",
                    "Abdução no Cabo - 3x12–15",
                    "Cardio Bike: 25–30 min"
                ]
            },
            quinta: {
                title: "Costas • Braços • Core",
                desc: "Escultura de Tronco e Abdômen",
                items: [
                    "Puxada Triângulo - 4x10–12",
                    "Remada Unilateral (Serrote) - 3x12",
                    "Face Pull com Corda - 3x15",
                    "Tríceps Pulley + Rosca Direta - 3x12",
                    "Prancha Abdominal - 3x45–60s",
                    "Abdominal Infra - 3x15–20",
                    "Cardio: 25–30 min"
                ]
            },
            sexta: {
                title: "Descanso Ativo & Recuperação",
                desc: "Recuperação Muscular Direcionada",
                items: [
                    "Alongamentos Leves",
                    "Mobilidade de Quadril",
                    "Hidratação Adicional",
                    "Sono reparador"
                ]
            },
            sabado: {
                title: "Glúteo Pump & Posterior",
                desc: "Modelagem e Exaustão Muscular",
                items: [
                    "Elevação Pélvica Unilateral - 3x12",
                    "Levantamento Terra Sumô - 4x10",
                    "Passada Caminhando - 3x20 passos",
                    "Cadeira Flexora - 3x12–15",
                    "Cadeira Abdutora - 3x20 (Dropset)"
                ]
            },
            domingo: {
                title: "Descanso Total & Planejamento",
                desc: "Preparação para a Próxima Semana",
                items: [
                    "Resumo semanal de conquistas",
                    "Organização do Meal Prep / Marmitas",
                    "Relaxamento e Descanso"
                ]
            }
        };

        const app = {
            init() {
                this.loadDB();
                this.updateDateHeader();
                this.nav('dashboard');
            },

            loadDB() {
                const saved = localStorage.getItem('van_fitness_db');
                if (saved) Object.assign(DB, JSON.parse(saved));
            },

            saveDB() {
                localStorage.setItem('van_fitness_db', JSON.stringify(DB));
            },

            toast(msg) {
                const t = document.getElementById('toast');
                t.innerText = msg;
                t.style.display = 'block';
                setTimeout(() => t.style.display = 'none', 2200);
            },

            updateDateHeader() {
                const d = new Date();
                d.setDate(d.getDate() + DB.selectedDayOffset);
                const options = { weekday: 'short', day: 'numeric', month: 'short' };
                document.getElementById('current-date-title').innerText = d.toLocaleDateString('pt-BR', options);
            },

            nav(screen) {
                document.querySelectorAll('.nav-item').forEach(el => el.classList.remove('active'));
                const btnMap = { dashboard: 0, alimentacao: 1, treinos: 2, agua: 3, perfil: 4 };
                if (btnMap[screen] !== undefined) document.querySelectorAll('.nav-item')[btnMap[screen]].classList.add('active');

                const vp = document.getElementById('app-viewport');
                vp.innerHTML = `<div class="view-screen">${this.screens[screen]()}</div>`;
            },

            selectDay(offset) {
                DB.selectedDayOffset = offset;
                this.saveDB();
                this.updateDateHeader();
                this.nav('dashboard');
            },

            toggleDailyTask(taskId) {
                const key = `day_${DB.selectedDayOffset}_${taskId}`;
                DB.checklistState[key] = !DB.checklistState[key];
                this.saveDB();
                this.nav('dashboard');
            },

            toggleExercise(dayKey, index) {
                const key = `${dayKey}_ex_${index}`;
                DB.workoutProgress[key] = !DB.workoutProgress[key];
                this.saveDB();
                this.nav('treinos');
            },

            addWater(amount) {
                DB.water.current = Math.min(DB.water.target, DB.water.current + amount);
                this.saveDB();
                this.toast(`+${amount}ml registrados! 💧`);
                this.nav('agua');
            },

            setNutriTab(tab) {
                DB.selectedNutriTab = tab;
                this.nav('alimentacao');
            },

            setWorkoutDay(day) {
                DB.selectedWorkoutDay = day;
                this.nav('treinos');
            },

            getDailyTasks() {
                const targetDate = new Date();
                targetDate.setDate(targetDate.getDate() + DB.selectedDayOffset);
                const dayOfWeek = targetDate.getDay(); // 0: Dom, 1: Seg, 2: Ter, 3: Qua, 4: Qui, 5: Sex, 6: Sab

                let workoutTitle = "Treino do Dia";
                if (dayOfWeek === 1) workoutTitle = "Treino: Glúteo Máximo & Posterior";
                else if (dayOfWeek === 2) workoutTitle = "Treino: Costas • Bíceps • Ombros";
                else if (dayOfWeek === 3) workoutTitle = "Treino: Quadríceps & Glúteo Médio";
                else if (dayOfWeek === 4) workoutTitle = "Treino: Costas • Braços • Core";
                else if (dayOfWeek === 5) workoutTitle = "Descanso Ativo & Mobilidade";
                else if (dayOfWeek === 6) workoutTitle = "Treino: Glúteo Pump";
                else if (dayOfWeek === 0) workoutTitle = "Descanso Total & Recuperação";

                return [
                    { id: 'water', text: `Meta de Água (${DB.water.target}ml)` },
                    { id: 'pre', text: 'Refeição: Pré-treino' },
                    { id: 'workout', text: workoutTitle },
                    { id: 'cafe', text: 'Refeição: Café da Manhã' },
                    { id: 'almoco', text: 'Refeição: Almoço' },
                    { id: 'lanche', text: 'Refeição: Lanche da Tarde' },
                    { id: 'jantar', text: 'Refeição: Jantar' }
                ];
            },

            screens: {
                dashboard() {
                    const tasks = app.getDailyTasks();
                    let completed = 0;
                    tasks.forEach(t => {
                        const key = `day_${DB.selectedDayOffset}_${t.id}`;
                        if (DB.checklistState[key]) completed++;
                    });
                    const pct = Math.round((completed / tasks.length) * 100);

                    // Gerar os dias do calendário (-2 até +4 dias)
                    let calHTML = '';
                    for (let i = -2; i <= 4; i++) {
                        const d = new Date();
                        d.setDate(d.getDate() + i);
                        const dayName = d.toLocaleDateString('pt-BR', { weekday: 'narrow' });
                        const dayNum = d.getDate();
                        const isActive = i === DB.selectedDayOffset ? 'active' : '';
                        calHTML += `
                            <div class="day-card ${isActive}" onclick="app.selectDay(${i})">
                                <div class="day-name">${dayName}</div>
                                <div class="day-num">${dayNum}</div>
                            </div>
                        `;
                    }

                    return `
                        <div class="calendar-bar">
                            ${calHTML}
                        </div>

                        <div class="card progress-ring-card">
                            <div class="ring-container">
                                <svg width="80" height="80">
                                    <circle cx="40" cy="40" r="32" stroke="#F0D5E1" stroke-width="8" fill="none"/>
                                    <circle cx="40" cy="40" r="32" stroke="#C97A9C" stroke-width="8" fill="none" stroke-dasharray="201" stroke-dashoffset="${201 - (201 * pct) / 100}" stroke-linecap="round"/>
                                </svg>
                                <div class="ring-text">${pct}%</div>
                            </div>
                            <div>
                                <h3>Progresso do Dia</h3>
                                <p style="font-size:0.85rem">${completed} de ${tasks.length} tarefas concluídas no dia selecionado.</p>
                            </div>
                        </div>

                        <div class="card">
                            <div class="card-header"><h3 class="card-title">Checklist Diário</h3></div>
                            ${tasks.map(t => {
                                const key = `day_${DB.selectedDayOffset}_${t.id}`;
                                const isDone = !!DB.checklistState[key];
                                return `
                                    <div class="check-item ${isDone ? 'completed' : ''}" onclick="app.toggleDailyTask('${t.id}')">
                                        <span class="check-txt">${t.text}</span>
                                        <div class="checkbox">${isDone ? '✓' : ''}</div>
                                    </div>
                                `;
                            }).join('')}
                        </div>

                        <div class="grid-2">
                            <div class="card stat-box" onclick="app.nav('agua')">
                                <div class="stat-lbl">Hidratação</div>
                                <div class="stat-val">${DB.water.current} / ${DB.water.target} ml</div>
                            </div>
                            <div class="card stat-box" onclick="app.nav('perfil')">
                                <div class="stat-lbl">Meta do Projeto</div>
                                <div class="stat-val">${DB.user.weight}kg ➔ ${DB.user.targetWeight}kg</div>
                            </div>
                        </div>
                    `;
                },

                alimentacao() {
                    const tab = DB.selectedNutriTab;
                    return `
                        <div class="subtabs">
                            <button class="subtab-btn ${tab === 'pretreino' ? 'active' : ''}" onclick="app.setNutriTab('pretreino')">Pré-Treino</button>
                            <button class="subtab-btn ${tab === 'cafe' ? 'active' : ''}" onclick="app.setNutriTab('cafe')">Café</button>
                            <button class="subtab-btn ${tab === 'almoco' ? 'active' : ''}" onclick="app.setNutriTab('almoco')">Almoço</button>
                            <button class="subtab-btn ${tab === 'lanche' ? 'active' : ''}" onclick="app.setNutriTab('lanche')">Lanche</button>
                            <button class="subtab-btn ${tab === 'sobremesa' ? 'active' : ''}" onclick="app.setNutriTab('sobremesa')">Sobremesas</button>
                            <button class="subtab-btn ${tab === 'jantar' ? 'active' : ''}" onclick="app.setNutriTab('jantar')">Jantar</button>
                        </div>

                        ${tab === 'pretreino' ? `
                            <div class="card">
                                <div class="card-header"><h3 class="card-title">🍌 Pré-Treino</h3></div>
                                <p><strong>Opções fáceis para energia rápida:</strong></p>
                                <br>
                                <div class="check-item"><span class="check-txt">• Banana</span></div>
                                <div class="check-item"><span class="check-txt">• Pão integral</span></div>
                            </div>
                        ` : ''}

                        ${tab === 'cafe' ? `
                            <div class="card">
                                <div class="card-header"><h3 class="card-title">☕ Café da Manhã</h3></div>
                                <p><strong>Opção 1:</strong></p>
                                <div class="check-item"><span class="check-txt">• 2 fatias de pão integral + 2 ovos</span></div>
                                <br>
                                <p><strong>Opção 2:</strong></p>
                                <div class="check-item"><span class="check-txt">• Banana + Pão integral + Requeijão Light</span></div>
                            </div>
                        ` : ''}

                        ${tab === 'almoco' ? `
                            <div class="card">
                                <div class="card-header"><h3 class="card-title">🥗 Almoço Balanceado</h3></div>
                                <div class="check-item"><span class="check-txt">• Arroz</span></div>
                                <div class="check-item"><span class="check-txt">• Feijão</span></div>
                                <div class="check-item"><span class="check-txt">• Carne ou Frango</span></div>
                                <div class="check-item"><span class="check-txt">• Salada fresca</span></div>
                                <div class="check-item"><span class="check-txt">• Couve ou Abobrinha</span></div>
                            </div>
                        ` : ''}

                        ${tab === 'lanche' ? `
                            <div class="card">
                                <div class="card-header"><h3 class="card-title">🍎 Lanche da Tarde</h3></div>
                                <div class="check-item"><span class="check-txt">• Frutas variadas da sua preferência</span></div>
                            </div>
                        ` : ''}

                        ${tab === 'sobremesa' ? `
                            <div class="card">
                                <div class="card-header"><h3 class="card-title">🍓 Sobremesas Fit</h3></div>
                                <div class="check-item"><span class="check-txt">• Gelatina Zero</span></div>
                                <div class="check-item"><span class="check-txt">• Morangos frescos</span></div>
                                <div class="check-item"><span class="check-txt">• Uvas congeladas</span></div>
                                <div class="check-item"><span class="check-txt">• Banana com canela aquecida</span></div>
                            </div>
                        ` : ''}

                        ${tab === 'jantar' ? `
                            <div class="card">
                                <div class="card-header"><h3 class="card-title">🍲 Jantar (Escolha 1)</h3></div>
                                <div class="check-item"><span class="check-txt">• Marmitas fit preparadas</span></div>
                                <div class="check-item"><span class="check-txt">• Omelete recheado</span></div>
                                <div class="check-item"><span class="check-txt">• Batata assada + Proteína</span></div>
                                <div class="check-item"><span class="check-txt">• Saladas completas</span></div>
                                <div class="check-item"><span class="check-txt">• Sopas leves</span></div>
                            </div>
                        ` : ''}
                    `;
                },

                treinos() {
                    const day = DB.selectedWorkoutDay;
                    const workout = workoutsData[day];

                    return `
                        <div class="card">
                            <label class="stat-lbl" style="display:block; margin-bottom:6px;">Selecione o Dia da Semana:</label>
                            <select class="select-custom" onchange="app.setWorkoutDay(this.value)">
                                <option value="segunda" ${day === 'segunda' ? 'selected' : ''}>Segunda-Feira — Glúteo & Posterior</option>
                                <option value="terca" ${day === 'terca' ? 'selected' : ''}>Terça-Feira — Costas, Bíceps & Ombros</option>
                                <option value="quarta" ${day === 'quarta' ? 'selected' : ''}>Quarta-Feira — Quadríceps & Glúteo Médio</option>
                                <option value="quinta" ${day === 'quinta' ? 'selected' : ''}>Quinta-Feira — Costas, Braços & Core</option>
                                <option value="sexta" ${day === 'sexta' ? 'selected' : ''}>Sexta-Feira — Descanso Ativo</option>
                                <option value="sabado" ${day === 'sabado' ? 'selected' : ''}>Sábado — Glúteo Pump & Posterior</option>
                                <option value="domingo" ${day === 'domingo' ? 'selected' : ''}>Domingo — Descanso Total</option>
                            </select>

                            <div class="card-header" style="margin-bottom:4px">
                                <h3 class="card-title">🏋️‍♀️ ${workout.title}</h3>
                            </div>
                            <p style="font-size:0.85rem; margin-bottom:14px; color:var(--primary-pink-dark); font-weight:600;">${workout.desc}</p>

                            ${workout.items.map((ex, idx) => {
                                const key = `${day}_ex_${idx}`;
                                const isDone = !!DB.workoutProgress[key];
                                return `
                                    <div class="check-item ${isDone ? 'completed' : ''}" onclick="app.toggleExercise('${day}', ${idx})">
                                        <span class="check-txt">${ex}</span>
                                        <div class="checkbox">${isDone ? '✓' : ''}</div>
                                    </div>
                                `;
                            }).join('')}

                            <button class="btn-primary" onclick="app.toast('Treino do dia finalizado com sucesso! 💪✨')">Concluir Treino de Hoje</button>
                        </div>
                    `;
                },

                agua() {
                    const pct = Math.min(100, Math.round((DB.water.current / DB.water.target) * 100));
                    return `
                        <div class="card" style="text-align:center">
                            <h3>Meta Diária de Água</h3>
                            <p style="margin-top:4px; font-weight:600; color:var(--primary-pink-dark);">${DB.water.current}ml de ${DB.water.target}ml (${pct}%)</p>
                            
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
                            <h3>Perfil da Vanessa</h3>
                            <br>
                            <div class="check-item"><span class="check-txt">Idade: ${DB.user.age} anos</span></div>
                            <div class="check-item"><span class="check-txt">Altura: ${DB.user.height}</span></div>
                            <div class="check-item"><span class="check-txt">Peso Atual: ${DB.user.weight} kg</span></div>
                            <div class="check-item"><span class="check-txt">Meta de Peso: ${DB.user.targetWeight} kg</span></div>
                        </div>
                        <div class="card">
                            <h3>Objetivos Principais</h3>
                            <p style="margin-top:8px; line-height:1.6">• Emagrecer e definir pernas/glúteos<br>• Desenhar costas para afinar a cintura<br>• Atingir 50kg com foco e constância</p>
                        </div>
                    `;
                }
            }
        };

        window.onload = () => app.init();
    </script>
</body>
</html>
