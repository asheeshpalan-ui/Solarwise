 SolarWise index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SolarWise | Smart Solar Energy</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f8faf9;
            color: #1e293b;
            line-height: 1.6;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.2rem 8%;
            background: #ffffff;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: #16a34a;
            text-decoration: none;
        }

        .navbar nav a {
            margin-left: 1.5rem;
            text-decoration: none;
            color: #334155;
            font-weight: 500;
        }

        .hero {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 4rem 8%;
            gap: 2rem;
            flex-wrap: wrap;
        }

        .hero-content {
            flex: 1;
            min-width: 300px;
        }

        .tag {
            display: inline-block;
            background: #dcfce7;
            color: #15803d;
            padding: 0.35rem 0.8rem;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-bottom: 1rem;
        }

        .hero h1 {
            font-size: 3rem;
            line-height: 1.2;
            margin-bottom: 1rem;
        }

        .hero h1 span {
            color: #16a34a;
        }

        .hero p {
            color: #475569;
            margin-bottom: 1.8rem;
            max-width: 500px;
        }

        .main-btn, .calculate-btn, .reset-btn {
            display: inline-block;
            background: #16a34a;
            color: #ffffff;
            padding: 0.9rem 1.8rem;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            border: none;
            cursor: pointer;
            font-size: 1rem;
            transition: background 0.2s;
        }

        .main-btn:hover, .calculate-btn:hover, .reset-btn:hover {
            background: #15803d;
        }

        .hero-image img {
            width: 100%;
            max-width: 480px;
            border-radius: 16px;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }

        .benefits, .calculator-section, .results-section {
            padding: 4rem 8%;
            text-align: center;
        }

        .benefit-grid, .results-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .benefit-card, .result-card {
            background: #ffffff;
            padding: 2rem 1.5rem;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
        }

        .benefit-icon, .result-icon {
            font-size: 2rem;
            margin-bottom: 0.75rem;
        }

        .calculator-box {
            max-width: 520px;
            margin: 2rem auto 0;
            background: #ffffff;
            padding: 2.5rem;
            border-radius: 16px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.06);
            text-align: left;
        }

        .form-group {
            margin-bottom: 1.25rem;
        }

        .form-group label {
            display: block;
            font-weight: 600;
            margin-bottom: 0.4rem;
        }

        .form-group input {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #cbd5e1;
            border-radius: 8px;
            font-size: 1rem;
        }

        .calculate-btn {
            width: 100%;
            margin-top: 0.5rem;
        }

        .note {
            font-size: 0.82rem;
            color: #64748b;
            margin-top: 1rem;
            text-align: center;
        }

        .result-card h3 {
            color: #16a34a;
            font-size: 1.5rem;
            margin-top: 0.3rem;
        }

        .result-message {
            margin: 2rem auto 1.5rem;
            padding: 1rem 1.5rem;
            background: #dcfce7;
            color: #166534;
            border-radius: 8px;
            max-width: 700px;
            font-weight: 500;
        }

        footer {
            background: #0f172a;
            color: #f8fafc;
            text-align: center;
            padding: 2.5rem 8%;
            margin-top: 2rem;
        }

        footer .copyright {
            font-size: 0.85rem;
            color: #94a3b8;
            margin-top: 0.5rem;
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <header class="navbar">
        <a href="#" class="logo">☀ SolarWise</a>
        <nav>
            <a href="#home">Home</a>
            <a href="#calculator">Calculator</a>
            <a href="#about">About</a>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <span class="tag">☘ CLEAN ENERGY, GREEN FUTURE</span>
            <h1>Make Every<br><span>Sunlight Count!</span></h1>
            <p>
                Discover your solar energy potential.
                Calculate electricity savings and contribute
                towards a cleaner, greener planet.
            </p>
            <a href="#calculator" class="main-btn">
                Calculate Solar Potential →
            </a>
        </div>

        <div class="hero-image">
            <img
                src="https://images.unsplash.com/photo-1509391366360-2e959784a276?w=900"
                alt="Solar panels under sunlight">
        </div>
    </section>

    <!-- Benefits -->
    <section class="benefits" id="about">
        <h2>Why Choose Solar Energy?</h2>
        <div class="benefit-grid">
            <div class="benefit-card">
                <div class="benefit-icon">☀️</div>
                <h3>Clean Energy</h3>
                <p>Generate electricity using renewable sunlight.</p>
            </div>

            <div class="benefit-card">
                <div class="benefit-icon">💰</div>
                <h3>Save Money</h3>
                <p>Estimate how solar power can reduce your electricity bill.</p>
            </div>

            <div class="benefit-card">
                <div class="benefit-icon">🌍</div>
                <h3>Protect Earth</h3>
                <p>Help reduce emissions from grid electricity.</p>
            </div>
        </div>
    </section>

    <!-- Solar Calculator -->
    <section class="calculator-section" id="calculator">
        <div class="section-heading">
            <span class="tag">SOLAR POWER CALCULATOR</span>
            <h2>Calculate Your Solar Potential</h2>
            <p>Enter your details to discover your estimated solar savings.</p>
        </div>

        <div class="calculator-box">
            <form id="solarForm">
                <div class="form-group">
                    <label for="units">Monthly Electricity Consumption (Units)</label>
                    <input
                        type="number"
                        id="units"
                        placeholder="Example: 450"
                        min="1"
                        step="any"
                        required>
                </div>

                <div class="form-group">
                    <label for="roof">Available Rooftop Area (sq. ft.)</label>
                    <input
                        type="number"
                        id="roof"
                        placeholder="Example: 500"
                        min="1"
                        step="any"
                        required>
                </div>

                <div class="form-group">
                    <label for="tariff">Electricity Price (₹ per unit)</label>
                    <input
                        type="number"
                        id="tariff"
                        placeholder="Example: 7"
                        min="0.01"
                        step="any"
                        required>
                </div>

                <button type="submit" class="calculate-btn">
                    Calculate My Solar Savings ☀️
                </button>
            </form>

            <p class="note">
                Estimates use 100 sq. ft. per kW and 4 units per kW per day.
                Actual results depend on location, weather, shading and system design.
            </p>
        </div>
    </section>

    <!-- Results -->
    <section class="results-section" id="results" hidden>
        <div class="section-heading">
            <span class="tag">YOUR SOLAR REPORT</span>
            <h2>Your Solar Energy Results</h2>
            <p>Here is your estimated renewable energy potential.</p>
        </div>

        <div class="results-grid">
            <div class="result-card">
                <div class="result-icon">⚡</div>
                <p>Recommended Solar Capacity</p>
                <h3 id="capacity">0 kW</h3>
            </div>

            <div class="result-card">
                <div class="result-icon">☀️</div>
                <p>Daily Energy Generation</p>
                <h3 id="daily">0 Units</h3>
            </div>

            <div class="result-card">
                <div class="result-icon">🔋</div>
                <p>Monthly Energy Generation</p>
                <h3 id="monthly">0 Units</h3>
            </div>

            <div class="result-card">
                <div class="result-icon">💰</div>
                <p>Estimated Monthly Savings</p>
                <h3 id="savings">₹0</h3>
            </div>

            <div class="result-card">
                <div class="result-icon">🌱</div>
                <p>Estimated CO₂ Avoided Monthly</p>
                <h3 id="carbon">0 kg</h3>
            </div>

            <div class="result-card">
                <div class="result-icon">🏠</div>
                <p>Rooftop Area Used</p>
                <h3 id="area">0 sq. ft.</h3>
            </div>
        </div>

        <div class="result-message" id="message"></div>

        <button type="button" class="reset-btn" onclick="resetCalculator()">
            Calculate Again ↻
        </button>
    </section>

    <!-- Footer -->
    <footer>
        <h2>☀ SolarWise</h2>
        <p>Make Every Sunlight Count!</p>
        <p class="copyright">
            © 2026 SolarWise | Building a Sustainable Future 🌱
        </p>
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", function () {
            const solarForm = document.getElementById("solarForm");
            const resultsSection = document.getElementById("results");

            solarForm.addEventListener("submit", function (event) {
                event.preventDefault();

                const units = parseFloat(document.getElementById("units").value);
                const roof = parseFloat(document.getElementById("roof").value);
                const tariff = parseFloat(document.getElementById("tariff").value);

                // 1 kW = 100 sq. ft. and generates 4 units/day (120 units/month)
                const requiredCapacity = units / 120;
                const maxRoofCapacity = roof / 100;
                const capacity = Math.min(requiredCapacity, maxRoofCapacity);

                const daily = capacity * 4;
                const monthly = daily * 30;
                const savings = monthly * tariff;
                const carbon = monthly * 0.82;
                const area = capacity * 100;

                document.getElementById("capacity").textContent = `${capacity.toFixed(2)} kW`;
                document.getElementById("daily").textContent = `${daily.toFixed(1)} Units`;
                document.getElementById("monthly").textContent = `${Math.round(monthly)} Units`;
                document.getElementById("savings").textContent = `₹${Math.round(savings).toLocaleString("en-IN")}`;
                document.getElementById("carbon").textContent = `${Math.round(carbon)} kg`;
                document.getElementById("area").textContent = `${Math.round(area)} sq. ft.`;

                const messageEl = document.getElementById("message");
                if (maxRoofCapacity < requiredCapacity) {

                    messageEl.textContent = `Your rooftop supports up to ${capacity.toFixed(2)} kW, covering ${Math.round((monthly / units) * 100)}% of your monthly electricity usage.`;
                } else {
                    messageEl.textContent = `Your rooftop can fit a ${capacity.toFixed(2)} kW system, covering 100% of your monthly electricity consumption!`;
                }

                resultsSection.hidden = false;
                resultsSection.scrollIntoView({ behavior: "smooth" });
            });
        });

        function resetCalculator() {
            document.getElementById("solarForm").reset();
            document.getElementById("results").hidden = true;
            document.getElementById("calculator").scrollIntoView({ behavior: "smooth" });
        }
    </script>
</body>
</html>'
'
