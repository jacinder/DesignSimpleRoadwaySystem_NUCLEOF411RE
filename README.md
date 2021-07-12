# DesignSimpleRoadwaySystem_NUCLEOF411RE
Design Simple Roadway System with NUCLEOF411RE using Modbus Protocol

[ hardware setting ]<br/>
- 사용재료: 
Modbus RTU relay
MAX485
MG90(servo motor)
CDS sensor
ESP-01 (x2)
LED (x6)

- server-client 통신망 구성도<br/>
<img width="452" alt="server-client통신망연결" src="https://user-images.githubusercontent.com/47296316/122634220-e583b880-d117-11eb-9b36-a0d9c79c5b2f.png">

- 센서 연결 구성도<br/>
<img width="452" alt="server-client센서연결" src="https://user-images.githubusercontent.com/47296316/122634192-b4a38380-d117-11eb-93f4-39fcdd86a968.png">


[ 실행 방법 ]<br/>
Modbus rtu relay에 연결된 보드에는 rtu_server.cpp를, client로 사용할 보드에는 client.cpp를 실행<br/>
client 보드에서의 조작으로 실행이 가능합니다.<br/>

client.cpp를 처음 실행을 시키면 VER0인 상태가 default입니다.<br/>
'*'로 pc입력 시 VER 변경이 가능합니다.<br/>

 VER 0: traffic control ver.<br/>
 VER 1: street light control ver.<br/><br/>

[ VER 0 ]<br/>
pc로 입력한 값으로 제어가 가능하다.<br/>
- '[' : open the roadway (traffic ligth ON & barricade ON)<br/>
- ']' : close the roadway (traffic light OFF & barricade OFF)<br><br>

[ VER 1 ]<br/>
가로등의 제어가 가능하다<br/>
- 'I' : 조도센서(TCP PORT에 연결)에서 값을 읽어 가로등을 제어합니다.<br><br>

→ <a href='https://www.youtube.com/watch?v=6me1nBNLveA'>실행영상📺</a> | 
<a href='https://docs.google.com/document/d/1Aib994tB63Aqfd_cv0hufCGR6FaU5ygOtQIRFCEY1po/edit?usp=sharing'>최종 보고서📑</a>
