# holidays-widget
Popup widget with information about holidays.

#add css
<link href="https://github.com/cookie7889/holidays-widget/blob/main/css/holidays.css" rel="stylesheet">

#add js
<script src="https://github.com/cookie7889/holidays-widget/blob/main/scripts/holidays.js"></script>

#init widget
let typeHoliday = 'march8',						//тип праздника, из доступного: новый год (newYear) и 8 марта (march8)
    btnText = 'График работы в праздники',		//текст на кнопке
    detailTitle = 'График работы в праздники:',	//заголовк внутри виджета
    detailText = `								
      <p><b>7 марта</b> - до 17:00</p>
      <p><b>8 марта</b> - выходной</p>
    `;											//текст внутри виджета
let holidays = new Holidays(
    typeHoliday,
    btnText,
    detailTitle,
    detailText,
)

holidays.init()
