<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shristi Srivastava - Full Stack Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.1);
        }

        header {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 30px;
            border-bottom: 3px solid #667eea;
        }

        h1 {
            font-size: 3em;
            color: #2d3748;
            margin-bottom: 10px;
        }

        .tagline {
            font-size: 1.3em;
            color: #667eea;
            font-weight: 600;
            margin: 10px 0;
        }

        .subtitle {
            font-size: 1.1em;
            color: #718096;
            margin-top: 10px;
        }

        h2 {
            color: #2d3748;
            font-size: 2em;
            margin: 40px 0 20px 0;
            padding-bottom: 10px;
            border-bottom: 3px solid #667eea;
        }

        h3 {
            color: #4a5568;
            font-size: 1.5em;
            margin: 25px 0 15px 0;
        }

        .code-block {
            background: #1a202c;
            color: #68d391;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
            overflow-x: auto;
            font-family: 'Courier New', monospace;
            font-size: 14px;
            line-height: 1.6;
        }

        .badge-container {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 20px 0;
            justify-content: center;
        }

        .badge {
            display: inline-block;
            padding: 8px 16px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border-radius: 20px;
            font-weight: bold;
            font-size: 0.9em;
        }

        .project-card {
            background: #f7fafc;
            border-left: 4px solid #667eea;
            padding: 20px;
            margin: 20px 0;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
        }

        .project-card h3 {
            color: #667eea;
            margin-top: 0;
        }

        .tech-stack {
            background: #edf2f7;
            padding: 15px;
            border-radius: 8px;
            margin: 15px 0;
        }

        .achievement {
            background: #f0fff4;
            border-left: 4px solid #48bb78;
            padding: 15px;
            margin: 10px 0;
            border-radius: 4px;
        }

        .achievement::before {
            content: "✅ ";
            font-weight: bold;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }

        .stat-card {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 25px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.3);
        }

        .stat-card h3 {
            color: white;
            font-size: 2.5em;
            margin: 0;
        }

        .stat-card p {
            margin: 10px 0 0 0;
            font-size: 1.1em;
        }

        .contact-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
            flex-wrap: wrap;
        }

        .contact-links a {
            padding: 12px 30px;
            background: #667eea;
            color: white;
            text-decoration: none;
            border-radius: 25px;
            font-weight: bold;
            transition: all 0.3s;
        }

        .contact-links a:hover {
            background: #764ba2;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .skill-category {
            background: #f7fafc;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        .skill-category h4 {
            color: #667eea;
            margin-bottom: 15px;
            font-size: 1.2em;
        }

        .skill-category ul {
            list-style: none;
            padding: 0;
        }

        .skill-category li {
            padding: 8px 0;
            color: #4a5568;
        }

        .skill-category li::before {
            content: "▸ ";
            color: #667eea;
            font-weight: bold;
        }

        .architecture-diagram {
            background: #1a202c;
            color: #68d391;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
            overflow-x: auto;
            font-family: 'Courier New', monospace;
            font-size: 12px;
            line-height: 1.4;
        }

        .collapsible {
            background-color: #667eea;
            color: white;
            cursor: pointer;
            padding: 18px;
            width: 100%;
            border: none;
            text-align: left;
            outline: none;
            font-size: 1.1em;
            font-weight: bold;
            border-radius: 8px;
            margin: 10px 0;
            transition: 0.3s;
        }

        .collapsible:hover {
            background-color: #5568d3;
        }

        .collapsible::after {
            content: '\002B';
            color: white;
            font-weight: bold;
            float: right;
            font-size: 1.5em;
        }

        .collapsible.active::after {
            content: "\2212";
        }

        .content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
            background-color: #f7fafc;
            padding: 0 20px;
            border-radius: 0 0 8px 8px;
        }

        .content.active {
            padding: 20px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }

        table th {
            background: #667eea;
            color: white;
            padding: 12px;
            text-align: left;
        }

        table td {
            padding: 12px;
            border-bottom: 1px solid #e2e8f0;
        }

        table tr:hover {
            background: #f7fafc;
        }

        .highlight {
            background: linear-gradient(120deg, #84fab0 0%, #8fd3f4 100%);
            padding: 2px 6px;
            border-radius: 3px;
            font-weight: bold;
        }

        @media (max-width: 768px) {
            .container {
                padding: 20px;
            }

            h1 {
                font-size: 2em;
            }

            h2 {
                font-size: 1.5em;
            }

            .stats-grid {
                grid-template-columns: 1fr;
            }
        }

        .emoji {
            font-size: 1.2em;
        }

        pre {
            background: #2d3748;
            color: #68d391;
            padding: 15px;
            border-radius: 8px;
            overflow-x: auto;
            margin: 15px 0;
        }

        code {
            font-family: 'Courier New', monospace;
            background: #edf2f7;
            padding: 2px 6px;
            border-radius: 3px;
            color: #e53e3e;
        }

        .profile-header {
            text-align: center;
            padding: 40px 0;
        }

        .intro-code {
            background: #1a2
