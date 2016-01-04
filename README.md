# loremInput

어딘가에서 주운 소스(영문버전)를 한글화 및 개선 했습니다.

## 사용방법

- js 소스(source.js)를 크롬, 사파리, 파이어폭스의 북마클릿으로 지정
- 또는 이 [링크](javascript:var auto={names:"변민철 최병대 허승연 전동춘 온수진 백영환 오혜연 진라임 전현지 채준탁 추우진 조민종 진신욱 조영미 강예원 최윤아 진문성 최소아 유정훈 허차오름 지희영 윤수미 차지담 한정순 강관창 봉순자 유태훈 지희수 차루나 조영재 온별빛 오송희 문준모 백지선 정익현 이혜정 변세찬 차미연 차신애 추새벽 정도희 한별 유익현 하정준 추승현 오세움 허별하 함인건 박영자 백태희 진근수 채진욱 봉경수 하우석 하나현 하시원 문태식 변나연 추혜원 지숙희 봉백기 유수경 천연이 진별찬 유건희 정송희 김호준 변영일 강단비 차영 천개벽 하혜라 차정숙 차윤재 하혜리 봉정혁 함하늬 봉하율 변영웅 진은설 유희민 하영재 변규태 이지현 백슬현 최희수 최다은 주진미 추수현 주승우 손설아 천손 오환종 조송희 온설희 하수완 윤아름 함진주 추문량 한영아",ids:"Steve Buscemi Catherine Keener Dermot Mulroney Danielle Zerneck James LeGros Rica Martens Peter Dinklage Kevin Corrigan Hilary Gilford Robert Wightman Tom Jarmusch Michael Griffiths Matthew Grace Ryan Bowker Francesca DiMauro",blurb:"긴지라 절찬리에 전은 학생은 손뼉을 바짝 죽었다네. 정보 지쳐나가는 손을 눈을 책에서 뜨거운지라, 아름다우냐? 마음조차 표현으로 이 사흘 거선의 설렁탕은. 차지하고 그는 하나 구경도 시대의 중 조밥도 음악을 듯싶다. 두개를 인간에 몹시 망토를 라고 빨리게. 마음이 몰라란 그들의 인제 잊을 트고, 올리기 내리었다. 동력은 얼마만인가 집이라 슬근슬근 여보게 가까운 입에서 듯하였다. 더 우는 나가지 손을 섰다. 무슨 기관과 청춘은 순식간에 자기 함께 말이 비는 하였다. 그는 하되, 방안에 그 안 모바일 교향악이다. 희망의 미친놈, 무슨 아마 것이다. 남비에 아니라 빠지짓 듯.",password:"secret",fillerup:function(){for(var e=document.getElementsByTagName("input"),t=document.getElementsByTagName("select"),a=document.getElementsByTagName("textarea"),n=0,s=t.length;s>n;n++){var r=t[n];if(-1==r.selectedIndex||!r.options[r.selectedIndex].value){var i=1;if("select-multiple"==r.type)var i=1+this.getRand(r.options.length-1);for(var o=0;i>o;o++){var l=this.getRand(r.options.length-1);r.options[l].selected="selected"}}}for(var n=0,s=a.length;s>n;n++){var d=a[n];d.value||(d.value=this.getRandomString(10)+"\n\n"+this.getRandomString(10))}for(var n=0,s=e.length;s>n;n++){var h=e[n],m=h.getAttribute("type");if(m||(m="text"),"checkbox"==m&&h.setAttribute("checked","checked"),"radio"==m){for(var g=!0,u=(h.name,h.form.elements[h.name]),o=0;o<u.length;o++)u[o].checked&&(g=!1);if(g){var l=this.getRand(u.length-1);u[l].setAttribute("checked","checked")}}"password"==m&&(h.value||(h.value=this.getPassword())),"date"==m&&(h.value||(h.value="1984-04-03")),"url"==m&&(h.value||(h.value="http://heem.net")),"email"==m&&(h.value||(h.value=this.getRandomIds(1)+"@example.org")),"text"==m&&(h.value||(h.value=-1!=h.name.indexOf("name")?this.getRandomName():-1!=h.name.indexOf("email")?this.getRandomIds()+"@example.org":-1!=h.name.indexOf("tel")?"010-0000-0000":-1!=h.name.indexOf("phone")?"010-0000-0000":this.getRandomString(1)))}},getRandomString:function(e){e||(e=5),this.words||(this.words=this.blurb.split(" "));for(var t="",a=0;e>a;a++)t+=this.words[this.getRand(this.words.length)-1],t+=e-1>a?" ":"";return t},getRandomName:function(){return this.split_names||(this.split_names=this.names.split(" ")),this.split_names[this.getRand(this.split_names.length)-1]},getRandomIds:function(e){e||(e=5),this.words||(this.words=this.ids.split(" "));for(var t="",a=0;e>a;a++)t+=this.words[this.getRand(this.words.length)-1],t+=e-1>a?" ":"";return t},getPassword:function(){return this.password||(this.password="secret"),this.password},getRand:function(e){return Math.round(e*Math.random())}};auto.fillerup();)를 북마크바로 드래그하여 추가
- <input>이 있는 페이지에서 클릭 

