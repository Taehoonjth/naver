# 네이버 실시간 검색어 내 마음대로 바꾸기
<img src='https://github.com/Taehoonjth/naver/blob/master/img/chrome_example.png?raw=true' alt='' width='800'>

## 네이버 방문
크롬 또는 파이어폭스로 새 탭, 또는 창으로 [네이버](https://www.naver.com)를 엽니다.
## 개발자 도구 열기
### 크롬의 경우
Ctrl+Shift+J (윈도우 / 리눅스) 또는 Cmd+Opt+J (맥)를 누릅니다. 아래 처럼 console이 뜨면 됩니다.
<img src='https://github.com/Taehoonjth/naver/blob/master/img/chrome_console.png?raw=true' alt='' width='800'>

### 파이어폭스의 경우

## 검색어 바꾸기
### 1위 검색어 바꾸기
1. 콘솔에 아래의 코드를 복사 붙여넣기 하세요.
2. 콤마 사이의 텍스트를 여러분이 원하는 것으로 바꾸세요(콤마는 그대로 유지하세요).
3. 엔터를 치세요.
4. 이제 네이버 실시간 검색어 1위를 확인해보세요.
```
var first = '여기를 바꾸세요';
document.getElementsByClassName('ah_k')[0].innerHTML = first;
document.getElementsByClassName('ah_k')[20].innerHTML = first;
document.getElementsByClassName('ah_k')[21].innerHTML = first;
```
<img src='https://github.com/Taehoonjth/naver/blob/master/img/chrome_first.png?raw=true' alt='' width='800'>
(외계인이 발견이 네이버 실시간 검색어 1위?)

### 모두 바꾸기
1위 만으로는 만족 못하시겠다면 이번에는 1위부터 1위부터 20위 까지 모두를 바꿔봅시다.
```
var first = '여기를 바꾸세요';
for (var i = 0; i < 41; i++) {
  document.getElementsByClassName('ah_k')[i].innerHTML = first;
}
```
<img src='https://github.com/Taehoonjth/naver/blob/master/img/chrome_every.png?raw=true' alt='' width='800'>

## 수고하셨습니다. 책으로 돌아가세요!
