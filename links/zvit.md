---
title: Отчет о поиске
layout: index_ru.liquid
permalink: /links/zvit.htm
data:
  relpath: "../"
  p: p6
---
# Отчет об информационном поиске

Представленный отчет позволяет оценить информационную ситуацию по теме магистерской работы.
Он является основным документальным подтверждением глубины и полноты информационного поиска,
а также служит для фиксации текущей ситуации в исследуемой области.

Поиск выполнен с использованием трех поисковых систем (Google, Яндекс, Bing).
Результаты сведены в таблицу. Всего произведено {{ site.data.search.num }} запросов, имеющих отношение к магистерской работе.
Из них три запроса соответствует названию магистерской работы на трех языках,
три запроса с ФИО руководителя, а также девять запросов с ключевыми понятиями по теме магистерской работы.

Ниже приведены две таблицы с отчетами о поиске, которые разделяет временной промежуток в два месяца,
а также ряд диаграмм, которые позволяют сравнить основные изменения, произошедшие за этот период.

<h2 class="cntr">Отчет о поиске за {{ site.data.search.date }} г.</h2>

<div class="cntr">
<table class="search">

<!------------- ЗАГОЛОВОК  ---------------->
<tr>
<td class="c1" style="font-weight: bold; text-align: center;"> Строка поиска</td>
<td class="cn"><a href="http://www.google.com.ua" target="_blank"><img src="../images/google.png" title="Google" border=0></a></td>
<td class="cn"><a href="http://www.yandex.ua" target="_blank"><img src="../images/yandex.png" title="Яндекс" border=0></a></td>
<td class="cn"><a href="http://www.bing.com" target="_blank"><img src="../images/bing.png" title="Bing.com" border=0></a></td>
</tr>

{% if site.data.search.ru %}
<!------------- РУССКИЙ ЯЗЫК  ---------------->
<tr>
<td class="cspan" colspan="4"> <p>На русском языке</p>

{% for result in site.data.search.ru %}

<tr class="result">
<td class="c1">{{ result.text }}</td>
<td class="cn"><a target="_blank" href="{{ result.google_url }}">{{ result.google_total_results }}</a></td>
<td class="cn"><a target="_blank" href="{{ result.yandex_url }}">{{ result.yandex_total_results }}</a></td>
<td class="cn"><a target="_blank" href="{{ result.bing_url }}">{{ result.bing_total_results }}</a></td>
</tr>
{% endfor %}
{% endif %}

{% if site.data.search.ua %}
<!------------- УКРАИНСКИЙ ЯЗЫК  ---------------->
<tr>
<td class="cspan" colspan="4"> <p>На украинском языке</p>

{% for result in site.data.search.ua %}

<tr class="result">
<td class="c1">{{ result.text }}</td>
<td class="cn"><a target="_blank" href="{{ result.google_url }}">{{ result.google_total_results }}</a></td>
<td class="cn"><a target="_blank" href="{{ result.yandex_url }}">{{ result.yandex_total_results }}</a></td>
<td class="cn"><a target="_blank" href="{{ result.bing_url }}">{{ result.bing_total_results }}</a></td>
</tr>
{% endfor %}
{% endif %}

{% if site.data.search.en %}
<!------------- АНГЛИЙСКИЙ ЯЗЫК  ---------------->
<tr>
<td class="cspan" colspan="4"> <p>На английском языке</p>

{% for result in site.data.search.en %}

<tr class="result">
<td class="c1">{{ result.text }}</td>
<td class="cn"><a target="_blank" href="{{ result.google_url }}">{{ result.google_total_results }}</a></td>
<td class="cn"><a target="_blank" href="{{ result.yandex_url }}">{{ result.yandex_total_results }}</a></td>
<td class="cn"><a target="_blank" href="{{ result.bing_url }}">{{ result.bing_total_results }}</a></td>
</tr>
{% endfor %}
{% endif %}

</table>

</div>

