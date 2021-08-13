<template>
  <div class="skill">
    <h1>What I can do?</h1>
    <h2>Programming Skills</h2>
    <div class="list">
        <p>Python</p>
        <p>Java</p>
        <p>Javascript</p>
        <p>C and C++</p>
    </div>
    <h2>Web and Frameworks</h2>
    <div class="list">
        <p>HTML</p>
        <p>CSS</p>
        <p>Bootstrap</p>
        <p>Tailwind</p>
        <p>Vue.js</p>
    </div>
    <h2>UI and UX</h2>
    <div class="list">
        <p>Figma & Adobe XD</p>
        <p>Wireframing</p>
        <p>User Centered Design</p>
        <p>Vue.js</p>
    </div>
    <h2>Graphic Design Software</h2>
    <div class="list">
        <p>Illustrator</p>
        <p>Photoshop</p>
        <p>After Effect</p>
        <p>Premiere Pro</p>
    </div>
    <h2>Project Development</h2>
    <div class="list">
        <p>Trello</p>
        <p>Miro</p>
        <p>FigJam</p>
        <p>ClickUp</p>
    </div>
  </div>
</template>

<style scoped>
.skill {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    text-align: start;
}

.list {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    text-align: start;
}

.list p{
    padding: 0.25em 1em;
    margin: 0em 1em;
    background: #2f80ed;
    border-radius: 32px;
    color: #fcfcfc;
    transition: 0.3s;
}
.list p:hover{
    padding: 0.25em 1em;
    margin: 0em 1em;
    background: #fcfcfc;
    border-radius: 32px;
    color: #2f80ed;
}

@media only screen and (max-width: 768px) {
    .list {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        text-align: start;
    }
    .list p{
    margin: .25em 0em;
    }
}
</style>