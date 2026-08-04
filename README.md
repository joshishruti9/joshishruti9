# <div align="center">Hi there! <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px"/> I'm Shruti Joshi</div>

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=2C9CCD&center=true&vCenter=true&width=435&lines=Software+Developer;Problem+Solver" alt="Typing SVG" />
</div>

## 👨‍💻 About Me
```java
public class SoftwareDeveloper {
    private final String name = "Shruti Joshi";
    private final String location = "Seattle, WA";
    private final String email = "joshishruti009@gmail.com";
    
    private final String[] expertise = {
        "Backend Development",
        "AI & Machine Learning",
        "Distributed Systems",
        "Software Testing",
        "Cloud Computing",
    };
    
    private final Map<String, String[]> techStack = Map.of(
        "Languages", new String[]{"Java", "Python", "Typescript", "C#"},
        "Backend", new String[]{"Spring Boot", "Apache Kafka", "PostgreSQL", "Redis", "RabbitMQ"},
        "DevOps", new String[]{"AWS", "Docker", "Kubernetes"},
        "Testing", new String[]{"Karate", "JMeter", "JUnit", "Cypress"},
        "AI/ML", new String[]{"PyTorch", "TensorFlow", "Transformers", "Langchain", "Generative AI"},
    );

    public String greet() {
        return "I'm passionate about building innovative solutions and exploring new technologies!";
    }
}
```
## 🚀 Featured Projects

<div align="center">
<table>
  <tr>
<td style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #fffbe6, #ffffff); border: 2px solid #FFD700;">
  <h3 align="center" style="font-size: 1.6em; margin-bottom: 0.2em;">
    🏆 <span style="color:#2C9CCD; font-weight:bold;">Distributed API Rate Limiting Service</span>
  </h3>
  <div align="left">
  <ul style="list-style-type: none; padding-left: 0;">
  <li>🔍 Evaluated fixed window, sliding window, leaky bucket, and token bucket algorithms against REST API traffic patterns; selected token bucket for its constant O(1) memory per client and native burst tolerance.</li>
  <li>⚛️ Implemented the token check-decrement-refill logic as an atomic Redis Lua script, using Redis's server-side clock (TIME) to eliminate clock-skew risk across distributed app instances.</li>
  <li>🔑 Designed a collision-free Redis key schema (clientId:endpoint) and a dynamic configuration API allowing per-client, per-endpoint capacity and refill-rate updates without redeploys.</li>
  <li>💡 Built a concurrency test using CountDownLatch to fire 200 simultaneous requests at a single bucket (capacity 100), verifying via atomic counters that the Lua script allowed exactly the configured limit with zero over-allocation under race conditions.</li>
  <li>📊 Built a React dashboard polling live token counts per client/endpoint, giving visibility into rate-limit state for debugging and monitoring.</li>
  </ul>
  <h4>Tech Stack</h4>
  <div align="center">
  <img src="https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white" alt="Java"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat&logo=springboot&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white" alt="Redis"/>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black" alt="React"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Lua-2C2D72?style=flat&logo=lua&logoColor=white" alt="Lua"/>
  <img src="https://img.shields.io/badge/JUnit5-25A162?style=flat&logo=junit5&logoColor=white" alt="JUnit5"/>
  </div>
  <div align="right" style="margin-top: 10px;">
  <a href="https://github.com/joshishruti9/RateLimiter">View Project →</a>
  </div>
  </div>
</td>
</tr>
<tr>
<td style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff);">
<h3 align="center">Scalable Video Streaming Platform</h3>
<p align="center">
<strong>Personal Project</strong><br>
</p>
<div align="left">
<ul style="list-style-type: none; padding-left: 0;">
<li>🎥 Built a video streaming platform as three independent microservices — a REST-based User Service, a gRPC-only Video Service, and an API Gateway bridging them for browsers.</li>
<li>🔐 Implemented a Strategy-pattern OAuth 2.0 framework with pluggable auth providers and stateless JWT verification with zero network calls per request.</li>
<li>📦 Used gRPC with real client- and server-streaming RPCs for chunked video upload and playback, cutting wire payload size by ~35-45% vs. REST/JSON.</li>
<li>⚡ Load-tested to 1,000+ concurrent connections with zero errors, and cut auth-check latency by ~88% (523ms → 61ms) by verifying tokens locally instead of over the network.</li>
<li>🗄️ Gave each service its own isolated database, following a database-per-service pattern for independent scaling and deployability.</li>
</ul>
<h4>Tech Stack</h4>
<div align="center">
<img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white" alt="Express"/>
<img src="https://img.shields.io/badge/gRPC-4285F4?style=flat&logo=google&logoColor=white" alt="gRPC"/>
<img src="https://img.shields.io/badge/Protocol_Buffers-4285F4?style=flat&logo=googlecloud&logoColor=white" alt="Protocol Buffers"/>
<img src="https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white" alt="SQLite"/>
<img src="https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white" alt="JWT"/>
<img src="https://img.shields.io/badge/Passport.js-34E27A?style=flat&logo=passport&logoColor=white" alt="Passport.js"/>
</div>
<div align="right" style="margin-top: 10px;">
<a href="https://github.com/joshishruti9/VideoStreamingPlatform">View Project →</a>
</div>
</div>
</td>
</tr>
<tr>
<td style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff);">
<h3 align="center">Movie Recommedation Service</h3>
<p align="center">
<strong>ML Project</strong><br>
</p>
<div align="left">
<ul style="list-style-type: none; padding-left: 0;">
<li>🧮 Implemented user-based collaborative filtering from scratch with vectorized NumPy operations, computing cosine similarity between a target user and every other user in a single matrix-vector operation instead of pairwise loops. </li>
<li>📊 Built a user-item rating matrix from the MovieLens dataset (~100K ratings across ~9,700 movies) with Pandas — merging ratings and movie metadata, then pivoting into the matrix collaborative filtering needs.</li>
<li>🎯 Designed a k-nearest-neighbors rating predictor that ranks users by similarity, selects the top-k neighbors, and computes a similarity-weighted average of their ratings to predict how a user would rate an unseen movie.</li>
<li>⚡ Reduced what would naively be an O(n²) pairwise similarity comparison into vectorized linear algebra (dot products and norms across the full matrix at once) — a meaningful performance-minded choice for a dataset this size.</li>
</ul>
<h4>Tech Stack</h4>
<div align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white" alt="Pandas"/>
<img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white" alt="NumPy"/>
</div>
<div align="right" style="margin-top: 10px;">
<a href="https://github.com/joshishruti9/MovieRecommenderSystem">View Project →</a>
</div>
</div>
</td>
</tr>
<tr>
<td style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff);">
<h3 align="center">NutriSync</h3>
<p align="center">
<strong>Personal Project</strong><br>
</p>
<div align="left">
<ul style="list-style-type: none; padding-left: 0;">
<li>🍽️ Built an AI-powered recipe search agent using LangChain and LlamaIndex to enable natural-language querying over a recipe dataset.</li>
<li>🔍 Indexed recipes into a vector store and exposed custom tools for ingredient-based search, cooking-time filtering, and nutrition lookups via an OpenAI GPT-3.5 agent.</li>
<li>📊 Processed structured recipe data with Pandas to power calorie calculations and multi-criteria filtering (time, ingredients, category).</li>
<li>🧠 Used a zero-shot ReAct agent architecture so the model dynamically decides which tool to call (search, nutrition, ingredients, or time filter) based on the user's query, rather than following a fixed pipeline.</li>
<li>💾 Persisted the vector index to disk so it only needs to be built once and can be reloaded for fast repeat queries instead of re-indexing every run.</li>
</ul>
<h4>Tech Stack</h4>
<div align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white" alt="OpenAI"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white" alt="LangChain"/>
<img src="https://img.shields.io/badge/LlamaIndex-000000?style=flat&logo=meta&logoColor=white" alt="LlamaIndex"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white" alt="Pandas"/>
<img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=flat&logo=googlecolab&logoColor=white" alt="Google Colab"/>
</div>
<div align="right" style="margin-top: 10px;">
<a href="https://github.com/joshishruti9/NutriSync">View Project →</a>
</div>
</div>
</td>
</tr>
<tr>
<td style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff);">
<h3 align="center">FocusMate</h3>
<p align="center">
<strong>SAAS Project</strong><br>
<em>Apr 2025 | Personal Project</em>
</p>
<div align="left">
<ul style="list-style-type: none; padding-left: 0;">
<li>🏗️ Built FocusMate as four independently deployable microservices (API Gateway, User, Task, Shop/Rewards) in TypeScript/Express, each with its own MongoDB database via Mongoose.</li>
<li>🔐 Implemented JWT-based authentication at the API Gateway plus Google OAuth login (google-auth-library) in the User Service, with unit tests that mock external calls using Jest.</li>
<li>🔄 Designed cross-service communication so completing a task in Task Service triggers a real HTTP call to User Service to award reward points, redeemable in the Shop Service.</li>
<li>🚀 Set up CI/CD with GitHub Actions — an orchestrator workflow triggers independent deployment jobs per service to Azure App Service on every push to main.</li>
<li>🧪 Wrote integration tests with Jest, Supertest, and mongodb-memory-server to test real database behavior without needing a live MongoDB instance.</li>
</ul>
<h4>Tech Stack</h4>
<div align="center">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white" alt="Express"/>
<img src="https://img.shields.io/badge/Angular-DD0031?style=flat&logo=angular&logoColor=white" alt="Angular"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white" alt="MongoDB"/>
<img src="https://img.shields.io/badge/Mongoose-880000?style=flat&logo=mongoose&logoColor=white" alt="Mongoose"/>
<img src="https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white" alt="JWT"/>
<img src="https://img.shields.io/badge/Google_OAuth-4285F4?style=flat&logo=google&logoColor=white" alt="Google OAuth"/>
<img src="https://img.shields.io/badge/Jest-C21325?style=flat&logo=jest&logoColor=white" alt="Jest"/>
<img src="https://img.shields.io/badge/Azure-0089D6?style=flat&logo=microsoftazure&logoColor=white" alt="Azure"/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
</div>
<div align="right" style="margin-top: 10px;">
<a href="https://github.com/joshishruti9/FocusMate">View Project →</a>
</div>
</div>
</td>
</tr>
<tr>
<td style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff);">
<h3 align="center">FakeNewsDetection</h3>
<p align="center">
<strong>Open Source Project</strong><br>
<em>Jan 2024 - Present | Personal</em>
</p>
<div align="left">
<ul style="list-style-type: none; padding-left: 0;">
<li>📰 Engineered linguistic and stylistic features for fake news classification — part-time-of-speech tagging with Stanford CoreNLP, Automated Readability Index scoring, and n-gram (bigram/trigram) extraction, feeding a Random Forest classifier trained on the labeled feature set.</li>
<li>🌐 Built a web-scraping similarity checker (using Jsoup) that searches for related online articles and computes Jaccard similarity against a given article's content, as a signal for cross-referencing claims.</li>
<li>🧹 Wrote a text preprocessing pipeline (stopword removal, tokenization) shared across every downstream feature extractor, so each feature module worked from consistently cleaned text.</li>
</li>🔗 Orchestrated the full feature-engineering pipeline — preprocessing → similarity, POS, and readability feature extraction → structured output — across both the fake and real news datasets.</li>
</ul>
<h4>Tech Stack</h4>
<div align="center">
<img src="https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white" alt="Java"/>
<img src="https://img.shields.io/badge/Weka-D5A021?style=flat&logo=apache&logoColor=white" alt="Weka"/>
<img src="https://img.shields.io/badge/Stanford_NLP-8C1515?style=flat&logo=stanford&logoColor=white" alt="Stanford NLP"/>
<img src="https://img.shields.io/badge/Jsoup-000000?style=flat&logo=java&logoColor=white" alt="Jsoup"/>
<img src="https://img.shields.io/badge/Apache_Ant-A81C7D?style=flat&logo=apacheant&logoColor=white" alt="Apache Ant"/>
</div>
<div align="right" style="margin-top: 10px;">
<a href="https://github.com/joshishruti9/FakeNewsDetection">View Project →</a>
</div>
</div>
</td>
</tr>
<tr>
<td style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff);">
<h3 align="center">PeopleSuite_SAAS_Platform</h3>
<p align="center">
<strong>Technical Challenge</strong><br>
<em>Feb 2024 | Project</em>
</p>
<div align="left">
<ul style="list-style-type: none; padding-left: 0;">
<li>🏢 Built PeopleSuite, a cloud-native employee management SaaS with Java Spring Boot microservices, AWS DynamoDB and S3, and Kubernetes-orchestrated deployment.</li>
</ul>
<h4>Tech Stack</h4>
<div align="center">
<img src="https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white" alt="Java"/>
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white" alt="Spring Boot"/>
<img src="https://img.shields.io/badge/AWS_DynamoDB-4053D6?style=flat&logo=amazondynamodb&logoColor=white" alt="AWS DynamoDB"/>
<img src="https://img.shields.io/badge/AWS_S3-569A31?style=flat&logo=amazons3&logoColor=white" alt="AWS S3"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" alt="Docker"/>
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
</div>
<div align="right" style="margin-top: 10px;">
<a href="https://github.com/joshishruti9/Coding-Challenge">View Project →</a>
</div>
</div>
</td>
</tr>
</table>
</div>

## 🛠️ Tech Stack
<div align="left">
  <h3>Languages & Frameworks</h3>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white" alt="Java"/>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black" alt="JavaScript"/>
<img src="https://img.shields.io/badge/C%23-239120?style=flat&logo=csharp&logoColor=white" alt="C#"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white" alt="Express"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" alt="FastAPI"/>
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white" alt="Spring Boot"/>
<img src="https://img.shields.io/badge/ASP.NET_Core-512BD4?style=flat&logo=dotnet&logoColor=white" alt="ASP.NET Core"/>
<img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Angular-DD0031?style=flat&logo=angular&logoColor=white" alt="Angular"/>

  
  <h3>Backend & Databases</h3>
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white" alt="MongoDB"/>
  
  <h3>DevOps & Cloud</h3>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="AWS"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=Jenkins&logoColor=white" alt="Jenkins"/>
  
  <h3>Testing & QA</h3>
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=Selenium&logoColor=white" alt="Selenium"/>
  <img src="https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white" alt="JUnit"/>
  <img src="https://img.shields.io/badge/Apache_JMeter-D22128?style=for-the-badge&logo=apache&logoColor=white" alt="JMeter"/>

## 📚 Education
<div align="center">
  <table style="width: 100%; border-collapse: separate; border-spacing: 20px;">
    <tr>
      <td width="50%" style="border-radius: 10px; padding: 25px; background: linear-gradient(to right, #f6f7f8, #ffffff); height: 100%; vertical-align: top;">
        <div style="display: flex; flex-direction: column; height: 100%;">
          <h3 align="center" style="margin: 0 0 15px 0;">🎓 Seattle University</h3>
          <p align="center" style="margin: 0 0 15px 0;">
            <strong>MS in Computer Science</strong><br>
            <em>GPA: 3.87/4.0 | 2024 - 2026</em><br>
            <img src="https://img.shields.io/badge/Seattle-WA-blue?style=flat&logo=location" alt="Location"/>
          </p>
          <details style="margin-top: auto;">
            <summary style="cursor: pointer;">📖 Coursework</summary>
            <div style="background: #f8f9fa; padding: 15px; border-radius: 5px; margin-top: 10px;">
              <ul style="list-style-type: none; padding-left: 0; margin: 0;">
                <li>🔢 Advanced Data Structures & Algorithms</li>
                <li>🤖 Machine Learning</li>
                <li>⚡ Distributed Systems</li>
                <li>🌐 Cloud Computing</li>
                <li>📊 Big Data Analytics</li>
              </ul>
            </div>
          </details>
          <div style="margin-top: 15px; text-align: center;">
            <img src="https://img.shields.io/badge/Dean's_List-FFD700?style=flat&logo=academic-cap" alt="Dean's Honor Roll"/>
          </div>
        </div>
      </td>
      <td width="50%" style="border-radius: 10px; padding: 25px; background: linear-gradient(to right, #f6f7f8, #ffffff); height: 100%; vertical-align: top;">
        <div style="display: flex; flex-direction: column; height: 100%;">
          <h3 align="center" style="margin: 0 0 15px 0;">🎓 Pune University</h3>
          <p align="center" style="margin: 0 0 15px 0;">
            <strong>B.E in Information Technology</strong><br>
            <em>GPA: 8.82/10 | 2016 - 2020</em><br>
            <img src="https://img.shields.io/badge/India-green?style=flat&logo=location" alt="Location"/>
          </p>
          <details style="margin-top: auto;">
            <summary style="cursor: pointer;">📖 Coursework</summary>
            <div style="background: #f8f9fa; padding: 15px; border-radius: 5px; margin-top: 10px;">
              <ul style="list-style-type: none; padding-left: 0; margin: 0;">
                <li>💻 Object-Oriented Programming</li>
                <li>🔢 Data Structures & Algorithms</li>
                <li>🌐 Computer Networks</li>
                <li>🖥️ Operating Systems</li>
                <li>📊 Database Management</li>
              </ul>
            </div>
          </details>
        </div>
      </td>
    </tr>
  </table>
</div>

## 💼 Professional Experience
<div align="center">
  <table>
    <tr>
      <td width="100%" style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff); margin-bottom: 20px;">
        <h3 align="center">🏢Shop Online New York</h3>
        <p align="center">
          <strong>Software Engineer Intern</strong><br>
          <em>Nov 2025 - Feb 2026 | New York, NY</em>
        </p>
        <div align="left">
          <ul style="list-style-type: none; padding-left: 0;">
            <li>🤖 Designed and implemented an <strong>RBAC-enabled</strong> order tracking system, integrating secure REST APIs to provide real-time order updates for <strong>1,000+</strong> users.</li>
            <li>🎯 Reduced initial page load time by <strong>25%</strong> via lazy loading and optimized Redux state management, improving user experience.</li>
            <li>⚡ Accelerated feature delivery by <strong>2 weeks</strong> using <strong>GitHub Copilot</strong> while validating business logic, edge cases and code quality.</li>
          </ul>
          <div align="center" style="margin-top: 15px;">
            <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" alt="TypeScript"/>
            <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
            <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black" alt="React"/>
            <img src="https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazon-aws&logoColor=white" alt="AWS"/>
          </div>
        </div>
      </td>
    </tr>
     <tr>
      <td width="100%" style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff); margin-bottom: 20px;">
        <h3 align="center">🏢Bilimetrix USA LLC</h3>
        <p align="center">
          <strong>Software Engineer Intern</strong><br>
          <em>Nov 2025 - Feb 2026 | Remote</em>
        </p>
        <div align="left">
          <ul style="list-style-type: none; padding-left: 0;">
            <li>🤖 Designed HIPAA-compliant patient reporting service using ASP.NET and C#, reducing diagnosis time from 10 min to 5 min with 100% unit test coverage.</li>
            <li>🎯 Resolved production defects through root cause analysis and component refactoring, improving application stability.</li>
          </ul>
          <div align="center" style="margin-top: 15px;">
            <img src="https://img.shields.io/badge/ASP.NET_Core-512BD4?style=flat&logo=dotnet&logoColor=white" alt="ASP.NET Core"/>
            <img src="https://img.shields.io/badge/C%23-239120?style=flat&logo=csharp&logoColor=white" alt="C#"/>
          </div>
        </div>
      </td>
    </tr>
    <tr>
      <td width="100%" style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff); margin-bottom: 20px;">
        <h3 align="center">🏢 Mastercard</h3>
        <p align="center">
          <strong>Software Development Engineer</strong><br>
          <em>Aug 2022 - Jan 2024 | Pune, India</em>
        </p>
        <div align="left">
          <ul style="list-style-type: none; padding-left: 0;">
            <li>📈 Designed and developed event-driven promotional systems using Java, React, Spring Boot, and Apache Kafka processing 250,000+ daily reward transactions with high availability and low latency.</li>
            <li>⏱️ Engineered a fault-tolerant event status reconciliation mechanism by introducing partial-failure classification and intelligent retry handling, reducing unnecessary retries by 40% while improving data consistency</li>
            <li>🔍 Led CI/CD automation using Jenkins and XLR, enabling test-gated deployments and reducing manual release overhead</li>
            <li>🎯 Debugged and resolved production issues in a real-time LiveChat platform, improving system reliability and ensuring uninterrupted customer communication</li>
            <li>🧪 Developed automated regression test suites for 5 microservices using Karate and Cypress, reducing regression defects.</li>
          </ul>
          <div align="center" style="margin-top: 15px;">
            <img src="https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white" alt="Java"/>
             <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Kafka"/>
            <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black" alt="React"/>
            <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white" alt="Spring Boot"/>
            <img src="https://img.shields.io/badge/Microservices-FF6F00?style=flat&logo=kubernetes&logoColor=white" alt="Microservices"/>
            <img src="https://img.shields.io/badge/JMeter-D22128?style=flat&logo=apache&logoColor=white" alt="JMeter"/>
            
          </div>
        </div>
      </td>
    </tr>
    <tr>
      <td width="100%" style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff); margin-bottom: 20px;">
        <h3 align="center">🏢 Accenture</h3>
        <p align="center">
          <strong>Associate Software Engineer</strong><br>
          <em>Dec 2020 - July 2022 | Pune, India</em>
        </p>
        <div align="left">
          <ul style="list-style-type: none; padding-left: 0;">
            <li>🚀 Built a stateless authentication service using Java, Spring Boot, RabbitMQ, Redis and JWT, supporting asynchronous OTP delivery for 10K+ users with 40 ms p99 latency.</li>
            <li>✅ Improved system observability by implementing Grafana dashboards and Prometheus monitoring, reducing production incident resolution time from 50 to 30 minutes.</li>
            <li>🧮 Modernized legacy SOAP services into RESTful APIs, improving scalability, maintainability, and service interoperability.</li>
          </ul>
          <div align="center" style="margin-top: 15px;">
            <img src="https://img.shields.io/badge/Jenkins-D24939?style=flat&logo=jenkins&logoColor=white" alt="Jenkins"/>
            <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white" alt="Postman"/>
            <img src="https://img.shields.io/badge/REST_API-FF6C37?style=flat&logo=rest&logoColor=white" alt="REST API"/>
            <img src="https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white" alt="Java"/>
          </div>
        </div>
      </td>
    </tr>
  </table>
</div>

## 🔗 Connect With Me
<div align="center">
  <a href="https://github.com/joshishruti9" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
  <a href="mailto:joshishruti009@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
</div>

---
<div align="center">
  <img src="https://komarev.com/ghpvc/?username=joshishruti9&color=brightgreen" alt="Profile Views"/>
  <br/>
  ⭐️ From <a href="https://github.com/joshishruti9/Aboutme">Shruti Joshi</a>
</div> 
