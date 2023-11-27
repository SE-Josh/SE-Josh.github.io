<template>
    <article>
        <section class="bigText">
            <p class="skills">
                <span class="title">{{ title }}</span> <br />
                <span>{{ skill1 }}<br /></span>
                <span>{{ skill2 }}<br /></span>
                <span>{{ skill3 }}<br /></span>
                <span>{{ skill4 }}</span>
                <span class="dot">.</span>
            </p>
        </section>
        <section class="content">
            <p class="intro">{{ intro }}<span class="dot">.</span></p>
        </section>
    </article>
</template>

<script scoped>
export default {
    name: "AboutMe",
    data() {
        return {
            title: "About Me",
            skill1: "System Architecture Design",
            skill2: "Frontend Development",
            skill3: "Modeling UML",
            skill4: "DevOps",
            intro: "I specialize in software development for both frontend and backend, with experience in designing and developing environments and systems. Graduating from the Software Engineering department, I have not only honed my software skills but also stayed updated on hardware and technology-related advancements. My aspiration is to remain a perpetual learner and embrace new knowledge, evolving into a well-rounded software developer",
        };
    },
};
</script>

<style scoped>
article {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    max-width: 750px;
    margin-left: auto;
    margin-right: auto;
    font-family: monospace;

    .content {
        text-align: left;
        flex: 1;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: flex-start;
        position: relative;

        .intro {
            background: linear-gradient(to right, #fcd8cc, #d0f1fa);
            background-clip: text;
            color: transparent;
            font-size: 15px;
            line-height: 24px;
            font-weight: 300;
            text-align: justify;
            margin: 0;
            transition: all 0.5s;

            .dot {
                color: #e2b714;
            }
        }
        .intro:hover {
            scale: 1.06;
            color: #fde8e0;
        }
    }

    .bigText {
        text-align: left;
        flex: 1;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: flex-start;
        position: relative;
        .skills {
            text-align: right;
            user-select: none;
            font-size: 24px;
            line-height: 34px;
            font-weight: bold;
            margin: 0;
            margin-bottom: 30px;
            z-index: 2;
            background: linear-gradient(to left, #fcd8cc, #b2edfb);
            background-clip: text;
            color: transparent;
            .title {
                font-size: 38px;
                font-weight: 700;
                letter-spacing: 2px;
                color: #e2b714;
            }
            .dot {
                color: #e2b714;
            }
        }
    }
}

@media (max-width: 768px) {
    article {
        flex-direction: column;
        gap: 5px;

        .content {
            flex: 2;
            align-items: flex-start;
            text-align: center;
            padding-left: 40px;
            padding-right: 40px;
            margin-bottom: 3px;

            .intro {
                font-size: 19px;
                text-align: left;
                line-height: 26px;
                background: linear-gradient(to left, #fcd8cc, #d0f1fa);
                background-clip: text;
                color: transparent;
            }
        }

        .bigText {
            display: flex;
            justify-content: flex-end;
            align-items: flex-end;
        }
    }
}
</style>
