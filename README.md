<div align="center">
  <img src="https://github.com/RuidongFang/AOMcodec_Fred/blob/master/AOMcodec_Fred_logo.png"><br><br>
</div>


## AOMcodec_Fred说明
</br></br>
## 平台搭建
1. build prerequisites：http://aomedia.org/build-prerequisites/
2. clone the AOM repository
    $ git clone https://aomedia.googlesource.com/aom
    $ cd aom
3. Configure and build AOM
    $ ./configure --enable-internal-stats --enable-debug --disable-install-docs --log=yes
    $ make
4. Run some encodes
    $ cd <test clip directory>
    $ run_tests 200 500 50 baseline
5. Make your changes to AOM
    $ run_tests 200 500 50 mytweak
6. generate an HTML-format report
    $ visual_metrics.py metrics_template.html "*stt" baseline mytweak > mytweak.html
7. View the report
    opening mytweak.html in a web browser
</br></br>
## 资源链接
### AV1发布平台
* Alliance for Open Media：http://aomedia.org/
### 码流分析工具
* AOM ANALYZER：https://people.xiph.org/~mbebenita/analyzer/
* aomanalyzer：https://github.com/mbebenita/aomanalyzer
### AV1源码
* 源码地址：https://aomedia.googlesource.com/aom
* 测试脚本：https://aomedia.googlesource.com/contributor-guide
### 测试视频序列
* Video Test Media：http://media.xiph.org/video/derf/
</br></br>
## 版权说明
***AOMcodec_Fred纯属个人业余研究，可能涉及到版权问题，如有涉及，请邮件说明（Fred1300216021@126.com），转载或分享AOMcodec_Fred请标注网址：https://github.com/RuidongFang/AOMcodec_Fred***
