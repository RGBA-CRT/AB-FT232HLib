# AB-FT232HLib
- FT232H(d2xx)�p ���p���C�u���� for [ActiveBasic4](https://www.activebasic.com/)
- ���p�Ȃ̂Ő݌v�̓N�\�ł����A����m�F�͂Ƃ�Ă���̂ŃT���v���R�[�h�Ƃ��Ă͎g����Ǝv���܂��B
- FTDI�Ђ�D2XX�h���C�o���K�v�ɂȂ�܂��B[[link]](http://www.ftdichip.com/Drivers/D2XX.htm)
- FT_Prog��p���ēK�؂ȃR���t�B�M�����[�V���������Ă��������B�T���v���e���v���[�g��config_eeprom.xml�ł��B

## �r���h�Ɏg�p����ꍇ
[USB-Si5351aCtrl](https://github.com/RGBA-CRT/USB-Si5351aCtrl)��FT232H-EPROM-PROG�Ȃǂ��r���h����ꍇ�A�����̃f�B���N�g�������̃��C�u�����̉��ɔz�u���Ă��������B�����̃��C�u������#include "../FT232HLib.sbp"�Ƃ��������ŎQ�Ƃ��Ă��܂��B

## �J���Ɏg�p����ꍇ
- **���p�Ȃ̂Ŏd�l���R���R������\��������܂��B**
- �h�L�������g�͂Ȃ��̂Ŋ֘A���|�W�g���ƍ��킹�Ďg������T���Ă�������
- D2XX.sbp��FT232HLib.sbp���C���N���[�h���A�f�o�C�X�p�̃R�[�h(��FSi5351a.sbp)���C���N���[�h���Ďg���܂��B
- FT232H�N���X��gpio, spi, i2c�N���X������Ɏ����Ă��܂��B
- spi, i2c�͎g�p�J�n����init()���Ăяo���Ă��������B
- **i2c�ȊO�́A�v���O�������ŃR�}���h�𗭂߂Ă����āAsendCommands()�Ŏ��ۂ�FT232H�����삷��Ƃ�������ɂȂ��Ă��܂��B**