<template>
    <article>
        <h1>
            SKILLS
            <div class="link" @click="goToPortfolio()">
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-link-45deg" viewBox="0 0 16 16">
                    <path
                        d="M4.715 6.542 3.343 7.914a3 3 0 1 0 4.243 4.243l1.828-1.829A3 3 0 0 0 8.586 5.5L8 6.086a1.002 1.002 0 0 0-.154.199 2 2 0 0 1 .861 3.337L6.88 11.45a2 2 0 1 1-2.83-2.83l.793-.792a4.018 4.018 0 0 1-.128-1.287z"
                    />
                    <path
                        d="M6.586 4.672A3 3 0 0 0 7.414 9.5l.775-.776a2 2 0 0 1-.896-3.346L9.12 3.55a2 2 0 1 1 2.83 2.83l-.793.792c.112.42.155.855.128 1.287l1.372-1.372a3 3 0 1 0-4.243-4.243L6.586 4.672z"
                    />
                </svg>
                Checkout Portfolio
            </div>
        </h1>
        <section class="skillCategory">
            <div class="category">
                <div class="title">Front-end</div>
                <div class="skill">React, React Native</div>
                <div class="skill">Vue 3</div>
                <div class="skill">Angular</div>
                <div class="skill">Bootstrap 5 & RWD</div>
                <div class="skill">Pixi, Three.js</div>
                <div class="skill">API integration</div>
                <div class="degree"><span class="gold">Expert.</span></div>
            </div>
            <div class="category">
                <div class="title">Back-end</div>
                <div class="skill">Node.js (Express)</div>
                <div class="skill">MariaDB</div>
                <div class="skill">Mocha</div>
                <div class="skill">JMeter</div>
                <div class="skill">Socket.io</div>
                <div class="skill">Docker</div>
                <div class="degree"><span class="silver">Advanced.</span></div>
            </div>
            <div class="category">
                <div class="title">Related</div>
                <div class="skill">PlantUML</div>
                <div class="skill">Firebase</div>
                <div class="skill">Azure Portal</div>
                <div class="skill">TensorFlow</div>
                <div class="skill">Blockly</div>
                <div class="skill">Puppeteer</div>
                <div class="degree"><span class="bronze">Intermediate.</span></div>
            </div>
        </section>
    </article>
</template>

<script scoped>
export default {
    name: "SkillsPortfolio",
    methods: {
        goToPortfolio() {
            window.open("/portfolio.pdf", "_blank");
        },
    },
};
</script>

<style>
article {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    max-width: 768px;
    margin-left: auto;
    margin-right: auto;
    font-family: monospace;
}
h1 {
    align-self: flex-start;
    font-size: 48px;
    color: #c0c0c0;
    margin-bottom: 15px;
    cursor: pointer;
    transition: all 0.8s;
}
h1:hover {
    color: #6f9bf1;
}
.link {
    font-size: 14px;
    cursor: pointer;
    display: flex;
    gap: 3px;
    color: #ffeb8a;
    transition: all 0.8s;
    padding: 5px;
}
.link:hover {
    background-color: #ffd500;
    color: #000000;
    padding-right: 50px;
    padding-left: 50px;
}
.gold {
    color: #ffd700;
}
.silver {
    color: #c0c0c0;
}
.bronze {
    color: #cd7f32;
}

.skillCategory {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: flex-start;
}
.category {
    flex: 1;
    position: relative;
    margin-right: 10px;
    border-right: 2px;
    text-align: left;
    padding-bottom: 30px;
    min-width: 240px;
    cursor: pointer;
    transition: all 0.8s;
}

.category:hover {
    scale: 1.2;
}

.title {
    padding-left: 12px;
    font-size: 30px;
    white-space: nowrap;
    font-weight: bold;  
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    color: #8f8e8e;
    margin-bottom: 5px;
}
.skill {
    padding-left: 14px;
    white-space: nowrap;
    margin-bottom: 2px;
}
.skill::before {
    content: "• ";
    color: #2f2f2f;
    font-size: 14px;
    margin-right: 5px;
}
.degree {
    white-space: nowrap;
    color: #838383;
    position: absolute;
    bottom: 0;
    right: 60px;
}

@media (max-width: 768px) {
    article {
        flex-direction: column;
        gap: 5px;
    }
    h1 {
        margin: 0;
    }
    .skillCategory {
        flex-direction: column;
        gap: 6px;
    }
    .degree {
        right: 0px;
    }
}
</style>
