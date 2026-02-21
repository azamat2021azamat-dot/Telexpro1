<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>TeleX PRO</title>
    <style>
        :root {
            --tg-bg: #0e1621;
            --tg-header: #17212b;
            --tg-active: #2b9cff;
            --tg-msg-in: #182533;
            --tg-msg-out: #2b5278;
            --tg-text: #ffffff;
            --tg-text-muted: #708499;
            --tg-owner: #f1c40f;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif; }
        
        body { 
            background: var(--tg-bg); 
            color: var(--tg-text); 
            height: 100vh; 
            display: flex; 
            flex-direction: column; 
            overflow: hidden;
            -webkit-tap-highlight-color: transparent;
        }

        /* HEADER */
        header { 
            background: var(--tg-header); 
            padding: 0 16px; 
            display: flex; 
            align-items: center; 
            height: 56px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.2);
            z-index: 100;
        }

        .back-btn { display: none; margin-right: 25px; cursor: pointer; font-size: 22px; color: white; }

        .header-info { display: flex; flex-direction: column; }
        .header-title { font-size: 19px; font-weight: 600; }
        .header-status { font-size: 13px; color: var(--tg-active); }

        /* SCREENS */
        .screen { flex: 1; overflow-y: auto; display: none; }
        .active { display: block; }
        #chatWindow.active { display: flex; flex-direction: column; background: url('https://user-images.githubusercontent.com/15075759/28719144-86dc0f70-73b1-11e7-911d-60d70fcded21.png'); background-size: cover; }

        /* LISTS (CHATS/CHANNELS) */
        .list-item { 
            padding: 10px 16px; 
            display: flex; 
            align-items: center; 
            cursor: pointer;
            transition: background 0.2s;
        }
        .list-item:active { background: rgba(255,255,255,0.05); }
        
        .avatar {
            width: 52px; height: 52px; border-radius: 50%;
            background: #2b5278; margin-right: 14px;
            display: flex; align-items: center; justify-content: center; 
            font-size: 20px; font-weight: bold; flex-shrink: 0;
        }

        .item-content { flex: 1; border-bottom: 0.5px solid #131c27; padding: 10px 0; }
        .item-top { display: flex; justify-content: space-between; margin-bottom: 4px; }
        .item-name { font-weight: 600; font-size: 16px; }
        .item-time { font-size: 12px; color: var(--tg-text-muted); }
        .item-msg { font-size: 14px; color: var(--tg-text-muted); white-space: nowrap; overflow: hidden; text-overflow: ellipsis; max-width: 250px; }

        /* CHAT WINDOW */
        #messages { flex: 1; padding: 12px; overflow-y: auto; display: flex; flex-direction: column; gap: 4px; }
        
        .bubble { 
            padding: 6px 12px; 
            border-radius: 14px; 
            max-width: 85%; 
            font-size: 15px; 
            line-height: 1.4;
            position: relative;
            box-shadow: 0 1px 2px rgba(0,0,0,0.1);
        }
        
        .bubble.me { 
            background: var(--tg-msg-out); 
            align-self: flex-end; 
            border-bottom-right-radius: 4px; 
        }
        
        .bubble.other { 
            background: var(--tg-msg-in); 
            align-self: flex-start; 
            border-bottom-left-radius: 4px; 
        }

        /* INPUT */
        .input-bar { 
            background: var(--tg-header); 
            padding: 8px 12px; 
            display: flex; 
            align-items: center; 
            gap: 10px;
        }
        .input-bar input { 
            flex: 1; border: none; background: transparent; 
            color: white; font-size: 16px; outline: none; padding: 5px 0;
        }
        .send-icon { color: var(--tg-active); cursor: pointer; font-size: 24px; font-weight: bold; }

        /* NAVIGATION BAR */
        .nav-bar { 
            display: flex; 
            background: var(--tg-header); 
            border-top: 1px solid #000;
            padding-bottom: env(safe-area-inset-bottom);
        }
        .nav-btn { 
            flex: 1; padding: 12px 0; text-align: center; 
            color: var(--tg-text-muted); cursor: pointer;
            transition: 0.2s;
        }
        .nav-btn.active { color: var(--tg-active); }
        .nav-label { font-size: 11px; margin-top: 4px; font-weight: 500; }

        /* PROFILE CARD */
        .profile-header { padding: 25px 16px; background: var(--tg-header); display: flex; align-items: center; }
        .profile-avatar { width: 70px; height: 70px; border-radius: 50%; background: var(--tg-active); font-size: 30px; display: flex; align-items: center; justify-content: center; margin-right: 20px; }
        .card { background: var(--tg-header); margin: 8px 0; padding: 15px 20px; border-bottom: 1px solid #0e1621; }
        .owner-gold { color: var(--tg-owner) !important; font-weight: bold; }

    </style>
</head>
<body>

<header>
    <div id="backBtn" class="back-btn" onclick="goBack()">←</div>
    <div class="header-info">
        <div id="headerTitle" class="header-title">TeleX PRO</div>
        <div id="headerStatus" class="header-status"></div>
    </div>
</header>

<div id="chats" class="screen active"></div>

<div id="chatWindow" class="screen">
    <div id="messages"></div>
    <div class="input-bar">
        <input id="msgInput" placeholder="Сообщение" onkeypress="if(event.key==='Enter') sendMessage()">
        <div class="send-icon" onclick="sendMessage()">➤</div>
    </div>
</div>

<div id="channels" class="screen"></div>
<div id="exchange" class="screen"></div>
<div id="profile" class="screen"></div>

<nav class="nav-bar" id="bottomNav">
    <div class="nav-btn active" onclick="showScreen('chats', this)">
        <div style="font-size: 20px;">💬</div>
        <div class="nav-label">Чаты</div>
    </div>
    <div class="nav-btn" onclick="showScreen('channels', this)">
        <div style="font-size: 20px;">📢</div>
        <div class="nav-label">Каналы</div>
    </div>
    <div class="nav-btn" onclick="showScreen('exchange', this)">
        <div style="font-size: 20px;">💰</div>
        <div class="nav-label">Биржа</div>
    </div>
    <div class="nav-btn" onclick="showScreen('profile', this)">
        <div style="font-size: 20px;">👤</div>
        <div class="nav-label">Профиль</div>
    </div>
</nav>

<script>
    const OWNER_EMAIL = "mesilohronaldogod@gmail.com";
    
    let user = JSON.parse(localStorage.getItem("teleUser")) || {
        name: "ADMIN 👑",
        email: OWNER_EMAIL,
        coins: 10000,
        anonymous: false
    };

    let chatsData = JSON.parse(localStorage.getItem("teleChats")) || [
        {id: 0, name: "Команда TeleX", messages: [{sender: "System", text: "Система готова к работе."}]},
        {id: 1, name: "Общий чат", messages: []}
    ];

    let currentChatId = null;
    const isOwner = user.email === OWNER_EMAIL;

    function showScreen(screenId, navEl) {
        currentChatId = null;
        document.querySelectorAll(".screen").forEach(s => s.classList.remove("active"));
        document.getElementById(screenId).classList.add("active");
        
        document.getElementById("backBtn").style.display = "none";
        document.getElementById("bottomNav").style.display = "flex";
        document.getElementById("headerTitle").innerText = "TeleX PRO";
        document.getElementById("headerStatus").innerText = "";

        if(navEl) {
            document.querySelectorAll(".nav-btn").forEach(n => n.classList.remove("active"));
            navEl.classList.add("active");
        }
        render();
    }

    function openChat(chatId) {
        currentChatId = chatId;
        const chat = chatsData.find(c => c.id === chatId);
        document.querySelectorAll(".screen").forEach(s => s.classList.remove("active"));
        document.getElementById("chatWindow").classList.add("active");
        
        document.getElementById("backBtn").style.display = "block";
        document.getElementById("bottomNav").style.display = "none";
        document.getElementById("headerTitle").innerText = chat.name;
        document.getElementById("headerStatus").innerText = "в сети";
        renderMessages();
    }

    function goBack() { showScreen('chats', document.querySelector('.nav-btn')); }

    function render() {
        const activeId = document.querySelector(".screen.active").id;
        if(activeId === 'chats') renderChats();
        if(activeId === 'profile') renderProfile();
        if(activeId === 'exchange') renderExchange();
    }

    function renderChats() {
        const container = document.getElementById("chats");
        container.innerHTML = "";
        chatsData.forEach(chat => {
            const lastMsg = chat.messages[chat.messages.length - 1];
            container.innerHTML += `
                <div class="list-item" onclick="openChat(${chat.id})">
                    <div class="avatar" style="${chat.id === 0 ? 'background: #f39c12; color: #000' : ''}">${chat.name[0]}</div>
                    <div class="item-content">
                        <div class="item-top">
                            <span class="item-name">${chat.name}</span>
                            <span class="item-time">12:00</span>
                        </div>
                        <div class="item-msg">${lastMsg ? lastMsg.text : 'Нет сообщений'}</div>
                    </div>
                </div>
            `;
        });
    }

    function renderMessages() {
        const container = document.getElementById("messages");
        container.innerHTML = "";
        const chat = chatsData.find(c => c.id === currentChatId);
        chat.messages.forEach(m => {
            container.innerHTML += `
                <div class="bubble ${m.sender === user.name ? 'me' : 'other'}">
                    ${m.text}
                </div>
            `;
        });
        container.scrollTop = container.scrollHeight;
    }

    function sendMessage() {
        const input = document.getElementById("msgInput");
        const text = input.value.trim();
        if(!text) return;
        const chat = chatsData.find(c => c.id === currentChatId);
        chat.messages.push({ sender: user.name, text: text });
        input.value = "";
        localStorage.setItem("teleChats", JSON.stringify(chatsData));
        renderMessages();
    }

    function renderProfile() {
        const div = document.getElementById("profile");
        div.innerHTML = `
            <div class="profile-header">
                <div class="profile-avatar" style="${isOwner ? 'background: var(--tg-owner); color: black;' : ''}">${user.name[0]}</div>
                <div>
                    <div style="font-size: 20px; font-weight: bold;">${user.name} ${isOwner ? '👑' : ''}</div>
                    <div style="color: var(--tg-text-muted); font-size: 14px;">${user.email}</div>
                </div>
            </div>
            <div class="card">
                <div style="color: var(--tg-active); font-size: 14px;">О себе</div>
                <div style="margin-top: 5px;">${isOwner ? 'Владелец системы TeleX PRO' : 'Пользователь'}</div>
            </div>
            <div class="card">
                <div style="color: var(--tg-active); font-size: 14px;">Баланс</div>
                <div style="font-size: 18px; font-weight: bold; margin-top: 5px;">${user.coins} 💰</div>
                ${isOwner ? `<button onclick="addCash()" style="margin-top:10px; padding: 5px 10px; background: var(--tg-owner); border:none; border-radius:5px; cursor:pointer">Добавить монеты (Owner)</button>` : ''}
            </div>
        `;
    }

    function addCash() {
        user.coins += 1000;
        localStorage.setItem("teleUser", JSON.stringify(user));
        renderProfile();
    }

    function renderExchange() {
        document.getElementById("exchange").innerHTML = `<div class="card"><h2 class="${isOwner ? 'owner-gold' : ''}">Биржа Активна</h2><p>Курс монеты: 1.25$</p></div>`;
    }

    render();
</script>
</body>
</html>
