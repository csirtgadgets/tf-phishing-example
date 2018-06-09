# tf-phishing-example

Based on the outstanding work by:

https://medium.com/slalom-engineering/detecting-malicious-requests-with-keras-tensorflow-5d5db06b4f28

```bash
$ mkvirtualenv tf
$ pip install pandas tensorflow keras
$ python train.py --file data.csv

$ python predict.py http://raganinfotech.com/ow/adb/0016dc3e2b506150a88aebc589eb12f9
[0.9533803]

$ python predict.py http://dvxtmac.com/home/Validation/login.php?cmd=login_submit
[0.48320338]

$ ./predict.py https://google.com
[0.69641]

$ ./predict.py https://google.com/about-us
[0.03857325]

```