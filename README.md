<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grow Greens Farm Fresh | Sustainable AgriTech Partnership</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #2e7d32;
            --secondary-color: #4caf50;
            --accent-color: #81c784;
            --dark-text: #212121;
            --light-bg: #f9fbf7;
            --white: #ffffff;
            --github-dark: #24292e;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--light-bg);
            color: var(--dark-text);
            line-height: 1.6;
        }

        /* Navigation */
        header {
            background-color: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
        }

        .logo {
            font-size: 1.3rem;
            font-weight: 800;
            color: var(--primary-color);
            text-decoration: none;
            letter-spacing: 0.5px;
        }

        nav {
            display: flex;
            align-items: center;
        }

        nav a {
            color: var(--dark-text);
            text-decoration: none;
            margin-left: 1.5rem;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--secondary-color);
        }

        .btn-github-nav {
            background-color: var(--github-dark);
            color: var(--white) !important;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 0.9rem;
            transition: background-color 0.3s, transform 0.2s !important;
        }

        .btn-github-nav:hover {
            background-color: #000000;
            transform: translateY(-1px);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(46, 125, 50, 0.85), rgba(27, 94, 32, 0.9)), url('
