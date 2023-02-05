# Number1
/*Задание 1


Необходимо создать функцию myFunction, которая принимает два числовых аргумента a и b,
Найти сумму четных чисел и их количество в диапазоне от a(начало диапазона) до b(конец диапазона)
Для вывода результата из функции используем console.log("ваш результат");*/




let a = 6;
do {console.log (a);
a ++;
} while (a %2 === 0);


let b = 4;
do {console.log (b);
b ++;
} while (a %2 === 0);


let AB = a + b
console.log (AB);
console.log ('сумма чётных чисел и их количество' + '/n' + AB.length);






































/*Задание 2


Необходимо создать функцию isPrime, которая принимает одно число num.
Функция определяет простое ли число (число называется простым, если оно делится только само на себя и на 1)
Функция должна возвращать значение типа boolean(true/false);*/


 let isBoolean;
 if ( typeof isBoolean == 'number') {
isBoolean=true;
}


console.log ( "isBoolean" , isBoolean ) ;  


function isPrime (isBoolean) {
                                                                     
let isBoleanSimple = isBoolean/isBoolean;
     if ( isBoleanSimple = 1) {
         console.log ( "это простое число!", true) ;
     }
    else {
        console.log (false)
    }


    let isBoleanSimple2 = isBoolean/1
     if ( isBoleanSimple2 == 'number') {
         console.log (true) ;
     } else {
         console.log (false)
     }




    }


    console.log ( isPrime (7));
/*Задание 3


Необходимо создать 2 функции getSqrtBySequentialSelection и getSqrtByBinarySearch каждая из которых
принимают один аргумент number(число) обе функции будут находить и возвращать корень натурального
числа с точностью до целого(аналогично вызову Math.sqrt(number)).
Соответственно результат выполнения у двух функций будет одинаковый, а реализация разная.
getSqrtBySequentialSelection будет находить корень методом последовательного подбора;
getSqrtByBinarySearch будет находить корень методом бинарного поиска;
Math.sqrt в задании использовать нельзя. */




let n;
let m = 64;
function getSqrtBySequentialSelection(m) {
    for (let i = 1; ;i++) {
        let q = i * i;
        if (m == q) return i;
        if (m < q) return i - 1;
    }
}
n = getSqrtBySequentialSelection(m);
console.log(n);
function getSqrtByBinarySearch(m) {
    let min = 1;
    let max = m;
    let prev = 0;
    for (;;) {
        let mid = (min + max) / 2;
        if (prev == mid) return mid;
        let q = mid * mid;
        if (m == q) return mid;
        if (m < q) max = mid;
        else min = mid;
        prev = mid;
    }
}
n = getSqrtByBinarySearch(m);
console.log(n);
/*Задание 4


Необходимо создать функцию getFactorial, которая принимает одно число n.
Функция возвращает факториал числа n.(n! = 1*2*…*n-1*n) */






function getFactorial (n) {
    if (typeof n == 'number') {
        return (n = 1*2*3*n-1*n)
    }
}


/* Задание 5


Необходимо создать функцию digitSum, которая принимает одно число y.
Функция возвращает сумму цифр заданного числа*/


let y = 11;
let sum = new Function ('y', 'return y+y;');
let result = sum (y, y);
console.log (result);
