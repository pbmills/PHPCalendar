# Calendar

A Calendar and Date handling library for PHP

## Some of the things you can do with this

```php


$cal = new calendar();


echo $cal->year(1981)->countDays();


echo $cal->month(2012, 7)->days()->last()->name();


foreach($cal->year(2001)->months()->nth(5)->weeks() as $week) {
  foreach($week->days() as $day) {
    echo $day->format('d.m.Y');
  }
}


echo $cal->date('01.08.2009')->minus('2years')->plus('38days)->month()->shortname();


foreach($cal->day(2012, 07, 10)->hours() as $hour) {
  foreach($hour->minutes() as $minute) {
    foreach($minute->seconds() as $second) {
       echo $second;
    }
  }  	
}

echo $cal->year(2000)->next()->months()->first()->next()->firstDay()->iso();


```

Also: check out the examples!

## More soon…

This is just a rough first version, but maybe you like it. Here are some of the things that need to be added:

- more docs
- improved examples
- timezone handling
- interval handling


