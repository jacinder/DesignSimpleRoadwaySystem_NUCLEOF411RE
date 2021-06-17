# DesignSimpleRoadwaySystem_NUCLEOF411RE
Design Simple Roadway System with NUCLEOF411RE using Modbus Protocol

[ hardware setting ]
- 사용재료: NUCLEO F411RE 보드 2개, TCPPORT-30M, Modbus RTU relay, MAX485, MG90(servo motor), CDS sensor, ESP-01 2개, LED(Y 4개, R 1개, G 1개)
- 

처음 실행을 시키면 VER0인 상태가 default입니다.
*로 pc입력 시 VER 변경이 가능합니다.
- VER 0: traffic control ver.
- VER 1: street light control ver.

[ VER 0 ]
pc로 입력한 값으로 제어가 가능하다.
- '[' : open the roadway (traffic ligth ON & barricade ON)
- ']' : close the roadway (traffic light OFF & barricade OFF)

[ VER 1 ]
가로등을 제어하는 버전으로,
'I'를 pc에서 터미널로 입력하면 조도센서(TCP)에서 값을 읽어 가로등을 제어합니다.


실행영상 ↓
https://www.youtube.com/watch?v=6me1nBNLveA

REFERENCE
TCPPORT-30M manual
http://www.comfilewiki.co.kr/ko/doku.php?id=tcpport:funtion_code%EB%B3%84_data_%EA%B5%AC%EC%A1%B0_%EB%B0%8F_%EB%94%94%EB%B0%94%EC%9D%B4%EC%8A%A4_%EC%A0%9C%EC%96%B4:index

RTU 

