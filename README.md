

<h1 align="center">  backjoonStudy </h1>
<br><br>
<h2> node.js로 백준 알고리즘 풀이 제출 </h2>
<h3> javascript로 풀 수 없어 node.js로 제출하기 <h3>
<br>
<p> fs 모듈 이용 </p>
<p>

// 파일을 읽어오기 위해 Node.js의 built-in file system module fs 사용
var fs = require('fs'); 

//input을 읽어와 변수로 선언 & 할당
// 그 내용을 input에 저장, toString(), split()을 사용해서
// Array로 저장된다.
var input = fs.readFileSync('/dev/stdin').toString().split(' ');

// input에서 지정한 value를 읽어와 다른 변수로 선언하고 활용
// toString메소드로 지금은 string이기 때문에, parseInt로 숫자로 형태변환을 해준다.
var a = parseInt(input[0]);
var b = parseInt(input[1]);

console.log(a + b)

* 백준 밖에서 풀어볼때는 input값을 담은 txt파일을 만들어서 readFileSync에 담으면 된다. 백준에서는 /dev/stdin을 넣으면 된다.

</p>



