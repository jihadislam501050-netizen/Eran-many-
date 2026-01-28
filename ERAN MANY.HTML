<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Earn Money - VIP Panel</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        @keyframes borderGlow {
            0% { border-color: #3b82f6; box-shadow: 0 0 10px #3b82f6; }
            33% { border-color: #9333ea; box-shadow: 0 0 15px #9333ea; }
            66% { border-color: #ec4899; box-shadow: 0 0 10px #ec4899; }
            100% { border-color: #3b82f6; box-shadow: 0 0 10px #3b82f6; }
        }

        body { background-color: #020617; color: white; font-family: 'Arial', sans-serif; overflow: hidden; }
        
        .glow-box { 
            background: #0f172a; 
            border: 2px solid; 
            animation: borderGlow 2.5s linear infinite; 
            border-radius: 15px; 
        }

        .hidden-section { display: none; }
        
        #minimize-dot { position: fixed; top: 6px; right: 6px; width: 4px; height: 4px; background: rgba(255,255,255,0.1); border-radius: 50%; z-index: 9999; }

        /* মেথড সিলেক্ট ইফেক্ট (আলো দিয়ে ভরে যাওয়া) */
        .method-btn { transition: 0.4s; position: relative; overflow: hidden; }
        .method-active { 
            background: #3b82f6 !important; 
            box-shadow: 0 0 30px #3b82f6, inset 0 0 20px #ffffff; 
            border-color: #fff !important;
            color: white !important;
            transform: scale(1.05);
        }

        #task-modal {
            position: fixed; inset: 0; background: rgba(0,0,0,0.9);
            display: none; align-items: center; justify-content: center; z-index: 10000;
        }
    </style>
</head>
<body onload="initApp()">

    <div id="minimize-dot"></div>

    <div id="task-modal">
        <div class="glow-box p-8 w-80 text-center">
            <h3 class="text-xl font-bold mb-4">বিজ্ঞাপন দেখুন</h3>
            <p class="text-gray-400 text-sm mb-6">দয়া করে <span id="timer" class="text-blue-500 font-bold text-lg">১৫</span> সেকেন্ড অপেক্ষা করুন...</p>
            <button id="close-task-btn" onclick="closeTask()" class="hidden w-full bg-red-600 py-2 rounded-lg font-bold">Cancel / Close</button>
        </div>
    </div>

    <div class="h-screen flex flex-col">
        
        <div class="p-4 flex justify-between items-center bg-gray-900/90 border-b border-gray-800">
            <i class="fa-solid fa-gem text-blue-400"></i>
            <h1 class="text-md font-black tracking-widest text-blue-400 uppercase">Earn Money</h1>
            <div id="user-photo" class="w-8 h-8 rounded-full bg-blue-600 border border-blue-400 overflow-hidden"></div>
        </div>

        <div id="sections" class="flex-1 overflow-y-auto p-4 pb-28">
            
            <section id="home-sec">
                <div class="glow-box p-5 mb-6">
                    <div class="flex items-center gap-4">
                        <div id="user-p-lg" class="w-14 h-14 rounded-full bg-blue-600 flex items-center justify-center text-xl font-bold border-2 border-white/20">U</div>
                        <div>
                            <p id="user-name" class="text-lg font-bold">Loading...</p>
                            <p class="text-xs text-green-400">ব্যালেন্স: ৳ <span id="balance-main">111.00</span></p>
                        </div>
                    </div>
                </div>

                <div class="grid grid-cols-2 gap-4 mb-4">
                    <div class="glow-box p-4 text-center">
                        <p class="text-[10px] text-gray-400">আজকের এড</p>
                        <p id="ads-count" class="text-xl font-black">0 / 35</p>
                    </div>
                    <div class="glow-box p-4 text-center">
                        <p class="text-[10px] text-gray-400">রেফারেল</p>
                        <p id="ref-count" class="text-xl font-black text-purple-400">0</p>
                    </div>
                </div>

                <div class="glow-box p-4 mt-2 cursor-pointer" onclick="copyReferLink()">
                    <p class="text-[10px] font-bold text-blue-400 mb-1 text-center">কপি করতে ক্লিক করুন (বোনাস ১১১৳)</p>
                    <div class="flex items-center justify-between bg-black/40 p-2 rounded border border-gray-700">
                        <span id="ref-link" class="text-[10px] truncate">https://t.me/Earn_Many_Bot?start=user718</span>
                        <i class="fa-solid fa-copy text-blue-500 text-xs"></i>
                    </div>
                </div>

                <div class="grid grid-cols-1 gap-4 mt-6">
                    <div class="glow-box p-4 flex items-center gap-4">
                        <i class="fa-solid fa-crown text-yellow-500 text-2xl"></i>
                        <div>
                            <h4 class="text-sm font-bold text-blue-400">VIP ADS</h4>
                            <p id="vip-ad-text" class="text-[10px] text-gray-400 italic">বিজ্ঞাপন লোড হচ্ছে...</p>
                        </div>
                    </div>
                    <div class="glow-box p-4 flex items-center gap-4">
                        <i class="fa-solid fa-bullhorn text-green-500 text-2xl"></i>
                        <div>
                            <h4 class="text-sm font-bold text-green-400">NOTICE BOARD</h4>
                            <p id="notice-ad-text" class="text-[10px] text-gray-400 italic">নতুন নোটিশ আসছে...</p>
                        </div>
                    </div>
                </div>
            </section>

            <section id="task-sec" class="hidden-section">
                <div class="glow-box p-10 text-center">
                    <div class="inline-block p-4 rounded-full bg-blue-500/10 mb-4">
                        <i class="fa-solid fa-circle-play text-6xl text-blue-500 animate-pulse"></i>
                    </div>
                    <h2 class="text-xl font-black mb-2 text-blue-400">ভিডিও টাস্ক</h2>
                    <p class="text-gray-400 text-xs mb-8 uppercase tracking-widest">একটি এ্যাড = ৫.০০ টাকা</p>
                    <button onclick="startTask()" id="task-btn" class="w-full bg-gradient-to-r from-blue-600 to-purple-600 py-4 rounded-2xl font-black shadow-lg">AD দেখতে ক্লিক করুন</button>
                </div>
            </section>

            <section id="withdraw-sec" class="hidden-section">
                <h3 class="mb-4 text-sm font-bold text-blue-400 uppercase text-center">পেমেন্ট মেথড</h3>
                <div class="grid grid-cols-3 gap-3 mb-6">
                    <button onclick="setMethod(this, 'bKash')" class="glow-box p-4 text-xs font-black method-btn">বিকাশ</button>
                    <button onclick="setMethod(this, 'Nagad')" class="glow-box p-4 text-xs font-black method-btn">নগদ</button>
                    <button onclick="setMethod(this, 'Rocket')" class="glow-box p-4 text-xs font-black method-btn">রকেট</button>
                </div>
                <div class="space-y-4">
                    <input type="number" id="w-phone" placeholder="আপনার একাউন্ট নম্বর দিন" class="glow-box w-full bg-transparent p-4 outline-none text-sm">
                    <input type="number" id="w-amount" placeholder="টাকার পরিমাণ (মিনিমাম ৫০০)" class="glow-box w-full bg-transparent p-4 outline-none text-sm">
                    <button onclick="requestWithdraw()" class="w-full bg-blue-600 py-4 rounded-2xl font-black text-lg">উত্তোলন</button>
                </div>
            </section>

        </div>

        <div class="fixed bottom-0 w-full bg-gray-950 border-t border-gray-800 flex justify-around p-4">
            <button onclick="showSec('home-sec', this)" class="nav-btn text-blue-500 flex flex-col items-center">
                <i class="fa-solid fa-house"></i><span class="text-[9px]">হোম</span>
            </button>
            <button onclick="showSec('task-sec', this)" class="nav-btn text-gray-500 flex flex-col items-center">
                <i class="fa-solid fa-play"></i><span class="text-[9px]">টাস্ক</span>
            </button>
            <button onclick="showSec('withdraw-sec', this)" class="nav-btn text-gray-500 flex flex-col items-center">
                <i class="fa-solid fa-wallet"></i><span class="text-[9px]">উত্তোলন</span>
            </button>
        </div>
    </div>

    <script>
        let tg = window.Telegram.WebApp;
        let balance = 111.00;
        let adsDone = 0;
        let selectedMethod = "";

        function initApp() {
            tg.expand();
            const user = tg.initDataUnsafe?.user;
            if (user) document.getElementById('user-name').innerText = user.first_name;
        }

        history.pushState(null, null, location.href);
        window.onpopstate = () => history.go(1);

        function showSec(id, btn) {
            document.querySelectorAll('section').forEach(s => s.classList.add('hidden-section'));
            document.getElementById(id).classList.remove('hidden-section');
            document.querySelectorAll('.nav-btn').forEach(b => b.classList.replace('text-blue-500', 'text-gray-500'));
            btn.classList.add('text-blue-500');
        }

        function copyReferLink() {
            navigator.clipboard.writeText(document.getElementById('ref-link').innerText);
            alert("লিঙ্ক কপি হয়েছে!");
        }

        // মেথড সিলেক্ট লজিক (আলোর ইফেক্টসহ)
        function setMethod(btn, m) {
            document.querySelectorAll('.method-btn').forEach(b => b.classList.remove('method-active'));
            btn.classList.add('method-active');
            selectedMethod = m;
        }

        // টাস্ক লজিক (৫ টাকা প্রতি অ্যাড)
        function startTask() {
            if (adsDone >= 35) return alert("আজকের লিমিট শেষ!");
            window.open("https://www.effectivegatecpm.com/wzacd8ppk?key=d5926c0ef7c1dc7212610c458cd5ff37", "_blank");

            document.getElementById('task-modal').style.display = 'flex';
            document.getElementById('close-task-btn').classList.add('hidden');
            let sec = 15;
            document.getElementById('timer').innerText = sec;

            let countdown = setInterval(() => {
                sec--;
                document.getElementById('timer').innerText = sec;
                if (sec <= 0) {
                    clearInterval(countdown);
                    document.getElementById('close-task-btn').classList.remove('hidden');
                    adsDone++;
                    balance += 5.00; // ৫ টাকা যোগ হবে
                    document.getElementById('ads-count').innerText = adsDone + " / 35";
                    document.getElementById('balance-main').innerText = balance.toFixed(2);
                }
            }, 1000);
        }

        function closeTask() {
            document.getElementById('task-modal').style.display = 'none';
        }

        function requestWithdraw() {
            const num = document.getElementById('w-phone').value;
            const amt = document.getElementById('w-amount').value;
            if(!selectedMethod) return alert("মেথড সিলেক্ট করুন!");
            if(!num) return alert("নম্বর দিন!");
            alert("কমপক্ষে ১২টি রেফার প্রয়োজন!");
        }

        setInterval(() => {
            const ads = ["নতুন VIP অফার!", "পেমেন্ট গ্যারান্টি!", "রেফার করুন 110৳"];
            document.getElementById('vip-ad-text').innerText = ads[Math.floor(Math.random() * ads.length)];
            document.getElementById('notice-ad-text').innerText = "প্রতি এ্যাড এখন ৫ টাকা!";
        }, 15000);
    </script>
</body>
</html>
