<template>
    <section id="banner" ref="bannerContainer">
        <article class="inner">
            <h1>
                <span>1학년 B반</span>
                <span>데이터사이언스기초</span>
            </h1>
            <div class="content">
                <div class="tInfo">
                    <span>
                    <span>이수구분 <span>교양학과</span></span>
                    <span>학점 <span>2학점</span></span>
                    <span>공동교수정보 <span class="btn">조회하기</span></span>
                    </span>
                </div>
                <div class="tInfo">
                    <span>
                    <span>대표교수 <span>이X땡</span></span>
                    <span>이메일 <span>bibibi@inhatc.ac.kr</span></span>
                    </span>
                </div>
            </div>
            <div class="blur"></div>
            <div class="arrow" @click="bannerToggle">
                <i class="fa-solid fa-chevron-up"></i>
            </div>
        </article>
    </section>
</template>

<script>

export default {
    methods: {
        bannerToggle() {
            const bannerContainer = this.$refs.bannerContainer;
            bannerContainer.classList.toggle("close");
        }
    }
}

</script>