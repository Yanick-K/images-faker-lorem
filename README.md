# images-faker-lorem
Image provider for faker

## Install
<code>composer require yanick-k/images-faker-lorem</code>


## Usage 
```php
use Faker\Factory as Faker;

$faker = Faker::create();
$faker->addProvider(new \Lorem\Faker\LoremSpaceProvider($faker));

 $url = $faker->loremSpaceUrl(\Mmo\Faker\LoremSpaceProvider::CATEGORY_FACE); // https://api.lorem.space/image/face?w=640&h=480
// download image to tmp dir
$path = $faker->loremSpace(\Mmo\Faker\LoremSpaceProvider::CATEGORY_FACE)
 ```