```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>KG Tracker</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #07111f;
            color: white;
            min-height: 100vh;
        }

        /* NAVBAR */
        nav {
            height: 75px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0 7%;
            border-bottom: 1px solid rgba(255,255,255,0.08);
            background: rgba(7,17,31,0.95);
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #38bdf8;
        }

        .logo span {
            color: white;
        }

        .nav-buttons {
            display: flex;
            gap: 12px;
        }

        .btn {
            text-decoration: none;
            padding: 11px 20px;
            border-radius: 8px;
            font-size: 14px;
            font-weight: bold;
            transition: 0.3s;
        }

        .login {
            color: white;
            border: 1px solid #334155;
        }

        .login:hover {
            background: #1e293b;
        }

        .start {
            background: #38bdf8;
            color: #07111f;
        }

        .start:hover {
            background: #0ea5e9;
            transform: translateY(-2px);
        }

        /* HERO */
        .hero {
            min-height: calc(100vh - 75px);
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 60px 20px;
        }

        .hero-content {
            max-width: 850px;
        }

        .badge {
            display: inline-block;
            padding: 8px 15px;
            border: 1px solid rgba(56,189,248,0.3);
            border-radius: 30px;
            color: #38bdf8;
            background: rgba(56,189,248,0.08);
            font-size: 13px;
            margin-bottom: 25px;
        }

        h1 {
            font-size: clamp(42px, 7vw, 78px);
            line-height: 1.05;
            margin-bottom: 25px;
        }

        h1 span {
            color: #38bdf8;
        }

        .description {
            max-width: 680px;
            margin: auto;
            color: #94a3b8;
            font-size: 18px;
            line-height: 1.7;
        }

        .hero-buttons {
            margin-top: 35px;
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .main-btn {
            display: inline-block;
            padding: 15px 28px;
            border-radius: 9px;
            text-decoration: none;
            font-weight: bold;
            background: #38bdf8;
            color: #07111f;
            transition: 0.3s;
        }

        .main-btn:hover {
            background: #0ea5e9;
            transform: translateY(-2px);
        }

        .secondary-btn {
            display: inline-block;
            padding: 15px 28px;
            border-radius: 9px;
            text-decoration: none;
            font-weight: bold;
            color: white;
            border: 1px solid #334155;
            transition: 0.3s;
        }

        .secondary-btn:hover {
            background: #1e293b;
        }

        /* FEATURES */
        .features {
            margin-top: 65px;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 18px;
        }

        .feature {
            background: rgba(255,255,255,0.04);
            border: 1px solid rgba(255,255,255,0.07);
            padding: 25px;
            border-radius: 14px;
        }

        .feature-icon {
            font-size: 28px;
            margin-bottom: 12px;
        }

        .feature h3 {
            margin-bottom: 8px;
            font-size: 17px;
        }

        .feature p {
            color: #94a3b8;
            font-size: 14px;
            line-height: 1.5;
        }

        /* FOOTER */
        footer {
            text-align: center;
            padding: 25px;
            color: #64748b;
            font-size: 13px;
            border-top: 1px solid rgba(255,255,255,0.06);
        }

        /* MOBILE */
        @media (max-width: 700px) {

            nav {
                padding: 0 20px;
            }

            .logo {
                font-size: 20px;
            }

            .login {
                display: none;
            }

            .hero {
                padding-top: 45px;
            }

            .description {
                font-size: 16px;
            }

            .features {
                grid-template-columns: 1fr;
            }

            h1 {
                font-size: 45px;
            }
        }
    </style>
</head>

<body>

    <!-- NAVIGATION -->
    <nav>

        <div class="logo">
            KG<span>Tracker</span>
        </div>

        <div class="nav-buttons">
            <a href="login.php" class="btn login">Login</a>
            <a href="login.php" class="btn start">Get Started</a>
        </div>

    </nav>


    <!-- HERO SECTION -->
    <main class="hero">

        <div class="hero-content">

            <div class="badge">
                Smart Business Management Platform
            </div>

            <h1>
                Manage Your Business
                <span>Smarter.</span>
            </h1>

            <p class="description">
                KG Tracker helps you manage employees, records,
                business information and performance from one
                simple and powerful dashboard.
            </p>


            <!-- BUTTONS -->
            <div class="hero-buttons">

                <a href="login.php" class="main-btn">
                    Login to Dashboard →
                </a>

                <a href="#features" class="secondary-btn">
                    Learn More
                </a>

            </div>


            <!-- FEATURES -->
            <div class="features" id="features">

                <div class="feature">

                    <div class="feature-icon">👥</div>

                    <h3>
                        Employee Management
                    </h3>

                    <p>
                        Manage employee information and
                        quickly find the people you need.
                    </p>

                </div>


                <div class="feature">

                    <div class="feature-icon">📊</div>

                    <h3>
                        Business Tracking
                    </h3>

                    <p>
                        Track important business records
                        and monitor your activities easily.
                    </p>

                </div>


                <div class="feature">

                    <div class="feature-icon">🤖</div>

                    <h3>
                        AI Assistant
                    </h3>

                    <p>
                        Ask questions about your business
                        data and get intelligent answers.
                    </p>

                </div>

            </div>

        </div>

    </main>


    <!-- FOOTER -->
    <footer>
        © 2026 KG Tracker. All rights reserved.
    </footer>

</body>
</html>
```
