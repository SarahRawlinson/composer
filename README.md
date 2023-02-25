This is a test for creating a composer library

use command

```

composer config repositories.sarahrawlinson-composer vcs https://github.com/SarahRawlinson/sarahs-test-composer.git

```

and then

```

composer require sarahrawlinson/sarahs-test-composer:dev-master

```

this should add the below to your composer.json and install the package

```

  "repositories": {
    "sarahrawlinson-composer": {
      "type": "vcs",
      "url": "https://github.com/SarahRawlinson/sarahs-test-composer.git"
    }
  },
  "require": {
    "sarahrawlinson/sarahs-test-composer": "dev-master"
  }

```

use the update command to pull changes

```

composer update sarahrawlinson/rawlinson

```

any issues use

```

composer remove sarahrawlinson/sarahs-test-composer

```

and then add the library back in using

```

composer require sarahrawlinson/sarahs-test-composer:dev-master

```

possible issues

* If a file is removed/renamed the original file that you have from a previous version will remain in the library  

to completely remove use command 

```

composer remove sarahrawlinson/sarahs-test-composer

```

then

```

composer config --unset repositories.sarahrawlinson-composer

```