# 인세인 기본 캐릭터 시트

기존에 업로드 되어 있는 인세인 시트의 로직을 기본바탕으로 하여 일부 기능을 재작업 및 추가 하였으며 전체적인 UI 디자인을 변경하였습니다.
사용 중 버그가 발생하는 경우에는 트위터 @tateck_trpg 계정으로 문의 주시길 바랍니다.

* [미리보기](#미리보기)
* [코드 활용](#코드-활용)

------------------------------

### 미리보기
<img src="https://raw.githubusercontent.com/tateck-develop/roll20CustomSheet/main/inSANe/insane_BASIC/guide.jpg" width="500px"></img>

* * *

### 코드 활용
#### 템플릿의 이용
```
&{template:InsaeContents}{{subject=제목}}{{desc=내용}} 
```
해당 코드를 이용 시, 시트에 포함된 디자인의 템플릿이 채팅창에 출력 됩니다.

#### 감정표의 수정
감정표의 경우, 기본적으로 1d6 감정표가 등록되어 있습니다.
이것을 자신이 사용하는 감정표로 수정하는 방법은 아래와 같습니다.

* html.html 파일
```
  <button class='old-roll' type='roll' value='&{template:InsaeContents} {{subject=감정표}}{{name=@{character_name}}}{{emotion_roll=[[1d6]]}}' title="감정표 굴림"></button>
```

위의 코드에서 emotion_roll=[[1d6]] 부분을 자신이 사용하는 감정표의 주사위로 변경합니다.

```
emotion_roll=[[2d6]]
```

아래의 코드를 찾아 내려갑니다. (Ctrl + F를 활용하시면 좋습니다.)
```
{{#emotion_roll}}
            <!-- 감정표 -->
            <div class="sheet-emotion-box">

                {{#rollTotal() emotion_roll 1}}<span class="sheet-p">공감</span> <span class="sheet-m">불신</span>{{/rollTotal() emotion_roll 1}}

                {{#rollTotal() emotion_roll 2}}<span class="sheet-p">우정</span> <span class="sheet-m">분노</span>{{/rollTotal() emotion_roll 2}}

                {{#rollTotal() emotion_roll 3}}<span class="sheet-p">애정</span> <span class="sheet-m">질투</span>{{/rollTotal() emotion_roll 3}}

                {{#rollTotal() emotion_roll 4}}<span class="sheet-p">충성</span> <span class="sheet-m">모멸</span>{{/rollTotal() emotion_roll 4}}

                {{#rollTotal() emotion_roll 5}}<span class="sheet-p">동경</span> <span class="sheet-m">열등감</span>{{/rollTotal() emotion_roll 5}}

                {{#rollTotal() emotion_roll 6}}<span class="sheet-p">광신</span> <span class="sheet-m">살의</span>{{/rollTotal() emotion_roll 6}}

            </div>
            <!-- // 감정표 -->
{{/emotion_roll}}
```
이 부분의 코드를 수정합니다.

플러스 감정은 
```<span class="sheet-p">감정 이름</span>```

마이너스 감정은
```<span class="sheet-m">감정 이름</span>```
의 형태로 수정합니다.


