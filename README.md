## strypt - String tool for testing strings
It's just a simple tool to test strings that I've created for CTF challenges

### Requirements
Python 3.5+
hashlib
argparse
base64
string

### Instalation
```
$ wget https://raw.githubusercontent.com/jersobh/strypt/master/strypt
$ chmod +x strypt 
$ sudo mv -v strypt /usr/local/bin 
```

To install the Python libraries globally:

```
$ sudo python3.6 -m pip install -r requirements.txt
```
Change the 3.6 for your own python version.

### Usage
Encoding:
```
$ strypt --encode teste
```
output:
```
md5 698dc19d489c4e4db73e28a713eab07b
sha1 2e6f9b0d5885b6010f9167787445617f553a735f
sha256 46070d4bf934fb0d4b06d9e2c46e346944e322444900a435d7d9a95e6d7435f5
sha384 20f8a4a8da1c889e7bf383c06620de04fe6489d855d6f47a50aa1e422485ddf04ec38f7cb0ace1c22c951bc479757555
sha512 b123e9e19d217169b981a61188920f9d28638709a5132201684d792b9264271b7f09157ed4321b1c097f7a4abecfc0977d40a7ee599c845883bd1074ca23c4af
base64 dGVzdGU=
```

Decoding: 

string
```
$ strypt --encode teste
```
output:
```
base64 teste
caesar ['dGVzdGU=', 'eGVaeGU=', 'fGVbfGU=', 'gGVcgGU=', 'hGVdhGU=', 'iGVeiGU=', 'jGVfjGU=', 'kGVgkGU=', 'lGVhlGU=', 'mGVimGU=', 'nGVjnGU=', 'oGVkoGU=', 'pGVlpGU=', 'qGVmqGU=', 'rGVnrGU=', 'sGVosGU=', 'tGVptGU=', 'uGVquGU=', 'vGVrvGU=', 'wGVswGU=', 'xGVtxGU=', 'yGVuyGU=', 'zGVvzGU=', 'aGVwaGU=']
```

base64
```
$ strypt --decode dGVzdGU=
```
output:
```
caesar ['teste', 'uftuf', 'vguvg', 'whvwh', 'xiwxi', 'yjxyj', 'zkyzk', 'alzal', 'bmabm', 'cnbcn', 'docdo', 'epdep', 'fqefq', 'grfgr', 'hsghs', 'ithit', 'juiju', 'kvjkv', 'lwklw', 'mxlmx', 'nymny', 'oznoz', 'paopa', 'qbpqb']
```
