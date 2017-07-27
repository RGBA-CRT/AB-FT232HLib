# AB-FT232HLib
- FT232H(d2xx)用 私用ライブラリ for [ActiveBasic4](https://www.activebasic.com/)
- 私用なので設計はクソですが、動作確認はとれているのでサンプルコードとしては使えると思います。
- FTDI社のD2XXドライバが必要になります。[[link]](http://www.ftdichip.com/Drivers/D2XX.htm)
- FT_Progを用いて適切なコンフィギュレーションをしてください。サンプルテンプレートはconfig_eeprom.xmlです。

## ビルドに使用する場合
[USB-Si5351aCtrl](https://github.com/RGBA-CRT/USB-Si5351aCtrl)やFT232H-EPROM-PROGなどをビルドする場合、それらのディレクトリをこのライブラリの下に配置してください。これらのライブラリは#include "../FT232HLib.sbp"という感じで参照しています。

## 開発に使用する場合
- **私用なので仕様がコロコロする可能性があります。**
- ドキュメントはないので関連リポジトリと合わせて使い方を探ってください
- D2XX.sbpとFT232HLib.sbpをインクルードし、デバイス用のコード(例：Si5351a.sbp)をインクルードして使います。
- FT232Hクラスはgpio, spi, i2cクラスを内部に持っています。
- spi, i2cは使用開始時にinit()を呼び出してください。
- **i2c以外は、プログラム側でコマンドを溜めていって、sendCommands()で実際にFT232Hが動作するという流れになっています。**