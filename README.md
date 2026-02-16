# top-up-game[to up.github.io.html](https://github.com/user-attachments/files/25335429/to.up.github.io.html)
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NexGen TopUp | Website Top Up Game Termurah</title>
    <style>
        /* --- 1. CSS MODERN & RESET --- */
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --primary: #6366f1; /* Indigo */
            --accent: #06b6d4; /* Cyan */
            --text: #f8fafc;
            --text-muted: #94a3b8;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }

        body {
            background-color: var(--bg-color);
            color: var(--text);
            padding-bottom: 50px;
        }

        /* --- HEADER --- */
        header {
            background: rgba(30, 41, 59, 0.8);
            backdrop-filter: blur(10px);
            padding: 20px;
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 1px solid #334155;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo { font-size: 1.5rem; font-weight: bold; color: var(--accent); text-transform: uppercase; letter-spacing: 2px; }
        .logo span { color: var(--primary); }

        /* --- HERO SECTION --- */
        .hero {
            text-align: center;
            padding: 60px 20px;
            background: linear-gradient(180deg, rgba(99, 102, 241, 0.1) 0%, rgba(15, 23, 42, 0) 100%);
        }
        .hero h1 { font-size: 2.5rem; margin-bottom: 10px; }
        .hero p { color: var(--text-muted); }

        /* --- CONTAINER --- */
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* --- SECTIONS --- */
        .section-title {
            margin: 40px 0 20px;
            font-size: 1.2rem;
            border-left: 4px solid var(--accent);
            padding-left: 10px;
        }

        /* --- GAME GRID --- */
        .game-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
            gap: 15px;
        }

        .game-card {
            background: var(--card-bg);
            border-radius: 12px;
            padding: 10px;
            text-align: center;
            cursor: pointer;
            transition: transform 0.2s, border 0.2s;
            border: 2px solid transparent;
        }

        .game-card:hover, .game-card.active {
            border-color: var(--primary);
            transform: translateY(-5px);
        }

        .game-icon {
            width: 60px;
            height: 60px;
            background: linear-gradient(45deg, #333, #555);
            border-radius: 12px;
            margin: 0 auto 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
        }

        /* --- FORM INPUT --- */
        .input-group {
            margin-bottom: 20px;
        }
        
        input[type="text"], input[type="number"] {
            width: 100%;
            padding: 15px;
            background: var(--card-bg);
            border: 1px solid #334155;
            color: white;
            border-radius: 8px;
            font-size: 1rem;
            outline: none;
        }
        
        input:focus { border-color: var(--accent); }

        /* --- ITEM GRID (NOMINAL) --- */
        .item-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
        }

        .item-card {
            background: var(--card-bg);
            padding: 15px;
            border-radius: 8px;
            cursor: pointer;
            border: 1px solid #334155;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .item-card:hover, .item-card.active {
            background: #28364d;
            border-color: var(--accent);
        }

        .price { color: var(--accent); font-weight: bold; }

        /* --- PAYMENT METHOD --- */
        .payment-card {
            background: white; /* Contrast for logos */
            color: black;
            padding: 10px;
            border-radius: 8px;
            margin-bottom: 10px;
            cursor: pointer;
            display: flex;
            align-items: center;
            font-weight: bold;
            border: 2px solid transparent;
        }

        .payment-card.active {
            border-color: var(--primary);
            background: #e0e7ff;
        }

        /* --- FOOTER & BUTTON --- */
        .sticky-footer {
            position: fixed;
            bottom: 0;
            left: 0;
            width: 100%;
            background: var(--card-bg);
            padding: 15px 20px;
            border-top: 1px solid #334155;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 -5px 20px rgba(0,0,0,0.5);
        }

        .total-price { font-size: 1.1rem; }
        .total-price span { color: var(--accent); font-weight: bold; font-size: 1.3rem; }

        .btn-buy {
            background: var(--primary);
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 50px;
            font-weight: bold;
            font-size: 1rem;
            cursor: pointer;
            transition: background 0.3s;
        }

        .btn-buy:hover { background: #4f46e5; }

        /* Helper to hide sections */
        .hidden { display: none; }
        
    </style>
</head>
<body>

    <header>
        <div class="logo">NexGen<span>TopUp</span></div>
        <div style="font-size: 0.9rem;">Masuk / Daftar</div>
    </header>

    <div class="hero">
        <h1>Top Up Game Kilat</h1>
        <p>Proses detik, harga termurah, 100% aman.</p>
    </div>

    <div class="container">
        
        <h2 class="section-title">1. Pilih Game</h2>
        <div class="game-grid">
            <div class="game-card" onclick="selectGame(this, 'Mobile Legends')">
                <div class="game-icon">⚔️</div>
                <div class="game-name">Mobile Legends</div>
            </div>
            <div class="game-card" onclick="selectGame(this, 'Free Fire')">
                <div class="game-icon">🔥</div>
                <div class="game-name">Free Fire</div>
            </div>
            <div class="game-card" onclick="selectGame(this, 'PUBG Mobile')">
                <div class="game-icon">🪖</div>
                <div class="game-name">PUBG Mobile</div>
            </div>
            <div class="game-card" onclick="selectGame(this, 'Genshin Impact')">
                <div class="game-icon">✨</div>
                <div class="game-name">Genshin Impact</div>
            </div>
        </div>

        <div id="topup-form" class="hidden">
            
            <h2 class="section-title">2. Masukkan ID Player</h2>
            <div class="input-group">
                <input type="text" id="userId" placeholder="Masukkan User ID (Contoh: 12345678)">
            </div>

            <h2 class="section-title">3. Pilih Nominal</h2>
            <div class="item-grid">
                <div class="item-card" onclick="selectItem(this, 3000)">
                    <span>💎 10 Diamonds</span>
                    <span class="price">Rp 3.000</span>
                </div>
                <div class="item-card" onclick="selectItem(this, 15000)">
                    <span>💎 50 Diamonds</span>
                    <span class="price">Rp 15.000</span>
                </div>
                <div class="item-card" onclick="selectItem(this, 30000)">
                    <span>💎 100 Diamonds</span>
                    <span class="price">Rp 30.000</span>
                </div>
                <div class="item-card" onclick="selectItem(this, 75000)">
                    <span>💎 250 Diamonds</span>
                    <span class="price">Rp 75.000</span>
                </div>
                <div class="item-card" onclick="selectItem(this, 150000)">
                    <span>💎 500 Diamonds</span>
                    <span class="price">Rp 150.000</span>
                </div>
                <div class="item-card" onclick="selectItem(this, 300000)">
                    <span>💎 1000 Diamonds</span>
                    <span class="price">Rp 300.000</span>
                </div>
            </div>

            <h2 class="section-title">4. Metode Pembayaran</h2>
            <div class="payment-card" onclick="selectPayment(this)">
                <span>QRIS (Dana/Gopay/OVO)</span>
            </div>
            <div class="payment-card" onclick="selectPayment(this)">
                <span>Virtual Account BCA</span>
            </div>
            <div class="payment-card" onclick="selectPayment(this)">
                <span>Indomaret / Alfamart</span>
            </div>

            <div style="height: 100px;"></div>
        </div>

    </div>

    <div class="sticky-footer hidden" id="footer-checkout">
        <div class="total-price">
            Total Bayar:<br>
            <span id="display-price">Rp 0</span>
        </div>
        <button class="btn-buy" onclick="processPayment()">Beli Sekarang</button>
    </div>

    <script>
        // --- JAVASCRIPT LOGIC ---
        
        let selectedPrice = 0;
        let selectedGameName = "";

        // Fungsi memilih game
        function selectGame(element, gameName) {
            // Hapus kelas active dari semua game
            document.querySelectorAll('.game-card').forEach(el => el.classList.remove('active'));
            // Tambah kelas active ke yang dipilih
            element.classList.add('active');
            
            // Tampilkan form
            document.getElementById('topup-form').classList.remove('hidden');
            selectedGameName = gameName;
            
            // Scroll sedikit ke bawah agar user tahu ada form
            setTimeout(() => {
                document.getElementById('userId').scrollIntoView({ behavior: 'smooth', block: 'center' });
            }, 300);
        }

        // Fungsi memilih nominal item
        function selectItem(element, price) {
            document.querySelectorAll('.item-card').forEach(el => el.classList.remove('active'));
            element.classList.add('active');
            
            selectedPrice = price;
            updateTotal();
            
            // Tampilkan footer checkout
            document.getElementById('footer-checkout').classList.remove('hidden');
        }

        // Fungsi memilih pembayaran (visual saja)
        function selectPayment(element) {
            document.querySelectorAll('.payment-card').forEach(el => el.classList.remove('active'));
            element.classList.add('active');
        }

        // Update tampilan harga total
        function updateTotal() {
            // Format angka ke Rupiah
            const formatted = new Intl.NumberFormat('id-ID', { style: 'currency', currency: 'IDR', minimumFractionDigits: 0 }).format(selectedPrice);
            document.getElementById('display-price').innerText = formatted;
        }

        // Simulasi tombol beli
        function processPayment() {
            const userId = document.getElementById('userId').value;
            
            if(!userId) {
                alert("Mohon masukkan User ID game Anda!");
                return;
            }

            if(selectedPrice === 0) {
                alert("Mohon pilih nominal top up!");
                return;
            }

            // Simulasi Sukses
            alert(`
            PESANAN DIKONFIRMASI!
            ---------------------
            Game: ${selectedGameName}
            ID: ${userId}
            Total: Rp ${selectedPrice.toLocaleString('id-ID')}
            
            Terima kasih telah berbelanja di NexGen TopUp!
            `);
        }
    </script>
</body>
</html>
