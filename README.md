<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FAQ Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }
        header {
            background: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        h1 {
            margin: 0;
        }
        .faq-list {
            padding: 0;
            list-style: none;
        }
        .faq-list li {
            background: #fff;
            margin-bottom: 5px;
            border: 1px solid #ddd;
        }
        .faq-list a {
            display: block;
            padding: 10px;
            text-decoration: none;
            color: #333;
            font-size: 20px;
        }
        .faq-list a:hover {
            background: #efefef;
        }
        .answer {
            display: none;
            padding: 10px;
            background: #fff;
            border: 1px solid #ddd;
            margin-bottom: 5px;
        }
    </style>
</head>
<body>
    <header>
        <h1>FAQ</h1>
    </header>
    <div class="container">
        <ul class="faq-list">
            <li>
                <a href="#" onclick="toggleAnswer(this)">What is QuantumultX?</a>
                <div class="answer">
                    QuantumultX is a powerful proxy client that supports various protocols and can capture and redirect TCP traffic.
                </div>
            </li>
            <li>
                <a href="#" onclick="toggleAnswer(this)">How do I install QuantumultX?</a>
                <div class="answer">
                    You can install QuantumultX from the official App Store. Follow the instructions provided during the installation process.
                </div>
            </li>
            <li>
                <a href="#" onclick="toggleAnswer(this)">Where can I find more configuration for QuantumultX?</a>
                <div class="answer">
                    Visit our GitHub repository for a variety of configurations and scripts shared by the community.
                </div>
            </li>
            <!-- Add more FAQ items here -->
        </ul>
    </div>

    <script>
        function toggleAnswer(element) {
            var answer = element.nextElementSibling;
            // Toggle the visibility of the answer
            if (answer.style.display === 'block') {
                answer.style.display = 'none';
            } else {
                answer.style.display = 'block';
            }
        }
    </script>
</body>
</html>
