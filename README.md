

<h1 align="center">  backjoonStudy ๐ง๐ปโ๐ป </h1>
<br><br>
<h2> node.js๋ก ๋ฐฑ์ค ์๊ณ ๋ฆฌ์ฆ ํ์ด ์ ์ถ โ๐ผ </h2>
<h3> javascript๋ก ํ ์ ์์ด node.js๋ก ์ ์ถํ๊ธฐ <h3>
  <p> ๋ชจ๋์ ์ถ๊ฐํด์ฃผ๋ฉด ๋ฌธ์ ํ๊ธฐ๊ฐ ๊ฐ๋ฅํ๋ค</p>
<br>
<p> 1๏ธโฃ fs ๋ชจ๋ ์ถ๊ฐํ๊ธฐ </p>
<p>
const fs = require("fs"); <br>
const input = fs.readFileSync("/dev/stdin").toString().split(' '); <br>
</p>
<p>๋ฌธ์์ด๋ก ๋ฐ์์จ ๋ฐ์ดํฐ๋ฅผ ' '๊ณต๋ฐฑ์ ๊ธฐ์ค์ผ๋ก ๋๋์ด์ input์ ๋ฐฐ์ด๋ก ์ ์ฅํ๋ ์ฝ๋ </p>
<p>2๏ธโฃ ๋ฌธ์  ํ๊ธฐ - ๋ชจ๋์ ์ถ๊ฐ ํด์ฃผ๋ฉด js๋ก ๋ฌธ์  ํ์ด๊ฐ ๊ฐ๋ฅํ๋ค </p>
<p>
const fs = require("fs"); <br>

const input = fs.readFileSync("/dev/stdin").toString().split(' '); <br>
const arr = []; <br>

for(let i=0; i<input.length;i++){ <br>
    arr.push(parseInt(input[i],10)); <br>
}

const a = arr[0]; <br>
const b = arr[1]; <br>


console.log(a+b);   <br>
</p>
<p> 3๏ธโฃ ์ ์ฝ๋๋ ์ด๋ ๊ฒ๋ ๋ณํ ๊ฐ๋ฅ </p>
<p>
const fs = require("fs"); <br>
const [a,b] = fs.readFileSync("/dev/stdin").toString().split(' ').map(v=>parseInt(v,10)); <br>
console.log(a+b); <br>
</p>
  
  
  


