# basilisk
print engine


```
文字列キャンバスを作ればいい。

String.prototype.splice = function(idx, rem, s) {
    return (this.slice(0, idx) + s + this.slice(idx + Math.abs(rem)));
};

String.prototype.clear=function(s){
 if(s===null) s=''
 return this.split('').map(d=>s).join('')
}

let aaa='foo bazxxxx'.splice(4,'bar '.length,'bar ')
console.log(aaa)

console.log(aaa.clear())

```


```
canvas(w,h,t)は文字列キャンバスを生成し、文字列で埋める。
echo(l,t) は、その行をクリアしてから、文字列を指定した行へ追加する。
echoAt(l,s,t)は、行列を指定し、文字列を指定した場所へ、上書きする。

```



```
