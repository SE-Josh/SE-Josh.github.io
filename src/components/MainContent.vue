<template>
    <main>
        <section class="picture">
            <img src="../assets/logo.png" alt="" />
            <!-- <img src="../assets/my-pic.png" alt="" /> -->
        </section>
        <section class="content">
            <p class="shadow">SoftWare Engineer</p>
            <!-- <p class="chineseName">ChiaHsuan</p> -->
            <div class="greeting">Hi! this is</div>
            <p class="name">Josh<span class="dot">.</span></p>
            <p class="intro">
                An enthusiastic software engineer passionate about technological knowledge, enjoys sports and games, and continuously enhances development skills while expanding horizons.
            </p>
        </section>
    </main>
</template>

<script>
export default {
    name: "MainContent",
};
</script>

<style scoped>
main {
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

        .shadow {
            user-select: none;
            position: absolute;
            color: #292828bc;
            font-weight: 900;
            font-size: 30px;
            line-height: 35px;
            margin: 0;
            margin-top: 41px;
            margin-left: 30px;
            z-index: 1;
            transition: color 1s;
        }

        .greeting {
            user-select: none;
            font-weight: bold;
            font-size: 30px;
            line-height: 60px;
            margin: 0;
            margin-bottom: 10px;
            z-index: 2;
            transition: all 1.5s;
        }

        .name {
            user-select: none;
            font-size: 72px;
            line-height: 60px;
            font-weight: bold;
            align-self: flex-end;
            margin: 0;
            margin-bottom: 30px;
            z-index: 2;
            transition: all 1.5s;
            .dot {
                color: #e2b714;
            }
        }

        .intro {
            color: #999;
            font-size: 15px;
            line-height: 24px;
            font-weight: 300;
            text-align: justify;
            margin: 0;
            transition: all 1.5s;
        }
    }

    .picture {
        flex: 1;
        opacity: 0.8;
        transition: all 1s;
    }
    .picture img {
        object-fit: cover;
        width: 75%;
    }
    .picture:hover {
        opacity: 1;
        scale: 1.05;
    }
}
.content:hover .greeting {
    padding-left: 50%;
    color: transparent;
}
.content:hover .name {
    padding-right: 40%;
    color: #e2b714;
}
.content:hover .intro {
    scale: 1.1;
}

.content:hover .shadow {
    color: #ffffff;
}

@media (max-width: 768px) {
    main {
        flex-direction: column;
        gap: 15px;

        .content {
            align-items: flex-start;
            text-align: center;
            padding-left: 40px;
            padding-right: 40px;
            margin-bottom: 3px;
            .name {
                margin-bottom: 5px;
            }

            .intro {
                font-size: 22px;
                text-align: justify;
                line-height: 26px;
            }
        }
        .content:hover .greeting {
            padding-left: 30%;
            color: transparent;
        }
    }

    .picture {
        display: flex;
        justify-content: center;
        align-items: flex-end;
        width: 90%;
        object-fit: cover;
    }

}
</style>
