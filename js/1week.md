#프로그래머스

javascript
function solution(array, commands) {
const answer = [];
for (let i =0; i<commands.length; i++){
let arr= array.slice(commands[i][0]-1 , commands[i][1])
arr.sort(function( a,b){
return a-b;
} );
answer.push(arr[commands[i][2] -1]);
}
