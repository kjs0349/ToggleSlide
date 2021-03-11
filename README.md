# ToggleSlide

토글 슬라이드 애니메이션을 만들어 보았습니다.

#### 구현 과정
1. 체크박스와 label을 연결!
2. 체크박스에 display: none; 를 주어 모습을 없애주고 label에 text-indent: -9999px; 를 주어 글씨도 없는 형태로 만들어 주었다.
3. label에 배경 색을 주고 opacity: 0.5; 값을 주어 체크 되기 전 흐릿한 상태를 만들어 주었다.
4. label에 position: relative; 값을 주고 label::after에 position: absolute; 값을 주고 작은 동그란 원 모양을 만들어 주었다.
5.
	#toggle-slide:checked + label {
    	opacity: 1;
	}
값을 이용해 체크 되었을 시 진하게 만들어 주었다.


6. 
		#toggle-slide:checked + label::after {
    	top: 5px;
    	left: 75px;
    	}
값을 이용해 위치를 변경시켜 주었다.
