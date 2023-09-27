<template>
    <article>
        <h1><span class="gold">Career</span> &<span class="blue"> Education</span></h1>
        <section class="timeline">
            <div class="timelineItem">
                <span class="educationTitle">DSSH</span>
                <br />
                <span class="at">General</span>
                <br />
                <span class="period">2015 - 2018</span>
            </div>
            <div class="timelineItem">
                <span class="educationTitle">NKNU</span>
                <br />
                <span class="at">Software Engineering</span>
                <br />
                <span class="period">2018 - 2022</span>
            </div>
            <div class="timelineItem">
                <span class="careerTitle">Frank-Chen</span>
                <br />
                <span class="at">Web Designer</span>
                <br />
                <span class="period">2021</span>
            </div>
            <div class="timelineItem">
                <span class="careerTitle">NKNU-IEC</span>
                <br />
                <span class="at">Assistant Engineer</span>
                <br />
                <span class="period">2021 - 2022</span>
            </div>
            <div class="timelineItem">
                <span class="careerTitle">GLSoft</span>
                <br />
                <span class="at">FrontEnd Engineer</span>
                <br />
                <span class="period">2023 - Present</span>
            </div>
        </section>
    </article>
</template>

<script>
export default {
    name: "EducationExperience",
};
</script>

<style scoped>
article {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    max-width: 750px;
    margin-left: auto;
    margin-right: auto;
    font-family: monospace;
}
h1 {
    font-size: 48px;
    color: #ffffff;
}
.blue {
    color: #6f9bf1;
}
.gold {
    color: #e2b714;
}
.timeline {
    display: flex;
    flex-direction: row-reverse;
    justify-content: flex-start;
    align-items: flex-start;
    gap: 5px;
}
.timelineItem {
    flex: 1;
    margin-right: 10px;
    border-right: 2px;
    text-align: left;
    cursor: pointer;
    transition: all 0.5s;
}
.timelineItem:hover {
    scale: 1.15;
}
.educationTitle {
    padding-left: 12px;
    border-left: 2px solid #6f9bf1;
    font-size: 30px;
    font-weight: bold;
    white-space: nowrap;
}
.careerTitle {
    padding-left: 12px;
    border-left: 2px solid #e2b714;
    font-size: 30px;
    font-weight: bold;
    white-space: nowrap;
}
.at {
    padding-left: 14px;
    white-space: nowrap;
}
.period {
    padding-left: 14px;
    white-space: nowrap;
    color: #838383;
}

@media (max-width: 768px) {
    article {
        flex-direction: column;
        gap: 25px;
    }
    .timeline {
        flex-direction: column-reverse;
        gap: 16px;
    }
}
</style>
