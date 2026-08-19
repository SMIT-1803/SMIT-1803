<h2 align="left">Hi, I'm Smit 👋</h2>

###

I'm a third year Computing Science student at Simon Fraser University (Burnaby, BC). Most of what I build lives on the backend: REST APIs, data pipelines, and a warehouse or two. I like problems where the hard part is getting the data right before anything downstream touches it, and I try to leave every project with tests, a schema, and a reason for each decision.

###

## 🌐 Socials

<div align="left">
  <a href="mailto:smitsachin1@gmail.com">
    <img src="https://img.shields.io/static/v1?message=Gmail&logo=gmail&label=&color=D14836&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="gmail logo" />
  </a>
  <a href="https://www.linkedin.com/in/smit-sfu/">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="linkedin logo" />
  </a>
</div>

###

## 💻 Tech Stack

**Languages**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

**Backend & Databases**

![Node.js](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![PostgreSQL](https://img.shields.io/badge/postgresql-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/mongodb-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=jsonwebtokens&logoColor=white)

**Data**

![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)

**Frontend**

![Next.js](https://img.shields.io/badge/next.js-black?style=for-the-badge&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Redux](https://img.shields.io/badge/redux-%23593d88.svg?style=for-the-badge&logo=redux&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)

**Tools & Infra**

![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/bash-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Render](https://img.shields.io/badge/Render-000000?style=for-the-badge&logo=render&logoColor=white)
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)
![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white)

**AI Tooling**

![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=claude&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)

###

## 🚀 Projects

### CourseCatch
*SFU course enrollment alerts, running twice a day on Render*

A Python service that checks 2,900 SFU course sections twice daily, compares each run against stored PostgreSQL state, and writes only the rows that actually changed instead of all 2,900. Checks for failed parsing and abnormal row counts run before any email goes out, so a bad scrape stops and alerts me instead of emailing every user. Students can watch a section for an open seat or for the waitlist queue dropping below a number they set. The Next.js frontend sits on Supabase with row-level security and one-time-code sign-in, switched over from magic links after SFU's mail scanner turned out to be consuming single-use tokens before delivery.

🔗 [GitHub](https://github.com/SMIT-1803/CourseCatch)

`Python` `PostgreSQL` `Next.js` `TypeScript` `Render` `Supabase`

---

### IPL Cricket Analytics
*Sports data warehouse and dashboard published on Tableau Public*

A star-schema warehouse in PostgreSQL built over 295,000+ ball-by-ball deliveries from 1,243 matches. A staging-based ELT pipeline lands raw CSV data and rebuilds the warehouse in a single transaction, and multi-CTE window-function queries compute rolling batting form, death-over economy, and dot-ball streaks. Indexing the striker foreign key behind the heaviest query and comparing plans with `EXPLAIN ANALYZE` cut its runtime from 46.7 ms to 24.5 ms.

🔗 [Dashboard](https://public.tableau.com/app/profile/smit.sanghvi/viz/IPLBall-by-BallAnalytics/IPLAnalytics20082026) · [GitHub](https://github.com/SMIT-1803/IPL-sql-analytics)

`PostgreSQL` `SQL` `Python` `psycopg2` `Tableau`

---

### Crypto Trading Bot
*Market data pipeline and backtesting engine running on AWS*

An 8-stage Python pipeline that loads, validates, and transforms OHLCV data for 3 assets across daily and 4H timeframes. A 4-check validation layer catches malformed rows before they reach strategy logic, and a parameterized backtester writes CSV and JSON reports across configurations. Strategy parameters were tuned on multi-year history and validated on a held-out one-year out-of-sample window, reaching a 52% win rate.

🔗 [GitHub](https://github.com/SMIT-1803/Crypto-Trading-Bot)

`Python` `Pandas` `NumPy` `Kraken API` `AWS EC2`

---

### JotDown
*REST API backend with authentication and end-to-end testing*

Nine RESTful endpoints across note and user resources, with input validation, structured MongoDB schemas, and soft- and permanent-delete flows. Routes are protected by JWT auth with access and refresh-token rotation, and every endpoint was tested end-to-end in Postman across valid and invalid inputs.

🔗 [GitHub](https://github.com/SMIT-1803/JotDown-REST-API)

`Node.js` `Express.js` `MongoDB` `JWT` `Postman`

---

### Blog Platform
*Full-stack publishing app deployed on Vercel*

A publishing platform with 7 routes and 15 reusable React components, backed by Appwrite for auth, database, and file storage. Full create, read, update, and delete flows sit behind protected routes, with Redux Toolkit keeping state consistent across public and authenticated views.

🔗 [Live Demo](https://smitsblog.vercel.app) · [GitHub](https://github.com/SMIT-1803)

`React` `Redux Toolkit` `Tailwind CSS` `Appwrite` `Vercel`

###
---
## 🙋 A bit more about me

- 🎓 BSc Computing Science @ SFU · expected Dec 2027
- 🧑‍🏫 Peer Tutor at Fraser International College, working with 40+ first-year students on data structures, OOP, and C++ memory management
- 🔨 Currently building CourseCatch, an enrollment alert service for SFU students
- 🔍 Looking for a software, data, or QA co-op
- 📍 Based in Burnaby, BC
- 🌱 Currently digging into data warehousing, analytical SQL, and Postgres row-level security
###

## 📬 Let's connect

📧 [sss101@sfu.ca](mailto:sss101@sfu.ca)
💼 [LinkedIn](https://www.linkedin.com/in/smit-sfu/)
🐙 [GitHub](https://github.com/SMIT-1803)

###
