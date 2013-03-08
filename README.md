AesCrypt Plugin
===============

Advanced Encryption Standard (AES) plugin for CakePHP

## Instalation ##

#### bootstrap.php ###
```
CakePlugin::load('AesCrypt');
```

#### AppController.php ####
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
