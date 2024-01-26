<template>
    <footer>
        <span class="hyperlink-list">
            <h3>Contact Information</h3>
            <p>
            Email: david.rodriguez220442@gmail.com <br>
            </p>
        </span>
        <span class="logos">
                <span id="follow-statement">Follow My Socials!</span>
                <div class="logo-icon">
                    <a href="https://www.linkedin.com/in/davidrodriguez2404/" target="_blank"><div id="linkedin-img"></div><span v-if="isHoveringLinkedIn" class="hide">LinkedIn</span></a>
                </div>
                <div class="logo-icon">
                    <a href="https://www.pinterest.com/davidrodriguez220443/" target="_blank"><div id="pinterest-img"></div><span v-if="isHoveringPinterest" class="hide">Pinterest</span></a>
                </div>
                <div class="logo-icon">
                    <a href="https://github.com/Starcity1" target="_blank"><div id="github-img"></div><span v-if="isHoveringGit" class="hide">GitHub</span></a>
                </div>
                <div class="logo-icon">
                    <a href="https://twitter.com/Dav_Rod24" target="_blank"><div id="twitter-img"></div><span v-if="isHoveringTwitter" class="hide">X</span></a>
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
    bottom: 0;
    margin-bottom: 0;
    width: 100vw;
    height: 7.5vw;
    background-color: gray;
    color: whitesmoke;
    font-weight: lighter;
    padding: 20px;
    overflow-x: scroll;
}

.hyperlink-list {
    display: inline-block;
}

.logos {
    position: absolute;
    top: 2vh;
    right: 15vw;
    display: inline-block;
}

.logo-icon {
    display: inline-block;
    padding: 5px;
    margin: 15px;
    transition: background-color 0.2s ease-in;
}

#linkedin-img {
    height: 35px;
    width: 35px;
    background: url("../assets/LinkedIn-logo-default.png") no-repeat;
    background-size: 35px;
}

#pinterest-img {
    height: 35px;
    width: 35px;
    background: url("../assets/pinterest-logo-default.png") no-repeat;
    background-size: 35px;
}
#github-img {
    height: 35px;
    width: 35px;
    background: url("../assets/github-logo-default.png") no-repeat;
    background-size: 35px;
}
#twitter-img {
    height: 35px;
    width: 35px;
    background: url("../assets/twitter-logo-default.png") no-repeat;
    background-size: 35px;
}

.logo-icon:hover {
    background-color: white;
}
</style>