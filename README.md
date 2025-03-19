# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Web Page</title>
    <link rel="stylesheet" href="style.css">
    <style>
        body {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        nav {
            background-color: #007bff;
            padding: 10px;
        }
        nav ul {
            display: flex;
            list-style: none;
            justify-content: space-around;
            margin: 0;
            padding: 0;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 8px 16px;
        }
        nav a:hover {
            background-color: #0056b3;
            border-radius: 4px;
        }
        .content {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            padding: 20px;
        }
        @media (min-width: 768px) {
            .content {
                grid-template-columns: 1fr 1fr;
            }
        }
        @media (min-width: 1024px) {
            .content {
                grid-template-columns: 1fr 1fr 1fr;
            }
        }
    </style>
</head>
<body>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <div class="content">
        <section>
            <h2>Section 1</h2>
            <p>This is some text for section 1.</p>
        </section>
        <section>
            <h2>Section 2</h2>
            <p>This is some text for section 2.</p>
        </section>
        <section>
            <h2>Section 3</h2>
            <p>This is some text for section 3.</p>
        </section>
    </div>
</body>
</html>
