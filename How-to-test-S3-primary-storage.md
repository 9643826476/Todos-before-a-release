Install https://github.com/jubos/fake-s3 and start it:

```bash
sudo gem install fakes3
mkdir /tmp/s3
fakes3 -r /tmp/s3 -p 4567
```

In there now a subfolder per bucket is created and every object is stored inside a folder in there.

Configure Nextcloud:

```php
'objectstore_multibucket' => [
	'class' => 'OC\\Files\\ObjectStore\\S3',
	'arguments' => [
		'bucket' => 'abc',
		'num_buckets' => 64,
		'key' => '123',
		'secret' => 'abc',
		'hostname' => 'localhost',
		'port' => '4567',
		'use_ssl' => false,
		'use_path_style' => 'true',
	],
],
```

OR

```php
'objectstore' => [
	'class' => 'OC\\Files\\ObjectStore\\S3',
	'arguments' => [
		'bucket' => 'abc',
		'key' => '123',
		'secret' => 'abc',
		'hostname' => 'localhost',
		'port' => '4567',
		'use_ssl' => false,
		'use_path_style' => 'true',
	],
],
```