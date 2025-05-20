<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ultimate Loan Calculator Suite | All-in-One Financial Tool</title>
    <meta name="description" content="Professional EMI calculators for Home Loans, Car Loans, Bike Loans, and Loan Moratorium calculations with detailed amortization schedules and interest comparisons">
    <meta name="keywords" content="EMI calculator, loan calculator, home loan, car loan, bike loan, financial planning">
    <link rel="canonical" href="https://www.yourdomain.com/loan-calculators">
    
    <!-- Google AdSense -->
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX" crossorigin="anonymous"></script>

    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --success: #27ae60;
            --danger: #c0392b;
            --light: #ecf0f1;
            --dark: #2c3e50;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', system-ui, sans-serif;
        }

        body {
            background: #f8f9fa;
            color: var(--dark);
            line-height: 1.6;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 2rem 1rem;
        }

        .calculator-tabs {
            display: flex;
            gap: 1rem;
            overflow-x: auto;
            padding: 1rem 0;
            margin-bottom: 2rem;
        }

        .tab-btn {
            background: var(--light);
            border: none;
            padding: 1rem 2rem;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s;
            white-space: nowrap;
            font-weight: 600;
        }

        .tab-btn.active {
            background: var(--secondary);
            color: white;
            box-shadow: 0 4px 15px rgba(52, 152, 219, 0.3);
        }

        .calculator-card {
            background: white;
            border-radius: 1.5rem;
            padding: 2.5rem;
            margin: 2rem 0;
            box-shadow: 0 10px 40px rgba(0,0,0,0.08);
        }

        .calculator-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            margin-top: 2rem;
        }

        .input-group {
            margin-bottom: 1.8rem;
        }

        .input-label {
            display: block;
            margin-bottom: 0.8rem;
            font-weight: 600;
            color: var(--dark);
            font-size: 1.05rem;
        }

        .input-field {
            width: 100%;
            padding: 1.2rem;
            border: 2px solid #e0e0e0;
            border-radius: 0.8rem;
            font-size: 1.1rem;
            transition: all 0.3s;
            background: #f8f9fa;
        }

        .input-field:focus {
            border-color: var(--secondary);
            background: white;
            box-shadow: 0 0 0 3px rgba(52, 152, 219, 0.1);
            outline: none;
        }

        .range-slider {
            width: 100%;
            margin-top: 1rem;
            height: 6px;
            border-radius: 3px;
            background: #e0e0e0;
            -webkit-appearance: none;
        }

        .range-slider::-webkit-slider-thumb {
            -webkit-appearance: none;
            width: 20px;
            height: 20px;
            background: var(--secondary);
            border-radius: 50%;
            cursor: pointer;
            transition: transform 0.2s;
        }

        .result-section {
            margin-top: 3rem;
            padding: 2rem;
            background: var(--light);
            border-radius: 1rem;
        }

        .amortization-table {
            overflow-x: auto;
            margin-top: 2rem;
            border-radius: 0.8rem;
            box-shadow: 0 2px 15px rgba(0,0,0,0.05);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: white;
            min-width: 600px;
        }

        th, td {
            padding: 1.2rem;
            text-align: center;
            border-bottom: 1px solid #eee;
        }

        th {
            background: var(--primary);
            color: white;
            font-weight: 600;
        }

        .pie-chart {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            margin: 0 auto;
            background: conic-gradient(
                var(--success) 0% var(--principal-percent),
                var(--danger) var(--principal-percent) 100%
            );
            transition: all 0.5s ease;
        }

        .ad-section {
            margin: 3rem 0;
            text-align: center;
            padding: 2rem;
            background: white;
            border-radius: 1rem;
            box-shadow: 0 5px 20px rgba(0,0,0,0.05);
        }

        @media (max-width: 768px) {
            .container {
                padding: 1rem;
            }
            .calculator-grid {
                grid-template-columns: 1fr;
            }
            .calculator-card {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header Ad -->
        <div class="ad-section">
            <ins class="adsbygoogle" style="display:block" data-ad-client="ca-pub-XXXXXXXXXXXXXXXX" data-ad-slot="1234567890"></ins>
        </div>

        <h1>Ultimate Loan Calculator Suite</h1>
        
        <nav class="calculator-tabs">
            <button class="tab-btn active" data-tab="home">🏠 Home Loan</button>
            <button class="tab-btn" data-tab="car">🚗 Car Loan</button>
            <button class="tab-btn" data-tab="bike">🏍 Two Wheeler</button>
            <button class="tab-btn" data-tab="compare">📊 Rate Compare</button>
            <button class="tab-btn" data-tab="moratorium">⏸ Moratorium</button>
        </nav>

        <!-- Home Loan Calculator -->
        <div class="calculator-card active-tab" id="home">
            <h2>🏠 Home Loan Calculator</h2>
            <div class="calculator-grid">
                <div>
                    <div class="input-group">
                        <label class="input-label">Loan Amount (₹)</label>
                        <input type="number" id="home-amount" class="input-field" value="5000000" step="100000">
                        <input type="range" class="range-slider" min="1000000" max="50000000" step="100000">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Interest Rate (%)</label>
                        <input type="number" id="home-rate" class="input-field" value="8.4" step="0.1">
                        <input type="range" class="range-slider" min="6" max="15" step="0.1">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Tenure (Years)</label>
                        <input type="number" id="home-tenure" class="input-field" value="20" min="5" max="30">
                        <input type="range" class="range-slider" min="5" max="30" step="1">
                    </div>
                </div>
                <div class="result-section">
                    <h3>Monthly EMI: ₹<span id="home-emi">0</span></h3>
                    <div class="chart-container">
                        <div class="pie-chart" style="--principal-percent: 50%"></div>
                        <div>
                            <p>Total Interest: ₹<span id="home-interest">0</span></p>
                            <p>Total Payment: ₹<span id="home-total">0</span></p>
                            <p>Loan Period: <span id="home-period">0</span> months</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="amortization-table">
                <table>
                    <thead><tr><th>Month</th><th>Principal</th><th>Interest</th><th>Balance</th></tr></thead>
                    <tbody id="home-schedule"></tbody>
                </table>
            </div>
        </div>

        <!-- Car Loan Calculator -->
        <div class="calculator-card" id="car" style="display:none;">
            <h2>🚗 Car Loan Calculator</h2>
            <div class="calculator-grid">
                <div>
                    <div class="input-group">
                        <label class="input-label">Loan Amount (₹)</label>
                        <input type="number" id="car-amount" class="input-field" value="800000" step="50000">
                        <input type="range" class="range-slider" min="100000" max="5000000" step="50000">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Interest Rate (%)</label>
                        <input type="number" id="car-rate" class="input-field" value="9.5" step="0.1">
                        <input type="range" class="range-slider" min="7" max="20" step="0.1">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Tenure (Years)</label>
                        <input type="number" id="car-tenure" class="input-field" value="5" min="1" max="7">
                        <input type="range" class="range-slider" min="1" max="7" step="0.5">
                    </div>
                </div>
                <div class="result-section">
                    <h3>Monthly EMI: ₹<span id="car-emi">0</span></h3>
                    <div class="chart-container">
                        <div class="pie-chart" style="--principal-percent: 50%"></div>
                        <div>
                            <p>Total Interest: ₹<span id="car-interest">0</span></p>
                            <p>Total Payment: ₹<span id="car-total">0</span></p>
                            <p>Loan Period: <span id="car-period">0</span> months</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="amortization-table">
                <table>
                    <thead><tr><th>Month</th><th>Principal</th><th>Interest</th><th>Balance</th></tr></thead>
                    <tbody id="car-schedule"></tbody>
                </table>
            </div>
        </div>

        <!-- Two Wheeler Loan Calculator -->
        <div class="calculator-card" id="bike" style="display:none;">
            <h2>🏍 Two Wheeler Loan Calculator</h2>
            <div class="calculator-grid">
                <div>
                    <div class="input-group">
                        <label class="input-label">Loan Amount (₹)</label>
                        <input type="number" id="bike-amount" class="input-field" value="100000" step="10000">
                        <input type="range" class="range-slider" min="50000" max="500000" step="10000">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Interest Rate (%)</label>
                        <input type="number" id="bike-rate" class="input-field" value="12.5" step="0.1">
                        <input type="range" class="range-slider" min="10" max="25" step="0.1">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Tenure (Years)</label>
                        <input type="number" id="bike-tenure" class="input-field" value="3" min="1" max="5">
                        <input type="range" class="range-slider" min="1" max="5" step="0.5">
                    </div>
                </div>
                <div class="result-section">
                    <h3>Monthly EMI: ₹<span id="bike-emi">0</span></h3>
                    <div class="chart-container">
                        <div class="pie-chart" style="--principal-percent: 50%"></div>
                        <div>
                            <p>Total Interest: ₹<span id="bike-interest">0</span></p>
                            <p>Total Payment: ₹<span id="bike-total">0</span></p>
                            <p>Loan Period: <span id="bike-period">0</span> months</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="amortization-table">
                <table>
                    <thead><tr><th>Month</th><th>Principal</th><th>Interest</th><th>Balance</th></tr></thead>
                    <tbody id="bike-schedule"></tbody>
                </table>
            </div>
        </div>

        <!-- Rate Comparison Calculator -->
        <div class="calculator-card" id="compare" style="display:none;">
            <h2>📊 Flat Rate vs Reducing Balance</h2>
            <div class="calculator-grid">
                <div>
                    <div class="input-group">
                        <label class="input-label">Loan Amount (₹)</label>
                        <input type="number" id="compare-amount" class="input-field" value="500000">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Interest Rate (%)</label>
                        <input type="number" id="compare-rate" class="input-field" value="10.5">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Tenure (Years)</label>
                        <input type="number" id="compare-tenure" class="input-field" value="5">
                    </div>
                </div>
                <div class="result-section">
                    <div class="comparison-result">
                        <h3>Flat Rate EMI: ₹<span id="flat-emi">0</span></h3>
                        <p>Total Interest: ₹<span id="flat-interest">0</span></p>
                    </div>
                    <div class="comparison-result">
                        <h3>Reducing Balance EMI: ₹<span id="reducing-emi">0</span></h3>
                        <p>Total Interest: ₹<span id="reducing-interest">0</span></p>
                    </div>
                    <div class="interest-saving">
                        <h4>You Save: ₹<span id="interest-saving">0</span></h4>
                        <p>With Reducing Balance</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Mid Content Ad -->
        <div class="ad-section">
            <ins class="adsbygoogle" style="display:block" data-ad-format="fluid" data-ad-layout-key="-gw-3+1f-3d+2z"></ins>
        </div>

        <!-- Moratorium Calculator -->
        <div class="calculator-card" id="moratorium" style="display:none;">
            <h2>⏸ EMI Moratorium Calculator</h2>
            <div class="calculator-grid">
                <div>
                    <div class="input-group">
                        <label class="input-label">Original Loan Amount (₹)</label>
                        <input type="number" id="moratorium-amount" class="input-field" value="1000000">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Interest Rate (%)</label>
                        <input type="number" id="moratorium-rate" class="input-field" value="9">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Original Tenure (Years)</label>
                        <input type="number" id="original-tenure" class="input-field" value="5">
                    </div>
                    <div class="input-group">
                        <label class="input-label">Moratorium Period (Months)</label>
                        <input type="number" id="moratorium-period" class="input-field" value="6" min="0" max="24">
                    </div>
                </div>
                <div class="result-section">
                    <h3>Revised EMI: ₹<span id="revised-emi">0</span></h3>
                    <div class="emi-breakdown">
                        <p>Additional Interest: ₹<span id="additional-interest">0</span></p>
                        <p>New Tenure: <span id="new-tenure">0</span> Months</p>
                        <p>Total Interest Paid: ₹<span id="total-moratorium-interest">0</span></p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Footer Ad -->
        <div class="ad-section">
            <ins class="adsbygoogle" style="display:block" data-ad-client="ca-pub-XXXXXXXXXXXXXXXX" data-ad-slot="0987654321"></ins>
        </div>
    </div>

    <script>
        const LoanManager = {
            currentTab: 'home',
            
            init() {
                this.bindTabs();
                this.bindInputs();
                this.initializeAds();
                this.updateAllCalculators();
            },

            bindTabs() {
                document.querySelectorAll('.tab-btn').forEach(btn => {
                    btn.addEventListener('click', (e) => {
                        this.currentTab = e.target.dataset.tab;
                        this.showTab(this.currentTab);
                        this.updateAllCalculators();
                    });
                });
            },

            bindInputs() {
                document.querySelectorAll('input').forEach(input => {
                    input.addEventListener('input', () => {
                        this.updateAllCalculators();
                    });
                });
            },

            showTab(tab) {
                document.querySelectorAll('.calculator-card').forEach(c => c.style.display = 'none');
                document.querySelectorAll('.tab-btn').forEach(t => t.classList.remove('active'));
                document.getElementById(tab).style.display = 'block';
                document.querySelector(`[data-tab="${tab}"]`).classList.add('active');
            },

            calculateEMI(principal, rate, years) {
                const monthlyRate = rate / 1200;
                const months = years * 12;
                const emi = (principal * monthlyRate * Math.pow(1 + monthlyRate, months)) / 
                          (Math.pow(1 + monthlyRate, months) - 1);
                return {
                    emi: emi,
                    totalInterest: emi * months - principal,
                    schedule: this.generateSchedule(principal, monthlyRate, emi, months)
                };
            },

            generateSchedule(P, r, emi, months) {
                let balance = P;
                return Array.from({length: months}, (_, month) => {
                    const interest = balance * r;
                    const principal = emi - interest;
                    balance -= principal;
                    return {
                        month: month + 1,
                        principal: Math.max(principal, 0),
                        interest: interest,
                        balance: Math.max(balance, 0)
                    };
                });
            },

            updateCalculator(type) {
                const amount = parseFloat(document.getElementById(`${type}-amount`).value) || 0;
                const rate = parseFloat(document.getElementById(`${type}-rate`).value) || 0;
                const tenure = parseFloat(document.getElementById(`${type}-tenure`).value) || 0;

                const { emi, totalInterest, schedule } = this.calculateEMI(amount, rate, tenure);
                
                document.getElementById(`${type}-emi`).textContent = emi.toFixed(2);
                document.getElementById(`${type}-interest`).textContent = totalInterest.toFixed(2);
                document.getElementById(`${type}-total`).textContent = (amount + totalInterest).toFixed(2);
                
                const principalPercent = (amount / (amount + totalInterest) * 100).toFixed(1);
                document.querySelector(`#${type} .pie-chart`).style.setProperty('--principal-percent', `${principalPercent}%`);

                const tbody = document.getElementById(`${type}-schedule`);
                tbody.innerHTML = schedule.map(entry => `
                    <tr>
                        <td>${entry.month}</td>
                        <td style="color: var(--success);">₹${entry.principal.toFixed(2)}</td>
                        <td style="color: var(--danger);">₹${entry.interest.toFixed(2)}</td>
                        <td>₹${entry.balance.toFixed(2)}</td>
                    </tr>
                `).join('');
            },

            updateComparison() {
                const amount = parseFloat(document.getElementById('compare-amount').value) || 0;
                const rate = parseFloat(document.getElementById('compare-rate').value) || 0;
                const tenure = parseFloat(document.getElementById('compare-tenure').value) || 0;

                const flatInterest = amount * (rate/100) * tenure;
                const flatEMI = (amount + flatInterest) / (tenure * 12);
                const reducing = this.calculateEMI(amount, rate, tenure);

                document.getElementById('flat-emi').textContent = flatEMI.toFixed(2);
                document.getElementById('flat-interest').textContent = flatInterest.toFixed(2);
                document.getElementById('reducing-emi').textContent = reducing.emi.toFixed(2);
                document.getElementById('reducing-interest').textContent = reducing.totalInterest.toFixed(2);
                document.getElementById('interest-saving').textContent = (flatInterest - reducing.totalInterest).toFixed(2);
            },

            updateMoratorium() {
                const amount = parseFloat(document.getElementById('moratorium-amount').value) || 0;
                const rate = parseFloat(document.getElementById('moratorium-rate').value) || 0;
                const tenure = parseFloat(document.getElementById('original-tenure').value) || 0;
                const moratorium = parseFloat(document.getElementById('moratorium-period').value) || 0;

                const monthlyInterest = amount * (rate / 1200);
                const accruedInterest = monthlyInterest * moratorium;
                const newPrincipal = amount + accruedInterest;
                const remainingMonths = tenure * 12 - moratorium;
                const { emi, totalInterest } = this.calculateEMI(newPrincipal, rate, remainingMonths / 12);

                document.getElementById('revised-emi').textContent = emi.toFixed(2);
                document.getElementById('additional-interest').textContent = accruedInterest.toFixed(2);
                document.getElementById('new-tenure').textContent = remainingMonths;
                document.getElementById('total-moratorium-interest').textContent = (totalInterest + accruedInterest).toFixed(2);
            },

            updateAllCalculators() {
                ['home', 'car', 'bike'].forEach(type => {
                    if(document.getElementById(`${type}-amount`)) {
                        this.updateCalculator(type);
                    }
                });
                this.updateComparison();
                this.updateMoratorium();
            },

            initializeAds() {
                (adsbygoogle = window.adsbygoogle || []).push({});
            }
        };

        // Initialize application
        document.addEventListener('DOMContentLoaded', () => LoanManager.init());
    </script>
</body>
</html>
