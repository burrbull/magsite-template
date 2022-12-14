---
title: Реферат
layout: index_ru.liquid
permalink: /diss/index.htm
data:
  relpath: "../"
  en: indexe.htm
---
# Реферат по теме выпускной работы

<h2>Содержание</h2>

<ul class=content>
  <li class=ct1><a href="#p0">Введение</a>
  <li class=ct1><a href="#p1">1. Актуальность темы</a>
  <li class=ct1><a href="#p2">2. Цель и задачи исследования, планируемые результаты</a>
  
  <li class=ct1><a href="#p3">3. Обзор исследований и разработок</a>
  <li class=ct2><a href="#p31">3.1 Обзор международных источников</a>
  <li class=ct2><a href="#p32">3.2 Обзор национальных источников</a>
  <li class=ct2><a href="#p33">3.3 Обзор локальных источников</a>
  
  <li class=ct1><a href="#p4">4. Подход к унификации синтеза автоматов Мура в базисе FPGA</a>
  <li class=ct1><a href="#p5">Выводы</a>
  
  <li class=ct1><a href="#ref">Список источников</a>
</ul>

<a name=p0></a>
<h2>Введение</h2>

<p>
Цифровые системы находят широкое применение и являются базовыми компонентами компьютерной техники, автоматики, робототехники,
производства, транспорта. Создание сверхбольших интегральных схем (СБИС), построение систем-на-кристалле (SoC – System-on-Chip),
развитие технологий программируемых пользователем вентильных матриц (FPGAs – Field-Programmable Gate Arrays) и сложных программируемых
логических устройств (CPLDs – Complex Programmable Logic Devices) изменили базис реализации цифровых систем и выдвинули повышенные
требования к процессу их разработки, что привело к широкому распространению систем автоматизированного проектирования (САПР) и
языков описания аппаратуры (HDLs – Hardware Description Languages), которые должны способствовать повышению качества результирующего
продукта, интенсификации проектных работ, всестороннему анализу и тестированию. Кроме того, были созданы новые, базисно-ориентированные
методы синтеза комбинационных и последовательностных логических схем, наибольшая эффективность от применения которых может быть
достигнута путем автоматизации и совместного комбинированного использования с уже известными алгоритмами.
</p>

<p> Модель конечного автомата, предложенная Э. Муром в 1956 году и названная в его честь (автомат Мура), как синхронная последовательностная
схема, является частью многих цифровых систем и применяется при построении устройств управления. Высокая сложность интегральных схем
(которая продолжает повышаться, следуя закону Г. Мура) и теоретический базис автоматных вычислений делает возможной реализацию
комплексных алгоритмов обработки информации. Однако, непосредственная реализация алгоритмов может приводить к неэффективному
использованию ресурсов кристалла и увеличению стоимости проекта.</p>

<a name=p1></a>
<h2>1. Актуальность темы</h2>

<p> Известен ряд методов аппаратурной оптимизации автомата Мура: минимизация количества состояний и их специфическое кодирование,
использование особенностей целевого базиса и алгоритма функционирования, многоуровневая реализация логической схемы. Указанные
методы обладают определенной эффективностью, но, для получения наиболее экономичной реализации автомата, должны применяться совместно.</p>

<p> Магистерская работа посвящена актуальной научной задаче разработки унифицированного подхода к синтезу автоматов Мура, направленного
на уменьшение аппаратурных затрат в результирующем устройстве и включающего алгоритмические, комбинаторные и схемотехнические
оптимизационные приемы. В качестве целевого базиса используются микросхемы FPGA фирмы Xilinx, сочетающие функциональность,
программируемость, реконфигурируемость и доступность широкому потребителю, а инструментальными средствами исследования выступают
САПР Xilinx ISE, Verilog HDL и Java SE.</p>

<a name='p2'></a>
<h2>2. Цель и задачи исследования, планируемые результаты</h2>

<p> Целью исследования является разработка подхода к унификации синтеза автоматов Мура, направленного на уменьшение аппаратурных
затрат в целевой FPGA-микросхеме.</p>

<p>Основные задачи исследования:</p>
<ol>
  <li>Анализ методов минимизации количества состояний в полностью определенных и частичных автоматах Мура.
  <li>Оценка способов уменьшения аппаратурных затрат путем кодирования состояний автоматов Мура.
  <li>Поиск и выявление характеристик существующих методов построения логических схем автоматов Мура и оценка возможностей их применения в базисе FPGA.
  <li>Объединение функционально различных направлений оптимизации автоматов Мура по аппаратурным затратам в унифицированный подход к синтезу и формирование рекомендаций по его использованию.
  <li> Разработка альтернативных вариантов основных этапов унифицированного процесса синтеза автоматов Мура и оценка их эффективности.
</ol>

<p><span class=itl>Объект исследования</span>: синтез автоматов Мура.</p>
<p><span class=itl>Предмет исследования</span>: объединение методов уменьшения аппаратурных затрат при реализации автоматов Мура в базисе микросхем FPGA.</p>

<p>В рамках магистерской работы планируется получение актуальных <span class=itl>научных результатов</span> по следующим направлениям:</p>
<ol>
  <li>Разработка подхода к унификации синтеза автоматов Мура, ориентированного на уменьшение аппаратурных затрат и включающего последние достижения абстрактной и структурной теории автоматов.
  <li>Определение областей применения различных вариантов основных этапов унифицированного процесса синтеза автоматов Мура.
  <li>Модификация известных методов построения логических схем автоматов Мура и оценка эффективности их применения в базисе FPGA.
</ol>

<p> Для экспериментальной оценки полученных теоретических результатов и формирования фундамента последующих исследований, в качестве <span class=itl>практических результатов</span> планируется
разработка кроссплатформенной, настраиваемой и функциональной системы автоматизированного проектирования автоматов Мура (САПРАМ)
со следующими свойствами:</p>
<ol>
  <li>Наличие собственного XML-ориентированного языка описания автоматов Мура.
  <li>Реализация подхода к унификации синтеза автоматов Мура, направленного на базис FPGA-микросхем фирмы Xilinx.
  <li>Возможность управления составом унифицированного процесса синтеза автоматов Мура и вариантами основных его этапов.
  <li>Генерация Verilog-файла, описывающего синтезированный автомат Мура и пригодного для обработки САПР Xilinx ISE с целью погружения в микросхему FPGA.
</ol>

<a name=p3></a>
<h2>3. Обзор исследований и разработок</h2>

<p> Поскольку автоматы Мура являются важной частью цифровых систем, то проблемы их синтеза, анализа, минимизации и реализации были
широко исследованы как американскими, европейскими, японскими учеными, так и отечественными специалистами. Вопросам реализации
цифровых устройств с помощью FPGA и Verilog HDL также посвящен ряд работ, в основном, исследователей западной школы.</p>

<a name=p31></a>
<h3>3.1 Обзор международных источников</h3>

<p> Концепция автомата Мура была сформулирована Э.&nbsp;Муром в его статье &laquo;Gedanken-experiments on sequential machines&raquo; [<a href="#ref1">1</a>]. Там же показана
сфера применения моделей с конечным количеством состояний и рассматривается широкий класс проблем абстрактной теории автоматов.
Другими источниками информации о классификациях, фундаментальных принципах функционирования, способах представления, математическом
смысле и приложениях конечных автоматов могут служить монографии Р.&nbsp;Миллера, А.&nbsp;Гилла, Д.&nbsp;Хопкрофта, М.&nbsp;Минского, М.&nbsp;Ито [<a href="#ref2">2</a>-<a href="#ref6">6</a>].</p>

<p> При разработке цифровых систем, автоматы Мура реализуются как синхронные последовательностные схемы, процессы анализа и синтеза
которых подробно изложены в современных книгах по логическому проектированию В.&nbsp;Нельсона, К.&nbsp;Бридинга, Д.&nbsp;Уэйкерли, М.&nbsp;Мано, Б.&nbsp;Уилкинсона и др. [<a href="#ref7">7</a>-<a href="#ref16">16</a>]. 
Вопросам использования языка описания аппаратуры Verilog при проектировании, моделировании и реализации
цифровых устройств посвящены работы П.&nbsp;Чу, М.&nbsp;Чилетти, П.&nbsp;Ашендена, С.&nbsp;Палниткара, А.К.&nbsp;Полякова [<a href="#ref17">17</a>-<a href="#ref25">25</a>]. 
Микросхемы FPGA – их архитектуры, свойства, области применения – являются предметом рассмотрения у К.&nbsp;Максфилда, И.&nbsp;Гроута, Б.&nbsp;Зайдмана, Р.И.&nbsp;Грушвицкого,
А.Х.&nbsp;Мурсаева, Е.П.&nbsp;Угрюмова [<a href="#ref26">26</a>-<a href="#ref29">29</a>].</p>

<p> В классических работах В.М.&nbsp;Глушкова и С.И.&nbsp;Баранова [<a href="#ref30">30</a>, <a href="#ref31">31</a>] изложена абстрактная и структурная теория автоматов, сформулирован
канонический метод структурного синтеза цифрового автомата, разработаны вопросы матричной реализации логических схем.</p>

<p>Минимизация количества состояний автоматов Мура – важный шаг проектирования, поскольку именно количество состояний определяет
разрядность кодирующего двоичного слова при структурном синтезе. Подходы к решению этой задачи в разное время разрабатывались
и совершенствовались М.&nbsp;Аведилло, Х.&nbsp;Куинтаной и Х.&nbsp;Хуэртасом (алгоритм ARNES, алгоритм SMAS) [<a href="#ref32">32</a>, <a href="#ref33">33</a>]; Х.-М.&nbsp;Чампарнаудом, А.&nbsp;Хорси и 
Т.&nbsp;Парантоэном (модификация алгоритма Бржожовски) [<a href="#ref34">34</a>]; С.&nbsp;Гореном и Ф.&nbsp;Фергюсоном (алгоритм CHESMIN) [<a href="#ref35">35</a>]; 
Х.&nbsp;Хигучи и Ю.&nbsp;Мацунагой (алгоритм SLIM) [<a href="#ref36">36</a>]; Х. Ху, Х.-К. Ксуэ и Д.-Н. Бианом (алгоритм HSM2) [<a href="#ref37">37</a>]; Д.-К.&nbsp;Рхо, Г.&nbsp;Хачтелем, Ф.&nbsp;Соменци 
и Р.&nbsp;Якоби (алгоритм STAMINA) [<a href="#ref38">38</a>]; Д.&nbsp;Хопкрофтом (наиболее эффективный существующий алгоритм минимизации) [<a href="#ref39">39</a>]; Р.&nbsp;Фурером и С.&nbsp;Новиком
(алгоритм OPTIMIST) [<a href="#ref40">40</a>]; Х.&nbsp;Пеной и А.&nbsp;Оливейрой (алгоритм BICA) [<a href="#ref41">41</a>]; Т.&nbsp;Камом, Т.&nbsp;Виллой, Р.&nbsp;Брайтоном и А.&nbsp;Санджиованни-Винцентелли
(алгоритм ISM) [<a href="#ref42">42</a>]. Некоторые методы минимизации полностью определенных и частичных автоматов оценены и описаны в работах [<a href="#ref14">14</a>, <a href="#ref43">43</a>].</p>

<p> Критичным для уровня аппаратурных затрат логической схемы автомата Мура выступает этап кодирования состояний, краткое описание
подходов к которому содержится в обзорной статье А. Слюсарчука [<a href="#ref44">44</a>]. В публикациях Д.&nbsp;Де Мишели, Р.&nbsp;Брайтона, 
А.&nbsp;Санджиованни-Винцентелли, А.&nbsp;Эль-Малеха, С.&nbsp;Саита, Ф.&nbsp;Кхана приведены эффективные алгоритмы кодирования состояний конечных автоматов
и устройств управления на их основе [<a href="#ref45">45</a>-<a href="#ref48">48</a>]. Оригинальные способы оптимизации кодирования и многоуровневой реализации рассмотрены в
работах С.&nbsp;Девадаса, Х.-К.&nbsp;Ма, А.&nbsp;Ньютона и А.&nbsp;Санджиованни-Винцентелли (алгоритм MUSTANG) [<a href="#ref49">49</a>]; К.&nbsp;Ду, Г.&nbsp;Хачтеля, Б.&nbsp;Лина и 
А.&nbsp;Ньютона (алгоритм MUSE) [<a href="#ref50">50</a>]; Х.&nbsp;Кубатовой и М.&nbsp;Беквара (алгоритм FEL-Code) [<a href="#ref51">51</a>]; Б.&nbsp;Лина и А.&nbsp;Ньютона (алгоритм JEDI) [<a href="#ref52">52</a>]; 
Т.&nbsp;Виллы и А.&nbsp;Санджиованни-Винцентелли (алгоритм NOVA) [<a href="#ref53">53</a>]; Б.&nbsp;Гупты, Х.&nbsp;Нараянана и М.&nbsp;Десая (алгоритм Two-Hot Encoding) [<a href="#ref54">54</a>]; 
М.&nbsp;Мартинеса, М.&nbsp;Аведилло, Х.&nbsp;Куинтаны и Х.&nbsp;Хуэртаса (алгоритм DISA) [<a href="#ref55">55</a>]. Известный унитарный способ кодирования состояний и его
приложение к проектированию автоматов для FPGA описаны у С.&nbsp;Голсона [<a href="#ref56">56</a>].</p>

<p>Применение аппарата эволюционных и генетических вычислений к кодированию состояний автоматов рассмотрено в [<a href="#ref57">57</a>-<a href="#ref61">61</a>]. 
Первые параллельные алгоритмы кодирования состояний, предназначенные для выполнения на высокопроизводительной компьютерной технике, –
ProperSTATE и ProperJEDI – были предложены в 1996 году Г.&nbsp;Хастеером в рамках проекта ProperCAD [<a href="#ref62">62</a>]. 
В 2004 году Д.&nbsp;Бадер и К.&nbsp;Маддури представили параллельный алгоритм кодирования состояний, ориентированный на симметричные мультипроцессорные системы
(SMP-системы), относящиеся к классу MIMD [<a href="#ref63">63</a>].
</p>

<p>Аппаратурно-оптимальная реализация логической схемы автомата Мура зависит от используемого целевого базиса. В работах А.А.&nbsp;Баркалова,
Л.А.&nbsp;Титаренко, С.&nbsp;Хмелевского, А.&nbsp;Буковца, Г.&nbsp;Селварая, М.&nbsp;Равски, Т.&nbsp;Лубы, В.А.&nbsp;Склярова, Р.&nbsp;Червински, Д.&nbsp;Каниа рассматриваются
методы построения конечных автоматов на базе CPLD, FPGA и встроенных блоков памяти ROM (Read-Only Memory) [<a href="#ref64">64</a>-<a href="#ref68">68</a>]. 
В статье А.А.&nbsp;Баркалова, Л.А.&nbsp;Титаренко и О.&nbsp;Хебды предлагается способ нестандартного представления кодов состояний, ориентированный на базис CPLD
и позволяющий оптимизировать логическую схему автомата Мура [<a href="#ref69">69</a>]</p>

<p>Комплексный обзор процесса синтеза автоматов Мура и Мили (с акцентом на возможности его автоматизации), а также обширная тематическая
библиография содержится в статье М. Перковски [<a href="#ref70">70</a>]. Примером реализованной программной системы синтеза и оптимизации
последовательностных схем является SIS, разработанная в Калифорнийском университете (США) и подробно освещенная в работе [<a href="#ref71">71</a>].</p>

<a name=p32></a>
<h3>3.2 Обзор национальных источников</h3>

<p>В Одесском национальном политехническом университете Е.Л.&nbsp;Полиным, К.В.&nbsp;Защелкиным, Ю.А.&nbsp;Ковалевым, Е.Н.&nbsp;Ивановой, А.А.&nbsp;Николенко
активно разрабатываются параллельные модели языка граф-схем алгоритмов (ГСА), методы синтеза цифровых управляющих устройств,
абстрактные композиционные автоматы, вопросы информационной технологии автоматизированного проектирования микропрограммных
автоматов [<a href="#ref72">72</a>-<a href="#ref76">76</a>].</p>

<p>И.В.&nbsp;Васильцовым (Тернопольская академия национальной экономики) предложен эволюционный подход к кодированию внутренних состояний
конечного автомата [<a href="#ref77">77</a>], а в статьях Л.А.&nbsp;Шуваловой, Д.Н.&nbsp;Моамара, Т.Ю.&nbsp;Уткиной (Черкасский государственный технологический университет)
[<a href="#ref78">78</a>] и С.Н.&nbsp;Сердюка (Запорожский национальный технический университет) [<a href="#ref79">79</a>] рассмотрены возможности автоматизированного анализа,
синтеза и верификации цифровых автоматов.</p>

<p>Проектирование цифровых устройств в базисе FPGA подробно освещено в работах В.И.&nbsp;Жабина, Н.А.&nbsp;Ковалева (НТУУ &laquo;Киевский политехнический
университет&raquo;) [<a href="#ref80">80</a>] и В.Н.&nbsp;Опанасенко, А.Н.&nbsp;Лисового, Е.В.&nbsp;Сороки (Институт кибернетики им. В.М.&nbsp;Глушкова НАН Украины) [<a href="#ref81">81</a>, <a href="#ref82">82</a>].</p>

<a name=p33></a>
<h3>3.3 Обзор локальных источников</h3>

<p>В Донецком национальном техническом университете (кафедра компьютерной инженерии) широко разрабатываются методы реализации логических
схем конечных автоматов, микропрограммных устройств управления (МУУ) и композиционных микропрограммных устройств управления (КМУУ)
в базисах SPLD (Simple Programmable Logic Device), CPLD, FPGA, ASIC (Application Specific Integrated Circuit).</p>

<p>В книгах А.А.&nbsp;Баркалова и Л.А.&nbsp;Титаренко детально рассмотрены алгоритмы построения управляющих (УА) и операционных (ОА) автоматов,
объединяемых для реализации цифровых устройств [<a href="#ref83">83</a>-<a href="#ref85">85</a>]. В качестве одного из способов организации УА часто используются автоматы Мура
и Мили [<a href="#ref30">30</a>], исследование аппаратурной оптимизации которых позволило авторам разработать ряд оригинальных подходов к синтезу логических
схем УА с &laquo;жесткой логикой&raquo;: многоуровневые структуры, принцип преобразования кодов объектов, возможности модификации исходных
граф-схем алгоритмов (ГСА), реализации на счетчиках, использование блоков памяти.</p>

<p>Статьи А.А.&nbsp;Баркалова, С.А.&nbsp;Ковалева, С.А.&nbsp;Цололо, А.В.&nbsp;Матвиенко, В.А.&nbsp;Саломатина, А.А.&nbsp;Красичкова посвящены оптимизации логической
схемы автомата Мура, реализуемой на CPLD, однородных программируемых логических интегральных схемах (ПЛИС), FPGA [<a href="#ref86">86</a>-<a href="#ref90">90</a>]. Авторы
предлагают использовать понятие псевдоэквивалентности состояний, особенности целевого базиса, специфические способы кодирования
внутренних состояний. Для эффективной реализации автоматов Мура на заказных схемах (ASICs), А.А.&nbsp;Баркаловым, Р.В.&nbsp;Мальчевой и 
К.А.&nbsp;Солдатовым были предложены метод кодирования наборов микроопераций и принцип расширения кодов состояний перехода [<a href="#ref91">91</a>, <a href="#ref92">92</a>].</p>

<p>Тематика адаптации UML (Unified Modeling Language), MDA (Model-Driven Architecture) и высокопроизводительных компьютерных технологий
(параллельных и распределенных систем) к синтезу и моделированию УА широко освещена в публикациях А.А.&nbsp;Баркалова, И.Я.&nbsp;Зеленёвой, 
А.А.&nbsp;Гриценко, С.А.&nbsp;Ковалева [<a href="#ref93">93</a>-<a href="#ref96">96</a>].</p>

<a name=p4></a>
<h2>4. Подход к унификации синтеза автоматов Мура в базисе FPGA</h2>
      
<p>Первые микросхемы FPGA были разработаны фирмой Xilinx в 1984 году и приобрели большую популярность, благодаря возможности реализации
сложных функций и относительно небольшой стоимости. Современные FPGA сочетают программируемость SPLD и CPLD, сохраняя основное
преимущество ASIC – объем реализуемых функций [<a href="#ref27">27</a>].</p>

<p>Неоптимизированные проекты цифровых систем, независимо от базиса реализации, могут иметь значительную избыточность и, следовательно,
неэффективно использовать аппаратные ресурсы [<a href="#ref84">84</a>]. Это приводит к актуализации задачи аппаратурной оптимизации, которая, в контексте
FPGA, сводится к снижению процента использования тех или иных внутренних блоков: LUT-элементов (LUT – Look-Up Table), модулей памяти,
схем синхронизации.</p>

<p> Аппаратурно-оптимальная реализация автоматов Мура требует совместного применения результатов абстрактной и структурной теории
автоматов: минимизации количества состояний (уменьшение мощности множества состояний автомата и, как следствие, разрядности двоичного
кода состояния), эффективного кодирования состояний (снижение уровня затрат при реализации функций следующего состояния), адаптации
логической схемы к используемому базису (качественное распределение ресурсов кристалла за счет использования встроенных блоков памяти
и особенностей организации внутренних модулей).</p>

<p>В статье [<a href="#ref97">97</a>] предлагается подход к унификации синтеза автоматов Мура, объединяющий указанные возможности оптимизации и направленный
на базис микросхем FPGA (рис. 1). Сущность этого подхода заключается в последовательном применении алгоритмического, комбинаторного
и схемотехнического этапов и использовании FPGA-ориентированных инструментальных средств: САПР и HDLs.</p>

<div class=img>
  <img src="images/unification_process.png" width=682 height=589 alt="Подход к унификации синтеза автоматов Мура">
  <p class=imgcaption>Рисунок 1 – Подход к унификации синтеза автоматов Мура</p>
</div>

<p>На первом шаге алгоритмического этапа синтеза, произвольная спецификация автомата Мура приводится к единому виду – таблице переходов.
Необходимость приведения связана с тем, что автомат Мура может быть задан с использованием различных форм представления: граф-схем,
диаграмм состояний, ASM-диаграмм (ASM – Algorithmic State Machine) [<a href="#ref13">13</a>, <a href="#ref14">14</a>, <a href="#ref83">83</a>]. Второй шаг алгоритмического этапа состоит в
минимизации количества состояний таблицы переходов. Для этого могут использоваться алгоритмы Бржожовски, ARNES, SMAS, CHESMIN,
SLIM, HSM2, STAMINA, OPTIMIST, BICA, ISM [<a href="#ref14">14</a>, <a href="#ref32">32</a>-<a href="#ref43">43</a>].</p>

<p>Комбинаторный этап направлен на эффективное кодирование состояний минимизированной таблицы переходов, а также получение
аппаратурно-минимальных функций следующего состояния и, при необходимости, выходных функций автомата. Значительное влияние способа
кодирования состояний на параметры результирующей логической схемы обусловило разработку различных подходов, направленных на
снижение расхода мощности, повышение быстродействия, минимизацию аппаратурных затрат. Последний из этих подходов может быть
использован на комбинаторном этапе синтеза путем применения, адаптации или модификации алгоритмов MUSTANG, MUSE, FEL-Code, JEDI,
NOVA, Two-Hot Encoding, DISA, унитарного и позиционно-двоичного кодирования состояний [<a href="#ref44">44</a>-<a href="#ref63">63</a>, <a href="#ref84">84</a>].</p>

<p>Схемотехнический этап процесса синтеза предполагает использование методов построения логической схемы автомата Мура, направленных
на уменьшение аппаратурных затрат целевой микросхемы. К таким методам относятся тривиальные и многоуровневые реализации,
структуры с преобразованием кодов объектов, схемы на счетчиках [<a href="#ref84">84</a>]. Поскольку современное цифровое проектирование на микросхемах
FPGA ориентировано на использование HDLs (в основном, VHDL и Verilog), то вторым шагом схемотехнического этапа выступает разработка
HDL-программы, описывающей автомат Мура и пригодной для обработки соответствующей САПР и погружения в микросхему.</p>

<p>Описанный унифицированный процесс синтеза может быть с успехом реализован автоматизированно и предполагать только управленческие
функции пользователя: описание автомата Мура и выбор используемых алгоритмов и структур. Кроме того, представленный подход
может применяться к ряду других современных базисов (CPLD, ASIC) и определять общее направление оптимизационных работ при синтезе
логических последовательностных схем.</p>

<p>Для оценки эффективности применения унифицированного процесса синтеза к конкретному примеру, были разработаны пять Verilog-программ,
описывающих заданный автомат Мура [<a href="#ref8">8</a>] (рис. 2) различными способами:</p>

<ol>
  <li>Реализация неминимизированного автомата Мура с помощью анализатора XST (Xilinx Synthesis Technology) [<a href="#ref98">98</a>]  (эксперимент 1).
  <li>Реализация минимизированного автомата Мура с помощью анализатора XST (эксперимент 2).
  <li>Реализация минимизированного автомата Мура по двухуровневой схеме [<a href="#ref85">85</a>] с позиционно-двоичным кодированием состояний.
      Использование ROM с асинхронным чтением [<a href="#ref98">98</a>] (эксперимент 3).
  <li>Реализация минимизированного автомата Мура по двухуровневой схеме с позиционно-двоичным кодированием состояний.
      Использование ROM с синхронным чтением [<a href="#ref98">98</a>] и дополнительного сигнала синхронизации (эксперимент 4).
  <li>Реализация минимизированного автомата Мура по двухуровневой схеме с позиционно-двоичным кодированием состояний.
      Использование ROM с синхронным чтением и заднего фронта основного сигнала синхронизации (эксперимент 5).
</ol>

<div class=img>
  <img src="images/animation.gif" width=594 height=420 alt="Диаграмма состояний автомата Мура">
  <p class=imgcaption>
  Рисунок 2 – Диаграмма состояний автомата Мура<br>(анимация: 10 кадров, 5 циклов повторения, 160 килобайт)<br>
  (<i>x<sub>i</sub></i> – входные сигналы, <i>y<sub>i</sub></i> – биты кода состояния, <i>z<sub>i</sub></i> – выходные сигналы)
  </p>
</div>

<p>Все исследования проводились с помощью САПР Xilinx ISE 13.1 для семейства FPGA Xilinx Spartan-3, а именно для микросхемы XC3S200.
Результаты совокупных аппаратурных затрат для пяти вариантов реализации графически показаны на рис. 3.</p>

<div class=img>
  <img src="images/synthesis_results.png" width=545 height=377 alt="Результаты экспериментальных исследований">
  <p class=imgcaption>Рисунок 3 – Результаты экспериментальных исследований</p>
</div>

<p>Если целью оптимизации являлось количество LUT-ячеек, то лучший результат был получен при использовании двухуровневой реализации
минимизированного автомата Мура с синхронным ROM и двумя сигналами синхронизации (эксперимент 4). По сравнению с экспериментом 1,
количество слайсов уменьшилось в 3 раза, количество триггеров – в 1,5 раза, а количество LUT-ячеек – в 2,5 раза. Однако, в этом
случае увеличилось общее количество выводов схемы, количество сигналов синхронизации и был задействован один модуль RAM (Random Access Memory).</p>

<a name=p5></a>
<h2>Выводы</h2>

<p>Качественный синтез цифровых систем, и автоматов Мура в частности, является одним из направлений логического проектирования и
представляет не только теоретико-исследовательский, но и практический интерес. Разработка оптимальных цифровых устройств открывает
путь к более полному использованию возможностей базиса реализации, &laquo;уплотнению&raquo; проектов, уменьшению материальных затрат.</p>

<p>Магистерская работа посвящена актуальной научной задаче объединения основных методов аппаратурной минимизации автоматов Мура.
В рамках проведенных исследований выполнено:</p>

<ol>
  <li>Разработана структура унифицированного процесса синтеза автоматов Мура и определены функции ее составляющих.
  <li>На основании анализа литературных источников выделены основные алгоритмы, которые могут быть использованы в предложенном подходе к унификации синтеза автоматов Мура.
  <li>Проведен ряд экспериментов по использованию унифицированного процесса синтеза автоматов Мура, проанализированы полученные результаты.
  <li>Рассмотрены возможности комплексной автоматизации разработанного подхода к унификации синтеза автоматов Мура,
      оценены требования к программному обеспечению, выполнен поиск функционально подобных программных продуктов синтеза
      последовательностных логических схем.
</ol>

<p>Дальнейшие исследования направлены на следующие аспекты:</p>
<ol>
  <li>Качественное совершенствование предложенного подхода к унификации синтеза автоматов Мура, его дополнение и расширение.
  <li>Определение границ эффективности различных вариантов основных этапов унифицированного процесса синтеза автоматов Мура.
  <li>Адаптация известных методов построения логических схем автоматов Мура к базису FPGA.
  <li>Разработка кроссплатформенной и функциональной системы автоматизированного проектирования автоматов Мура (САПРАМ), реализующей предложенный унифицированный процесс синтеза.
</ol>
        
<p>При написании данного реферата магистерская работа еще не завершена. Окончательное завершение: декабрь 2011 года. Полный текст работы
и материалы по теме могут быть получены у автора или его руководителя после указанной даты.</p>

<a name=ref></a>
<h2>Список источников</h2>
<ol>
  <li><a name="ref1"></a>Moore E.F. Gedanken-experiments on sequential machines / E.F. Moore // Automata studies, Annals of mathematical studies. – 1956. – vol. 34. – pp. 129-153.
  <li><a name="ref2"></a>Гилл А. Введение в теорию конечных автоматов / А. Гилл. – М.: Наука, 1966. – 272 с.
  <li><a name="ref3"></a>Миллер Р. Теория переключательных схем / Р. Миллер. – М.: Наука, 1971. – Том 2: Последовательностные схемы и машины. – 304 с.
  <li><a name="ref4"></a>Минский М. Вычисления и автоматы / М. Минский. – М.: Мир, 1971. – 364 с.
  <li><a name="ref5"></a>Хопкрофт Д. Введение в теорию автоматов, языков и вычислений / Д. Хопкрофт, Р. Мотвани, Д. Ульман. – М.: Издательский дом &laquo;Вильямс&raquo;, 2002. – 528 с.
  <li><a name="ref6"></a>Ito M. Algebraic theory of automata and languages / M. Ito. – World Scientific Publishing, 2004. – 199 pp.
  <li><a name="ref7"></a>Голдсуорт Б. Проектирование цифровых логических устройств / Б. Голдсуорт. – М.: Машиностроение, 1985. – 288 с.
  <li><a name="ref8"></a>Уилкинсон Б. Основы проектирования цифровых схем / Б. Уилкинсон. – М.: Издательский дом &laquo;Вильямс&raquo;, 2004. – 320 с.
  <li><a name="ref9"></a>Уэйкерли Д. Проектирование цифровых устройств / Д. Уэйкерли. – М.: Постмаркет, 2002. – Том 2. – 528 с.
  <li><a name="ref10"></a>Breeding K. Digital design fundamentals / K. Breeding. – Prentice Hall, 1992. – 446 pp.
  <li><a name="ref11"></a>Holdsworth B. Digital logic design / B. Holdsworth, C. Woods. – Prentice Hall, 2002. – 519 pp.
  <li><a name="ref12"></a>Lala P. Principles of modern digital design / P. Lala. – Wiley, 2007. – 419 pp.
  <li><a name="ref13"></a>Mano M. Digital design / M. Mano. – Prentice Hall, 2003. – 516 pp.
  <li><a name="ref14"></a>Nelson V. Digital logic circuit analysis and design / V. Nelson, H. Nagle, J. Irwin, B. Carroll. – Prentice Hall, 1995. – 842 pp.
  <li><a name="ref15"></a>Shiva S. Introduction to logic design / S. Shiva. – CRC Press, 1998. – 628 pp.
  <li><a name="ref16"></a>Singh A. Foundation of switching theory and logic design / A. Singh. – New Age International, 2008. – 412 pp.
  <li><a name="ref17"></a>Поляков А.К. Языки VHDL и VERILOG в проектировании цифровой аппаратуры / А.К. Поляков. – М.: СОЛОН-Пресс, 2003. – 320 с.
  <li><a name="ref18"></a>Ashenden P. Digital design: an embedded systems approach using Verilog / P. Ashenden. – Morgan Kaufmann Publishers, 2008. – 557 pp.
  <li><a name="ref19"></a>Chu P. FPGA prototyping by Verilog examples / P. Chu. – Wiley, 2008. – 488 pp.
  <li><a name="ref20"></a>Ciletti M. Advanced digital design with the Verilog HDL / M. Ciletti. – Prentice Hall, 2005. – 986 pp.
  <li><a name="ref21"></a>Minns P. FSM-based digital design using Verilog HDL / P. Minns, I. Elliott. – Wiley, 2008. – 391 pp.
  <li><a name="ref22"></a>Lee J. Verilog quickstart: a practical guide to simulation and synthesis in Verilog / J. Lee. – Springer, 2002. – 355 pp.
  <li><a name="ref23"></a>Lee W. Verilog coding for logic synthesis / W. Lee. – Wiley, 2003. – 336 pp.
  <li><a name="ref24"></a>Padmanabhan T. Design through Verilog HDL / T. Padmanabhan, B. Bala Tripura Sundari. – Wiley, 2004. – 455 pp.
  <li><a name="ref25"></a>Palnitkar S. Verilog HDL. A guide to digital design and synthesis / S. Palnitkar. – SunSoft Press, 1996. – 396 pp.
  <li><a name="ref26"></a>Грушвицкий Р.И. Проектирование систем на микросхемах программируемой логики / Р.И. Грушвицкий, А.Х. Мурсаев, Е.П. Угрюмов. – СПб.: БХВ-Петербург, 2002. – 608 с.
  <li><a name="ref27"></a>Максфилд К. Проектирование на ПЛИС. Курс молодого бойца / К. Максфилд. – М.: Издательский дом &laquo;Додэка-XXI&raquo;, 2007. – 408 с.
  <li><a name="ref28"></a>Grout I. Digital systems design with FPGAs / I. Grout. – Elsevier, 2008. – 724 pp.
  <li><a name="ref29"></a>Zeidman B. Designing with FPGAs and CPLDs / B. Zeidman. – Elsevier, 2002. – 224 pp.
  <li><a name="ref30"></a>Баранов С.И. Синтез микропрограммных автоматов (граф-схемы и автоматы) / С.И. Баранов. – Л.: Энергия, 1979. – 232 с.
  <li><a name="ref31"></a>Глушков В.М. Синтез цифровых автоматов / В.М. Глушков. – М.: Государственное издательство физико-математической литературы, 1962. – 476 с.
  <li><a name="ref32"></a>Avedillo M.J. New approach to the state reduction in incompletely specified sequential machines / M.J. Avedillo, J.M. Quintana, J.L. Huertas // Proceedings of IEEE International Symposium on Circuits and Systems. – New Orleans, 1990. – pp. 440-443.
  <li><a name="ref33"></a>Avedillo M.J. SMAS: a program for the concurrent state reduction and state assignment of finite state machines / M.J. Avedillo, J.M. Quintana, J.L. Huertas // Proceedings of IEEE International Symposium on Circuits and Systems. – 1991. – vol. 3. – pp. 1781-1784.
  <li><a name="ref34"></a>Champarnaud J.-M. Split and minimizing: Brzozowski's algorithm / J.-M. Champarnaud, A. Khorsi, T. Paranthoen // Prague Stringology Conference. – Prague, 2002. – pp. 96-104.
  <li><a name="ref35"></a>Goren S. CHESMIN: a heuristic for state reduction in incompletely specified finite state machines / S. Goren, F. Ferguson // Proceedings of the Conference on Design, Automation and Test in Europe. – 2002. – pp. 248-254.
  <li><a name="ref36"></a>Higuchi H. A fast state reduction algorithm for incompletely specified finite state machines / H. Higuchi, Y. Matsunaga // 33rd Annual Conference of Design Automation. – Las Vegas, 1996. – pp. 463-466.
  <li><a name="ref37"></a>Hu H. HSM2: a new heuristic state minimization algorithm for finite state machine / H. Hu, H.-X. Xue, J.-N. Bian // Journal of Computer Science and Technology. – 2004. – № 19 (5). – pp. 729-733.
  <li><a name="ref38"></a>Rho J.-K. Exact and heuristic algorithms for the minimization of incompletely specified state machines / J.-K. Rho, G. Hachtel, F. Somenzi, R. Jacoby // IEEE Transactions on Computer-Aided Design. – 1994. – vol. 13. – pp. 167-177.
  <li><a name="ref39"></a>Xu Y. Describing an n log n algorithm for minimizing states in deterministic finite automaton [Электронный ресурс]. – Режим доступа: <a href="http://www.cs.sun.ac.za/rw711/documentation/hopcroft2.pdf">http://www.cs.sun.ac.za...</a>.
  <li><a name="ref40"></a>Fuhrer R.M. OPTIMIST: state minimization for optimal 2-level logic implementation / R.M. Fuhrer, S.M. Nowick // Proceedings of International Conference of Computer-Aided Design. – 1997. – pp. 308-315.
  <li><a name="ref41"></a>Pena J.M. A new algorithm for exact reduction of incompletely specified finite state machines / J.M. Pena, A.L. Oliveira // IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems. – 1999. – vol. 18 (11). – pp. 1619-1632.
  <li><a name="ref42"></a>Kam T. A fully implicit algorithm for exact state minimization / T. Kam, T. Villa, R. Brayton, A. Sangiovanni-Vincentelli // Proceedings of the Design Automation Conference. – 1994. – pp. 684-690.
  <li><a name="ref43"></a>Almeida M. On the performance of automata minimization algorithms / M. Almeida, N. Moreira, R. Reis // Technical Report Series: DCC-2007-03. – 2007. – 12 pp.
  <li><a name="ref44"></a>Slusarczyk A. State assignment techniques – short review [Электронный ресурс]. – Режим доступа: <a href="http://web.cecs.pdx.edu/~mperkows/nov17/051.slusarczyk-state-assignment-review.pdf">http://web.cecs.pdx.edu/~mperkows...</a>.
  <li><a name="ref45"></a>De Micheli G. KISS: a program for optimal state assignment of finite state machines / G. De Micheli, R. Brayton, A. Sangiovanni-Vincentelli // Proceedings of IEEE International Conference of Computer-Aided Design. – Santa Clara, 1984. – pp. 209-211.
  <li><a name="ref46"></a>De Micheli G. Optimal state assignment for finite state machines / G. De Micheli, R. Brayton, A. Sangiovanni-Vincentelli // IEEE Transactions on Computer-Aided Design. – 1985. – pp. 269-285.
  <li><a name="ref47"></a>De Micheli G. Optimal encoding of control logic / G. De Micheli // Proceedings of the International Conference on Circuits and Computer Design. – 1984. – pp. 16-22.
  <li><a name="ref48"></a>El-Maleh A. Finite state machine state assignment for area and power minimization / A. El-Maleh, S.M. Sait, F.N. Khan // Proceedings of IEEE International Symposium on Circuits and Systems. – 2006. – pp. 5303-5306.
  <li><a name="ref49"></a>Devadas S. MUSTANG: state assignment of finite state machines targeting multilevel logic implementations / S. Devadas, H.-K. Ma, A.R. Newton, A. Sangiovanni-Vincentelli // IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems. – 1998. – vol. 7 (12). – pp. 1290-1300.
  <li><a name="ref50"></a>Du X. MUSE: a multilevel symbolic encoding algorithm for state assignment / X. Du, G. Hachtel, B. Lin, A.R. Newton // IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems. – 1991. – vol. 10 (1). – pp. 28-38.
  <li><a name="ref51"></a>Kubatova H. FEL-Code: FSM internal state encoding method / H. Kubatova, M. Becvar // Proceedings of 5th International Workshop on Boolean Problems. – Freiberg, 2002. – pp. 109-114.
  <li><a name="ref52"></a>Lin B. Synthesis of multiple level logic from symbolic high-level description languages / B. Lin, A.R. Newton // Proceedings of the International Conference on VLSI. – Munich, 1989. – pp. 187-196.
  <li><a name="ref53"></a>Villa T. NOVA: state assignment of finite-state machines for optimal two-level logic implementation / T. Villa, A. Sangiovanni-Vincentelli // IEEE Transactions on Computer-Aided Design. – 1990. – pp. 905-924.
  <li><a name="ref54"></a>Gupta, B.N.V.M. A state assignment scheme targeting performance and area / B.N.V.M. Gupta, H. Narayanan, M.P. Desai // Proceedings of 12th International Conference on VLSI Design. – 1999. – pp. 378-383.
  <li><a name="ref55"></a>Martinez M. A dynamic model for the state assignment problem / M. Martinez, M.J. Avedillo, J.M. Quintana, J.L. Huertas // Proceedings of Design, Automation and Test in Europe. – Paris, 1998. – pp. 835-839.
  <li><a name="ref56"></a>Golson S. One-hot state machine design for FPGAs / S. Golson // Proceedings of the 3rd PLD Design Conference. – Santa Clara, 1993. – pp. 1-6.
  <li><a name="ref57"></a>Almaini A. State assignment of finite state machines using a genetic algorithm / A. Almaini, J. Miller, P. Thomson, S. Billina // IEEE Proceedings on Computer and Digital Techniques. – 1995. – pp. 279-286.
  <li><a name="ref58"></a>Amaral J. Designing genetic algorithms for the state assignment problem / J. Amaral, K. Turner, J. Chosh // IEEE Transactions on Systems, Man, and Cybernetics. – 1995. – vol. 25. – pp. 659-694.
  <li><a name="ref59"></a>Chyzy M. Evolutionary algorithm for state assignment of finite state machines / M. Chyzy, W. Kosinski // Artificial Intelligence Methods. – Gliwice, 2003. – pp. 51-52.
  <li><a name="ref60"></a>Nedjah N. Evolutionary synthesis of synchronous finite state machines / N. Nedjah, L.M. Mourelle // Evolvable Machines. – Berlin, 2004. – pp. 103-128.
  <li><a name="ref61"></a>Chattopadhyay S. Area conscious state assignment with flip-flop and output polarity selection for finite state machine synthesis – a genetic algorithm approach / S. Chattopadhyay // The Computer Journal. – 2005. – vol. 48 (4). – pp. 443-450.
  <li><a name="ref62"></a>Hasteer G. Parallel algorithms for state assignment of finite state machines. Master's thesis. – University of Illinois, 1996. – 58 pp.
  <li><a name="ref63"></a>Bader D.A. A parallel state assignment algorithm for finite state machines / D.A. Bader, K. Madduri // Proceedings of IEEE Conference on High-Performance Computing. – Bangalore, 2004. – pp. 297-308.
  <li><a name="ref64"></a>Sklyarov V. Synthesis and implementation of RAM-based finite state machines in FPGAs / V. Sklyarov // Proceedings of Conference on Field Programmable Logic. – Villach, 2000. – pp. 718-728.
  <li><a name="ref65"></a>Barkalov A. Optimization of Moore FSM implemented with CPLD based on PAL macrocells / A. Barkalov, L. Titarenko, S. Chmielewski // Радиотехника. – 2008. – № 155. – pp. 191-195.
  <li><a name="ref66"></a>Bukowiec A. State machines synthesis and implementation into FPGAs with multiple encoding of states / A. Bukowiec, A. Barkalov, L. Titarenko // Radioelectronics and Informatics. – 2008. – № 4. – pp. 43-48.
  <li><a name="ref67"></a>Czerwinski R. Synthesis of finite state machines for CPLDs / R. Czerwinski, D. Kania // International Journal of Applied Mathematics and Computer Science – Special Section: Robot Control Theory. – 2009. – vol. 19 (4). – pp. 647-659.
  <li><a name="ref68"></a>Selvaraj H. FSM implementation in embedded memory blocks of programmable logic devices using functional decomposition / H. Selvaraj, M. Rawski, T. Luba // Proceedings of International Conference on Information Technology: Coding and Computing. – Las Vegas, 2002. – pp. 355-360.
  <li><a name="ref69"></a>Barkalov A. Synthesis of Moore finite state machine with nonstandard presentation of state codes / A. Barkalov, L. Titarenko, O. Hebda // Proceedings of KNWS'2010. – Swinoujscie, 2010. – pp. 11-14.
  <li><a name="ref70"></a>Perkowski M. Digital design automation – finite state machine design [Электронный ресурс]. – Режим доступа: <a href="http://web.cecs.pdx.edu/~mperkows/PerkowskiGoogle/finite-sm.pdf">http://web.cecs.pdx.edu/~mperkows...</a>.
  <li><a name="ref71"></a>Sentovich E.M. SIS: a system for sequential circuit synthesis / E.M. Sentovich, K.J. Singh, L. Lavagno, C. Moon, R. Murgai, A. Saldanha, H. Savoj, P.R. Stephan, R.K. Brayton, A. Sangiovanni-Vincentelli // Technical Report UCB/ERL M92/41. – Berkley, 1992. – 52 pp.
  <li><a name="ref72"></a>Защелкин К.В. Информационная технология автоматизированного проектирования цифровых управляющих устройств / К.В. Защелкин, Е.Н. Иванова // Электромашиностроение и электрооборудование. – 2009. – № 72. – С. 68-72.
  <li><a name="ref73"></a>Николенко А.А. Алгоритмические особенности автоматизированного проектирования микропрограммных автоматов / А.А. Николенко, Ю.А. Ковалев, К.В. Защелкин // Электромашиностроение и электрооборудование. – 2000. – № 54. – С. 91-95.
  <li><a name="ref74"></a>Полин Е.Л. Абстрактные композиционные автоматы / Е.Л. Полин, К.В. Защелкин // Труды Одесского политехнического университета. – Одесса, 2006. – № 1 (25). – С. 88-94.
  <li><a name="ref75"></a>Полин Е.Л. Параллельная модель языка граф-схем алгоритмов и ее интерпретация абстрактными автоматами / Е.Л. Полин, К.В. Защелкин // Электромашиностроение и электрооборудование. – 2005. – № 65. – С. 70-79.
  <li><a name="ref76"></a>Полин Е.Л. Язык кластерных граф-схем алгоритмов и основанный на нем метод синтеза цифровых управляющих устройств / Е.Л. Полин, К.В. Защелкин // Электромашиностроение и электрооборудование. – 2008. – № 71. –С. 68-73.
  <li><a name="ref77"></a>Vasiltsov I. Evolutionary technique to elementary coding of the internal states of the state machine / I. Vasiltsov // Proceedings of the 2002 NASA/DoD Conference on Evolvable Hardware. – 2002. – pp. 63-64.
  <li><a name="ref78"></a>Шувалова Л.А. Структура программного комплекса синтеза и верификации моделей цифровых автоматов / Л.А. Шувалова, Д.Н. Моамар, Т.Ю. Уткина // Системи обробки інформації. – Харьков, 2010. – № 5.  – С. 149-152.
  <li><a name="ref79"></a>Сердюк С.М. Аналізатор скінченних цифрових автоматів / С.М. Сердюк // Вісник Житомирського державного технологічного університету. – Житомир, 2010. – № 1 (52). – С. 146-151.
  <li><a name="ref80"></a>Жабин В.И. Исследование методов построения вычислительных устройств на основе FPGA / В.И. Жабин, Н.А. Ковалев // Технология и конструирование в электронной аппаратуре. – 2002. – № 2. – С. 35-39.
  <li><a name="ref81"></a>Опанасенко В.Н. Проектирование и физическая верификация цифровых устройств на ПЛИС / В.Н. Опанасенко, А.Н. Лисовый, Е.В. Сорока // Комп'ютерні засоби, мережі та системи. – 2008. – № 7. – С. 76-85.
  <li><a name="ref82"></a>Опанасенко В.М. Формалізація процесу проектування обчислювальних пристроїв та систем на базі ПЛІС / В.М. Опанасенко, О.М. Лісовий // Комп'ютерні засоби, мережі та системи. – 2009. – № 8. – С. 58-63.
  <li><a name="ref83"></a>Barkalov A.A. Synthesis of operational and control automata / A.A. Barkalov, L.A. Titarenko. – Donetsk: DonNTU, TechPark DonNTU UNITECH, 2009. – 256 pp.
  <li><a name="ref84"></a>Баркалов А.А. Синтез микропрограммных автоматов на заказных и программируемых СБИС / А.А. Баркалов, Л.А. Титаренко. – Донецк: ДонНТУ, Технопарк ДонНТУ УНИТЕХ, 2009. – 336 с.
  <li><a name="ref85"></a>Баркалов А.А. Синтез устройств управления на программируемых логических устройствах / А.А. Баркалов. – Донецк: ДонНТУ, 2002. – 262 с.
  <li><a name="ref86"></a>Баркалов А.А. Оптимизация схемы МПА Мура на CPLD / А.А. Баркалов, С.А. Ковалев, С.А. Цололо // Материалы Восьмого международного научно-практического семинара &laquo;Практика и перспективы развития партнерства в сфере высшей школы&raquo;. – Донецк-Таганрог, 2007. – Том 3. – С. 26-36.
  <li><a name="ref87"></a>Баркалов А.А. Оптимизация логической схемы автомата Мура на FPGA / А.А. Баркалов, А.А. Красичков, С.А. Цололо // Наукові праці ДонНТУ. – Донецк, 2006. – (Серия &laquo;Проблеми моделювання та автоматизації проектування динамічних систем&raquo;). – № 5 (116). – С. 162-168.
  <li><a name="ref88"></a>Баркалов А.А. Оптимизация логической схемы автомата Мура на CPLD / А.А. Баркалов, А.В. Матвиенко, С.А. Цололо // Комп'ютерні засоби, мережі та системи. – 2007. – № 6. – С. 46-51.
  <li><a name="ref89"></a>Баркалов А.А. Оптимизация схемы автомата Мура на однородных ПЛИС / А.А. Баркалов, А.В. Матвиенко, С.А. Цололо // Комп'ютерні засоби, мережі та системи. – 2009. – № 8. – С. 45-51.
  <li><a name="ref90"></a>Баркалов А.А. Исследование смешанного кодирования состояний для автомата Мура / А.А. Баркалов, В.А. Саломатин, А.А. Красичков, С.А. Цололо // Материалы III научно-практической конференции &laquo;Донбас-2020: наука і техніка – виробництву&raquo;. – Донецк, 2006. – С. 459-562.
  <li><a name="ref91"></a>Баркалов А.А. Матричная реализация автомата Мура с кодированием наборов микроопераций / А.А. Баркалов, Р.В. Мальчева, К.А. Солдатов // Наукові праці ДонНТУ. – Донецк, 2010. –  (Серия &laquo;Проблеми моделювання та автоматизації проектування&raquo;). – № 8 (168). – С. 133-143.
  <li><a name="ref92"></a>Баркалов А.А. Матричная реализация автомата Мура с расширением кодов состояний перехода / А.А. Баркалов, Р.В. Мальчева, К.А. Солдатов // Наукові праці ДонНТУ. – Донецк, 2010. – (Серия &laquo;Інформатика, кібернетика та обчислювальна техніка&raquo;). – № 11 (164). – С. 79-83.
  <li><a name="ref93"></a>Баркалов А.А. Адаптация MDA для моделирования управляющих автоматов в стандартах UML / А.А. Баркалов, И.Я. Зеленёва, А.А. Гриценко // Радіоелектроніка, інформатика, управління. – Запорожье, 2006. – № 1 (15). – С. 33-37.
  <li><a name="ref94"></a>Баркалов А.А. Проектирование и реализация цифровых систем управления с использованием MDA / А.А. Баркалов, И.Я. Зеленёва, А.А. Гриценко // Материалы III научно-практической конференции &laquo;Донбас-2020: наука і техніка – виробництву&raquo;. – Донецк, 2006. – С. 463-467.
  <li><a name="ref95"></a>Баркалов А.А. Синтез управляющих автоматов с использованием распределенных и параллельных систем // А.А. Баркалов, И.Я. Зеленёва, А.А. Гриценко // Радіоелектроніка, інформатика, управління. – Запорожье, 2010. – № 1 (22). – С. 128-134.
  <li><a name="ref96"></a>Баркалов А.А. Модельно-ориентированный подход к разработке САПР управляющих автоматов / А.А. Баркалов, И.Я. Зеленёва, С.А. Ковалев, А.А. Гриценко // Материалы Пятого международного научно-практического семинара &laquo;Практика и перспективы развития партнерства в сфере высшей школы&raquo;. – Донецк-Таганрог, 2006. – Том 1. – С. 38-43.
  <li><a name="ref97"></a>Ковалев С.А. Подход к унификации процесса синтеза МПА Мура для FPGA / С.А. Ковалев, И.Я. Зеленёва, Е.Р. Татолов // Материалы Двенадцатого международного научно-практического семинара &laquo;Практика и перспективы развития партнерства в сфере высшей школы&raquo;. – Донецк-Таганрог, 2011. – Том 2. – С. 45-48.
  <li><a name="ref98"></a>XST User Guide for Virtex-4, Virtex-5, Spartan-3, and Newer CPLD Devices [Электронный ресурс]. – Режим доступа: <a href="http://www.xilinx.com/support/documentation/sw_manuals/xilinx13_1/xst.pdf">http://www.xilinx.com/support...</a>.
</ol>
