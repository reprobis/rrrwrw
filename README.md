# 인세인 황량일취몽 시나리오 (w.연호) 전용 커스텀 시트

이 인세인 커스텀 시트는 기존에 배포하던 롤20 커스텀 인세인 시트에서, 연호님의 황량일취몽 시나리오 전용으로 커스텀 되었습니다. (장면표, 특기 등)
사용 중 버그가 발생하는 경우에는 트위터 @tateck_trpg 계정으로 문의 주시길 바랍니다.

* [미리보기](#미리보기)
* [코드 활용](#코드-활용)

------------------------------

### 미리보기
<img src="https://raw.githubusercontent.com/tateck-develop/roll20CustomSheet/main/inSANe/insane_A_desolate_dream/guide.jpg" width="500px"></img>

* * *

### 코드 활용
#### 템플릿의 이용
```
&{template:InsaeContents}{{subject=제목}}{{name=제목상단 작은이름}}{{content=설명글 출력}}
```
해당 코드를 이용 시, 시트에 포함된 디자인의 템플릿이 채팅창에 출력 됩니다.

#### 로고변경
<img src="https://i.imgur.com/2D2aBzb.png" width="186px"></img>

html 소스코드의 80번 라인 (Ctrl + F : 로고)에 사용되고 있는 이미지코드를 변경하여 로고를 변경하거나 제거할 수 있습니다.
로고의 사이즈는 width:186px / height:240px 에 최적화 되어 있습니다.