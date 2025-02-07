<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI 宣传网站</title>
    <link rel="stylesheet" href="styles.css">
    <script src="https://cdn.jsdelivr.net/npm/tsparticles@2.11.0/tsparticles.bundle.min.js"></script>
</head>
<body>
    <!-- 粒子动画背景 -->
    <div id="particles-js"></div>

    <!-- 页面内容 -->
    <header>
        <h1>智能 AI 未来</h1>
        <p>探索 AI 的无限可能，开启智能新时代</p>
        <a href="#features" class="cta-button">了解更多</a>
    </header>

    <!-- 关键功能展示 -->
    <section id="features">
        <div class="feature">
            <h2>自动化</h2>
            <p>提高效率，减少人工成本</p>
        </div>
        <div class="feature">
            <h2>智能学习</h2>
            <p>机器学习算法助力创新</p>
        </div>
        <div class="feature">
            <h2>数据分析</h2>
            <p>精准预测和洞察趋势</p>
        </div>
    </section>

    <script src="script.js"></script>
</body>
</html>body, html {
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100%;
    font-family: Arial, sans-serif;
    color: white;
    background: black;
    text-align: center;
}

/* 粒子背景 */
#particles-js {
    position: absolute;
    width: 100%;
    height: 100%;
    z-index: -1;
}

/* 头部区域 */
header {
    position: relative;
    top: 40%;
    transform: translateY(-50%);
    z-index: 1;
}

h1 {
    font-size: 3rem;
    margin: 0;
}

p {
    font-size: 1.5rem;
    margin: 10px 0;
}

.cta-button {
    display: inline-block;
    padding: 10px 20px;
    font-size: 1.2rem;
    color: black;
    background: white;
    border-radius: 5px;
    text-decoration: none;
    margin-top: 20px;
    transition: 0.3s;
}

.cta-button:hover {
    background: #ddd;
}

/* 关键功能展示 */
#features {
    display: flex;
    justify-content: center;
    gap: 20px;
    padding: 50px 10px;
}

.feature {
    background: rgba(255, 255, 255, 0.1);
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    text-align: center;
}tsParticles.load("particles-js", {
    particles: {
        number: {
            value: 100
        },
        color: {
            value: "#ffffff"
        },
        shape: {
            type: "circle"
        },
        opacity: {
            value: 0.5,
            random: true
        },
        size: {
            value: 3,
            random: true
        },
        move: {
            enable: true,
            speed: 2
        }
    },
    interactivity: {
        events: {
            onHover: {
                enable: true,
                mode: "repulse"
            }
        }
    }
});