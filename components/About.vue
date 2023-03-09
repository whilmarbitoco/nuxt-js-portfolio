<template>
          <div class="container">
            <h2>About Me</h2>
            <div class="section-container">
                <section class="one">
                    <div class="img-container">
                        <img src="coding.png" alt="A photo of me" />
                    </div>
                </section>
                <section class="two">
                    <h3>Who am I?</h3>
                    <p>
                        Hi there! My name is Whilmar Bitoco, and I'm a Web
                        Developer. I'm passionate about technology and have been
                        developing my skills in programming. In my free time, I
                        enjoy reading and drinking coffee.
                    </p>
                    <div class="interest">
                        <h3>My Interests</h3>
                        <ul>
                            <li>
                              <font-awesome-icon icon="chess"/>
                              Chess</li>
                            <li><font-awesome-icon icon="book"/> Reading</li>
                            <li><font-awesome-icon icon="code"/> Programming</li>
                        </ul>
                    </div>
                    <div class="skills">
                        <h3>My Skills</h3>
                        <ul>
                            <li>
                                <span>HTML</span>
                                <div class="progress-bar">
                                    <div
                                        class="progress"
                                        style="width: 80%"
                                    ></div>
                                </div>
                            </li>
                            <li>
                                <span>CSS</span>
                                <div class="progress-bar">
                                    <div
                                        class="progress"
                                        style="width: 75%"
                                    ></div>
                                </div>
                            </li>
                            <li>
                                <span>JavaScript</span>
                                <div class="progress-bar">
                                    <div
                                        class="progress"
                                        style="width: 60%"
                                    ></div>
                                </div>
                            </li>
                            <li>
                                <span>Vue.js</span>
                                <div class="progress-bar">
                                    <div
                                        class="progress"
                                        style="width: 80%"
                                    ></div>
                                </div>
                            </li>
                            <li>
                                <span>Express.js</span>
                                <div class="progress-bar">
                                    <div
                                        class="progress"
                                        style="width: 70%"
                                    ></div>
                                </div>
                            </li>
                            <li>
                                <span>SQLITE</span>
                                <div class="progress-bar">
                                    <div
                                        class="progress"
                                        style="width: 65%"
                                    ></div>
                                </div>
                            </li>
                        </ul>
                    </div>
                </section>
            </div>
  </div>
</template>

<script>
export default {
  name: 'About',
  
}
</script>

<style scoped>
  img {
    width: 100%;
    /*height: 100%;*/
}

.container {
    margin: 1rem;
}

h2 {
    text-align: center;
}

.section-container {
    /* background: #f2f2f2; */
    width: 90vw;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

section {
    width: 50%;
    padding: 1rem;
}

.two p {
    padding: 1rem;
}

.skills {
    margin-top: 2rem;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    margin-bottom: 0.5rem;
}

.interest ul {
    padding: 1rem;
}

.fa {
    color: #56b4c9;
    font-size: 1.5rem;
    margin-right: 0.5rem;
}

span {
    display: inline-block;
    width: 100px;
    font-weight: bold;
}

.progress-bar {
    height: 10px;
    background-color: #f5f5f5;
    border-radius: 10px;
    overflow: hidden;
}

.progress {
    height: 100%;
    background-color: #56b4c9;
}

@media screen and (max-width: 550px) {
    .section-container {
        flex-direction: column;
    }
    section {
        width: 100%;
    }
}

</style>
