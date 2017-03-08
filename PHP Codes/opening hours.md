https://github.com/coryetzkorn/php-store-hours

http://www.drcoen.com/2015/02/opening-hours-done-right-in-php-and-mysql/

https://www.quora.com/How-do-I-show-dynamic-office-opening-times-on-my-website

https://murze.be/2016/10/managing-opening-hours-php/   https://github.com/spatie/opening-hours



--

https://codecanyon.net/item/business-hours-ultimate-for-wordpress/19202409?s_rank=2

https://codecanyon.net/item/business-hours-pro-wordpress-plugin/9414879?s_rank=7

https://codecanyon.net/item/openhours-highlight-your-opening-closing-hours/8231178?s_rank=8

prenre un existant et étendre
-> https://wptavern.com/how-to-extend-a-wordpress-plugin-without-losing-your-changes

ou alors le prendre dans le theme



------------

https://github.com/spatie/opening-hours

-- ajouter les exceptions dynamiquement

$openingHours = OpeningHours::create([
    'monday' => ['09:00-12:00', '13:00-18:00'],
    'tuesday' => ['09:00-12:00', '13:00-18:00'],
    'wednesday' => ['09:00-12:00'],
    'thursday' => ['09:00-12:00', '13:00-18:00'],
    'friday' => ['09:00-12:00', '13:00-20:00'],
    'saturday' => ['09:00-12:00', '13:00-16:00'],
    'sunday' => [],
    'exceptions' => [ 
        '2016-11-11' => ['09:00-12:00'],
        '2016-12-25' => [],
    ],
]);

