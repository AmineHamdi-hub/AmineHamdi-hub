<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profile Introduction</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .container {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 40px;
            max-width: 800px;
            width: 100%;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            animation: fadeIn 0.8s ease-out;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        h1 {
            font-size: 2.5em;
            color: #333;
            margin-bottom: 30px;
            text-align: center;
            animation: slideDown 0.6s ease-out;
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .intro-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 25px;
            padding: 15px;
            border-radius: 10px;
            background: rgba(102, 126, 234, 0.05);
            transition: all 0.3s ease;
            opacity: 0;
            animation: slideIn 0.5s ease-out forwards;
        }

        .intro-item:nth-child(1) { animation-delay: 0.1s; }
        .intro-item:nth-child(2) { animation-delay: 0.2s; }
        .intro-item:nth-child(3) { animation-delay: 0.3s; }
        .intro-item:nth-child(4) { animation-delay: 0.4s; }
        .intro-item:nth-child(5) { animation-delay: 0.5s; }
        .intro-item:nth-child(6) { animation-delay: 0.6s; }
        .intro-item:nth-child(7) { animation-delay: 0.7s; }
        .intro-item:nth-child(8) { animation-delay: 0.8s; }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        .intro-item:hover {
            background: rgba(102, 126, 234, 0.1);
            transform: translateX(10px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .emoji {
            font-size: 1.8em;
            margin-right: 15px;
            min-width: 40px;
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-5px);
            }
        }

        .intro-item:hover .emoji {
            animation: spin 0.5s ease;
        }

        @keyframes spin {
            from {
                transform: rotate(0deg);
            }
            to {
                transform: rotate(360deg);
            }
        }

        .content {
            flex: 1;
        }

        .label {
            font-weight: bold;
            color: #667eea;
            margin-bottom: 5px;
            font-size: 1.1em;
        }

        .text {
            color: #555;
            line-height: 1.6;
        }

        .editable {
            background: rgba(255, 255, 255, 0.8);
            border: 2px dashed #667eea;
            padding: 8px;
            border-radius: 5px;
            color: #999;
            font-style: italic;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .editable:hover {
            background: rgba(102, 126, 234, 0.1);
            border-style: solid;
            color: #667eea;
        }

        @media (max-width: 600px) {
            .container {
                padding: 25px;
            }

            h1 {
                font-size: 2em;
            }

            .emoji {
                font-size: 1.5em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Hi there! 👋</h1>
        
        <div class="intro-item">
            <div class="emoji">🔭</div>
            <div class="content">
                <div class="label">Current Focus</div>
                <div class="text">Working on exciting new projects that push boundaries</div>
            </div>
        </div>

        <div class="intro-item">
            <div class="emoji">🌱</div>
            <div class="content">
                <div class="label">Learning Journey</div>
                <div class="text">Deep diving into Agentic AI and its real-world applications</div>
            </div>
        </div>

        <div class="intro-item">
            <div class="emoji">👯</div>
            <div class="content">
                <div class="label">Collaboration</div>
                <div class="text">Looking to collaborate on meaningful, real-world projects</div>
            </div>
        </div>

        <div class="intro-item">
            <div class="emoji">🤔</div>
            <div class="content">
                <div class="label">Looking for Help With</div>
                <div class="text editable">Your specific needs here...</div>
            </div>
        </div>

        <div class="intro-item">
            <div class="emoji">💬</div>
            <div class="content">
                <div class="label">Ask Me About</div>
                <div class="text editable">Your expertise areas here...</div>
            </div>
        </div>

        <div class="intro-item">
            <div class="emoji">📫</div>
            <div class="content">
                <div class="label">How to Reach Me</div>
                <div class="text editable">Your contact info here...</div>
            </div>
        </div>

        <div class="intro-item">
            <div class="emoji">😄</div>
            <div class="content">
                <div class="label">Pronouns</div>
                <div class="text editable">Your pronouns here...</div>
            </div>
        </div>

        <div class="intro-item">
            <div class="emoji">⚡</div>
            <div class="content">
                <div class="label">Fun Fact</div>
                <div class="text editable">Something interesting about you...</div>
            </div>
        </div>
    </div>
</body>
</html>
