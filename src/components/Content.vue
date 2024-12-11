<template>
    <section id="content">
        <div class="inner">
            <article class="menuContainer">
                <select name="" id="">
                    <option value="" selected>데이터사이언스기초</option>
                    <option value="">자바스크립트</option>
                    <option value="">컴퓨터구조</option>
                    <option value="">파이썬프로그래밍</option>
                </select>
                <div class="bar"></div>
                <div class="list">
                    <ul>
                        <li v-for="(menu, index) in menuItems" :key="index">
                            <span>{{ menu.title }}</span>
                            <ul>
                                <li v-for="(item, idx) in menu.items" :key="idx">{{ item }}</li>
                            </ul>
                        </li>
                    </ul>
                </div>
                <div class="bar"></div>
                <div class="dailyBtn">내 할일보기</div>
            </article>
    
            <article class="contentBox">
                <div class="title">
                    <span>
                        <a href="#">홈</a> >
                        <a href="#">강의실</a> >
                        <a href="#">데이터사이언스기초</a> >
                        <a href="#">학습 목차</a>
                    </span>
                </div>

                <div class="contentTab">
                    <span>
                        <span class="select">학습 목차</span>
                        <span>강의 목록</span>
                    </span>
                </div>

                <div class="content">
                    <div class="expl">
                    <span>
                        <span>온라인 학습현황</span>
                        <span>
                            - 학습완료: 각 주차의 학습기간 내에 강의 콘텐츠의 출석인정 기준시간 이상 학습한 경우<br />
                            - 학습중/학습안함: 학습해야 할 강의 콘텐츠의 출석인정 기준시간 만큼 학습을 완료하지 못한 경우로 결석 처리
                        </span>
                    </span>
                    <span>
                        <span>온라인</span>
                        <span>
                            <span class="end"></span> 학습완료
                            <span class="ing"></span> 학습중
                            <span class="fuck"></span> 학습안함
                        </span>
                    </span>
                    </div>
                </div>

                <div class="table">
                    <table>
                        <thead>
                            <tr>
                                <th class="fisrt">
                                    온라인 출석률
                                    <span class="statusBar"><span class="bar"></span></span>
                                </th>
                                <th v-for="(week, index) in weekData" :key="index">
                                    {{ week.week }}
                                    <span>{{ week.date }}</span>
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <th class="fisrt">강의영상</th>
                                <td v-for="(week, index) in weekData" :key="index">
                                    <span>
                                        <span>{{ week.content }}</span>
                                        <span :class="`statusBar ${week.status}`">
                                            <span class="bar"></span>
                                        </span>
                                        <span>교안 다운로드</span>
                                    </span>
                                </td>
                            </tr>
                            <tr v-for="(row, idx) in ['공지사항', '질의응답', '과 제', '학습자료실']" :key="idx">
                                <th class="fisrt">{{ row }}</th>
                                <td v-for="week in weekData" :key="week.week"></td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </article>
        </div>
    </section>
</template>

<script setup>

const menuItems = [
    {
        title: "학습 목차",
        items: ["학습 목차", "강의 목록"],
    },
    {
        title: "학습 정보",
        items: ["공지사항", "질의응답", "자료공유", "상담게시판"],
    },
    {
        title: "학습 활동",
        items: ["출석", "과제", "토론", "시험", "설문"],
    },
    {
        title: "확습 현황",
        items: ["학습 현황"],
    },
    {
        title: "과목 정보",
        items: ["평가 계획서", "강의 계획서", "과목 정보"],
    },
    {
        title: "성적",
        items: ["성적보기"],
    },
];

const weekData = [
    { week: "1주차", date: "2024-10-05 ~ 2024-10-10", status: "end", content: "강의 1주차 내용" },
    { week: "2주차", date: "2024-10-05 ~ 2024-10-10", status: "ing", content: "강의 2주차 내용" },
    { week: "3주차", date: "2024-10-05 ~ 2024-10-10", status: "fuck", content: "강의 3주차 내용" },
];

</script>
