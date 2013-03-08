AesCrypt Plugin
===============

Advanced Encryption Standard (AES) plugin for CakePHP - URL friendly

## Installation ##

#### git clone ###
```
git clone https://github.com/slaven/AesCrypt.git app/Plugin/AesCrypt
```

#### Add to bootstrap.php ###
```
CakePlugin::load('AesCrypt');
```

#### Add to AppController.php ####
```
App::uses('AesCrypt', 'AesCrypt.Lib');
```

#### Usage in Controller / View ####
```
/* Test array */
$testArrEnc = AesCrypt::encrypt( array('name' => 'test') );
debug($testArrEnc);
$testArrDec = AesCrypt::decrypt($testArrEnc);
debug($testArrDec);
```

```
/* Test string */
$testStrEnc = AesCrypt::encryptStr('test');
debug($testStrEnc);
$testStrDec = AesCrypt::decryptStr($testStrEnc);
debug($testStrDec);
```
