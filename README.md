<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>이력서 - 김은하 (HR 담당)</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Pretendard Font -->
    <link rel="stylesheet" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.9/dist/web/static/pretendard.min.css" />
    
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --sidebar-bg: #1e293b; /* slate-800 */
            --sidebar-text: #f8fafc; /* slate-50 */
            --accent-color: #2563eb; /* blue-600 */
            --text-main: #334155; /* slate-700 */
            --text-light: #64748b; /* slate-500 */
            --bg-body: #f1f5f9; /* slate-100 */
            --bg-card: #ffffff;
            --border-color: #e2e8f0; /* slate-200 */
        }

        body {
            font-family: 'Pretendard', 'Noto Sans KR', sans-serif;
            background-color: var(--bg-body);
            color: var(--text-main);
            line-height: 1.6;
        }

        /* Timeline Styles */
        .timeline-container {
            position: relative;
            border-left: 2px solid var(--border-color);
            margin-left: 0.75rem;
            padding-bottom: 1rem;
        }

        .timeline-item {
            position: relative;
            margin-bottom: 2.5rem;
            margin-left: 1.5rem;
        }

        .timeline-item:last-child {
            margin-bottom: 0;
        }

        .timeline-dot {
            position: absolute;
            left: -29px; /* -1.5rem (margin) - 5px (half of border diff) */
            top: 0.375rem;
            width: 0.875rem;
            height: 0.875rem;
            border-radius: 9999px;
            background-color: var(--accent-color);
            border: 3px solid white;
            box-shadow: 0 0 0 2px var(--border-color);
        }

        /* Tag Styles */
        .tag-badge {
            display: inline-block;
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--sidebar-text);
            padding: 0.35rem 0.75rem;
            border-radius: 9999px;
            font-size: 0.8125rem;
            margin-right: 0.5rem;
            margin-bottom: 0.5rem;
            border: 1px solid rgba(255, 255, 255, 0.15);
            transition: all 0.2s;
        }
        
        .tag-badge:hover {
            background-color: rgba(255, 255, 255, 0.2);
            border-color: rgba(255, 255, 255, 0.3);
        }

        .skill-category {
            color: #94a3b8; /* slate-400 */
            font-size: 0.875rem;
            margin-bottom: 0.5rem;
            margin-top: 1.25rem;
            font-weight: 500;
        }

        /* Print optimization */
        @media print {
            body { background-color: white; }
            .print-shadow-none { box-shadow: none !important; }
            .print-rounded-none { border-radius: 0 !important; }
            aside { background-color: #f8fafc !important; color: #1e293b !important; border-right: 1px solid #e2e8f0; }
            aside .tag-badge { background-color: #e2e8f0 !important; color: #1e293b !important; border: none; }
            aside .skill-category { color: #64748b !important; }
            aside .text-slate-200, aside .text-slate-300, aside .text-slate-400 { color: #475569 !important; }
            .timeline-dot { box-shadow: none; border-color: #e2e8f0; }
        }
    </style>
</head>
<body class="py-10 px-4 sm:px-6 lg:px-8 print:py-0 print:px-0">

    <div class="max-w-[1100px] mx-auto bg-[var(--bg-card)] shadow-2xl rounded-2xl overflow-hidden flex flex-col lg:flex-row print:shadow-none print:rounded-none">
        
        <!-- ================= LEFT SIDEBAR ================= -->
        <aside class="w-full lg:w-[340px] bg-[var(--sidebar-bg)] text-[var(--sidebar-text)] p-8 md:p-10 flex flex-col shrink-0">
            
            <div class="flex justify-center mb-8">
                <div class="w-48 h-48 md:w-56 md:h-56 rounded-full overflow-hidden border-4 border-slate-600 shadow-xl relative bg-slate-700 flex-shrink-0">
                    <!-- 웹에서 정상 출력되는 이미지 URL 적용 -->
                    <img src="https://mail.google.com/mail/u/0?ui=2&ik=0a74396729&attid=0.1&permmsgid=msg-a:r-554721291308048536&th=1a0bd007e3ee8172&view=fimg&fur=ip&permmsgid=msg-a:r-554721291308048536&sz=s0-l75-ft&attbid=ANGjdJ_3ucjAlUi7oumOeaOdRHECNSHX3_iyShVzwALRSzFicwpKQD0hTX4M_LodoLJVJOC47qdeDCN4VYG2yWOIzkDxJzKbhQunJQM0Prd_kCt3VQ9XVU6APu0KKmc&disp=emb&realattid=ii_mu9aqp310&zw" alt="김은하 프로필" class="w-full h-full object-cover">
                </div>
            </div>

            <div class="mb-10">
                <h2 class="text-lg font-bold border-b border-slate-600 pb-2 mb-4 tracking-widest text-slate-300 uppercase">Contact</h2>
                <ul class="space-y-4">
                    <li class="flex items-center">
                        <div class="w-8 h-8 rounded-full bg-slate-700/50 flex items-center justify-center mr-3 text-blue-400">
                            <i class="fas fa-phone"></i>
                        </div>
                        <span class="text-slate-200 text-sm font-medium">010-8311-0510</span>
                    </li>
                    <li class="flex items-center">
                        <div class="w-8 h-8 rounded-full bg-slate-700/50 flex items-center justify-center mr-3 text-blue-400">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <span class="text-slate-200 text-sm font-medium">ii4z6ii@naver.com</span>
                    </li>
                    <li class="flex items-center">
                        <div class="w-8 h-8 rounded-full bg-slate-700/50 flex items-center justify-center mr-3 text-blue-400">
                            <i class="fas fa-user"></i>
                        </div>
                        <span class="text-slate-200 text-sm font-medium">여성 · 1993년생</span>
                    </li>
                </ul>
            </div>

            <div class="mb-10">
                <h2 class="text-lg font-bold border-b border-slate-600 pb-2 mb-4 tracking-widest text-slate-300 uppercase">Education</h2>
                <div>
                    <h3 class="font-semibold text-white text-base">전북대학교</h3>
                    <p class="text-slate-300 text-sm mt-1">화학 학사</p>
                    <p class="text-slate-400 text-xs mt-1">2011 ~ 2016</p>
                </div>
            </div>

            <div class="mb-6 flex-grow">
                <h2 class="text-lg font-bold border-b border-slate-600 pb-2 mb-4 tracking-widest text-slate-300 uppercase">Skills</h2>
                
                <div class="skill-category"><i class="fas fa-toolbox mr-2"></i>HR Tools</div>
                <div class="flex flex-wrap mb-2">
                    <span class="tag-badge">나인하이어</span>
                    <span class="tag-badge">레몬베이스</span>
                    <span class="tag-badge">에버타임</span>
                    <span class="tag-badge">영림원ERP</span>
                    <span class="tag-badge">위하고</span>
                    <span class="tag-badge">네이버웍스</span>
                    <span class="tag-badge">슬랙</span>
                    <span class="tag-badge">노션</span>
                    <span class="tag-badge">flex</span>
                </div>

                <div class="skill-category"><i class="fas fa-star mr-2"></i>Expertise</div>
                <div class="flex flex-wrap mb-2">
                    <span class="tag-badge">HRM</span>
                    <span class="tag-badge">인사기획</span>
                    <span class="tag-badge">인사평가</span>
                    <span class="tag-badge">노무·노사관리</span>
                    <span class="tag-badge">조직문화</span>
                    <span class="tag-badge">성과관리</span>
                </div>

                <div class="skill-category"><i class="fas fa-language mr-2"></i>Languages</div>
                <div class="flex flex-wrap mb-2">
                    <span class="tag-badge">영어 (업무상 소통 가능)</span>
                </div>

                <div class="skill-category"><i class="fas fa-certificate mr-2"></i>Certificates</div>
                <div class="flex flex-wrap">
                    <span class="tag-badge">운전면허 2종보통</span>
                    <span class="tag-badge">영사기능사</span>
                </div>
            </div>
        </aside>

        <!-- ================= RIGHT MAIN CONTENT ================= -->
        <main class="w-full p-8 md:p-12 lg:p-14 bg-white">
            
            <!-- Header -->
            <header class="mb-12">
                <h1 class="text-5xl font-extrabold text-slate-800 mb-3 tracking-tight">김은하</h1>
                <h2 class="text-2xl font-semibold text-blue-600">HR 담당 <span class="text-lg text-slate-500 font-normal ml-1 border-l border-slate-300 pl-2">과장급 지원</span></h2>
            </header>

            <!-- About Me -->
            <section class="mb-14">
                <h3 class="text-2xl font-bold text-slate-800 border-b-2 border-slate-100 pb-3 mb-5 flex items-center">
                    <i class="fas fa-user-circle text-slate-300 mr-3 text-xl"></i> 자기소개
                </h3>
                <div class="text-slate-600 space-y-4 leading-relaxed text-[15px] font-medium break-keep">
                    <p>
                        남유에프엔씨는 아이보들 CCP크림 누적 판매 68만 개, 올리브영 입점 6개월 만의 정규 POG 확정, 2025년 올리브영 매출 전년 대비 160% 성장과 판매 랭킹 1위라는 성과를 자사몰 중심의 D2C 사업 구조 위에서 만들어낸 조직입니다. 브랜드와 매출이 함께 빠르게 확장되는 동안 그 성장을 뒷받침할 HR 체계를 지금 만들어가는 단계라는 점에 매력을 느껴 지원을 결심했습니다.
                    </p>
                    <p>
                        채용부터 HRM, Payroll, 평가·보상, 조직문화까지 HR 전 영역을 직접 운영해 온 경험이 이 포지션과 맞닿아 있다고 생각합니다. 2023년 입사자 94명 전원의 채용을 리드했고, 이후에는 조직이 83명에서 270명 이상으로 성장하는 동안 HRM 체계와 근로감독 대응을 단독으로 맡아 법적 이슈 없이 조직을 운영했습니다. 급여 테이블을 직접 설계해 지금까지 관리하고 있고, 근태툴과 ATS를 전환하며 제도를 정비한 경험도 있어 성장 단계에서 필요한 HR 실무와 체계화를 함께 다뤄본 것이 강점이라 생각합니다.
                    </p>
                    <p>
                        공고에서 말씀하신 것처럼 입사 초기에는 기존 HR 담당자와 업무를 파악하고, 이후 담당 영역을 나누어 독립적으로 운영하는 방식에도 잘 맞을 것이라 생각합니다. 지금까지 채용, HRM, 평가·보상 전반을 스스로 기획하고 운영해 온 만큼, 남유에프엔씨의 성장 속도에 맞는 HR 담당자로서 빠르게 기여하고 싶습니다.
                    </p>
                </div>
            </section>

            <!-- Core Competencies -->
            <section class="mb-14">
                <h3 class="text-2xl font-bold text-slate-800 border-b-2 border-slate-100 pb-3 mb-6 flex items-center">
                    <i class="fas fa-gem text-blue-500 mr-3 text-xl"></i> 핵심역량
                </h3>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-5">
                    
                    <!-- Card 1 -->
                    <div class="bg-white rounded-xl p-6 border border-slate-200 shadow-[0_4px_20px_-4px_rgba(0,0,0,0.05)] hover:shadow-[0_8px_30px_-4px_rgba(0,0,0,0.1)] hover:-translate-y-1 transition-all duration-300">
                        <div class="w-12 h-12 rounded-lg bg-blue-50 text-blue-600 flex items-center justify-center mb-5">
                            <i class="fas fa-users-cog text-xl"></i>
                        </div>
                        <h4 class="font-bold text-lg mb-3 text-slate-800 break-keep">HR 제너럴리스트 운영력</h4>
                        <p class="text-sm text-slate-600 leading-relaxed break-keep">
                            채용, HRM·노무, Payroll, 평가·보상, 조직문화까지 HR 전 영역을 4년간 직접 수행
                        </p>
                    </div>

                    <!-- Card 2 -->
                    <div class="bg-white rounded-xl p-6 border border-slate-200 shadow-[0_4px_20px_-4px_rgba(0,0,0,0.05)] hover:shadow-[0_8px_30px_-4px_rgba(0,0,0,0.1)] hover:-translate-y-1 transition-all duration-300">
                        <div class="w-12 h-12 rounded-lg bg-indigo-50 text-indigo-600 flex items-center justify-center mb-5">
                            <i class="fas fa-chart-line text-xl"></i>
                        </div>
                        <h4 class="font-bold text-lg mb-3 text-slate-800 break-keep">급성장 조직의 HR 체계화</h4>
                        <p class="text-sm text-slate-600 leading-relaxed break-keep">
                            조직이 83명에서 270명 이상으로 성장하는 동안 규정과 프로세스를 정비하고 근로감독 대응을 단독 수행해 법적 이슈 0건 유지
                        </p>
                    </div>

                    <!-- Card 3 -->
                    <div class="bg-white rounded-xl p-6 border border-slate-200 shadow-[0_4px_20px_-4px_rgba(0,0,0,0.05)] hover:shadow-[0_8px_30px_-4px_rgba(0,0,0,0.1)] hover:-translate-y-1 transition-all duration-300">
                        <div class="w-12 h-12 rounded-lg bg-emerald-50 text-emerald-600 flex items-center justify-center mb-5">
                            <i class="fas fa-coins text-xl"></i>
                        </div>
                        <h4 class="font-bold text-lg mb-3 text-slate-800 break-keep">제도 개선과 비용 효율화 주도</h4>
                        <p class="text-sm text-slate-600 leading-relaxed break-keep">
                            급여 테이블 설계·관리, 근태툴 전환으로 월 이용료 약 44% 절감(73만원→41만원), ATS·ERP 도입 리드
                        </p>
                    </div>

                </div>
            </section>

            <!-- Experience -->
            <section>
                <div class="flex items-center justify-between border-b-2 border-slate-100 pb-3 mb-8">
                    <h3 class="text-2xl font-bold text-slate-800 flex items-center">
                        <i class="fas fa-briefcase text-slate-400 mr-3 text-xl"></i> 경력
                    </h3>
                    <span class="text-sm font-bold text-blue-600 bg-blue-50 px-3 py-1 rounded-full border border-blue-100">총 9년 5개월</span>
                </div>
                
                <div class="timeline-container">
                    
                    <!-- Job 1 -->
                    <div class="timeline-item">
                        <div class="timeline-dot"></div>
                        <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-3">
                            <div>
                                <h4 class="text-xl font-bold text-slate-900">OLIVE INTERNATIONAL</h4>
                                <p class="text-blue-600 font-semibold mt-1">성장지원본부 피플팀 · HRM 담당</p>
                            </div>
                            <div class="mt-2 md:mt-0 md:text-right">
                                <span class="inline-block bg-slate-100 text-slate-700 text-sm font-semibold px-3 py-1 rounded-md border border-slate-200">2022.12 ~ 재직 중 <span class="font-normal text-slate-500">(3년 9개월)</span></span>
                            </div>
                        </div>
                        
                        <div class="mt-5 space-y-5 text-[15px] text-slate-700 bg-slate-50 p-5 rounded-xl border border-slate-100">
                            <div>
                                <strong class="text-slate-900 flex items-center mb-2"><i class="fas fa-check text-blue-500 mr-2 text-xs"></i>채용 <span class="text-slate-500 text-sm font-normal ml-2">(2022.12 ~ 2023.10)</span></strong>
                                <ul class="list-disc list-outside ml-6 space-y-1.5 text-slate-600 break-keep">
                                    <li>채용 전 과정을 직접 리드, 2023년 입사자 94명 전원 채용 완료 (마케터 직군 중심)</li>
                                    <li>이력서 스크리닝, 다이렉트 소싱, 서치펌 관리와 최종 처우협의 전담</li>
                                    <li>ATS(나인하이어) 도입과 채용 홈페이지 제작을 주도해 채용 프로세스를 체계화</li>
                                    <li>2023.10 이후 HRM과 평가·보상으로 담당 영역을 옮겨 현재까지 운영</li>
                                </ul>
                            </div>
                            <div>
                                <strong class="text-slate-900 flex items-center mb-2"><i class="fas fa-check text-blue-500 mr-2 text-xs"></i>HRM · 노무</strong>
                                <ul class="list-disc list-outside ml-6 space-y-1.5 text-slate-600 break-keep">
                                    <li>근로감독 대응 서류 준비부터 노무법인 협의, 취업규칙 수정신고, 감독관 응대까지 전 과정을 단독 수행해 법적 이슈 0건으로 종결</li>
                                    <li>인사 규정 기획, 제정, 가이드 작성과 운영을 주도, 조직도와 재직자 현황 관리</li>
                                    <li>근로계약서 등 각종 계약서, 입퇴사 서류 관리, 퇴직 프로세스 기획과 운영, 외국인 근로자 10명 이상 비자와 체류기간 관리</li>
                                    <li>재직 인원 83명(2022.12)에서 270명 이상(2026.09)으로 조직이 성장하는 동안 HRM 체계 운영, 정부지원금 신청과 관리</li>
                                    <li>근태 관리(에버타임), 연차·초과근로 수당 관리, 근태 규정 제정</li>
                                </ul>
                            </div>
                            <div>
                                <strong class="text-slate-900 flex items-center mb-2"><i class="fas fa-check text-blue-500 mr-2 text-xs"></i>Payroll</strong>
                                <ul class="list-disc list-outside ml-6 space-y-1.5 text-slate-600 break-keep">
                                    <li>아웃소싱 업체(HRM+)와 연계해 신규입사자, 퇴사자, 무급휴가, 초과근무 내역 전달과 자료 검증, 마감, 입금 신청까지 담당</li>
                                    <li>월 급여 대상 인원이 290명(2026.08 기준)으로 늘어나는 동안 지속 운영, 퇴직연금 관리와 지급, 연말정산 진행(아웃소싱 협업)</li>
                                </ul>
                            </div>
                            <div>
                                <strong class="text-slate-900 flex items-center mb-2"><i class="fas fa-check text-blue-500 mr-2 text-xs"></i>평가 · 보상</strong>
                                <ul class="list-disc list-outside ml-6 space-y-1.5 text-slate-600 break-keep">
                                    <li>급여 테이블을 직접 설계해 현재까지 관리, 연봉계약서 작성과 성과급 지급, 급여 반영 진행</li>
                                    <li>분기 평가 대상 86명(2023.12~2024.02)에 대해 평가 항목 배포, 자료 전달, 결과 산출 진행</li>
                                    <li>레몬베이스 도입을 주도해 분기별 평가 체계를 신설</li>
                                </ul>
                            </div>
                            <div>
                                <strong class="text-slate-900 flex items-center mb-2"><i class="fas fa-check text-blue-500 mr-2 text-xs"></i>조직문화</strong>
                                <ul class="list-disc list-outside ml-6 space-y-1.5 text-slate-600 break-keep">
                                    <li>워크샵, 송년회 등 사내 행사 기획과 운영을 주도, 직접 기획한 행사는 100~200명 규모로 재직자 전체 참여</li>
                                    <li>타사 30곳 복리후생 사례를 조사·비교해 스낵바, 난임휴가 등 복지 제도를 제안, 검토 기반 마련, 노션 홈 화면 리뉴얼로 사내 정보 가독성 개선</li>
                                </ul>
                            </div>
                            <div>
                                <strong class="text-slate-900 flex items-center mb-2"><i class="fas fa-check text-blue-500 mr-2 text-xs"></i>HR 제도 · 프로세스 개선</strong>
                                <ul class="list-disc list-outside ml-6 space-y-1.5 text-slate-600 break-keep">
                                    <li>근태툴을 위하고에서 에버타임으로 전환 주도, 120명 기준 월 이용료 73만원에서 41만원으로 절감</li>
                                    <li>ERP(영림원) 도입 시 인사 기본 셋팅, 조직도, 사원명부, 급여 셋팅 담당</li>
                                    <li>ATS 나인하이어 도입, 비교 견적으로 조건을 협상해 채용 프로세스 효율화</li>
                                    <li>현재 HRIS (flex) 도입 셋팅 진행중</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <!-- Job 2 -->
                    <div class="timeline-item">
                        <div class="timeline-dot bg-slate-400 border-white"></div>
                        <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-2">
                            <div>
                                <h4 class="text-lg font-bold text-slate-800">(주)워시스왓</h4>
                                <p class="text-slate-600 font-medium mt-1">TA · 피플팀</p>
                            </div>
                            <div class="mt-2 md:mt-0 md:text-right">
                                <span class="inline-block bg-slate-50 text-slate-600 text-sm font-medium px-3 py-1 rounded-md border border-slate-200">2022.09 ~ 2022.12 <span class="text-slate-400">(4개월)</span></span>
                            </div>
                        </div>
                        <div class="mt-3 text-[15px] text-slate-600 pl-2">
                            <ul class="list-disc list-outside ml-4 space-y-1 break-keep">
                                <li>그리팅 기반 채용 전 과정 수행과 채용 홈페이지 기획, 사내 문화행사와 타운홀 운영 지원</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Job 3 -->
                    <div class="timeline-item">
                        <div class="timeline-dot bg-slate-400 border-white"></div>
                        <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-2">
                            <div>
                                <h4 class="text-lg font-bold text-slate-800">(주)맨파워그룹코리아</h4>
                                <p class="text-slate-600 font-medium mt-1">대리 · 스태핑솔루션</p>
                            </div>
                            <div class="mt-2 md:mt-0 md:text-right">
                                <span class="inline-block bg-slate-50 text-slate-600 text-sm font-medium px-3 py-1 rounded-md border border-slate-200">2021.08 ~ 2022.09 <span class="text-slate-400">(1년 2개월)</span></span>
                            </div>
                        </div>
                        <div class="mt-3 text-[15px] text-slate-600 pl-2">
                            <ul class="list-disc list-outside ml-4 space-y-1 break-keep">
                                <li>파견직과 정규직 채용, 다이렉트 소싱, 도급 4개처 운영과 관리, 인보이스 작성과 청구</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Job 4 -->
                    <div class="timeline-item">
                        <div class="timeline-dot bg-slate-400 border-white"></div>
                        <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-2">
                            <div>
                                <h4 class="text-lg font-bold text-slate-800">메가박스중앙(주)</h4>
                                <p class="text-slate-600 font-medium mt-1">대리 · 운영본부</p>
                            </div>
                            <div class="mt-2 md:mt-0 md:text-right">
                                <span class="inline-block bg-slate-50 text-slate-600 text-sm font-medium px-3 py-1 rounded-md border border-slate-200">2017.04 ~ 2021.08 <span class="text-slate-400">(4년 5개월)</span></span>
                            </div>
                        </div>
                        <div class="mt-3 text-[15px] text-slate-600 pl-2">
                            <ul class="list-disc list-outside ml-4 space-y-1 break-keep">
                                <li>크루 채용, 근태·급여·복리후생 관리, 인건비 예산 집계와 보고, 법정교육 운영</li>
                            </ul>
                        </div>
                    </div>

                </div>
            </section>
        </main>
    </div>

</body>
</html>
