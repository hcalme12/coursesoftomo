<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Liste de Courses</title>
    <meta name="theme-color" content="#4F46E5">
    <link rel="manifest" href="data:application/json;base64,eyJuYW1lIjoiTGlzdGUgZGUgQ291cnNlcyIsInNob3J0X25hbWUiOiJDb3Vyc2VzIiwic3RhcnRfdXJsIjoiLyIsImRpc3BsYXkiOiJzdGFuZGFsb25lIiwidGhlbWVfY29sb3IiOiIjNEY0NkU1IiwiYmFja2dyb3VuZF9jb2xvciI6IiNGOUZBRkIiLCJpY29ucyI6W3sic3JjIjoiZGF0YTppbWFnZS9zdmcreG1sO2Jhc2U2NCxQSE4yWnlCM2FXUjBhRDBpTWpRaUlHaGxhV2RvZEQwaU1qUWlJSFpwWlhkQ2IzZzlJakFnTUNBeU5DQXlOQ0lnWm1sc2JEMGlibTl1WlNJZ2VHMXNibk05SW1oMGRIQTZMeTkzZDNjdWR6TXViM0puTHpJd01EQXZjM1puSWo0OGNHRjBhQ0JrUFNKTk9TNHdReTQxTFM0Mk5EZzNJRGMxTGpRSUNEUWdNaklnTkZ3aU1UQXVPREF4TVRNeElERXdZek12Tnk0eElEQWdNamtnTXpJdU16RnNMall6TnlBd1l6RXVPRElnTUM0ME9UTWdNakF1TlRCMGVEYzFMblEwSUdabGJUOWlJREU0SUM0NU9DOGdlRGNnTXpReUlHaGRJbTQ4TDNkOGVsOGdabWxzYkQwaUkwUkNORGRFSWlCemRISnZhMlU5SWpJaUx6NDhMM04yWnowaUlpQnphWHBsUFNJeU5DSWdkSGx3WlQwaWFXMWhaMlV2Y0c1bklpQnphWHBsY3owaU1qUWdNalFpZlY4PTsgSURAaUFBQUFCa0VRQUFBQkFBQUFBQT09In1dfQ==">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            color: #333;
        }

        .container {
            max-width: 400px;
            margin: 0 auto;
            padding: 20px;
            min-height: 100vh;
        }

        .header {
            text-align: center;
            color: white;
            margin-bottom: 30px;
            padding: 20px 0;
        }

        .header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .card {
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            padding: 25px;
            margin-bottom: 20px;
            backdrop-filter: blur(10px);
        }

        .input-group {
            margin-bottom: 20px;
        }

        .input-group label {
            display: block;
            font-weight: 600;
            margin-bottom: 8px;
            color: #4F46E5;
        }

        .input-field {
            width: 100%;
            padding: 15px;
            border: 2px solid #E5E7EB;
            border-radius: 12px;
            font-size: 16px;
            transition: all 0.3s ease;
        }

        .input-field:focus {
            outline: none;
            border-color: #4F46E5;
            box-shadow: 0 0 0 3px rgba(79, 70, 229, 0.1);
        }

        .btn {
            background: linear-gradient(135deg, #4F46E5, #7C3AED);
            color: white;
            border: none;
            padding: 15px 25px;
            border-radius: 12px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
            margin-top: 10px;
        }

        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(79, 70, 229, 0.3);
        }

        .btn:active {
            transform: translateY(0);
        }

        .btn-secondary {
            background: linear-gradient(135deg, #10B981, #059669);
        }

        .btn-danger {
            background: linear-gradient(135deg, #EF4444, #DC2626);
        }

        .list-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px;
            background: #F9FAFB;
            border-radius: 12px;
            margin-bottom: 10px;
            border-left: 4px solid #4F46E5;
            transition: all 0.3s ease;
        }

        .list-item.completed {
            background: #ECFDF5;
            border-left-color: #10B981;
            text-decoration: line-through;
            opacity: 0.7;
        }

        .list-item.extra {
            background: #FEF3C7;
            border-left-color: #F59E0B;
        }

        .remove-btn {
            background: #EF4444;
            color: white;
            border: none;
            border-radius: 50%;
            width: 30px;
            height: 30px;
            cursor: pointer;
            font-size: 14px;
            transition: all 0.3s ease;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            margin-top: 20px;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.9);
            padding: 15px;
            border-radius: 12px;
            text-align: center;
        }

        .stat-number {
            font-size: 2rem;
            font-weight: bold;
            color: #4F46E5;
        }

        .stat-label {
            font-size: 0.9rem;
            color: #6B7280;
            margin-top: 5px;
        }

        .progress-bar {
            width: 100%;
            height: 8px;
            background: #E5E7EB;
            border-radius: 4px;
            overflow: hidden;
            margin: 15px 0;
        }

        .progress-fill {
            height: 100%;
            background: linear-gradient(135deg, #10B981, #059669);
            border-radius: 4px;
            transition: width 0.3s ease;
        }

        .section-title {
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 15px;
            color: #374151;
        }

        .hidden {
            display: none;
        }

        .emoji {
            font-size: 1.2rem;
            margin-right: 8px;
        }

        @media (max-width: 480px) {
            .container {
                padding: 15px;
            }
            
            .header h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>🛒 Ma Liste</h1>
            <p>Organise tes courses comme un pro !</p>
        </div>

        <!-- Étape 1: Création de la liste -->
        <div id="create-phase" class="card">
            <div class="section-title">📝 Créer ma liste de courses</div>
            <div class="input-group">
                <label for="new-item">Ajouter un article</label>
                <input type="text" id="new-item" class="input-field" placeholder="Ex: Pain, Lait, Pommes..." onkeypress="handleKeyPress(event, 'add')">
            </div>
            <button onclick="addItem()" class="btn">➕ Ajouter</button>
            
            <div id="initial-list"></div>
            
            <button onclick="startShopping()" class="btn btn-secondary" id="start-btn" style="display:none;">🛍️ Commencer les courses</button>
        </div>

        <!-- Étape 2: Shopping -->
        <div id="shopping-phase" class="card hidden">
            <div class="section-title">🛍️ Je suis en courses</div>
            <div class="input-group">
                <label for="taken-item">J'ai pris...</label>
                <input type="text" id="taken-item" class="input-field" placeholder="Qu'est-ce que tu as pris ?" onkeypress="handleKeyPress(event, 'take')">
            </div>
            <button onclick="takeItem()" class="btn">✅ J'ai pris ça</button>
            <button onclick="showResults()" class="btn btn-secondary">📊 Voir le résumé</button>
        </div>

        <!-- Étape 3: Résultats -->
        <div id="results-phase" class="card hidden">
            <div class="section-title">📊 Résumé de tes courses</div>
            
            <div class="progress-bar">
                <div class="progress-fill" id="progress"></div>
            </div>
            
            <div class="stats">
                <div class="stat-card">
                    <div class="stat-number" id="completion-rate">0%</div>
                    <div class="stat-label">Complété</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number" id="extra-items">0</div>
                    <div class="stat-label">Articles en plus</div>
                </div>
            </div>

            <div id="results-content"></div>
            
            <button onclick="restart()" class="btn btn-danger">🔄 Nouvelle liste</button>
        </div>
    </div>

    <script>
        let initialList = [];
        let takenItems = [];

        function handleKeyPress(event, action) {
            if (event.key === 'Enter') {
                if (action === 'add') addItem();
                if (action === 'take') takeItem();
            }
        }

        function addItem() {
            const input = document.getElementById('new-item');
            const item = input.value.trim().toLowerCase();
            
            if (item && !initialList.includes(item)) {
                initialList.push(item);
                input.value = '';
                updateInitialList();
                document.getElementById('start-btn').style.display = 'block';
            }
        }

        function removeItem(item) {
            initialList = initialList.filter(i => i !== item);
            updateInitialList();
            if (initialList.length === 0) {
                document.getElementById('start-btn').style.display = 'none';
            }
        }

        function updateInitialList() {
            const container = document.getElementById('initial-list');
            if (initialList.length === 0) {
                container.innerHTML = '';
                return;
            }

            container.innerHTML = `
                <div class="section-title" style="margin-top: 20px;">Ma liste (${initialList.length} articles)</div>
                ${initialList.map(item => `
                    <div class="list-item">
                        <span class="emoji">📦</span> ${item}
                        <button class="remove-btn" onclick="removeItem('${item}')">×</button>
                    </div>
                `).join('')}
            `;
        }

        function takeItem() {
            const input = document.getElementById('taken-item');
            const item = input.value.trim().toLowerCase();
            
            if (item && !takenItems.includes(item)) {
                takenItems.push(item);
                input.value = '';
                
                // Feedback visuel
                const feedback = document.createElement('div');
                feedback.style.cssText = 'position:fixed;top:50%;left:50%;transform:translate(-50%,-50%);background:#10B981;color:white;padding:15px 25px;border-radius:12px;z-index:1000;font-weight:600;';
                feedback.textContent = `✅ "${item}" ajouté !`;
                document.body.appendChild(feedback);
                
                setTimeout(() => feedback.remove(), 2000);
            }
        }

        function startShopping() {
            if (initialList.length === 0) {
                alert('Ajoute au moins un article à ta liste !');
                return;
            }
            
            document.getElementById('create-phase').classList.add('hidden');
            document.getElementById('shopping-phase').classList.remove('hidden');
        }

        function showResults() {
            document.getElementById('shopping-phase').classList.add('hidden');
            document.getElementById('results-phase').classList.remove('hidden');
            
            analyzeResults();
        }

        function analyzeResults() {
            const taken = new Set(takenItems);
            const initial = new Set(initialList);
            
            const completed = [...initial].filter(item => taken.has(item));
            const missing = [...initial].filter(item => !taken.has(item));
            const extra = [...taken].filter(item => !initial.has(item));
            
            const completionRate = initial.size > 0 ? Math.round((completed.length / initial.size) * 100) : 0;
            
            // Mise à jour des stats
            document.getElementById('completion-rate').textContent = `${completionRate}%`;
            document.getElementById('extra-items').textContent = extra.length;
            document.getElementById('progress').style.width = `${completionRate}%`;
            
            // Contenu détaillé
            const resultsContent = document.getElementById('results-content');
            resultsContent.innerHTML = `
                ${completed.length > 0 ? `
                    <div style="margin-top: 20px;">
                        <div class="section-title">✅ Articles pris de la liste (${completed.length})</div>
                        ${completed.map(item => `
                            <div class="list-item completed">
                                <span class="emoji">✅</span> ${item}
                            </div>
                        `).join('')}
                    </div>
                ` : ''}
                
                ${missing.length > 0 ? `
                    <div style="margin-top: 20px;">
                        <div class="section-title">❌ Articles manqués (${missing.length})</div>
                        ${missing.map(item => `
                            <div class="list-item">
                                <span class="emoji">❌</span> ${item}
                            </div>
                        `).join('')}
                    </div>
                ` : `<div style="margin-top: 20px; text-align: center; color: #10B981; font-weight: 600;">🎉 Bravo ! Tu as tout pris de ta liste !</div>`}
                
                ${extra.length > 0 ? `
                    <div style="margin-top: 20px;">
                        <div class="section-title">➕ Articles en plus (${extra.length})</div>
                        ${extra.map(item => `
                            <div class="list-item extra">
                                <span class="emoji">➕</span> ${item}
                            </div>
                        `).join('')}
                    </div>
                ` : ''}
            `;
        }

        function restart() {
            initialList = [];
            takenItems = [];
            
            document.getElementById('results-phase').classList.add('hidden');
            document.getElementById('create-phase').classList.remove('hidden');
            
            document.getElementById('new-item').value = '';
            document.getElementById('taken-item').value = '';
            document.getElementById('initial-list').innerHTML = '';
            document.getElementById('start-btn').style.display = 'none';
        }

        // Installation PWA
        let deferredPrompt;
        window.addEventListener('beforeinstallprompt', (e) => {
            e.preventDefault();
            deferredPrompt = e;
            
            // Afficher un bouton d'installation après 5 secondes
            setTimeout(() => {
                if (deferredPrompt) {
                    const installBtn = document.createElement('button');
                    installBtn.textContent = '📱 Installer l\'app';
                    installBtn.className = 'btn';
                    installBtn.style.position = 'fixed';
                    installBtn.style.bottom = '20px';
                    installBtn.style.right = '20px';
                    installBtn.style.width = 'auto';
                    installBtn.style.zIndex = '1000';
                    
                    installBtn.onclick = () => {
                        deferredPrompt.prompt();
                        deferredPrompt.userChoice.then(() => {
                            deferredPrompt = null;
                            installBtn.remove();
                        });
                    };
                    
                    document.body.appendChild(installBtn);
                }
            }, 5000);
        });
    </script>
</body>
</html>
