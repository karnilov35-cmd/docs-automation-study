<!doctype html>
<html lang="ru">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>02. Описание API — docs-automation-study</title>
<meta name="description" content="Учебная документация по практической работе 3.4: Docs-as-Code, GitHub Pages, PlantUML, OpenAPI.">
<link rel="stylesheet" href="../assets/style.css">
</head>
<body>
<header class="site-header">
  <div class="wrap">
    <a class="brand" href="../index.html"><span class="brand-mark">DS</span> docs-automation-study</a>
    <nav class="top-nav">
      <a href="../index.html">Главная</a>
      <a href="../docs/01_intro.html">Введение</a>
      <a href="../docs/02_api.html">API</a>
      <a href="../docs/03_report.html">Отчёт</a>
      <a href="../api/index.html">Swagger UI</a>
    </nav>
  </div>
</header>
<div class="layout">
  <aside class="sidebar">
    <h2>Документация</h2>
    <nav>
      <a href="../index.html" class="">Главная</a>
      <a href="../docs/01_intro.html" class="">01. Введение</a>
      <a href="../docs/02_api.html" class="active">02. Описание API</a>
      <a href="../docs/03_report.html" class="">03. Отчёт о работе</a>
      <a href="../api/index.html">Swagger UI</a>
    </nav>
    <div class="meta">
      Практическая работа 3.4<br>
      Docs-as-Code<br><br>
      <span class="badge">main</span>
    </div>
  </aside>
  <main class="content">
<h1 id="api">Описание API</h1>
<p>Функция входа принимает логин и пароль.</p>
<h2 id="_1">Эндпоинт</h2>
<p><code>POST /login</code></p>
<h2 id="_2">Параметры запроса</h2>
<table>
<thead>
<tr>
<th>Поле</th>
<th>Тип</th>
<th>Обязательное</th>
<th>Описание</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>login</code></td>
<td>string</td>
<td>да</td>
<td>Логин пользователя</td>
</tr>
<tr>
<td><code>password</code></td>
<td>string</td>
<td>да</td>
<td>Пароль пользователя</td>
</tr>
</tbody>
</table>
<h2 id="_3">Пример запроса</h2>
<pre><code class="language-json">{
  &quot;login&quot;: &quot;student&quot;,
  &quot;password&quot;: &quot;secret123&quot;
}
</code></pre>
<h2 id="_4">Ответы</h2>
<table>
<thead>
<tr>
<th>Код</th>
<th>Описание</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>200</code></td>
<td>Успешная авторизация, возвращается токен</td>
</tr>
<tr>
<td><code>401</code></td>
<td>Неверный логин или пароль</td>
</tr>
</tbody>
</table>
<h2 id="_5">Интерактивная документация</h2>
<p>Спецификация OpenAPI находится в файле <code>openapi/openapi.yaml</code>.<br>
На её основе Swagger UI строит интерактивный справочник с кнопкой<br>
<strong>Try it out</strong>.</p>
  </main>
</div>
<footer class="site-footer">
  <div class="line">© 2026 Карнилов Д. Е., группа ИСП-241/9. Учебный проект по автоматизации технической документации.</div>
</footer>
</body>
</html>
