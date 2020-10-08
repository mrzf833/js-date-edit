# js-date-edit
var d = new Date("2020-10-08T14:59:10.353844Z");
let month = d.getMonth()+1;
let day = d.getDate();
let hour = d.getHours();
let minute = d.getMinutes();
let second = d.getSeconds();
let output = d.getFullYear() + "-" +
              ((""+month).length<2 ? '0' : "") + month + "-" +
              ((""+day).length<2 ? "0" : "") + day + ' ' + hour + ':' + 
              (("" + minute).length < 2 ? '0' : '') + minute + ':' + 
              (("" + second).length < 2 ? '0' : '') + second ;
document.getElementById("demo").innerHTML = output;
