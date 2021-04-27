# 마기카로기아
* [미리보기](#미리보기)
* [코드 활용](#코드-활용)

------------------------------

### 미리보기
<img src="https://raw.githubusercontent.com/tateck-develop/roll20CustomSheet/main/magica_logia/magi_BASIC/guide.png" width="500px"></img>

* * *

### 코드 활용
#### 템플릿의 이용
```
&{template:MagiDice}{{name=상단텍스트}}{{title=제목}}{{subtitle=중간제목}}{{content=글 내용}}
```
해당 코드를 이용 시, 시트에 포함된 디자인의 템플릿이 채팅창에 출력 됩니다.
사용하지 않은 항목은 출력되지 않습니다.

```
&{template:MagiSpell}{{text=회심의 역작이..!}}
```
해당 코드를 이용 시, 주구 영창과 동일한 효과의 템플릿이 채팅창에 출력됩니다.

------------------------------
## Update
* 2020.10.12 : 가변특기 굴리는 selectbox 쪽에 짐승/꿈 잘못 표기된 부분 수정
* 2020.10.12 : 주구 효과 관련 템플릿 추가
* 2020.10.12 : 장서 판정 시 수정치 출력 부분 수정
* 2020.10.12 : 혼의 특기 목표치 5 -> 6으로 변경
* 2020.10.12 : 앵커란 10 고정, 상흔 표기 시 특기표에 표시 되도록 적용
* 2020.10.12 : 최대 마력 입력칸에서, <최대마력> 이름 클릭 시 마력결정 주사위 굴림 추가
* 2020.10.12 : 원한 > 원환 표기 수정
* 2020.10.15 : 별 분야 앞에 갭 추가
* 2020.10.20 : 장서칸 10개 이후 주사위 오류 수정
* 2020.10.23 : 지정특기 영역에 가변 특기 기능으로 분야 추가
* 2020.10.23 : 가이드 텍스트 색상 조정
* 2020.10.23 : 장서 지정특기 selectbox 입력 소스코드 추가 업로드
* 2021.03.12 : 롤20 업데이트에 따른 패치 적용