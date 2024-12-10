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
                        <li>
                            <span>학습 목차</span>
                            <ul>
                                <li>학습 목차</li>
                                <li>강의 목록</li>
                            </ul>
                        </li>
                        <li>
                            <span>학습 정보</span>
                            <ul>
                                <li>공지사항</li>
                                <li>질의응답</li>
                                <li>자료공유</li>
                                <li>상담게시판</li>
                            </ul>
                        </li>
                        <li>
                            <span>학습 활동</span>
                            <ul>
                                <li>출석</li>
                                <li>과제</li>
                                <li>토론</li>
                                <li>시험</li>
                                <li>설문</li>
                            </ul>
                        </li>
                        <li>
                            <span>확습 현황</span>
                            <ul>
                                <li>학습 현황</li>
                            </ul>
                        </li>
                        <li>
                            <span>과목 정보</span>
                            <ul>
                                <li>평가 계획서</li>
                                <li>강의 계획서</li>
                                <li>과목 정보</li>
                            </ul>
                        </li>
                        <li>
                            <span>성적</span>
                            <ul>
                                <li>성적보기</li>
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
                        <a href="#">홈</a>
                        >
                        <a href="#">강의실</a>
                        >
                        <a href="#">데이터사이언스기초</a>
                        >
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
                                - 학습완료: 각 주차의 학습기간 내에 강의 콘텐츠의 출석인정 기준시간 이상 학습한 경우<br>
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
                                    <span class="statusBar">
                                        <span class="bar"></span>
                                    </span>
                                </th>
                                <th>
                                    1주차
                                    <span>2024-10-05 ~ 2024-10-10</span>
                                </th>
                                <th>
                                    2주차
                                    <span>2024-10-05 ~ 2024-10-10</span>
                                </th>
                                <th>
                                    3주차
                                    <span>2024-10-05 ~ 2024-10-10</span>
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <th class="fisrt">강의영상</th>
                                <td>
                                    <span>
                                        <span>가나다라마바사아자차카타파하</span>
                                        <span class="statusBar end">
                                            <span class="bar"></span>
                                        </span>
                                        <span>교안 다운로드</span>
                                    </span>
                                </td>
                                <td>
                                    <span>
                                        <span>뭘봐?</span>
                                        <span class="statusBar ing">
                                            <span class="bar"></span>
                                        </span>
                                        <span>교안 다운로드</span>
                                    </span>
                                </td>
                                <td>
                                    <span>
                                        <span>널봐</span>
                                        <span class="statusBar fuck">
                                            <span class="bar"></span>
                                        </span>
                                        <span>교안 다운로드</span>
                                    </span>
                                </td>
                            </tr>
                            <tr>
                                <th class="fisrt">공지사항</th>
                                <td></td>
                                <td></td>
                                <td></td>
                            </tr>
                            <tr>
                                <th class="fisrt">질의응답</th>
                                <td></td>
                                <td></td>
                                <td></td>
                            </tr>
                            <tr>
                                <th class="fisrt">과 제</th>
                                <td></td>
                                <td></td>
                                <td></td>
                            </tr>
                            <tr>
                                <th class="fisrt">학습자료실</th>
                                <td></td>
                                <td></td>
                                <td></td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </article>
        </div>
    </section>
</template>