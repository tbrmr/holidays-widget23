# holidays-widget
Popup widget with information about holidays.

<h2>add css</h2>
<pre>&lt;link href="https://github.com/tbrmr/holidays-widget23/blob/main/css/holidays.css" rel="stylesheet"&gt;</pre>

<h2>add js</h2>
<pre><script src="https://github.com/tbrmr/holidays-widget23/blob/main/scripts/holidays.js"></script></pre>

<h2>init widget</h2>

<pre>let typeHoliday = 'march8',				//тип праздника, из доступного: новый год (newYear) и 8 марта (march8). "custom" - можно использовать свою иконку. 
    btnText = 'График работы в праздники',	        //текст на кнопке
    detailTitle = 'График работы в праздники:',	        //заголовк внутри виджета
    detailText = '								
      &lt;p&gt;&lt;b&gt;7 марта&lt;/b&gt; - до 17:00&lt;/p&gt;
      &lt;p&gt;&lt;b&gt;8 марта&lt;/b&gt; - выходной&lt;/p&gt;
    ',						        //текст внутри виджета
    bgColor= 'rgba(0,0,0,0)', //цвет фона круга, rgba с нулями - для прозрачности
     widgetPosition = "left", //варианты left/right, по умолчанию right
    icon = '&lt;img src="ball.png"&gt;'; //иконка, если выбран вариант custom
    
let holidays = new Holidays(
            typeHoliday,
            btnText,
            detailTitle,
            detailText,
            bgColor,
            widgetPosition,
            icon
)

holidays.init()</pre>
