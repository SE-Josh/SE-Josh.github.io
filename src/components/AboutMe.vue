<template>
    <article>
        <section class="bigText">
            <p class="skills">
                <span class="title">About Me</span> <br />
                <span class="light">System Architecture Design</span><br />
                Frontend Development <br />
                <span class="hint">Modeling UML</span><br />
                <span class="light">DevOps</span><span class="dot">.</span>
            </p>
        </section>
        <section class="content">
            <p class="intro">
                I specialize in software development for both frontend and backend, with experience <span class="trans"> in</span> designing and developing environme<span class="trans">nts and</span>
                systems. Graduating from the <span class="trans">Software</span> Engineering department, I have <span class="trans">not only honed</span> my software skills but also
                <span class="trans">stayed updated on</span> hardware and technology<span class="trans">-related advancements.</span> My aspiration is<span class="trans"> to remain a perpetual</span>
                learner and <span class="trans">embrace new knowledge, evolving</span> into a <span class="trans">well-rounded software developer.</span>
            </p>
        </section>
    </article>
</template>

<script scoped>
export default {
    name: "AboutMe",
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
            color: #d6d6d6;
            font-size: 15px;
            line-height: 24px;
            font-weight: 300;
            text-align: justify;
            margin: 0;
            transition: all 0.5s;
            cursor: pointer;
            .trans {
                color: #222222;
                transition: all 0.5s;
            }
        }
        .intro:hover {
            color: #ffffff;
            scale: 1.06;
            .trans {
                color: #ffffff;
            }
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
        .shadow {
            text-align: right;
            user-select: none;
            position: absolute;
            color: #cab888bc;
            font-weight: 900;
            font-size: 30px;
            line-height: 60px;
            margin: 0;
            margin-top: 28px;
            margin-left: 30px;
            z-index: 1;
        }

        .greeting {
            align-self: flex-end;
            user-select: none;
            font-weight: bold;
            font-size: 30px;
            line-height: 60px;
            margin: 0;
            margin-bottom: 10px;
            z-index: 2;
        }

        .skills {
            color: #e0c256;
            text-align: right;
            user-select: none;
            font-size: 24px;
            line-height: 34px;
            font-weight: bold;
            margin: 0;
            margin-bottom: 30px;
            z-index: 2;
            .title {
                font-size: 18px;
                font-weight: 600;
                font-family: Courier;
            }
            .dot {
                color: #e2b714;
            }
            .light {
                color: #dfdfdf;
            }
            .hint {
                color: #9e9a9a;
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
                color: #777;

                .trans {
                    color: #777;
                }
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
