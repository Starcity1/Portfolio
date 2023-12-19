<template>
    <footer>
        <span class="hyperlink-list">
            <h3>Contact Information</h3>
            <p>
            Email: david.rodriguez220442@gmail.com <br>
            Discord: ascension6726 <br>
            </p>
        </span>
        <span class="logos">
                <div class="logo-icon">
                    <a href="https://www.linkedin.com/in/davidrodriguez2404/" target="_blank"><img src="../assets/LinkedIn-logo-highlighted.png" alt="."><span v-if="isHoveringLinkedIn" class="hide">LinkedIn</span></a>
                </div>
                <div class="logo-icon">
                    <a href="https://www.pinterest.com/davidrodriguez220443/" target="_blank"><img src="../assets/pinterest-logo-default.png" alt="."><span v-if="isHoveringPinterest" class="hide">Pinterest</span></a>
                </div>
                <div class="logo-icon">
                    <a href="https://github.com/Starcity1" target="_blank"><img src="../assets/github-logo-default.png" alt="."><span v-if="isHoveringGit" class="hide">GitHub</span></a>
                </div>
                <div class="logo-icon">
                    <a href="https://twitter.com/Dav_Rod24" target="_blank"><img src="../assets/twitter-logo-default.png" alt="."><span v-if="isHoveringTwitter" class="hide">X</span></a>
                </div>
        </span>
    </footer>
</template>

<script>
export default {
    name: "MyFooter",
    data() {
        return {
            isHoveringLinkedIn: false,
            isHoveringPinterest: false,
            isHoveringGit: false,
            isHoveringTwitter: false,
        }
    }
}
</script>

<style>
footer {
    position: absolute;
    width: 100vw;
    background-color: gray;
    color: whitesmoke;
    font-weight: lighter;
    bottom: 0;
    padding: 20px;
}

.hyperlink-list {
    display: inline-block;
}

.logos {
    position: absolute;
    top: 0vh;
    right: 10vw;
    display: inline-block;
}

.logo-icon {
    display: inline-block;
    padding: 5px;
    margin: 15px;
}

.logo-icon img {
    max-width: 3vw;
}

.logo-icon:hover {
    background-color: white;
}
</style>