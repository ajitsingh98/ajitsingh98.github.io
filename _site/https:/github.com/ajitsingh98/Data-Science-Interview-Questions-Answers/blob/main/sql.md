

<!doctype html>
<html lang="en" class="no-js">
  <head>
    

<meta charset="utf-8">



<!-- begin SEO -->









<title>SQL Interview Questions and Answers - Data Science Corner</title>







<meta property="og:locale" content="en-US">
<meta property="og:site_name" content="Data Science Corner">
<meta property="og:title" content="SQL Interview Questions and Answers">


  <link rel="canonical" href="http://localhost:4000/https:/github.com/ajitsingh98/Data-Science-Interview-Questions-Answers/blob/main/sql.md">
  <meta property="og:url" content="http://localhost:4000/https:/github.com/ajitsingh98/Data-Science-Interview-Questions-Answers/blob/main/sql.md">



  <meta property="og:description" content="This contains questions from SQL joins, rank, window functions etc">





  

  












  <script type="application/ld+json">
    {
      "@context" : "http://schema.org",
      "@type" : "Person",
      "name" : "Ajit Kumar Singh",
      "url" : "http://localhost:4000",
      "sameAs" : null
    }
  </script>






<!-- end SEO -->


<link href="http://localhost:4000/feed.xml" type="application/atom+xml" rel="alternate" title="Data Science Corner Feed">

<!-- http://t.co/dKP3o1e -->
<meta name="HandheldFriendly" content="True">
<meta name="MobileOptimized" content="320">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<script>
  document.documentElement.className = document.documentElement.className.replace(/\bno-js\b/g, '') + ' js ';
</script>

<!-- For all browsers -->
<link rel="stylesheet" href="http://localhost:4000/assets/css/main.css">

<meta http-equiv="cleartype" content="on">
    

<!-- start custom head snippets -->

<link rel="apple-touch-icon" sizes="57x57" href="http://localhost:4000/images/apple-touch-icon-57x57.png?v=M44lzPylqQ">
<link rel="apple-touch-icon" sizes="60x60" href="http://localhost:4000/images/apple-touch-icon-60x60.png?v=M44lzPylqQ">
<link rel="apple-touch-icon" sizes="72x72" href="http://localhost:4000/images/apple-touch-icon-72x72.png?v=M44lzPylqQ">
<link rel="apple-touch-icon" sizes="76x76" href="http://localhost:4000/images/apple-touch-icon-76x76.png?v=M44lzPylqQ">
<link rel="apple-touch-icon" sizes="114x114" href="http://localhost:4000/images/apple-touch-icon-114x114.png?v=M44lzPylqQ">
<link rel="apple-touch-icon" sizes="120x120" href="http://localhost:4000/images/apple-touch-icon-120x120.png?v=M44lzPylqQ">
<link rel="apple-touch-icon" sizes="144x144" href="http://localhost:4000/images/apple-touch-icon-144x144.png?v=M44lzPylqQ">
<link rel="apple-touch-icon" sizes="152x152" href="http://localhost:4000/images/apple-touch-icon-152x152.png?v=M44lzPylqQ">
<link rel="apple-touch-icon" sizes="180x180" href="http://localhost:4000/images/apple-touch-icon-180x180.png?v=M44lzPylqQ">
<link rel="icon" type="image/png" href="http://localhost:4000/images/favicon-32x32.png?v=M44lzPylqQ" sizes="32x32">
<link rel="icon" type="image/png" href="http://localhost:4000/images/android-chrome-192x192.png?v=M44lzPylqQ" sizes="192x192">
<link rel="icon" type="image/png" href="http://localhost:4000/images/favicon-96x96.png?v=M44lzPylqQ" sizes="96x96">
<link rel="icon" type="image/png" href="http://localhost:4000/images/favicon-16x16.png?v=M44lzPylqQ" sizes="16x16">
<link rel="manifest" href="http://localhost:4000/images/manifest.json?v=M44lzPylqQ">
<link rel="mask-icon" href="http://localhost:4000/images/safari-pinned-tab.svg?v=M44lzPylqQ" color="#000000">
<link rel="shortcut icon" href="/images/favicon.ico?v=M44lzPylqQ">
<meta name="msapplication-TileColor" content="#000000">
<meta name="msapplication-TileImage" content="http://localhost:4000/images/mstile-144x144.png?v=M44lzPylqQ">
<meta name="msapplication-config" content="http://localhost:4000/images/browserconfig.xml?v=M44lzPylqQ">
<meta name="theme-color" content="#ffffff">
<link rel="stylesheet" href="http://localhost:4000/assets/css/academicons.css"/>


<!-- Support for MatJax -->
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<!-- end custom head snippets -->

  </head>

  <body>

    <!--[if lt IE 9]>
<div class="notice--danger align-center" style="margin: 0;">You are using an <strong>outdated</strong> browser. Please <a href="http://browsehappy.com/">upgrade your browser</a> to improve your experience.</div>
<![endif]-->
    

<div class="masthead">
  <div class="masthead__inner-wrap">
    <div class="masthead__menu">
      <nav id="site-nav" class="greedy-nav">
        <button><div class="navicon"></div></button>
        <ul class="visible-links">
          <li class="masthead__menu-item masthead__menu-item--lg"><a href="http://localhost:4000/">Data Science Corner</a></li>
          
            
            <li class="masthead__menu-item"><a href="http://localhost:4000/interview_preparation/">Interview Preparation</a></li>
          
            
            <li class="masthead__menu-item"><a href="http://localhost:4000/portfolio/">Portfolio</a></li>
          
            
            <li class="masthead__menu-item"><a href="http://localhost:4000/year-archive/">Blog Posts</a></li>
          
            
            <li class="masthead__menu-item"><a href="http://localhost:4000/files/resume.pdf">CV</a></li>
          
            
            <li class="masthead__menu-item"><a href="http://localhost:4000/markdown/">Guide</a></li>
          
        </ul>
        <ul class="hidden-links hidden"></ul>
      </nav>
    </div>
  </div>
</div>

    





<div id="main" role="main">
  


  <div class="sidebar sticky">
  



<div itemscope itemtype="http://schema.org/Person">

  <div class="author__avatar">
    
    	<img src="http://localhost:4000/images/profile.png" class="author__avatar" alt="Ajit Kumar Singh">
    
  </div>

  <div class="author__content">
    <h3 class="author__name">Ajit Kumar Singh</h3>
    
    <p class="author__bio">Data Scientist</p>
  </div>

  <div class="author__urls-wrapper">
    <button class="btn btn--inverse">Follow</button>
    <ul class="author__urls social-icons">
      <!-- Font Awesome icons / Biographic information  -->
      
        <li><i class="fa-solid fa-location-dot icon-pad-right" aria-hidden="true"></i>India</li>
      
      
        <li><i class="fa fa-solid fa-building-columns icon-pad-right" aria-hidden="true"></i>Pixis.AI</li>
      
      
      
        <li><a href="mailto:sajit9285@gmail.com"><i class="fas fa-fw fa-envelope icon-pad-right" aria-hidden="true"></i>Email</a></li>
      

      <!-- Font Awesome and Academicons icons / Academic websites -->
            
      
      
      
                              
      

      <!-- Font Awesome icons / Repositories and software development -->
      
            
            
      
        <li><a href="https://github.com/ajitsingh98"><i class="fab fa-fw fa-github icon-pad-right" aria-hidden="true"></i>Github</a></li>
      
            
            

      <!-- Font Awesome icons / Social media -->
      
      
            
      
                  
                  
      
            
            
      
        <li><a href="https://www.linkedin.com/in/sajit9285"><i class="fab fa-fw fa-linkedin icon-pad-right" aria-hidden="true"></i>LinkedIn</a></li>
            
      
      
        <li><a href="sajit9285"><i class="fab fa-fw fa-medium icon-pad-right" aria-hidden="true"></i>Medium</a></li>
            
                  
            
      
            
            
      
        <li><a href="https://twitter.com/bayesian_walker"><i class="fab fa-fw fa-x-twitter icon-pad-right" aria-hidden="true"></i>X (formerly Twitter)</a></li>
      
              
      
                      
      
      
            
    </ul>
  </div>
</div>

  
  </div>


  <article class="page" itemscope itemtype="http://schema.org/CreativeWork">
    <meta itemprop="headline" content="SQL Interview Questions and Answers">
    <meta itemprop="description" content="This contains questions from SQL joins, rank, window functions etc">
    
    

    <div class="page__inner-wrap">
      
        <header>
          <h1 class="page__title" itemprop="headline">SQL Interview Questions and Answers
</h1>
          
        
        
            
        </header>
      

      <section class="page__content" itemprop="text">
        <h2 id="topics">Topics</h2>

<ul>
  <li><a href="#sql-questions">SQL Questions</a></li>
</ul>

<p>Consider you have a <code class="language-plaintext highlighter-rouge">worker</code> table with following fields:</p>
<ul>
  <li>first_name</li>
  <li>last_name</li>
  <li>salary</li>
  <li>worker_id(Primary Key)</li>
  <li>department</li>
  <li>department_name</li>
</ul>

<p>Along with you have some meta data tables like <code class="language-plaintext highlighter-rouge">title</code> and <code class="language-plaintext highlighter-rouge">bonus</code> which contains following fields:</p>

<ul>
  <li><code class="language-plaintext highlighter-rouge">title</code></li>
</ul>

<h2 id="sql-questions">SQL Questions</h2>

<p>Q. How do you retrieve the first name from the Worker table using an alias “WORKER NAME”?</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>first_name</b> AS worker_name FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. How can you convert the first name from the Worker table to uppercase?</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>UPPER(first_name)</b> AS first_name FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. What SQL query would you use to fetch distinct department names from the Worker table?</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>DISTINCT department</b> FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. How can you select the first three characters of the first name from the Worker table?</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>SUBSTRING(first_name, 1, 3)</b> AS first_name FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. Write a query to find the position of ‘s’ in the first name “Manish” within the Worker table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>POSITION('s' IN first_name)</b> AS position_of_s FROM <b>Worker</b> WHERE first_name = 'Manish';
    </p>
</details>

<hr />

<p>Q. How do you trim whitespace from the right side of the first name in the Worker table?</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>RTRIM(first_name)</b> AS trimmed_first_name FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. Write a query to remove whitespace from the left side of the department field in the Worker table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>LTRIM(department)</b> AS trimmed_department FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. How can you fetch unique department names from the Worker table and display their lengths?</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>DISTINCT department</b>, <b>LENGTH(department)</b> AS department_length FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. What query would replace ‘a’ with ‘A’ in the first name from the Worker table?</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>REPLACE(first_name, 'a', 'A')</b> AS first_name FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. How do you concatenate the first name and last name from the Worker table into a single column “COMPLETE NAME”?</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT <b>CONCAT(first_name, ' ', last_name)</b> AS complete_name FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. Write a query to list all worker details from the Worker table ordered by first name in ascending order.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> ORDER BY first_name ASC;
    </p>
</details>

<hr />

<p>Q. How can you list all worker details from the Worker table ordered by first name ascending and department descending?</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> ORDER BY first_name ASC, department DESC;
    </p>
</details>

<hr />

<p>Q. Write a query to fetch details for Workers with the first names “</p>

<p>Manish” and “Arhan” from the Worker table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE first_name IN ('Manish', 'Arhan');
    </p>
</details>

<hr />

<p>Q. Write a query to list details of workers excluding first names “Manish” and “Arhan” from the Worker table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE first_name NOT IN ('Manish', 'Arhan');
    </p>
</details>

<hr />

<p>Q. Write a query to fetch details of Workers with the department name “Admin”.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE department_name = 'Admin';
    </p>
</details>

<hr />

<p>Q. Write a query to fetch details of Workers whose first name contains ‘a’.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE first_name LIKE '%a%';
    </p>
</details>

<hr />

<p>Q. Write a query to fetch details of Workers whose first name ends with ‘a’.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE first_name LIKE '%a';
    </p>
</details>

<hr />

<p>Q. Write a query to fetch details of Workers whose first name ends with ‘h’ and contains six alphabets.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE first_name LIKE '%h' AND CHAR_LENGTH(first_name) = 6;
    </p>
</details>

<hr />

<p>Q. Write a query to fetch details of Workers whose salary lies between 100000 and 500000.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE salary BETWEEN 100000 AND 500000;
    </p>
</details>

<hr />

<p>Q. Write a query to list Workers who joined in February 2014.</p>

<details><summary><b>Answer</b></summary>
    <p>
    -- Assuming there's a joining_date field in the Worker table, which is not listed in the initial table information.
    -- SELECT  FROM <b>Worker</b> WHERE YEAR(joining_date) = 2014 AND MONTH(joining_date) = 2;
    -- This answer is based on an assumed field not explicitly mentioned in the table schema provided.
    </p>
</details>

<hr />

<p>Q. Write a query to fetch the count of employees working in the department ‘Admin’.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT COUNT() FROM <b>Worker</b> WHERE department_name = 'Admin';
    </p>
</details>

<hr />

<p>Q. Write a query to fetch worker names with salaries between 50000 and 100000.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT CONCAT(first_name, ' ', last_name) AS full_name, salary FROM <b>Worker</b> WHERE salary BETWEEN 50000 AND 100000;
    </p>
</details>

<hr />

<p>Q. Write a query to fetch the number of workers for each department in descending order.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT department, COUNT() AS num_workers FROM <b>Worker</b> GROUpBY department ORDER BY num_workers DESC;
    </p>
</details>

<hr />

<p>Q. Write a query to list details of Workers who are also Managers, assuming a title table contains info about worker titles.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT w. FROM <b>Worker w</b> JOIN <b>title t</b> ON w.worker_id = t.worker_id WHERE t.worker_title = 'Manager';
    </p>
</details>

<hr />

<p>Q. Write a query to count the number of titles in the organization of different types.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT worker_title, COUNT() FROM <b>title</b> GROUpBY worker_title HAVING COUNT() &gt; 1;
    </p>
</details>

<hr />

<p>Q. Write a query to show only odd rows from the Worker table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE MOD(worker_id, 2) = 1;
    </p>
</details>

<hr />

<p>Q. Write a query to show only even rows from the Worker table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE MOD(worker_id, 2) = 0;
    </p>
</details>

<hr />

<p>Q. Write a query to clone a new table from another table (e.g., worker_clone from worker).</p>

<details><summary><b>Answer</b></summary>
    <p>
    -- Step1: Create a clone table with the same structure as Worker
    CREATE TABLE <b>worker_clone</b> LIKE <b>Worker</b>;
    </p>
    <p>
    -- Step2: Copy all data from Worker to worker_clone
    INSERT INTO <b>worker_clone</b> SELECT  FROM <b>Worker</b>;
    </p>
</details>

<hr />

<p>Q. Write a query to fetch intersecting records of two tables (worker and worker_clone).</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT w. FROM <b>Worker w</b> INNER JOIN <b>worker_clone wc</b> ON w.worker_id = wc.worker_id;
    </p>
</details>

<hr />

<p>Q. Write a query to show records from one table that another table does not have.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT w. FROM <b>Worker w</b> LEFT JOIN <b>worker_clone wc</b> ON w.worker_id = wc.worker_id WHERE wc.worker_id IS NULL;
    </p>
</details>

<hr />

<p>Q. Write a query to show the current date and time.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT NOW();
    </p>
</details>

<hr />

<p>Q. Write a query to show the topn (e.g., 5) records of a table ordered by descending salary.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT 

 FROM <b>Worker</b> ORDER BY salary DESC LIMIT 5;
    </p>
</details>

<hr />

<p>Q. Write a query to determine the nth (e.g., 5th) highest salary from a table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT DISTINCT salary FROM <b>Worker</b> ORDER BY salary DESC LIMIT 1 OFFSET 4;
    </p>
</details>

<hr />

<p>Q. Write a query to find the 5th highest salary without using the LIMIT keyword.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT salary FROM <b>Worker</b> w1 WHERE 4 = (SELECT COUNT(DISTINCT w2.salary) FROM <b>Worker</b> w2 WHERE w2.salary &gt; w1.salary);
    </p>
</details>

<hr />

<p>Q. Write a query to list employees with the same salary.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT w1. FROM <b>Worker</b> w1, <b>Worker</b> w2 WHERE w1.salary = w2.salary AND w1.worker_id != w2.worker_id;
    </p>
</details>

<hr />

<p>Q. Write a query to show the second highest salary from a table using a sub-query.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT MAX(salary) FROM <b>Worker</b> WHERE salary NOT IN (SELECT MAX(salary) FROM Worker);
    </p>
</details>

<hr />

<p>Q. Write a query to show one row twice in results from a table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE worker_id = (SELECT MIN(worker_id) FROM Worker) UNION ALL SELECT  FROM <b>Worker</b> WHERE worker_id = (SELECT MIN(worker_id) FROM Worker);
    </p>
</details>

<hr />

<p>Q. Write a query to list worker ids who do not receive a bonus.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT worker_id FROM <b>Worker</b> WHERE worker_id NOT IN (SELECT worker_id FROM <b>bonus</b>);
    </p>
</details>

<hr />

<p>Q. Write a query to fetch the first 50% records from a table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> WHERE worker_id &lt;= (SELECT FLOOR(COUNT() / 2) FROM Worker);
    </p>
</details>

<hr />

<p>Q. Write a query to fetch the departments that have less than 4 people in them.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT department, COUNT() AS dept_count FROM <b>Worker</b> GROUPBY department HAVING dept_count &lt; 4;
    </p>
</details>

<hr />

<p>Q. Write a query to show all departments along with the number of people in there.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT department, COUNT() AS dept_count FROM <b>Worker</b> GROUpBY department;
    </p>
</details>

<hr />

<p>Q. Write a query to show the last record from a table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> ORDER BY worker_id DESC LIMIT 1;
    </p>
</details>

<hr />

<p>Q. Write a query to fetch the first row of a table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> ORDER BY worker_id ASC LIMIT 1;
    </p>
</details>

<hr />

<p>Q. Write a query to fetch the last five records from a table.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT  FROM <b>Worker</b> ORDER BY worker_id DESC LIMIT 5;
    </p>
</details>

<hr />

<p>Q. Write a query to print the names of employees having the highest salary in each department.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT w.department, w.first_name, w.salary FROM <b>Worker w</b> INNER JOIN (SELECT department, MAX(salary) AS max_salary FROM Worker GROUpBY department) AS dept_max ON w.department = dept_max.department AND w.salary = dept_max.max_salary;
    </p>
</details>

<hr />

<p>Q. Write a query to fetch three max salaries from a table using a co-related subquery.</p>

<details><summary><b>Answer</b></summary>
    <p>
    SELECT DISTINCT salary FROM <b>Worker w1</b> WHERE 3 &gt;= (SELECT COUNT(DISTINCT w2.salary) FROM <b>Worker w2</b> WHERE w2.salary &gt;= w1.salary) ORDER BY salary DESC;
    </p>
</details>

<hr />


        

        
      </section>

      <footer class="page__meta">
        
        




      </footer>

      

<section class="page__share">
  
    <h4 class="page__share-title">Share on</h4>
  

  <a href="https://twitter.com/intent/tweet?text=http://localhost:4000/https:/github.com/ajitsingh98/Data-Science-Interview-Questions-Answers/blob/main/sql.md" class="btn btn--twitter" title="Share on Twitter"><i class="fab fa-twitter" aria-hidden="true"></i><span> Twitter</span></a>

  <a href="https://www.facebook.com/sharer/sharer.php?u=http://localhost:4000/https:/github.com/ajitsingh98/Data-Science-Interview-Questions-Answers/blob/main/sql.md" class="btn btn--facebook" title="Share on Facebook"><i class="fab fa-facebook" aria-hidden="true"></i><span> Facebook</span></a>

  <a href="https://www.linkedin.com/shareArticle?mini=true&url=http://localhost:4000/https:/github.com/ajitsingh98/Data-Science-Interview-Questions-Answers/blob/main/sql.md" class="btn btn--linkedin" title="Share on LinkedIn"><i class="fab fa-linkedin" aria-hidden="true"></i><span> LinkedIn</span></a>
</section>

      


  <nav class="pagination">
    
      <a href="http://localhost:4000/interview_preparation/2024-02-17-paper-title-number-4" class="pagination--pager" title="Paper Title Number 4
">Previous</a>
    
    
      <a href="#" class="pagination--pager disabled">Next</a>
    
  </nav>

    </div>

    
  </article>

  
  
</div>


    <div class="page__footer">
      <footer>
        <!-- start custom footer snippets -->
<a href="/sitemap/">Sitemap</a>
<!-- end custom footer snippets -->

        

<div class="page__footer-follow">
  <ul class="social-icons">
    
      <li><strong>Follow:</strong></li>
    
    
    
    
      <li><a href="http://github.com/ajitsingh98"><i class="fab fa-github" aria-hidden="true"></i> GitHub</a></li>
    
    
    <li><a href="http://localhost:4000/feed.xml"><i class="fa fa-fw fa-rss-square" aria-hidden="true"></i> Feed</a></li>
  </ul>
</div>

<div class="page__footer-copyright">&copy; 2024 Ajit Kumar Singh. Powered by <a href="http://jekyllrb.com" rel="nofollow">Jekyll</a> &amp; <a href="https://github.com/academicpages/academicpages.github.io">AcademicPages</a>, a fork of <a href="https://mademistakes.com/work/minimal-mistakes-jekyll-theme/" rel="nofollow">Minimal Mistakes</a>.</div>

      </footer>
    </div>

    <script src="http://localhost:4000/assets/js/main.min.js"></script>




  <script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', '', 'auto');
  ga('send', 'pageview');
</script>






  </body>
</html>

