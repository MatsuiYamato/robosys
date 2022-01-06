## ロボットシステム学　課題１

課題１としてmyled.cを作成しましたので添削よろしくお願いします。
※DCモータを動かすプログラムを作成していたのですが回路を作成するパーツが足らなかったため、回路ができ次第再提出させていただく可能性があります。  

# プログラムの概要

　講義内で作成したmyled.cのプログラムを自分なりに改造し以下の動作をするように変更しました。  
 
 
　1.　PWM制御によって数秒間やや暗くLEDが点灯する。  
　2.　明度の比較のため数秒間LED が明るく点灯する。  
　3.　消灯する。  
# プログラムの使用手順
 _インストール_  
 git clone https://github.com/MatsuiYamato/robosys.git  
 cd robosys  
 make  
 sudo insmod myled.ko　　
 sudo chmod a666 /dev/myled0
 
 _実行_  
 echo 1 > /dev/myled0  
 
 _アンインストール_  
 sudo rmmod myled  
 
# 工夫・アピール点
　PWM制御によってLEDの明るさを調節する。  
 ※肉眼だとLEDが暗く見えるが、カメラで撮影するとゆっくり明滅してるように見えてしまった。
# 使用したもの
 * RaspberryPi4  
 * ブレッドボード  
 * ジャンパー線  
 * 抵抗  
 * LED  
 
 # 実演動画
 https://youtu.be/KH6Zxg79mbg
 
 # ライセンス
 　GNU General Public License ver3.0
 
　


