Datepicker
==========

The one and only datepicker with no dependencies.

How to
----------
* Include
```
<script src="datepicker.js"></script>
```
* Select
```
var elem = document.querySelector('#date');
```
* Apply
```
new Datepicker(elem);
```

With jQuery:

* Include
```
<script src="jquery.datepicker.js"></script>
```
* Apply
```
$('#date').datepicker();
```

Actually getting a date from datepicker
----------

Each time the date changes and when it first starts up, the `onDateChanged` option will be called with the selected date as its first argument.

Pass it an options object as the second argument.

```javascript
/* Print the new date on the console */
new Datepicker(elem, {
  onDateChanged: function (newDate) {
    console.log(newDate);
  }
});
```

More options
----------

Override names of months...

```javascript
/* Months in spanish */
new Datepicker(elem, {
  onDateChanged: function (newDate) {
    console.log(newDate);
  }
  monthNames: ['Enero', 'Febrero', 'Marzo', 'Abril', 'Mayo', 'Junio', 'Julio', 'Agosto', 'Setiembre', 'Octubre', 'Noviembre', 'Diciembre']
})
```

...and names of days too.

```javascript
/* Months and days in spanish */
new Datepicker(elem, {
  onDateChanged: function (newDate) {
    console.log(newDate);
  }
  monthNames: ['Enero', 'Febrero', 'Marzo', 'Abril', 'Mayo', 'Junio', 'Julio', 'Agosto', 'Setiembre', 'Octubre', 'Noviembre', 'Diciembre'],
  dayNames: ['Domingo', 'Lunes', 'Martes', 'Miercoles', 'Jueves', 'Viernes', 'Sabado']
})
```

Contributing
-----------

Seriously? Thank you!

Use it
-----------
Copyright (c) 2013 Federico Baña.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
