<template>
    <section id="banner" ref="bannerContainer" :class="{ close: isClosed }">
        <article class="inner">
            <h1>
                <span>{{ classInfo.grade }} {{ classInfo.class }}</span>
                <span>{{ classInfo.subject }}</span>
            </h1>
            <div class="content">
                <div class="tInfo">
                    <span>
                        <span>이수구분 <span>{{ classInfo.category }}</span></span>
                        <span>학점 <span>{{ classInfo.credit }}</span></span>
                        <span>공동교수정보 <span class="btn">조회하기</span></span>
                    </span>
                </div>
                <div class="tInfo">
                    <span>
                        <span>대표교수 <span>{{ classInfo.professor }}</span></span>
                        <span>이메일 <span>{{ classInfo.email }}</span></span>
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

<script setup>

import { ref } from "vue";

const classInfo = {
    grade: "1학년",
    class: "B반",
    subject: "데이터사이언스기초",
    category: "교양학과",
    credit: "2학점",
    professor: "이X땡",
    email: "bibibi@inhatc.ac.kr",
};

const isClosed = ref(false);

const bannerToggle = () => {
    isClosed.value = !isClosed.value;
};

</script>