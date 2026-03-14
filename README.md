# Biomastery
This makes bio efficient , effective and easy to understand.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BioMastery | Grade 9 FBISE Study Hub</title>
    <style>
        :root { --primary: #27ae60; --secondary: #2980b9; --dark: #2c3e50; --gold: #f1c40f; --light: #ecf0f1; }
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; margin: 0; background: #f4f7f6; color: var(--dark); line-height: 1.6; }
        
        /* Navigation & Header */
        nav { background: var(--dark); color: white; padding: 1rem 5%; display: flex; justify-content: space-between; align-items: center; position: sticky; top: 0; z-index: 100; }
        .logo { font-size: 1.5rem; font-weight: bold; color: var(--primary); }
        .wallet-display { background: var(--primary); padding: 5px 15px; border-radius: 20px; font-weight: bold; }

        .container { max-width: 1100px; margin: 20px auto; padding: 0 20px; display: grid; grid-template-columns: 1fr 320px; gap: 30px; }
        
        /* Ad & Revenue Sections */
        .ad-box { background: #dfe6e9; border: 2px dashed #b2bec3; text-align: center; padding: 20px; margin-bottom: 20px; color: #636e72; border-radius: 8px; font-size: 0.8rem; }
        
        /* Content Cards */
        .card { background: white; padding: 25px; border-radius: 12px; margin-bottom: 25px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); border-left: 5px solid var(--secondary); }
        h2 { color: var(--secondary); margin-top: 0; }
        .btn { display: inline-block; padding: 10px 20px; border: none; border-radius: 5px; cursor: pointer; font-weight: bold; text-decoration: none; transition: 0.3s; text-align: center; }
        .btn-study { background: var(--secondary); color: white; }
        .btn-premium { background: var(--gold); color: var(--dark); width: 100%; margin-top: 10px; }

        /* Tablet/Mobile Responsive */
        @media (max-width: 850px) { .container { grid-template-columns: 1fr; } }
    </style>
</head>
<body>

<nav>
    <div class="logo">BioMastery 🧬</div>
    <div class="wallet-display">Earnings: $<span id="balance">0.00</span></div>
</nav>

<div class="container">
    <main>
        <div class="ad-box">AD REVENUE SPACE (Google AdSense Code Goes Here)</div>

        <section class="card">
            <h2>1. Mitosis: Growth & Repair 🩹</h2>
            <p>Master how somatic cells divide. Key for your FBISE exams!</p>
            <ul>
                <li><strong>Prophase:</strong> Chromatin condenses; nucleus disappears.</li>
                <li><strong>Metaphase:</strong> Chromosomes line up in the middle.</li>
                <li><strong>Anaphase:</strong> Sister chromatids pull apart.</li>
                <li><strong>Telophase:</strong> Two new nuclei form.</li>
            </ul>
            <p><em>Pro-Tip:</em> Remember the <strong>Phragmoplast</strong> in plants vs. <strong>Cleavage Furrow</strong> in animals!</p>
            <button class="btn btn-study" onclick="simulateEarn(0.05)">Complete Lesson (Earn $0.05)</button>
        </section>

        <section class="card">
            <h2>2. Meiosis: Genetic Variation 🎲</h2>
            <p>Understand the "Reduction Division" and why we are all unique.</p>
            <p><strong>Crossing Over:</strong> Occurs in Prophase I at the <strong>Chiasmata</strong>. This swaps DNA between homologous chromosomes!</p>
            <button class="btn btn-study" onclick="simulateEarn(0.10)">Take Meiosis Quiz (Earn $0.10)</button>
        </section>

        <section class="card">
            <h2>3. Non-Disjunction Errors ⚠️</h2>
            <p>What happens when chromosomes fail to separate?</p>
            <ul>
                <li><strong>Trisomy 21:</strong> Down's Syndrome (Extra chromosome).</li>
                <li><strong>Monosomy:</strong> Missing a chromosome (e.g., Turner's Syndrome).</li>
            </ul>
        </section>
    </main>

    <aside>
        <div class="card" style="border-left: 5px solid var(--gold);">
            <h3 style="margin-top:0">💰 Premium Notes</h3>
            <p><small>Get the full PDF diagrams for your final exam prep.</small></p>
            <div style="border-top: 1px solid #eee; padding-top: 10px;">
                <strong>The Ultimate Bio Chart</strong>
                <p style="font-size: 0.8rem; color: #666;">Mitosis vs Meiosis Detailed Comparison</p>
                <a href="#" class="btn btn-premium">BUY PDF - $0.99</a>
            </div>
        </div>

        <div class="ad-box" style="height: 250px;">SIDEBAR AD UNIT</div>
    </aside>
</div>

<script>
    let earnings = 0.00;
    function simulateEarn(amount) {
        earnings += amount;
        document.getElementById('balance').innerText = earnings.toFixed(2);
        alert("Action tracked! Your creator revenue has been updated.");
    }
</script>

</body>
</html>
