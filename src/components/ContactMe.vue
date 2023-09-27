<template>
    <article>
        <div class="my-pic">
            <img src="../assets/my-pic.png" alt="" />
        </div>
        <h1 class="contactMe">Contact Me</h1>
        <section class="contactInfo">
            <div class="item" @click="handleLink('mail')">
                <div class="top">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-inbox-fill" viewBox="0 0 16 16">
                        <path
                            d="M4.98 4a.5.5 0 0 0-.39.188L1.54 8H6a.5.5 0 0 1 .5.5 1.5 1.5 0 1 0 3 0A.5.5 0 0 1 10 8h4.46l-3.05-3.812A.5.5 0 0 0 11.02 4H4.98zm-1.17-.437A1.5 1.5 0 0 1 4.98 3h6.04a1.5 1.5 0 0 1 1.17.563l3.7 4.625a.5.5 0 0 1 .106.374l-.39 3.124A1.5 1.5 0 0 1 14.117 13H1.883a1.5 1.5 0 0 1-1.489-1.314l-.39-3.124a.5.5 0 0 1 .106-.374l3.7-4.625z"
                        />
                    </svg>
                    Email
                </div>
                <div class="info">chiahsuan</div>
            </div>
            <div class="item" @click="handleLink('insta')">
                <div class="top">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-instagram" viewBox="0 0 16 16">
                        <path
                            d="M8 0C5.829 0 5.556.01 4.703.048 3.85.088 3.269.222 2.76.42a3.917 3.917 0 0 0-1.417.923A3.927 3.927 0 0 0 .42 2.76C.222 3.268.087 3.85.048 4.7.01 5.555 0 5.827 0 8.001c0 2.172.01 2.444.048 3.297.04.852.174 1.433.372 1.942.205.526.478.972.923 1.417.444.445.89.719 1.416.923.51.198 1.09.333 1.942.372C5.555 15.99 5.827 16 8 16s2.444-.01 3.298-.048c.851-.04 1.434-.174 1.943-.372a3.916 3.916 0 0 0 1.416-.923c.445-.445.718-.891.923-1.417.197-.509.332-1.09.372-1.942C15.99 10.445 16 10.173 16 8s-.01-2.445-.048-3.299c-.04-.851-.175-1.433-.372-1.941a3.926 3.926 0 0 0-.923-1.417A3.911 3.911 0 0 0 13.24.42c-.51-.198-1.092-.333-1.943-.372C10.443.01 10.172 0 7.998 0h.003zm-.717 1.442h.718c2.136 0 2.389.007 3.232.046.78.035 1.204.166 1.486.275.373.145.64.319.92.599.28.28.453.546.598.92.11.281.24.705.275 1.485.039.843.047 1.096.047 3.231s-.008 2.389-.047 3.232c-.035.78-.166 1.203-.275 1.485a2.47 2.47 0 0 1-.599.919c-.28.28-.546.453-.92.598-.28.11-.704.24-1.485.276-.843.038-1.096.047-3.232.047s-2.39-.009-3.233-.047c-.78-.036-1.203-.166-1.485-.276a2.478 2.478 0 0 1-.92-.598 2.48 2.48 0 0 1-.6-.92c-.109-.281-.24-.705-.275-1.485-.038-.843-.046-1.096-.046-3.233 0-2.136.008-2.388.046-3.231.036-.78.166-1.204.276-1.486.145-.373.319-.64.599-.92.28-.28.546-.453.92-.598.282-.11.705-.24 1.485-.276.738-.034 1.024-.044 2.515-.045v.002zm4.988 1.328a.96.96 0 1 0 0 1.92.96.96 0 0 0 0-1.92zm-4.27 1.122a4.109 4.109 0 1 0 0 8.217 4.109 4.109 0 0 0 0-8.217zm0 1.441a2.667 2.667 0 1 1 0 5.334 2.667 2.667 0 0 1 0-5.334z"
                        />
                    </svg>
                    Instagram
                </div>
                <div class="info">87osh</div>
            </div>
            <div class="item" @click="handleLink('facebook')">
                <div class="top">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-facebook" viewBox="0 0 16 16">
                        <path
                            d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z"
                        />
                    </svg>
                    Facebook
                </div>
                <div class="info">Josh Lin</div>
            </div>
            <div class="item" @click="handleLink('medium')">
                <div class="top">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-medium" viewBox="0 0 16 16">
                        <path
                            d="M9.025 8c0 2.485-2.02 4.5-4.513 4.5A4.506 4.506 0 0 1 0 8c0-2.486 2.02-4.5 4.512-4.5A4.506 4.506 0 0 1 9.025 8zm4.95 0c0 2.34-1.01 4.236-2.256 4.236-1.246 0-2.256-1.897-2.256-4.236 0-2.34 1.01-4.236 2.256-4.236 1.246 0 2.256 1.897 2.256 4.236zM16 8c0 2.096-.355 3.795-.794 3.795-.438 0-.793-1.7-.793-3.795 0-2.096.355-3.795.794-3.795.438 0 .793 1.699.793 3.795z"
                        />
                    </svg>
                    Medium
                </div>
                <div class="info">Josh</div>
            </div>
            <div class="item" @click="handleLink('github')">
                <div class="top">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-github" viewBox="0 0 16 16">
                        <path
                            d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"
                        />
                    </svg>
                    Github
                </div>
                <div class="info">SE-Josh</div>
            </div>
        </section>
    </article>
</template>

<script>
export default {
    name: "ContactMe",
    methods: {
        handleLink(str) {
            if (str === "mail") {
                window.open("mailto:chiahsuan@webglsoft.com");
            } else if (str === "insta") {
                window.open("https://www.instagram.com/87osh/");
            } else if (str === "facebook") {
                window.open("https://www.facebook.com/profile.php?id=100000105046744");
            } else if (str === "medium") {
                window.open("https://medium.com/@jokezxcv");
            } else if (str === "github") {
                window.open("https://github.com/SE-Josh");
            }
        },
    },
};
</script>

<style scoped>
article {
    display: flex;
    flex-direction: column;
}
.contactInfo {
    display: flex;
    flex-direction: row;
    gap: 15px;
}
.item {
    flex: 1;
    display: flex;
    flex-direction: column;
    gap: 10px;
    font-size: 20px;
    align-items: flex-start;
    user-select: none;
    cursor: pointer;
    transition: all 1s;
}
.item:hover {
    color: #6f9bf1;
    scale: 1.4;
    padding-left: 35px;
    padding-right: 35px;
}
.top {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    gap: 10px;
}
.info {
    text-align: left;
    opacity: 0;
    font-size: 10px;
}
.item:hover .info {
    display: block;
    font-size: 10px;
    color: #666666;
    opacity: 1;
}
.contactMe {
    align-self: flex-start;
    font-size: 48px;
    color: #c0c0c0;
    margin-top: 0px;
    margin-bottom: 15px;
    cursor: pointer;
    border-bottom: 2px solid #6f9af100;
    user-select: none;
    transition: all 1s;
    padding-bottom: 5%;
}
.contactMe:hover {
    color: #ffd700;
    border-bottom: 2px solid #ffd700;
    padding-left: 30%;
    padding-right: 23%;
    cursor: none;
}
.my-pic {
    margin-bottom: 5px;    
    opacity: 0.6;
    transition: all 1s;
    cursor: pointer;
}
.my-pic img {
    max-height: 200px;
    width: auto;
}
.my-pic:hover {
    opacity: 1;
}

@media (max-width: 768px) {
    .contactInfo {
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        align-self: flex-start;
    }
    .contactMe {
        margin-top: 5px;
    }
    .contactMe:hover {
        color: #ffd700;
        scale: 1.05;
        padding: 0;
        border: 0;
    }
}
</style>
