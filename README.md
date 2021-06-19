# DesignSimpleRoadwaySystem_NUCLEOF411RE
Design Simple Roadway System with NUCLEOF411RE using Modbus Protocol

[ hardware setting ]
- 사용재료: 
Modbus RTU relay
MAX485
MG90(servo motor)
CDS sensor
ESP-01 (x2)
LED (x6)

server-client 통신망 구성도
<img width="452" alt="server-client통신망연결" src="https://user-images.githubusercontent.com/47296316/122634220-e583b880-d117-11eb-9b36-a0d9c79c5b2f.png">

센서 연결 구성도
<img width="452" alt="server-client센서연결" src="https://user-images.githubusercontent.com/47296316/122634192-b4a38380-d117-11eb-93f4-39fcdd86a968.png">


[ 실행 방법 ]
Modbus rtu relay에 연결된 보드에는 rtu_server.cpp를, client로 사용할 보드에는 client.cpp를 실행
client 보드에서의 조작으로 실행이 가능합니다.

client.cpp를 처음 실행을 시키면 VER0인 상태가 default입니다.
'*'로 pc입력 시 VER 변경이 가능합니다.
 VER 0: traffic control ver.
 VER 1: street light control ver.

[ VER 0 ]
pc로 입력한 값으로 제어가 가능하다.
- '[' : open the roadway (traffic ligth ON & barricade ON)
- ']' : close the roadway (traffic light OFF & barricade OFF)

[ VER 1 ]
가로등을 제어하는 버전으로,
'I'를 pc에서 터미널로 입력하면 조도센서(TCP)에서 값을 읽어 가로등을 제어합니다.

실행영상 → https://www.youtube.com/watch?v=6me1nBNLveA
과제 제출용 최종 보고서 → https://docs.google.com/document/d/1Aib994tB63Aqfd_cv0hufCGR6FaU5ygOtQIRFCEY1po/edit?usp=sharing
