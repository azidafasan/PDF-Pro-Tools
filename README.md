# PDF-Pro-Tools
All PDF tools a unique place
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PDF Pro Tools - Free Online PDF Converter & Editor | Convert, Compress, Edit PDFs</title>
    <meta name="description" content="Free PDF tools for 3 months! Convert, compress, edit PDFs online. Image to PDF, Word to PDF, PDF to Word, merge, split & more. No installation required.">
    <meta name="keywords" content="pdf converter, pdf editor, word to pdf, pdf to word, image to pdf, compress pdf, merge pdf, split pdf, online pdf tools, free pdf tools">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-purple: #8a2be2;
            --dark-purple: #6a0dad;
            --light-purple: #b19cd9;
            --neon-purple: #bf00ff;
            --neon-blue: #00bfff;
            --light-blue: #87ceeb;
            --glass-bg: rgba(255, 255, 255, 0.1);
            --glass-border: rgba(255, 255, 255, 0.2);
            --text-light: #f0f0f0;
            --text-dark: #333;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #1a1a2e, #16213e, #0f3460);
            color: var(--text-light);
            min-height: 100vh;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Header Styles */
        header {
            padding: 20px 0;
            position: relative;
            z-index: 100;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .logo i {
            font-size: 2.5rem;
            color: var(--neon-blue);
            text-shadow: 0 0 10px var(--neon-blue);
        }

        .logo h1 {
            font-size: 1.8rem;
            font-weight: 700;
            background: linear-gradient(90deg, var(--neon-purple), var(--neon-blue));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .nav-links {
            display: flex;
            gap: 30px;
            align-items: center;
        }

        .nav-links a {
            color: var(--text-light);
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            position: relative;
        }

        .nav-links a:hover {
            color: var(--neon-blue);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--neon-blue);
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .auth-buttons {
            display: flex;
            gap: 15px;
        }

        .auth-btn {
            padding: 8px 20px;
            border-radius: 50px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .login-btn {
            background: transparent;
            border: 1px solid var(--neon-blue);
            color: var(--neon-blue);
        }

        .login-btn:hover {
            background: var(--neon-blue);
            color: var(--text-dark);
        }

        .signup-btn {
            background: linear-gradient(90deg, var(--primary-purple), var(--neon-blue));
            border: none;
            color: white;
            box-shadow: 0 5px 15px rgba(138, 43, 226, 0.4);
        }

        .signup-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(138, 43, 226, 0.6);
        }

        /* Free Trial Banner */
        .free-trial-banner {
            background: linear-gradient(90deg, #ff9a00, #ff5e00);
            color: white;
            text-align: center;
            padding: 10px;
            font-weight: 600;
            border-radius: 10px;
            margin: 20px 0;
            box-shadow: 0 5px 15px rgba(255, 154, 0, 0.4);
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 60px 0;
            margin-bottom: 40px;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 20px;
            background: linear-gradient(90deg, var(--neon-purple), var(--neon-blue));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-shadow: 0 0 15px rgba(191, 0, 255, 0.3);
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
            color: var(--light-blue);
        }

        .cta-button {
            display: inline-block;
            padding: 12px 30px;
            background: linear-gradient(90deg, var(--primary-purple), var(--neon-blue));
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(138, 43, 226, 0.4);
            cursor: pointer;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(138, 43, 226, 0.6);
        }

        /* Ad Section */
        .ad-section {
            margin: 40px 0;
            text-align: center;
        }

        .ad-container {
            background: var(--glass-bg);
            border: 1px solid var(--glass-border);
            border-radius: 15px;
            padding: 20px;
            backdrop-filter: blur(10px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            min-height: 100px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--light-blue);
        }

        .ad-label {
            font-size: 0.8rem;
            color: var(--light-blue);
            text-align: center;
            margin-bottom: 5px;
        }

        /* Tools Grid */
        .tools-section {
            margin: 60px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            font-size: 2rem;
            color: var(--neon-blue);
            text-shadow: 0 0 10px rgba(0, 191, 255, 0.3);
        }

        .tools-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
        }

        .tool-card {
            background: var(--glass-bg);
            border: 1px solid var(--glass-border);
            border-radius: 15px;
            padding: 25px;
            text-align: center;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            position: relative;
        }

        .tool-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(138, 43, 226, 0.2);
            border-color: var(--neon-purple);
        }

        .tool-icon {
            font-size: 2.5rem;
            margin-bottom: 15px;
            color: var(--neon-blue);
            text-shadow: 0 0 10px var(--neon-blue);
        }

        .tool-card h3 {
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: var(--text-light);
        }

        .tool-card p {
            color: var(--light-blue);
            margin-bottom: 20px;
            font-size: 0.9rem;
        }

        .tool-button {
            display: inline-block;
            padding: 8px 20px;
            background: rgba(0, 191, 255, 0.2);
            color: var(--neon-blue);
            border: 1px solid var(--neon-blue);
            border-radius: 50px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .tool-button:hover {
            background: var(--neon-blue);
            color: var(--text-dark);
        }

        .free-badge {
            position: absolute;
            top: 10px;
            right: 10px;
            background: linear-gradient(90deg, #00c853, #64dd17);
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.7rem;
            font-weight: 600;
        }

        .watermark-notice {
            font-size: 0.8rem;
            color: #ff9a00;
            margin-top: 10px;
        }

        /* Pricing Section */
        .pricing-section {
            margin: 80px 0;
        }

        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .pricing-card {
            background: var(--glass-bg);
            border: 1px solid var(--glass-border);
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            position: relative;
        }

        .pricing-card.featured {
            border-color: var(--neon-blue);
            transform: scale(1.05);
        }

        .pricing-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(138, 43, 226, 0.2);
        }

        .pricing-card.featured:hover {
            transform: scale(1.05) translateY(-10px);
        }

        .pricing-badge {
            position: absolute;
            top: -10px;
            left: 50%;
            transform: translateX(-50%);
            background: linear-gradient(90deg, var(--primary-purple), var(--neon-blue));
            color: white;
            padding: 5px 20px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        .pricing-title {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: var(--neon-blue);
        }

        .pricing-price {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: var(--text-light);
        }

        .pricing-period {
            font-size: 1rem;
            color: var(--light-blue);
        }

        .pricing-features {
            list-style-type: none;
            margin-bottom: 30px;
            text-align: left;
        }

        .pricing-features li {
            padding: 8px 0;
            color: var(--light-blue);
        }

        .pricing-features li i {
            color: var(--neon-blue);
            margin-right: 10px;
        }

        .pricing-button {
            display: block;
            width: 100%;
            padding: 12px;
            border-radius: 50px;
            font-weight: 600;
            text-align: center;
            text-decoration: none;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .basic-button {
            background: transparent;
            border: 1px solid var(--neon-blue);
            color: var(--neon-blue);
        }

        .basic-button:hover {
            background: var(--neon-blue);
            color: var(--text-dark);
        }

        .premium-button {
            background: linear-gradient(90deg, var(--primary-purple), var(--neon-blue));
            border: none;
            color: white;
            box-shadow: 0 5px 15px rgba(138, 43, 226, 0.4);
        }

        .premium-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(138, 43, 226, 0.6);
        }

        .business-button {
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid var(--light-blue);
            color: var(--light-blue);
        }

        .business-button:hover {
            background: rgba(255, 255, 255, 0.2);
        }

        /* Payment Options */
        .payment-options {
            margin-top: 20px;
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .payment-option {
            background: rgba(255, 255, 255, 0.1);
            padding: 8px 15px;
            border-radius: 10px;
            font-size: 0.8rem;
            display: flex;
            align-items: center;
            gap: 5px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .payment-option:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: scale(1.05);
        }

        /* Chatbot */
        .chatbot-container {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1000;
        }

        .chatbot-button {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(90deg, var(--primary-purple), var(--neon-blue));
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(138, 43, 226, 0.4);
            transition: all 0.3s ease;
        }

        .chatbot-button:hover {
            transform: scale(1.1);
        }

        .chatbot-button i {
            font-size: 1.5rem;
            color: white;
        }

        .chatbot-window {
            position: absolute;
            bottom: 70px;
            right: 0;
            width: 350px;
            height: 450px;
            background: var(--glass-bg);
            border: 1px solid var(--glass-border);
            border-radius: 15px;
            backdrop-filter: blur(10px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            display: none;
            flex-direction: column;
            overflow: hidden;
        }

        .chatbot-header {
            padding: 15px;
            background: rgba(0, 0, 0, 0.2);
            border-bottom: 1px solid var(--glass-border);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .chatbot-title {
            font-weight: 600;
            color: var(--neon-blue);
        }

        .chatbot-close {
            cursor: pointer;
            color: var(--light-blue);
        }

        .chatbot-messages {
            flex: 1;
            padding: 15px;
            overflow-y: auto;
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        .message {
            padding: 10px 15px;
            border-radius: 15px;
            max-width: 80%;
            font-size: 0.9rem;
        }

        .bot-message {
            background: rgba(0, 191, 255, 0.2);
            align-self: flex-start;
            border-bottom-left-radius: 5px;
        }

        .user-message {
            background: rgba(138, 43, 226, 0.2);
            align-self: flex-end;
            border-bottom-right-radius: 5px;
        }

        .chatbot-input {
            padding: 15px;
            border-top: 1px solid var(--glass-border);
            display: flex;
            gap: 10px;
        }

        .chatbot-input input {
            flex: 1;
            padding: 10px 15px;
            border-radius: 50px;
            border: 1px solid var(--glass-border);
            background: rgba(255, 255, 255, 0.1);
            color: var(--text-light);
            outline: none;
        }

        .chatbot-input button {
            padding: 10px 15px;
            border-radius: 50px;
            border: none;
            background: var(--neon-blue);
            color: white;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .chatbot-input button:hover {
            background: var(--primary-purple);
        }

        /* Auth Modals */
        .modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.7);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 2000;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }

        .modal.active {
            opacity: 1;
            visibility: visible;
        }

        .modal-content {
            background: linear-gradient(135deg, #1a1a2e, #16213e);
            width: 400px;
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            border: 1px solid var(--glass-border);
            backdrop-filter: blur(10px);
            transform: translateY(-20px);
            transition: all 0.3s ease;
        }

        .modal.active .modal-content {
            transform: translateY(0);
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .modal-title {
            font-size: 1.5rem;
            color: var(--neon-blue);
        }

        .modal-close {
            cursor: pointer;
            color: var(--light-blue);
            font-size: 1.2rem;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: var(--light-blue);
        }

        .form-group input {
            width: 100%;
            padding: 12px 15px;
            border-radius: 10px;
            border: 1px solid var(--glass-border);
            background: rgba(255, 255, 255, 0.1);
            color: var(--text-light);
            outline: none;
            transition: all 0.3s ease;
        }

        .form-group input:focus {
            border-color: var(--neon-blue);
        }

        .form-button {
            width: 100%;
            padding: 12px;
            border-radius: 50px;
            border: none;
            background: linear-gradient(90deg, var(--primary-purple), var(--neon-blue));
            color: white;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 10px;
        }

        .form-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(138, 43, 226, 0.4);
        }

        .form-footer {
            text-align: center;
            margin-top: 20px;
            color: var(--light-blue);
        }

        .form-footer a {
            color: var(--neon-blue);
            text-decoration: none;
        }

        /* Payment Modal */
        .payment-modal {
            width: 500px;
        }

        .payment-methods {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin: 20px 0;
        }

        .payment-method {
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid var(--glass-border);
            border-radius: 10px;
            padding: 15px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .payment-method:hover, .payment-method.active {
            border-color: var(--neon-blue);
            background: rgba(0, 191, 255, 0.1);
        }

        .payment-method i {
            font-size: 2rem;
            margin-bottom: 10px;
            color: var(--neon-blue);
        }

        .payment-details {
            margin-top: 20px;
            display: none;
        }

        .payment-details.active {
            display: block;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 40px 0;
            margin-top: 60px;
            border-top: 1px solid var(--glass-border);
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-bottom: 20px;
        }

        .footer-links a {
            color: var(--light-blue);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-links a:hover {
            color: var(--neon-blue);
        }

        .copyright {
            color: var(--light-blue);
            font-size: 0.9rem;
        }

        /* Watermark Preview */
        .watermark-preview {
            margin-top: 20px;
            padding: 20px;
            background: rgba(0, 0, 0, 0.2);
            border-radius: 10px;
            text-align: center;
        }

        .watermark-preview p {
            margin-bottom: 10px;
            color: var(--light-blue);
        }

        .watermark-example {
            position: relative;
            width: 100%;
            height: 200px;
            background: white;
            border-radius: 5px;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #333;
            font-weight: bold;
            overflow: hidden;
        }

        .watermark-text {
            position: absolute;
            font-size: 3rem;
            color: rgba(0, 0, 0, 0.1);
            transform: rotate(-45deg);
            pointer-events: none;
        }

        /* SEO Content Section */
        .seo-content {
            margin: 60px 0;
            background: var(--glass-bg);
            border-radius: 15px;
            padding: 40px;
            backdrop-filter: blur(10px);
        }

        .seo-content h2 {
            color: var(--neon-blue);
            margin-bottom: 20px;
            font-size: 1.8rem;
        }

        .seo-content h3 {
            color: var(--light-blue);
            margin: 25px 0 15px;
            font-size: 1.4rem;
        }

        .seo-content p {
            margin-bottom: 15px;
            color: var(--text-light);
            line-height: 1.7;
        }

        .seo-content ul {
            margin-left: 20px;
            margin-bottom: 20px;
        }

        .seo-content li {
            margin-bottom: 10px;
            color: var(--light-blue);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                gap: 20px;
            }

            .nav-links {
                gap: 15px;
            }

            .hero h2 {
                font-size: 2.2rem;
            }

            .tools-grid {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            }

            .pricing-grid {
                grid-template-columns: 1fr;
            }

            .pricing-card.featured {
                transform: scale(1);
            }

            .pricing-card.featured:hover {
                transform: translateY(-10px);
            }

            .chatbot-window {
                width: 300px;
            }

            .payment-modal {
                width: 90%;
            }

            .payment-methods {
                grid-template-columns: repeat(2, 1fr);
            }

            .seo-content {
                padding: 20px;
            }
        }

        @media (max-width: 480px) {
            .hero h2 {
                font-size: 1.8rem;
            }

            .tools-grid {
                grid-template-columns: 1fr;
            }

            .modal-content {
                width: 90%;
            }

            .chatbot-window {
                width: 280px;
                right: -20px;
            }

            .payment-methods {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-file-pdf"></i>
                    <h1>PDF Pro Tools</h1>
                </div>
                <nav class="nav-links">
                    <a href="#tools">Tools</a>
                    <a href="#pricing">Pricing</a>
                    <a href="#how-it-works">How It Works</a>
                    <a href="#contact">Contact</a>
                    <div class="auth-buttons">
                        <button class="auth-btn login-btn" id="login-btn">Login</button>
                        <button class="auth-btn signup-btn" id="signup-btn">Sign Up</button>
                    </div>
                </nav>
            </div>
        </header>

        <div class="free-trial-banner">
            <i class="fas fa-gift"></i> ALL TOOLS FREE FOR 3 MONTHS! No watermarks, no limits. Enjoy premium features for free during our launch period.
        </div>

        <section class="hero">
            <h2>Professional PDF Tools for All Your Needs</h2>
            <p>Convert, compress, edit, and manage your documents with our powerful online tools. Fast, secure, and easy to use.</p>
            <a href="#tools" class="cta-button">Explore Free Tools</a>
        </section>

        <div class="ad-section">
            <div class="ad-label">Advertisement</div>
            <div class="ad-container">
                <!-- Ad Space 1 - Can be replaced with Google AdSense or other ad code -->
                <div id="ca-app-pub-3020392667373286/7884340398">
                    <p>Ad Space - Perfect for monetization</p>
                </div>
            </div>
        </div>

        <section class="tools-section" id="tools">
            <h2 class="section-title">All-in-One PDF Tools - FREE FOR 3 MONTHS</h2>
            <div class="tools-grid">
                <!-- Conversion Tools -->
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-image tool-icon"></i>
                    <h3>Image to PDF</h3>
                    <p>Convert JPG, PNG, and other images to PDF format</p>
                    <button class="tool-button" data-tool="image-to-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-word tool-icon"></i>
                    <h3>Word to PDF</h3>
                    <p>Convert DOC and DOCX files to PDF format</p>
                    <button class="tool-button" data-tool="word-to-pdf">Use Tool</button>
                    <div class="watermark-notice">Always free - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-pdf tool-icon"></i>
                    <h3>PDF to Image</h3>
                    <p>Extract images from PDF files or convert pages to images</p>
                    <button class="tool-button" data-tool="pdf-to-image">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-alt tool-icon"></i>
                    <h3>PDF to Word</h3>
                    <p>Convert PDF files to editable Word documents</p>
                    <button class="tool-button" data-tool="pdf-to-word">Use Tool</button>
                    <div class="watermark-notice">Always free - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-excel tool-icon"></i>
                    <h3>Excel to PDF</h3>
                    <p>Convert XLS and XLSX files to PDF format</p>
                    <button class="tool-button" data-tool="excel-to-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-pdf tool-icon"></i>
                    <h3>PDF to Excel</h3>
                    <p>Extract tables from PDF to Excel spreadsheets</p>
                    <button class="tool-button" data-tool="pdf-to-excel">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-powerpoint tool-icon"></i>
                    <h3>PDF to PowerPoint</h3>
                    <p>Convert PDF files to editable PowerPoint presentations</p>
                    <button class="tool-button" data-tool="pdf-to-ppt">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-code tool-icon"></i>
                    <h3>HTML to PDF</h3>
                    <p>Convert web pages and HTML files to PDF</p>
                    <button class="tool-button" data-tool="html-to-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-compress-alt tool-icon"></i>
                    <h3>Image Compressor</h3>
                    <p>Reduce image file size without losing quality</p>
                    <button class="tool-button" data-tool="image-compressor">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-archive tool-icon"></i>
                    <h3>PDF Compressor</h3>
                    <p>Reduce PDF file size while maintaining quality</p>
                    <button class="tool-button" data-tool="pdf-compressor">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-word tool-icon"></i>
                    <h3>Word Compressor</h3>
                    <p>Reduce Word document file size</p>
                    <button class="tool-button" data-tool="word-compressor">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-cut tool-icon"></i>
                    <h3>Split PDF</h3>
                    <p>Split PDF files into multiple documents</p>
                    <button class="tool-button" data-tool="split-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-object-group tool-icon"></i>
                    <h3>Merge PDF</h3>
                    <p>Combine multiple PDF files into one document</p>
                    <button class="tool-button" data-tool="merge-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-signature tool-icon"></i>
                    <h3>Sign PDF</h3>
                    <p>Add digital signatures to PDF documents</p>
                    <button class="tool-button" data-tool="sign-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-tint tool-icon"></i>
                    <h3>Watermark PDF</h3>
                    <p>Add text or image watermarks to PDF files</p>
                    <button class="tool-button" data-tool="watermark-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-sync-alt tool-icon"></i>
                    <h3>Rotate PDF</h3>
                    <p>Rotate PDF pages to correct orientation</p>
                    <button class="tool-button" data-tool="rotate-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-unlock tool-icon"></i>
                    <h3>Unlock PDF</h3>
                    <p>Remove password protection from PDF files</p>
                    <button class="tool-button" data-tool="unlock-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-lock tool-icon"></i>
                    <h3>Protect PDF</h3>
                    <p>Add password protection to PDF documents</p>
                    <button class="tool-button" data-tool="protect-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-sort tool-icon"></i>
                    <h3>Organize PDF</h3>
                    <p>Reorder, delete, or rearrange PDF pages</p>
                    <button class="tool-button" data-tool="organize-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-file-contract tool-icon"></i>
                    <h3>PDF to PDF/A</h3>
                    <p>Convert PDF to archival PDF/A format</p>
                    <button class="tool-button" data-tool="pdf-to-pdfa">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-tools tool-icon"></i>
                    <h3>Repair PDF</h3>
                    <p>Fix corrupted or damaged PDF files</p>
                    <button class="tool-button" data-tool="repair-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-sort-numeric-down tool-icon"></i>
                    <h3>Page Numbers</h3>
                    <p>Add page numbers to PDF documents</p>
                    <button class="tool-button" data-tool="page-numbers">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-scanner tool-icon"></i>
                    <h3>Scan to PDF</h3>
                    <p>Convert scanned documents to searchable PDF</p>
                    <button class="tool-button" data-tool="scan-to-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-eye tool-icon"></i>
                    <h3>OCR PDF</h3>
                    <p>Extract text from scanned PDFs with OCR</p>
                    <button class="tool-button" data-tool="ocr-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-code-branch tool-icon"></i>
                    <h3>Compare PDF</h3>
                    <p>Compare two PDF files and highlight differences</p>
                    <button class="tool-button" data-tool="compare-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-highlighter tool-icon"></i>
                    <h3>Redact PDF</h3>
                    <p>Permanently remove sensitive information</p>
                    <button class="tool-button" data-tool="redact-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-crop tool-icon"></i>
                    <h3>Crop PDF</h3>
                    <p>Adjust margins and crop PDF pages</p>
                    <button class="tool-button" data-tool="crop-pdf">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
                <div class="tool-card">
                    <div class="free-badge">FREE</div>
                    <i class="fas fa-project-diagram tool-icon"></i>
                    <h3>Create Workflow</h3>
                    <p>Automate multiple PDF tasks in sequence</p>
                    <button class="tool-button" data-tool="create-workflow">Use Tool</button>
                    <div class="watermark-notice">Free for 3 months - No watermark</div>
                </div>
            </div>
        </section>

        <div class="ad-section">
            <div class="ad-label">Advertisement</div>
            <div class="ad-container">
                <!-- Ad Space 2 - Can be replaced with Google AdSense or other ad code -->
                <div id="ca-app-pub-3020392667373286/7884340398">
                    <p>Ad Space - Perfect for monetization</p>
                </div>
            </div>
        </div>

        <section class="pricing-section" id="pricing">
            <h2 class="section-title">Choose Your Plan</h2>
            <div class="pricing-grid">
                <div class="pricing-card">
                    <div class="pricing-badge">FREE TRIAL</div>
                    <h3 class="pricing-title">Basic</h3>
                    <div class="pricing-price">₹0<span class="pricing-period">/month</span></div>
                    <ul class="pricing-features">
                        <li><i class="fas fa-check"></i> Access to essential PDF tools</li>
                        <li><i class="fas fa-check"></i> Limited document processing</li>
                        <li><i class="fas fa-check"></i> Basic conversion tools</li>
                        <li><i class="fas fa-check"></i> Watermark after 3 months (except Word to PDF & PDF to Word)</li>
                        <li><i class="fas fa-check"></i> Standard customer support</li>
                    </ul>
                    <button class="pricing-button basic-button">Get Started Free</button>
                    
                    <div class="watermark-preview">
                        <p>After 3 Months - Watermark Example:</p>
                        <div class="watermark-example">
                            <div class="watermark-text">Documented by PDF PRO Tools</div>
                            <p>Your document content appears here</p>
                        </div>
                    </div>
                </div>
                <div class="pricing-card featured">
                    <div class="pricing-badge">MOST POPULAR</div>
                    <h3 class="pricing-title">Premium</h3>
                    <div class="pricing-price">₹249<span class="pricing-period">/month</span></div>
                    <div style="font-size: 0.9rem; color: var(--light-blue); margin-bottom: 15px;">₹400/month billed monthly | Save 20% with yearly plan</div>
                    <ul class="pricing-features">
                        <li><i class="fas fa-check"></i> Full access to all PDF tools</li>
                        <li><i class="fas fa-check"></i> Unlimited document processing</li>
                        <li><i class="fas fa-check"></i> Access across Web, Mobile, and Desktop</li>
                        <li><i class="fas fa-check"></i> Digital Signatures</li>
                        <li><i class="fas fa-check"></i> Advanced workflows</li>
                        <li><i class="fas fa-check"></i> Ad-free experience</li>
                        <li><i class="fas fa-check"></i> Priority customer support</li>
                        <li><i class="fas fa-check"></i> No watermarks - Ever!</li>
                    </ul>
                    <button class="pricing-button premium-button" id="premium-payment-btn">Upgrade to Premium</button>
                    <div class="payment-options">
                        <div class="payment-option" data-method="stripe"><i class="fab fa-cc-stripe"></i> Stripe</div>
                        <div class="payment-option" data-method="paypal"><i class="fab fa-cc-paypal"></i> PayPal</div>
                        <div class="payment-option" data-method="razorpay"><i class="fas fa-rupee-sign"></i> Razorpay</div>
                        <div class="payment-option" data-method="phonepe"><i class="fas fa-mobile-alt"></i> PhonePe</div>
                        <div class="payment-option" data-method="cards"><i class="fas fa-credit-card"></i> Cards</div>
                    </div>
                </div>
                <div class="pricing-card">
                    <div class="pricing-badge">COMING SOON</div>
                    <h3 class="pricing-title">Business</h3>
                    <div class="pricing-price">Custom</div>
                    <ul class="pricing-features">
                        <li><i class="fas fa-check"></i> All Premium features</li>
                        <li><i class="fas fa-check"></i> Team management</li>
                        <li><i class="fas fa-check"></i> Advanced security</li>
                        <li><i class="fas fa-check"></i> Custom workflows</li>
                        <li><i class="fas fa-check"></i> Dedicated account manager</li>
                        <li><i class="fas fa-check"></i> API access</li>
                        <li><i class="fas fa-check"></i> Bulk processing</li>
                        <li><i class="fas fa-check"></i> 24/7 premium support</li>
                    </ul>
                    <button class="pricing-button business-button">Contact Sales</button>
                </div>
            </div>
        </section>

        <div class="ad-section">
            <div class="ad-label">Advertisement</div>
            <div class="ad-container">
                <!-- Ad Space 3 - Can be replaced with Google AdSense or other ad code -->
                <div id="ca-app-pub-3020392667373286/1812814112">
                    <p>Ad Space - Perfect for monetization</p>
                </div>
            </div>
        </div>

        <!-- SEO Content Section -->
        <section class="seo-content">
            <h2>Free Online PDF Tools - Convert, Edit, and Manage Your Documents</h2>
            <p>PDF Pro Tools offers a comprehensive suite of online PDF utilities that help you work with documents efficiently. Our platform provides everything you need for PDF conversion, editing, compression, and management - all available for free during our 3-month launch period.</p>
            
            <h3>Why Choose PDF Pro Tools?</h3>
            <p>Our PDF tools are designed with user experience in mind. Whether you're converting Word to PDF, compressing large files, or editing document properties, our intuitive interface makes the process simple and straightforward.</p>
            
            <h3>Key Features of Our PDF Tools:</h3>
            <ul>
                <li><strong>PDF Conversion:</strong> Convert between PDF and various formats including Word, Excel, PowerPoint, images, and HTML</li>
                <li><strong>PDF Editing:</strong> Merge, split, rotate, watermark, and organize PDF pages with ease</li>
                <li><strong>PDF Compression:</strong> Reduce file size without compromising quality</li>
                <li><strong>Security Features:</strong> Protect PDFs with passwords or remove security restrictions</li>
                <li><strong>OCR Technology:</strong> Extract text from scanned documents and images</li>
            </ul>
            
            <h3>How to Use Our PDF Tools</h3>
            <p>Using our PDF tools is simple. Just select the tool you need, upload your file, and let our system process it. Within seconds, you'll have your converted, edited, or compressed document ready for download.</p>
            
            <h3>Free PDF Tools for Everyone</h3>
            <p>During our launch period, all PDF tools are completely free to use with no watermarks or limitations. After 3 months, basic functionality will remain free with watermarks on certain outputs, while premium features will be available through our affordable subscription plans.</p>
        </section>

        <!-- Chatbot -->
        <div class="chatbot-container">
            <div class="chatbot-button" id="chatbot-toggle">
                <i class="fas fa-comment-dots"></i>
            </div>
            <div class="chatbot-window" id="chatbot-window">
                <div class="chatbot-header">
                    <div class="chatbot-title">PDF Pro Assistant</div>
                    <div class="chatbot-close" id="chatbot-close"><i class="fas fa-times"></i></div>
                </div>
                <div class="chatbot-messages" id="chatbot-messages">
                    <div class="message bot-message">
                        Hello! I'm your PDF assistant. How can I help you today?
                    </div>
                    <div class="message bot-message">
                        Could you please provide your name?
                    </div>
                </div>
                <div class="chatbot-input">
                    <input type="text" id="chatbot-input" placeholder="Type your message...">
                    <button id="chatbot-send"><i class="fas fa-paper-plane"></i></button>
                </div>
            </div>
        </div>

        <!-- Login Modal -->
        <div class="modal" id="login-modal">
            <div class="modal-content">
                <div class="modal-header">
                    <h3 class="modal-title">Login to Your Account</h3>
                    <div class="modal-close" id="login-close"><i class="fas fa-times"></i></div>
                </div>
                <div class="form-group">
                    <label for="login-email">Email</label>
                    <input type="email" id="login-email" placeholder="Enter your email">
                </div>
                <div class="form-group">
                    <label for="login-password">Password</label>
                    <input type="password" id="login-password" placeholder="Enter your password">
                </div>
                <button class="form-button">Login</button>
                <div class="form-footer">
                    Don't have an account? <a href="#" id="show-signup">Sign up</a>
                </div>
            </div>
        </div>

        <!-- Signup Modal -->
        <div class="modal" id="signup-modal">
            <div class="modal-content">
                <div class="modal-header">
                    <h3 class="modal-title">Create New Account</h3>
                    <div class="modal-close" id="signup-close"><i class="fas fa-times"></i></div>
                </div>
                <div class="form-group">
                    <label for="signup-name">Full Name</label>
                    <input type="text" id="signup-name" placeholder="Enter your full name">
                </div>
                <div class="form-group">
                    <label for="signup-email">Email</label>
                    <input type="email" id="signup-email" placeholder="Enter your email">
                </div>
                <div class="form-group">
                    <label for="signup-password">Password</label>
                    <input type="password" id="signup-password" placeholder="Create a password">
                </div>
                <div class="form-group">
                    <label for="signup-confirm">Confirm Password</label>
                    <input type="password" id="signup-confirm" placeholder="Confirm your password">
                </div>
                <button class="form-button">Sign Up</button>
                <div class="form-footer">
                    Already have an account? <a href="#" id="show-login">Login</a>
                </div>
            </div>
        </div>

        <!-- Payment Modal -->
        <div class="modal" id="payment-modal">
            <div class="modal-content payment-modal">
                <div class="modal-header">
                    <h3 class="modal-title">Upgrade to Premium</h3>
                    <div class="modal-close" id="payment-close"><i class="fas fa-times"></i></div>
                </div>
                <div class="form-group">
                    <label>Select Payment Method</label>
                    <div class="payment-methods">
                        <div class="payment-method" data-method="stripe">
                            <i class="fab fa-cc-stripe"></i>
                            <div>Stripe</div>
                        </div>
                        <div class="payment-method" data-method="paypal">
                            <i class="fab fa-cc-paypal"></i>
                            <div>PayPal</div>
                        </div>
                        <div class="payment-method" data-method="razorpay">
                            <i class="fas fa-rupee-sign"></i>
                            <div>Razorpay</div>
                        </div>
                        <div class="payment-method" data-method="phonepe">
                            <i class="fas fa-mobile-alt"></i>
                            <div>PhonePe</div>
                        </div>
                        <div class="payment-method" data-method="cards">
                            <i class="fas fa-credit-card"></i>
                            <div>Credit/Debit Card</div>
                        </div>
                        <div class="payment-method" data-method="emi">
                            <i class="fas fa-calendar-alt"></i>
                            <div>EMI (Yearly)</div>
                        </div>
                    </div>
                </div>
                
                <div class="payment-details" id="stripe-details">
                    <div class="form-group">
                        <label>Card Number</label>
                        <input type="text" placeholder="1234 5678 9012 3456">
                    </div>
                    <div class="form-group">
                        <label>Expiry Date</label>
                        <input type="text" placeholder="MM/YY">
                    </div>
                    <div class="form-group">
                        <label>CVV</label>
                        <input type="text" placeholder="123">
                    </div>
                    <button class="form-button">Pay ₹249/month</button>
                </div>
                
                <div class="payment-details" id="paypal-details">
                    <p>You will be redirected to PayPal to complete your payment</p>
                    <button class="form-button">Continue to PayPal</button>
                </div>
                
                <div class="payment-details" id="razorpay-details">
                    <p>You will be redirected to Razorpay to complete your payment</p>
                    <button class="form-button">Pay ₹249/month</button>
                </div>
                
                <div class="payment-details" id="phonepe-details">
                    <p>Scan the QR code with PhonePe to complete payment</p>
                    <div style="text-align: center; margin: 20px 0;">
                        <div style="width: 150px; height: 150px; background: #eee; margin: 0 auto; display: flex; align-items: center; justify-content: center;">
                            QR Code
                        </div>
                    </div>
                </div>
                
                <div class="payment-details" id="cards-details">
                    <div class="form-group">
                        <label>Card Number</label>
                        <input type="text" placeholder="1234 5678 9012 3456">
                    </div>
                    <div class="form-group">
                        <label>Expiry Date</label>
                        <input type="text" placeholder="MM/YY">
                    </div>
                    <div class="form-group">
                        <label>CVV</label>
                        <input type="text" placeholder="123">
                    </div>
                    <button class="form-button">Pay ₹249/month</button>
                </div>
                
                <div class="payment-details" id="emi-details">
                    <p>EMI option is available for yearly plans. Please contact support for more information.</p>
                    <button class="form-button">Contact Support</button>
                </div>
            </div>
        </div>

        <footer>
            <div class="footer-links">
                <a href="#">Privacy Policy</a>
                <a href="#">Terms of Service</a>
                <a href="#">Support</a>
                <a href="#">API</a>
            </div>
            <p class="copyright">© 2023 PDF Pro Tools. All rights reserved.</p>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Authentication modals
            const loginBtn = document.getElementById('login-btn');
            const signupBtn = document.getElementById('signup-btn');
            const loginModal = document.getElementById('login-modal');
            const signupModal = document.getElementById('signup-modal');
            const loginClose = document.getElementById('login-close');
            const signupClose = document.getElementById('signup-close');
            const showSignup = document.getElementById('show-signup');
            const showLogin = document.getElementById('show-login');

            // Chatbot elements
            const chatbotToggle = document.getElementById('chatbot-toggle');
            const chatbotWindow = document.getElementById('chatbot-window');
            const chatbotClose = document.getElementById('chatbot-close');
            const chatbotMessages = document.getElementById('chatbot-messages');
            const chatbotInput = document.getElementById('chatbot-input');
            const chatbotSend = document.getElementById('chatbot-send');

            // Payment elements
            const premiumPaymentBtn = document.getElementById('premium-payment-btn');
            const paymentModal = document.getElementById('payment-modal');
            const paymentClose = document.getElementById('payment-close');
            const paymentMethods = document.querySelectorAll('.payment-method');
            const paymentDetails = document.querySelectorAll('.payment-details');

            // Tool buttons
            const toolButtons = document.querySelectorAll('.tool-button');

            // Auth modal functions
            function openLoginModal() {
                loginModal.classList.add('active');
            }

            function closeLoginModal() {
                loginModal.classList.remove('active');
            }

            function openSignupModal() {
                signupModal.classList.add('active');
            }

            function closeSignupModal() {
                signupModal.classList.remove('active');
            }

            // Payment modal functions
            function openPaymentModal() {
                paymentModal.classList.add('active');
            }

            function closePaymentModal() {
                paymentModal.classList.remove('active');
            }

            // Chatbot functions
            function toggleChatbot() {
                chatbotWindow.style.display = chatbotWindow.style.display === 'flex' ? 'none' : 'flex';
            }

            function addMessage(message, isUser = false) {
                const messageDiv = document.createElement('div');
                messageDiv.classList.add('message');
                messageDiv.classList.add(isUser ? 'user-message' : 'bot-message');
                messageDiv.textContent = message;
                chatbotMessages.appendChild(messageDiv);
                chatbotMessages.scrollTop = chatbotMessages.scrollHeight;
            }

            function processChatbotInput() {
                const message = chatbotInput.value.trim();
                if (message === '') return;

                addMessage(message, true);
                chatbotInput.value = '';

                // Simulate bot response
                setTimeout(() => {
                    if (message.toLowerCase().includes('name')) {
                        addMessage("Thank you! Now could you please provide your email address?");
                    } else if (message.includes('@')) {
                        // Simple email validation
                        if (/^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/.test(message)) {
                            addMessage("Great! Now please provide your contact number (10 digits):");
                        } else {
                            addMessage("That doesn't look like a valid email. Please enter a genuine email address:");
                        }
                    } else if (/^\d{10}$/.test(message)) {
                        addMessage("Perfect! All our tools are free for 3 months with no watermarks. Would you like to know more about our premium plans for after the trial?");
                    } else if (message.toLowerCase().includes('yes') || message.toLowerCase().includes('premium')) {
                        addMessage("Great! After the 3-month free trial, our Premium plan costs ₹400/month or ₹249/month if billed yearly. It includes full access to all tools, unlimited processing, and no watermarks. Would you like to upgrade?");
                    } else if (message.toLowerCase().includes('no') || message.toLowerCase().includes('later')) {
                        addMessage("No problem! You can continue using our free tools for 3 months. Feel free to ask if you have any questions.");
                    } else {
                        addMessage("I'm here to help with any questions about our PDF tools. How can I assist you?");
                    }
                }, 1000);
            }

            // Tool button functionality
            function handleToolClick() {
                const tool = this.getAttribute('data-tool');
                alert(`Opening ${tool} tool. In a real application, this would launch the specific tool interface. All tools are free for 3 months with no watermarks!`);
            }

            // Payment method selection
            function selectPaymentMethod(method) {
                // Remove active class from all methods
                paymentMethods.forEach(pm => pm.classList.remove('active'));
                
                // Add active class to selected method
                const selectedMethod = document.querySelector(`.payment-method[data-method="${method}"]`);
                selectedMethod.classList.add('active');
                
                // Hide all payment details
                paymentDetails.forEach(detail => detail.classList.remove('active'));
                
                // Show selected payment details
                const selectedDetail = document.getElementById(`${method}-details`);
                if (selectedDetail) {
                    selectedDetail.classList.add('active');
                }
            }

            // Event listeners for auth modals
            loginBtn.addEventListener('click', openLoginModal);
            signupBtn.addEventListener('click', openSignupModal);
            loginClose.addEventListener('click', closeLoginModal);
            signupClose.addEventListener('click', closeSignupModal);
            showSignup.addEventListener('click', function(e) {
                e.preventDefault();
                closeLoginModal();
                openSignupModal();
            });
            showLogin.addEventListener('click', function(e) {
                e.preventDefault();
                closeSignupModal();
                openLoginModal();
            });

            // Event listeners for payment
            premiumPaymentBtn.addEventListener('click', openPaymentModal);
            paymentClose.addEventListener('click', closePaymentModal);
            
            // Event listeners for payment methods
            paymentMethods.forEach(method => {
                method.addEventListener('click', function() {
                    const methodName = this.getAttribute('data-method');
                    selectPaymentMethod(methodName);
                });
            });

            // Close modals when clicking outside
            window.addEventListener('click', function(e) {
                if (e.target === loginModal) {
                    closeLoginModal();
                }
                if (e.target === signupModal) {
                    closeSignupModal();
                }
                if (e.target === paymentModal) {
                    closePaymentModal();
                }
            });

            // Event listeners for chatbot
            chatbotToggle.addEventListener('click', toggleChatbot);
            chatbotClose.addEventListener('click', toggleChatbot);
            chatbotSend.addEventListener('click', processChatbotInput);
            chatbotInput.addEventListener('keypress', function(e) {
                if (e.key === 'Enter') {
                    processChatbotInput();
                }
            });

            // Event listeners for tool buttons
            toolButtons.forEach(button => {
                button.addEventListener('click', handleToolClick);
            });

            // Pricing button functionality
            const pricingButtons = document.querySelectorAll('.pricing-button');
            pricingButtons.forEach(button => {
                button.addEventListener('click', function() {
                    const plan = this.closest('.pricing-card').querySelector('.pricing-title').textContent;
                    if (plan === 'Basic') {
                        openSignupModal();
                    } else if (plan === 'Premium') {
                        openPaymentModal();
                    } else if (plan === 'Business') {
                        alert('Our Business plan is coming soon. Please contact our sales team for more information.');
                    }
                });
            });

            // Simulate ad loading
            setTimeout(() => {
                const adSpaces = document.querySelectorAll('.ad-container');
                adSpaces.forEach(space => {
                    space.innerHTML = '<p>Advertisement loaded successfully</p>';
                });
            }, 2000);

            // Initialize payment method
            selectPaymentMethod('stripe');
        });
    </script>
</body>
</html>
