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
<em>Dec 2023 - Present | Research</em>
</p>
<div align="left">
<ul style="list-style-type: none; padding-left: 0;">
<li>🌐 Solved last-mile delivery optimization using advanced ML algorithms, reducing delivery times by 25%</li>
<li>⚡ Implemented dynamic route recalculation based on real-time traffic and weather conditions</li>
<li>📊 Achieved 15% reduction in fuel consumption through predictive analytics and route optimization</li>
</ul>
<h4>Tech Stack</h4>
<div align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white" alt="Jupyter"/>
<img src="https://img.shields.io/badge/Machine_Learning-FF6F00?style=flat&logo=scikit-learn&logoColor=white" alt="ML"/>
<img src="https://img.shields.io/badge/LLaMA-FF6F00?style=flat&logo=llama&logoColor=white" alt="LLaMA"/>
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
<li>📚 Created a production-ready implementation of 23 GoF patterns to solve common enterprise architectural challenges</li>
<li>🔧 Demonstrated pattern applications in microservices, event-driven systems, and distributed computing</li>
<li>✅ Built comprehensive test suites and documentation to guide developers in selecting optimal patterns</li>
</ul>
<h4>Tech Stack</h4>
<div align="center">
<img src="https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white" alt="Java"/>
<img src="https://img.shields.io/badge/JUnit-25A162?style=flat&logo=junit5&logoColor=white" alt="JUnit"/>
<img src="https://img.shields.io/badge/Design_Patterns-FF6F00?style=flat&logo=java&logoColor=white" alt="Design Patterns"/>
</div>
<div align="right" style="margin-top: 10px;">
<a href="https://github.com/joshishruti9/FakeNewsDetection">View Project →</a>
</div>
</div>
</td>
</tr>
<tr>
<td style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff);">
<h3 align="center">TypeScript Event Management System</h3>
<p align="center">
<strong>Technical Challenge</strong><br>
<em>Feb 2024 | Project</em>
</p>
<div align="left">
<ul style="list-style-type: none; padding-left: 0;">
<li>🎯 Engineered a scalable RSVP system handling concurrent user responses with optimized performance</li>
<li>✨ Implemented domain-driven design with clean architecture principles for maintainable code</li>
<li>✅ Achieved 100% test coverage using Jest, with comprehensive integration and unit tests</li>
</ul>
<h4>Tech Stack</h4>
<div align="center">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Jest-C21325?style=flat&logo=jest&logoColor=white" alt="Jest"/>
<img src="https://img.shields.io/badge/Clean_Code-00ACC1?style=flat&logo=javascript&logoColor=white" alt="Clean Code"/>
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
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white" alt="Swift"/>
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow"/>
  
  <h3>Backend & Databases</h3>
  <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Kafka"/>
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis"/>
  
  <h3>DevOps & Cloud</h3>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="AWS"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=Jenkins&logoColor=white" alt="Jenkins"/>
  
  <h3>Testing & QA</h3>
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=Selenium&logoColor=white" alt="Selenium"/>
  <img src="https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white" alt="JUnit"/>
  <img src="https://img.shields.io/badge/Apache_JMeter-D22128?style=for-the-badge&logo=apache&logoColor=white" alt="JMeter"/>
  <img src="https://img.shields.io/badge/Appium-43B02A?style=for-the-badge&logo=appium&logoColor=white" alt="Appium"/>
</div>

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
        </div>
      </td>
      <td width="50%" style="border-radius: 10px; padding: 25px; background: linear-gradient(to right, #f6f7f8, #ffffff); height: 100%; vertical-align: top;">
        <div style="display: flex; flex-direction: column; height: 100%;">
          <h3 align="center" style="margin: 0 0 15px 0;">🎓 Pune University</h3>
          <p align="center" style="margin: 0 0 15px 0;">
            <strong>B.Tech in Computer Science</strong><br>
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
          <div style="margin-top: 15px; text-align: center;">
            <img src="https://img.shields.io/badge/Dean's_List-FFD700?style=flat&logo=academic-cap" alt="Dean's List"/>
            <img src="https://img.shields.io/badge/Top_5%25-FF6B6B?style=flat&logo=star" alt="Top 5%"/>
          </div>
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
          <em>Nov 2025 - Feb 2026 | Remote</em>
        </p>
        <div align="left">
          <ul style="list-style-type: none; padding-left: 0;">
            <li>🤖 Built multimodal AI system for visually impaired using Snapdragon hardware</li>
            <li>🎯 Achieved <strong>85% captioning accuracy</strong> with <strong>300ms inference latency</strong></li>
            <li>⚡ Optimized model inference by <strong>30%</strong> using ONNX quantization and CoreML</li>
          </ul>
          <div align="center" style="margin-top: 15px;">
            <img src="https://img.shields.io/badge/Swift-FA7343?style=flat&logo=swift&logoColor=white" alt="Swift"/>
            <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python"/>
            <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white" alt="PyTorch"/>
            <img src="https://img.shields.io/badge/LLaMA-FF6F00?style=flat&logo=llama&logoColor=white" alt="LLaMA"/>
            <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white" alt="TensorFlow"/>
            <img src="https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazon-aws&logoColor=white" alt="AWS"/>
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
            <li>📈 Improved product quality by <strong>45%</strong> through load and performance testing automation</li>
            <li>⏱️ Reduced testing time by <strong>25%</strong> using ML-based test prioritization</li>
            <li>🔍 Implemented flaky test detection using Isolation Forest algorithm</li>
          </ul>
          <div align="center" style="margin-top: 15px;">
            <img src="https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white" alt="Java"/>
            <img src="https://img.shields.io/badge/JMeter-D22128?style=flat&logo=apache&logoColor=white" alt="JMeter"/>
            <img src="https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white" alt="Grafana"/>
            <img src="https://img.shields.io/badge/Selenium-43B02A?style=flat&logo=selenium&logoColor=white" alt="Selenium"/>
            <img src="https://img.shields.io/badge/Machine_Learning-FF6F00?style=flat&logo=scikit-learn&logoColor=white" alt="ML"/>
          </div>
        </div>
      </td>
    </tr>
    <tr>
      <td width="100%" style="border-radius: 10px; padding: 20px; background: linear-gradient(to right, #f6f7f8, #ffffff); margin-bottom: 20px;">
        <h3 align="center">🏢 Accenture</h3>
        <p align="center">
          <strong>Software Development Engineer</strong><br>
          <em>Dec 2020 - July 2022 | Pune, India</em>
        </p>
        <div align="left">
          <ul style="list-style-type: none; padding-left: 0;">
            <li>🚀 Increased deployment frequency by <strong>20%</strong> through CI/CD pipeline implementation</li>
            <li>✅ Reduced critical errors by <strong>25%</strong> through comprehensive backend testing</li>
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
  <a href="https://leetcode.com/u/mishrasaumya511/" target="_blank">
    <img src="https://img.shields.io/badge/-LeetCode-FFA116?style=for-the-badge&logo=LeetCode&logoColor=black" alt="LeetCode"/>
  </a>
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
