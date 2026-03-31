<!DOCTYPE html>
<html class="light" lang="ko">
<head>
    <meta charset="utf-8"/>
    <meta content="width=device-width, initial-scale=1.0" name="viewport"/>
    <title>Vitality Dashboard - Mobile View</title>
    <script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700;800&amp;family=Inter:wght@400;500;600&amp;display=swap" rel="stylesheet"/>
    <link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
    <script id="tailwind-config">
        tailwind.config = {
            darkMode: "class",
            theme: {
                extend: {
                    colors: {
                        "on-primary-fixed": "#000000",
                        "inverse-primary": "#618bff",
                        "on-surface-variant": "#555881",
                        "on-tertiary": "#ffefef",
                        "on-error-container": "#570008",
                        "on-tertiary-fixed": "#39000d",
                        "on-secondary-fixed": "#004a22",
                        "surface-variant": "#d9daff",
                        "inverse-on-surface": "#9799c6",
                        "tertiary-fixed": "#ff909d",
                        "surface-container": "#e7e6ff",
                        "error-dim": "#9f0519",
                        "surface-tint": "#0050d4",
                        "on-secondary-container": "#005f2e",
                        "secondary-dim": "#005c2c",
                        "outline-variant": "#a7aad7",
                        "primary-fixed-dim": "#658eff",
                        "on-surface": "#282b51",
                        "inverse-surface": "#06092f",
                        "secondary-fixed-dim": "#5def8f",
                        "surface-container-highest": "#d9daff",
                        "surface-bright": "#f8f5ff",
                        "secondary": "#006a34",
                        "on-tertiary-fixed-variant": "#760726",
                        "on-error": "#ffefee",
                        "error": "#b31b25",
                        "secondary-container": "#6dfe9c",
                        "on-background": "#282b51",
                        "tertiary": "#a53046",
                        "on-secondary": "#cdffd4",
                        "surface-container-high": "#e0e0ff",
                        "on-primary-fixed-variant": "#00266e",
                        "primary-container": "#7b9cff",
                        "background": "#f8f5ff",
                        "on-primary": "#f1f2ff",
                        "surface-dim": "#cfd1ff",
                        "primary": "#2563EB",
                        "tertiary-container": "#ff909d",
                        "on-primary-container": "#001e5a",
                        "surface": "#f8f5ff",
                        "outline": "#71749e",
                        "error-container": "#fb5151",
                        "on-tertiary-container": "#67001f",
                        "secondary-fixed": "#6dfe9c",
                        "tertiary-fixed-dim": "#ff788b",
                        "tertiary-dim": "#95233b",
                        "on-secondary-fixed-variant": "#006a34",
                        "primary-dim": "#1e40af",
                        "surface-container-low": "#f1efff",
                        "surface-container-lowest": "#ffffff",
                        "primary-fixed": "#7b9cff"
                    },
                    fontFamily: {
                        "headline": ["Plus Jakarta Sans"],
                        "body": ["Inter"],
                        "label": ["Inter"]
                    },
                    borderRadius: {"DEFAULT": "1rem", "lg": "2rem", "xl": "3rem", "full": "9999px"},
                },
            },
        }
    </script>
    <style>
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
        }
        body {
            font-family: 'Plus Jakarta Sans', 'Inter', sans-serif;
            background-color: #e5e7eb; /* 바깥 배경색 */
        }
        /* 스크롤바 숨기기 */
        .hide-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .hide-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
        /* 모바일 프레임 내부 스크롤 허용 */
        .mobile-container {
            max-width: 430px;
            margin: 0 auto;
            background-color: #f8f5ff;
            min-height: 100vh;
            position: relative;
            box-shadow: 0 0 50px rgba(0,0,0,0.1);
            overflow-x: hidden;
        }
    </style>
</head>
<body class="text-on-surface">

    <!-- Mobile Wrapper -->
    <div class="mobile-container flex flex-col">
        
        <!-- TopAppBar (Sticky to the container) -->
        <header class="sticky top-0 w-full z-50 bg-[#f8f5ff]/80 backdrop-blur-xl flex justify-between items-center px-6 py-4">
            <div class="flex items-center gap-3">
                <div class="w-10 h-10 rounded-full bg-primary-container flex items-center justify-center overflow-hidden">
                    <img alt="사용자 프로필" class="w-full h-full object-cover" src="https://lh3.googleusercontent.com/aida-public/AB6AXuBvlQfPw-xCcCAFccE9JV2avydtXlFe8gxS8wkZ_j-LxEnnHnHAieWE38eoss-MHqjgN4BQ1swUKK58jTYHhbbE0xLO57tdHArUFEaPNXT4QF4xQtWd12xlUkPxHoiZFALwA9COHVGp8YbpVX1X_ztlJcaSV_vbxUKjL1P_3RrLc8Olx56838gNezqjDUFW3xOAPnZAK0OafYWP2jOpiD5LLEAgXG6L_L_n5njyoj_Qx9TCY0f3qOvMd9f8kLyx7Q6bDNKhY5GxrX4"/>
                </div>
                <h1 class="text-2xl font-extrabold tracking-tighter text-primary font-headline">Vitality</h1>
            </div>
            <button class="w-10 h-10 flex items-center justify-center text-on-surface-variant hover:opacity-80 transition-opacity active:scale-95 duration-200">
                <span class="material-symbols-outlined" data-icon="notifications">notifications</span>
            </button>
        </header>

        <main class="flex-grow pt-4 pb-20 px-6">
            <!-- Morning Greeting & Quote Section -->
            <section class="mb-10">
                <h2 class="text-[2rem] font-headline font-extrabold leading-tight tracking-tight mb-2">안녕하세요, 민수님.</h2>
                <div class="p-6 bg-surface-container-low rounded-lg border-l-4 border-primary">
                    <p class="italic text-on-surface-variant font-body text-md leading-relaxed">
                        "시작하는 비결은 바로 시작하는 것이다."
                    </p>
                    <span class="block mt-2 font-label text-[0.7rem] uppercase tracking-[0.05em] font-semibold text-primary">— 마크 트웨인</span>
                </div>
            </section>

            <!-- Today's Lectures -->
            <section class="mb-10">
                <div class="flex justify-between items-end mb-6">
                    <h3 class="text-lg font-headline font-bold text-on-surface">오늘의 강의</h3>
                    <span class="font-label text-[0.7rem] uppercase tracking-[0.05em] font-semibold text-primary">전체 일정</span>
                </div>
                <div class="flex gap-4 overflow-x-auto hide-scrollbar pb-4 -mx-6 px-6">
                    <!-- Card 1 -->
                    <div class="min-w-[240px] p-5 bg-surface-container-lowest rounded-lg shadow-[0_12px_32px_rgba(40,43,81,0.04)] flex flex-col justify-between border border-outline-variant/20">
                        <div>
                            <div class="flex justify-between items-start mb-4">
                                <span class="px-2 py-1 bg-secondary-container text-on-secondary-container rounded-full font-label text-[0.6rem] font-bold uppercase tracking-wider">진행 중</span>
                                <span class="material-symbols-outlined text-primary text-xl" data-icon="school">school</span>
                            </div>
                            <h4 class="text-lg font-headline font-bold mb-1">고급 미적분학</h4>
                            <p class="text-on-surface-variant font-body text-xs mb-4">A홀 • 피터슨 박사</p>
                        </div>
                        <div class="flex items-center gap-2 text-primary font-semibold">
                            <span class="material-symbols-outlined text-sm" data-icon="schedule">schedule</span>
                            <span class="text-xs">09:00 - 10:30 AM</span>
                        </div>
                    </div>
                    <!-- Card 2 -->
                    <div class="min-w-[240px] p-5 bg-surface-container-low rounded-lg flex flex-col justify-between border-2 border-transparent hover:border-primary/10 transition-colors">
                        <div>
                            <div class="flex justify-between items-start mb-4">
                                <span class="px-2 py-1 bg-surface-container-highest text-on-surface-variant rounded-full font-label text-[0.6rem] font-bold uppercase tracking-wider">다음 강의</span>
                                <span class="material-symbols-outlined text-on-surface-variant text-xl" data-icon="biotech">biotech</span>
                            </div>
                            <h4 class="text-lg font-headline font-bold mb-1">유기 화학</h4>
                            <p class="text-on-surface-variant font-body text-xs mb-4">402호 • 밀러 교수</p>
                        </div>
                        <div class="flex items-center gap-2 text-on-surface-variant font-semibold">
                            <span class="material-symbols-outlined text-sm" data-icon="schedule">schedule</span>
                            <span class="text-xs">11:00 - 12:30 PM</span>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Bento Grid: Assignments & Progress -->
            <div class="flex flex-col gap-8">
                <!-- Today's To-do Checklist -->
                <section>
                    <div class="flex justify-between items-center mb-6">
                        <h3 class="text-lg font-headline font-bold text-on-surface">오늘의 할 일</h3>
                        <span class="material-symbols-outlined text-on-surface-variant cursor-pointer" data-icon="filter_list">filter_list</span>
                    </div>
                    <div class="space-y-4">
                        <!-- Task Item 1 -->
                        <div class="p-5 bg-surface-container-lowest rounded-lg shadow-[0_4px_20px_rgba(40,43,81,0.02)] flex items-center justify-between group border border-outline-variant/10">
                            <div class="flex items-center gap-4">
                                <div class="w-6 h-6 rounded-full border-2 border-primary flex items-center justify-center cursor-pointer transition-colors hover:bg-primary/5">
                                    <span class="material-symbols-outlined text-primary text-sm hidden" data-icon="check">check</span>
                                </div>
                                <div>
                                    <h4 class="text-sm font-bold text-on-surface">물리 문제집 #4 제출</h4>
                                    <p class="text-[12px] text-on-surface-variant font-medium">열역학 및 유체</p>
                                </div>
                            </div>
                            <div class="text-right">
                                <p class="text-[12px] font-bold text-tertiary uppercase tracking-wider">4시간</p>
                                <p class="text-[9px] font-label text-on-surface-variant uppercase tracking-widest font-bold">남음</p>
                            </div>
                        </div>
                        <!-- Task Item 2 -->
                        <div class="p-5 bg-surface-container-lowest rounded-lg shadow-[0_4px_20px_rgba(40,43,81,0.02)] flex items-center justify-between group border border-outline-variant/10">
                            <div class="flex items-center gap-4">
                                <div class="w-6 h-6 rounded-full border-2 border-outline flex items-center justify-center cursor-pointer hover:border-primary transition-colors"></div>
                                <div>
                                    <h4 class="text-sm font-bold text-on-surface">자료구조 실습</h4>
                                    <p class="text-[12px] text-on-surface-variant font-medium">힙 구현</p>
                                </div>
                            </div>
                            <div class="text-right">
                                <p class="text-[12px] font-bold text-on-surface-variant uppercase tracking-wider">2일</p>
                                <p class="text-[9px] font-label text-on-surface-variant uppercase tracking-widest font-bold">남음</p>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- Progress Section -->
                <section class="flex flex-col gap-6">
                    <h3 class="text-lg font-headline font-bold text-on-surface">진행 상황</h3>
                    <div class="p-6 bg-surface-container-high rounded-lg flex flex-col justify-between shadow-sm">
                        <h4 class="text-md font-headline font-bold mb-4">개인 목표</h4>
                        <div class="space-y-6">
                            <div>
                                <div class="flex justify-between items-center mb-2">
                                    <span class="text-xs font-semibold">독서 챌린지</span>
                                    <span class="text-xs font-bold text-primary">72%</span>
                                </div>
                                <div class="w-full h-2.5 bg-surface-container-highest rounded-full overflow-hidden">
                                    <div class="h-full bg-gradient-to-r from-primary to-primary-container rounded-full" style="width: 72%"></div>
                                </div>
                            </div>
                            <div>
                                <div class="flex justify-between items-center mb-2">
                                    <span class="text-xs font-semibold">코딩 프로젝트</span>
                                    <span class="text-xs font-bold text-secondary">45%</span>
                                </div>
                                <div class="w-full h-2.5 bg-surface-container-highest rounded-full overflow-hidden">
                                    <div class="h-full bg-gradient-to-r from-secondary to-secondary-fixed rounded-full" style="width: 45%"></div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- Daily Stat Card -->
                    <div class="p-6 bg-primary rounded-lg text-on-primary shadow-xl shadow-primary/20 flex items-center gap-4">
                        <div class="w-12 h-12 rounded-full bg-white/20 flex items-center justify-center">
                            <span class="material-symbols-outlined" data-icon="bolt">bolt</span>
                        </div>
                        <div>
                            <p class="text-xl font-bold">12일째</p>
                            <p class="text-[10px] font-label uppercase tracking-widest opacity-80">학습 스트릭</p>
                        </div>
                    </div>
                </section>
            </div>
        </main>

        <!-- Floating Quick Add Task Button (Positioned relative to the mobile container) -->
        <button class="absolute bottom-28 right-6 w-14 h-14 bg-gradient-to-br from-primary to-primary-dim text-white rounded-full shadow-lg flex items-center justify-center active:scale-90 transition-transform z-40">
            <span class="material-symbols-outlined text-3xl" data-icon="add">add</span>
        </button>

        <!-- BottomNavBar (Sticky to the bottom of the container) -->
        <nav class="sticky bottom-0 left-0 w-full flex justify-around items-center px-4 pb-6 pt-3 bg-surface/90 backdrop-blur-lg z-50 shadow-[0_-12px_32px_rgba(40,43,81,0.04)] border-t border-outline-variant/10">
            <a class="flex flex-col items-center justify-center bg-primary text-white rounded-full px-5 py-2 transition-all duration-300 active:scale-90" href="#">
                <span class="material-symbols-outlined text-[20px]" data-icon="home_max" style="font-variation-settings: 'FILL' 1;">home_max</span>
                <span class="font-body text-[9px] font-semibold mt-0.5">홈</span>
            </a>
            <a class="flex flex-col items-center justify-center text-on-surface-variant px-5 py-2 hover:text-primary transition-colors active:scale-90" href="#">
                <span class="material-symbols-outlined text-[20px]" data-icon="calendar_today">calendar_today</span>
                <span class="font-body text-[9px] font-semibold mt-0.5">일정</span>
            </a>
            <a class="flex flex-col items-center justify-center text-on-surface-variant px-5 py-2 hover:text-primary transition-colors active:scale-90" href="#">
                <span class="material-symbols-outlined text-[20px]" data-icon="assignment_turned_in">assignment_turned_in</span>
                <span class="font-body text-[9px] font-semibold mt-0.5">할 일</span>
            </a>
            <a class="flex flex-col items-center justify-center text-on-surface-variant px-5 py-2 hover:text-primary transition-colors active:scale-90" href="#">
                <span class="material-symbols-outlined text-[20px]" data-icon="auto_awesome_motion">auto_awesome_motion</span>
                <span class="font-body text-[9px] font-semibold mt-0.5">습관</span>
            </a>
        </nav>
    </div>

</body>
</html>
