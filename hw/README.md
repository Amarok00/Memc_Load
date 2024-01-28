# Usage

## Run:

cd to directory with memc_load.py

`$ python3 -m memc_load [-t --test] [-l --log] [--maxworkers] [--loginfo] [--dry] [--pattern] [--idfa] [--gaid] [--adid] [--dvid]`

Example
`python memc_load.py --pattern "/home/dmitriy/Загрузки/tars/*.tsv.gz" --dry`

* --test: run tests
* --log: store logs in filename
* --maxworkers: maximum workers
* --loginfo: if set, loglevel would be forced to INFO (even in --dry)
* --dry: dryrun without writing into memchached, logs would go to file or stdout
* --pattern: dir and name pattern to find .gz files to process
* --idfa, --gaid, --adid, --dvid: server addresses to store device memc's



## Example run



head:

```[2024.01.21 18:06:51] I Memc loader started with options: {'test': False, 'log': None, 'maxworkers': 5, 'loginfo': False, 'dry': True, 'pattern': '/home/dmitriy/Загрузки/tars/*.tsv.gz', 'idfa': '127.0.0.1:33013', 'gaid': '127.0.0.1:33014', 'adid': '127.0.0.1:33015', 'dvid': '127.0.0.1:33016'}
[2024.01.21 18:06:51] D Writer 0 started
[2024.01.21 18:06:51] D Writer 1 started
[2024.01.21 18:06:51] D Writer 2 started
[2024.01.21 18:06:51] D Writer 3 started
[2024.01.21 18:06:51] D Writer 4 started
[2024.01.21 18:06:51] I Processing /home/dmitriy/Загрузки/tars/20170929000000.tsv.gz
|#                                                                             | 0 Elapsed Time: 0:00:00[2024.01.21 18:06:51] D 127.0.0.1:33013 - idfa:e7e1a50c0ec2747ca56cd9e1558c0d7c -> apps: 7942 apps: 8519 apps: 4232 apps: 3032 apps: 4766 apps: 9283 apps: 5682 apps: 155 apps: 5779 apps: 2260 apps: 3624 apps: 1358 apps: 2432 apps: 1212 apps: 528 apps: 8182 apps: 9061 apps: 9628 apps: 2055 apps: 4821 apps: 3550 apps: 4964 apps: 6924 apps: 6737 apps: 3784 apps: 5428 apps: 6980 apps: 8137 apps: 2129 apps: 8751 apps: 3000 apps: 5495 apps: 5674 apps: 3023 apps: 818 apps: 2864 apps: 8250 apps: 768 apps: 6931 apps: 3493 apps: 3749 apps: 8053 apps: 8815 apps: 8448 apps: 8757 apps: 272 apps: 5951 apps: 2831 apps: 7186 apps: 157 apps: 1629 apps: 2021 apps: 3338 apps: 9020 apps: 6679 apps: 8679 apps: 1477 apps: 7488 apps: 3751 apps: 7399 apps: 8556 apps: 5500 apps: 5333 apps: 3873 apps: 7070 apps: 3018 apps: 2734 apps: 4273 apps: 3723 apps: 4528 apps: 4657 apps: 4014 lat: 67.7835424444 lon: -22.8044005471
[2024.01.21 18:06:51] D 127.0.0.1:33013 - idfa:f5ae5fe6122bb20d08ff2c2ec43fb4c4 -> apps: 4877 apps: 7862 apps: 7181 apps: 6071 apps: 2107 apps: 2826 apps: 2293 apps: 3103 apps: 9433 apps: 2794 apps: 4303 apps: 7500 apps: 5637 apps: 8935 apps: 6772 apps: 2481 apps: 1614 apps: 3946 apps: 7013 apps: 690 apps: 9474 apps: 1655 apps: 9718 apps: 4862 apps: 3367 apps: 3869 apps: 4255 apps: 9431 apps: 7333 apps: 5471 apps: 3267 apps: 7439 apps: 7202 apps: 7310 apps: 7875 apps: 1468 apps: 8146 apps: 9617 apps: 4336 apps: 8747 apps: 7815 lat: -104.68583244 lon: -51.24448376
[2024.01.21 18:06:51] D 127.0.0.1:33014 - gaid:3261cf44cbe6a00839c574336fdf49f6 -> apps: 7462 apps: 1115 apps: 5205 apps: 6700 apps: 865 apps: 5317 apps: 4967 apps: 2104 apps: 7993 apps: 6357 apps: 2385 apps: 8639 apps: 2306 apps: 5712 apps: 5326 apps: 9929 apps: 7781 apps: 1402 apps: 8830 apps: 1978 apps: 6443 apps: 3372 apps: 6379 apps: 5426 apps: 7847 apps: 8485 apps: 8983 apps: 1938 apps: 4809 apps: 2095 apps: 6887 apps: 2720 apps: 1074 apps: 1499 apps: 7165 apps: 4922 apps: 5969 apps: 6655 apps: 241 apps: 8738 apps: 1336 apps: 7334 apps: 465 apps: 4866 apps: 3402 apps: 634 apps: 9813 apps: 6343 apps: 2686 apps: 2214 apps: 7140 apps: 4818 apps: 92 apps: 1072 apps: 4784 apps: 2376 apps: 2086 apps: 5639 apps: 6314 apps: 9411 apps: 7888 apps: 8187 apps: 8766 apps: 7524 apps: 9002 apps: 3567 apps: 3563 apps: 360 apps: 8949 apps: 2780 apps: 8299 apps: 2460 apps: 1274 apps: 1474 apps: 3030 apps: 2221 apps: 3467 apps: 9094 apps: 9014 apps: 4475 apps: 4180 apps: 2205 apps: 481 apps: 7125 apps: 1237 lat: 137.790839567 lon: 56.8403675248
[2024.01.21 18:06:51] D 127.0.0.1:33016 - dvid:94584df26efb6afd43b30609328f3d75 -> apps: 4046 apps: 5305 apps: 7503 apps: 1192 apps: 1354 apps: 4875 apps: 6216 apps: 529 apps: 4067 apps: 7003 apps: 8900 apps: 3945 apps: 9099 apps: 9054 apps: 9322 apps: 173 apps: 739 apps: 3807 apps: 5133 apps: 8353 apps: 4358 apps: 2781 apps: 6015 apps: 5538 lat: 165.364801883 lon: -67.9991374849
[2024.01.21 18:06:51] D 127.0.0.1:33013 - idfa:26658aeb53c5c03222c631843cdd7332 -> apps: 6700 apps: 858 apps: 9532 apps: 3236 apps: 7959 apps: 8317 apps: 6388 apps: 681 apps: 8245 apps: 5269 apps: 4705 apps: 6292 apps: 7872 apps: 9589 apps: 1585 apps: 7849 apps: 1363 lat: -147.210946651 lon: 71.561943603
[2024.01.21 18:06:51] D 127.0.0.1:33015 - adid:ca468fbb41ae6bd0b75fde1246a89bd1 -> apps: 9772 apps: 8573 apps: 4607 apps: 7464 apps: 1577 apps: 1787 apps: 3632 apps: 7132 apps: 3893 apps: 1666 apps: 6507 apps: 3155 apps: 3740 apps: 6983 apps: 6699 apps: 5447 apps: 5396 apps: 6798 apps: 2664 apps: 5283 apps: 6939 apps: 209 apps: 3454 lat: 48.1968937235 lon: 51.05440249
[2024.01.21 18:06:51] D 127.0.0.1:33014 - gaid:5094cde0cddb48a4ff1614fd9dd513bd -> apps: 6824 apps: 4323 apps: 6216 apps: 3329 apps: 1821 apps: 1523 apps: 5459 apps: 7692 apps: 4747 apps: 5208 apps: 4761 apps: 9914 apps: 8859 apps: 3338 apps: 1743 apps: 6192 apps: 7606 apps: 2489 apps: 5741 apps: 3523 apps: 1246 apps: 2606 apps: 9289 apps: 356 apps: 5073 apps: 7280 apps: 9401 apps: 4100 apps: 6056 apps: 6968 apps: 945 apps: 2252 apps: 7478 apps: 1609 apps: 2747 apps: 6526 apps: 7728 apps: 9443 apps: 855 apps: 8607 apps: 8683 apps: 2594 apps: 5446 apps: 4610 apps: 9568 apps: 4415 apps: 8264 apps: 3165 apps: 8491 apps: 8790 apps: 5422 apps: 2578 apps: 2777 apps: 7192 apps: 1764 apps: 5408 apps: 7366 apps: 9707 apps: 7545 apps: 1398 apps: 3989 apps: 5209 apps: 4442 apps: 458 apps: 7892 lat: 8.08101490477 lon: 22.1430848316
[2024.01.21 18:06:51] D 127.0.0.1:33013 - idfa:aab56963000aad2eaaf515db9ed855d8 -> apps: 1537 apps: 2883 apps: 3885 apps: 432 apps: 4161 apps: 5585 apps: 9449 apps: 6117 apps: 3799 apps: 2540 apps: 6627 apps: 5774 apps: 499 apps: 5871 apps: 6140 apps: 6629 apps: 7061 apps: 6880 apps: 7669 apps: 204 apps: 4637 apps: 3641 apps: 497 apps: 8976 apps: 2163 apps: 437 apps: 8702 apps: 7771 apps: 6420 apps: 4226 apps: 2461 apps: 7533 apps: 8938 apps: 95 apps: 6750 apps: 3487 apps: 6745 apps: 3295 apps: 8174 apps: 9423 apps: 608 apps: 982 apps: 3393 apps: 4462 apps: 2441 apps: 8958 apps: 7492 apps: 4435 apps: 6675 apps: 5009 apps: 500 apps: 2827 apps: 7823 apps: 4423 apps: 4913 apps: 1799 apps: 6438 apps: 4911 apps: 1568 apps: 213 apps: 8546 apps: 2363 apps: 8465 apps: 3572 apps: 8410 apps: 7086 apps: 4384 apps: 394 lat: -119.489831986 lon: -55.7049523367
[2024.01.21 18:06:51] D 127.0.0.1:33015 - adid:3b2c5da2bc240933fbfe2334eafd952a -> apps: 4923 apps: 5062 apps: 7809 apps: 4487 apps: 1916 apps: 2323 apps: 9787 apps: 848 apps: 3928 lat: 37.6159831853 lon: -71.5094064462
```
...

tail:

`[2024.01.21 22:39:12] D 127.0.0.1:33016 - dvid:bd9a5b7e1516d62b813d9f4ce6dbf6ee -> apps: 7710 apps: 5450 apps: 6857 apps: 7460 apps: 1177 apps: 3196 apps: 8734 apps: 1303 apps: 2542 apps: 5132 apps: 8621 apps: 7646 apps: 34 apps: 7879 apps: 5236 apps: 5031 apps: 8161 apps: 3816 apps: 3627 apps: 9300 apps: 1704 apps: 1321 apps: 987 apps: 6547 apps: 9787 apps: 8964 apps: 8816 apps: 1909 apps: 6986 apps: 9963 apps: 166 apps: 1849 apps: 4791 apps: 8005 apps: 851 apps: 5687 apps: 26 lat: -47.8291071322 lon: 73.0047398598 `
`[2024.01.21 22:39:12] D 127.0.0.1:33015 - adid:c0c402f15b5ae9ae94884143d79e7845 -> apps: 9098 apps: 4677 apps: 6924 apps: 8995 apps: 4671 apps: 2094 apps: 2610 apps: 2776 apps: 912 apps: 1349 apps: 8222 apps: 4253 apps: 8337 apps: 938 apps: 9849 apps: 1059 apps: 7488 apps: 367 apps: 9214 apps: 3795 apps: 4492 apps: 7535 apps: 7054 apps: 6023 apps: 3428 apps: 1758 apps: 4783 apps: 1538 apps: 2034 apps: 8483 apps: 4706 apps: 9267 apps: 4268 apps: 3790 apps: 211 apps: 8522 apps: 1614 apps: 2532 apps: 600 apps: 9464 apps: 9351 apps: 1518 apps: 8905 apps: 182 apps: 6939 apps: 7207 apps: 4457 apps: 7945 apps: 1320 apps: 8516 apps: 747 apps: 2043 apps: 3625 apps: 3639 apps: 1039 apps: 3026 apps: 5384 apps: 1785 apps: 5039 apps: 4322 apps: 7260 apps: 1928 apps: 9704 apps: 5615 apps: 6106 apps: 633 apps: 9501 apps: 5478 apps: 3676 apps: 1668 apps: 1429 apps: 1989 apps: 1756 apps: 9268 apps: 1068 apps: 3688 apps: 9642 apps: 7455 apps: 6800 apps: 6169 apps: 6890 apps: 5375 apps: 8743 apps: 3439 apps: 9878 apps: 7333 apps: 3282 apps: 929 apps: 5256 apps: 8557 apps: 5080 apps: 7256 lat: -21.2056085252 lon: -17.3329838649 `
`[2024.01.21 22:39:13] I Errors: 0, Processed: 3422995`
`[2024.01.21 22:39:13] I Acceptable error rate (0.0). Successfull load`

(Elapsed Time: 0:19:45)
