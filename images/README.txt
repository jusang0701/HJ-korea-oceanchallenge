* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --ocean-dark: #0a3d62;
  --ocean: #1e6fa8;
  --ocean-light: #eaf4fb;
  --sand: #f9f7f2;
  --text: #24313c;
  --toss: #0064ff;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: "Apple SD Gothic Neo", "Malgun Gothic", "Noto Sans KR", sans-serif;
  color: var(--text);
  line-height: 1.7;
}

.top-banner {
  background: var(--ocean-dark);
  color: #fff;
  text-align: center;
  padding: 8px;
  font-size: 14px;
}

.navbar {
  position: sticky;
  top: 0;
  z-index: 100;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 14px 5%;
  background: rgba(255, 255, 255, .95);
  box-shadow: 0 2px 10px rgba(0, 0, 0, .08);
}

.logo {
  font-size: 20px;
  font-weight: 800;
  color: var(--ocean-dark);
  text-decoration: none;
}

.logo span {
  color: var(--ocean);
}

.navbar nav a {
  margin-left: 18px;
  text-decoration: none;
  color: var(--text);
  font-size: 15px;
}

.navbar nav a:hover {
  color: var(--ocean);
}

.nav-cta {
  background: var(--ocean);
  color: #fff !important;
  padding: 8px 14px;
  border-radius: 20px;
}

#menu-toggle {
  display: none;
  font-size: 24px;
  background: none;
  border: none;
  cursor: pointer;
}

/* ===== 히어로 섹션 ===== */
.hero {
  height: 90vh;
  background: url("https://images.unsplash.com/photo-1505142468610-359e7d316be0?w=1600&q=75") center/cover no-repeat;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.hero-overlay {
  background: rgba(6, 40, 61, .55);
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 20px;
  color: #fff;
}

.hero h1 {
  font-size: clamp(32px, 6vw, 60px);
  letter-spacing: 1px;
}

.hero p {
  font-size: clamp(16px, 2.5vw, 22px);
  margin: 14px 0 28px;
}

.hero-buttons {
  display: flex;
  gap: 14px;
  flex-wrap: wrap;
  justify-content: center;
}

/* ===== 버튼 ===== */
.btn {
  display: inline-block;
  padding: 12px 28px;
  border-radius: 30px;
  border: none;
  text-decoration: none;
  font-size: 16px;
  font-weight: 700;
  cursor: pointer;
  transition: transform .15s, opacity .15s;
}

.btn:hover {
  transform: translateY(-2px);
  opacity: .9;
}

.btn-primary {
  background: var(--ocean);
  color: #fff;
}

.btn-outline {
  background: transparent;
  color: #fff;
  border: 2px solid #fff;
}

.btn-outline-dark {
  background: transparent;
  color: var(--ocean-dark);
  border: 2px solid var(--ocean-dark);
}

.btn-toss {
  background: var(--toss);
  color: #fff;
}

/* ===== 핵심 가치 카드 ===== */
.values {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 24px;
  padding: 60px 8%;
  background: var(--sand);
}

.value-card,
.apply-card {
  background: #fff;
  border-radius: 16px;
  padding: 32px 24px;
  text-align: center;
  box-shadow: 0 4px 16px rgba(0, 0, 0, .06);
}

.value-icon {
  font-size: 40px;
  margin-bottom: 12px;
}

.value-card h3,
.apply-card h3 {
  color: var(--ocean-dark);
  margin-bottom: 10px;
}

/* ===== 공통 섹션 ===== */
.section {
  padding: 80px 8%;
}

.section-alt {
  background: var(--ocean-light);
}

.section-title {
  text-align: center;
  font-size: clamp(26px, 4vw, 36px);
  color: var(--ocean-dark);
}

.section-sub {
  text-align: center;
  color: var(--ocean);
  margin: 6px 0 40px;
  font-weight: 600;
}

.about-box {
  max-width: 760px;
  margin: 0 auto;
  font-size: 17px;
}

.about-box p {
  margin-bottom: 16px;
}

/* ===== 갤러리 ===== */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 14px;
}

.gallery-grid img {
  width: 100%;
  height: 240px;
  object-fit: cover;
  border-radius: 12px;
  transition: transform .25s;
}

.gallery-grid img:hover {
  transform: scale(1.03);
}

/* ===== 일정 표 ===== */
.table-wrap {
  overflow-x: auto;
  max-width: 900px;
  margin: 0 auto;
}

.schedule-table {
  width: 100%;
  border-collapse: collapse;
  background: #fff;
}

.schedule-table th,
.schedule-table td {
  padding: 14px 16px;
  border-bottom: 1px solid #e3e9ee;
  text-align: left;
}

.schedule-table th {
  background: var(--ocean-dark);
  color: #fff;
}

/* ===== 준비물 체크리스트 ===== */
.packing-list {
  max-width: 640px;
  margin: 0 auto;
  display: grid;
  gap: 10px;
}

.packing-list label {
  background: #fff;
  padding: 14px 18px;
  border-radius: 10px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, .05);
  cursor: pointer;
  display: flex;
  align-items: center;
  gap: 12px;
}

.packing-list input {
  width: 18px;
  height: 18px;
  accent-color: var(--ocean);
}

/* ===== 가이드북 / 후원 ===== */
.guidebook-box {
  text-align: center;
  max-width: 640px;
  margin: 0 auto;
}

.guidebook-box p {
  margin-bottom: 20px;
  font-size: 17px;
}

.account-box {
  background: var(--sand);
  border-radius: 14px;
  padding: 24px;
  margin-top: 10px;
}

.account-number {
  font-size: 18px;
  font-weight: 700;
  color: var(--ocean-dark);
  margin: 8px 0 14px;
}

.small-note {
  font-size: 14px;
  color: #6b7a87;
  margin-bottom: 12px;
}

/* ===== 참가신청 / 참가비 카드 ===== */
.apply-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 24px;
  max-width: 900px;
  margin: 0 auto;
}

.apply-card p {
  margin-bottom: 20px;
}

/* ===== 푸터 ===== */
.footer {
  background: var(--ocean-dark);
  color: #cfe3f0;
  text-align: center;
  padding: 40px 20px;
}

.footer .copyright {
  font-size: 13px;
  margin-top: 10px;
  opacity: .7;
}

/* ===== 모바일 반응형 ===== */
@media (max-width: 768px) {
  #menu-toggle {
    display: block;
  }

  .navbar nav {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    right: 0;
    background: #fff;
    flex-direction: column;
    padding: 16px;
    box-shadow: 0 8px 16px rgba(0, 0, 0, .1);
  }

  .navbar nav.open {
    display: flex;
  }

  .navbar nav a {
    margin: 8px 0;
  }
}
