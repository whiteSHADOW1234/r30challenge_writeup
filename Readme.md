# r30challenge
![](https://i.imgur.com/PAaWJJp.png)

- Press the red button to start this game

## Zero Level
![](https://i.imgur.com/IAhh1Nk.png)

- Pass the token it gave in the format `/lv1.php?token=xxx`

<!-- ANSWER: https://r30challenge.herokuapp.com/lv1.php?token=r30:start -->

## First Level
![](https://i.imgur.com/q1PMAnV.png)

```javascript=
// try to get the decimal number of the binary number it gave
var name = '100101001001100001110';
var result = parseInt(name,2);
console.log(res);

>>> 1217294

// try to convert it to String (base 18)
var name = '100101001001100001110';
var result = parseInt(name,2);
var res = result.toString(18);
console.log(result);

>>> bad18 
//pass this string as the token and it successfully bring us to the next level
```
- .toString() in javascript could convert every kind of data to String except for "null" and "undefined"

<!-- ANSWER: https://r30challenge.herokuapp.com//lv2.php?token=bad18 -->

### Look these to learn more
1. https://medium.com/unalai/%E8%AA%8D%E8%AD%98-parseint-parsefloat-%E8%88%87-number-%E8%BD%89%E6%8F%9B%E6%88%90%E6%95%B8%E5%AD%97%E7%9A%84%E4%B8%89%E7%A8%AE%E6%96%B9%E6%B3%95-276640aedb4e
2. https://codertw.com/%E5%89%8D%E7%AB%AF%E9%96%8B%E7%99%BC/254123/


## Second Level
![](https://i.imgur.com/ta1pIcR.png)

- Turn DevTools in Chrome by pressing F12
- Find the hidden token in the HTML file

<!-- ANSWER: https://r30challenge.herokuapp.com//lv3.php?token=divsurprise -->


## Third Level
![](https://i.imgur.com/SLEzGtW.png)

- Turn DevTools in Chrome by pressing F12
- Find the hidden token in the HTML file

<!-- ANSWER: https://r30challenge.herokuapp.com//lv4.php?token=commentfaker -->


## Fourth Level
![](https://i.imgur.com/t1W3O83.png)

- Find the token in the screen and pass it but it failed
- Open the `/lv4.js` file and you'll find a new key in it.
- Pass it and get this
![](https://i.imgur.com/bseRA4v.png)
- Try to stop loading it by pressing "ESC" while the screen pops out
- And you'll be able to access the Fifth Level

<!-- ANSWER: https://r30challenge.herokuapp.com//lv5.php?token=csspersona! -->

## Fifth Level
![](https://i.imgur.com/r15yPKq.png)

- Uhhh... the token is on the screen

<!-- ANSWER: https://r30challenge.herokuapp.com/lv6.php?token=windowhack -->

## Sixth Level

### Solution - 1
![](https://i.imgur.com/UwiqLnc.png)
- Type "window" and hit Enter in DevTool's console
- The tocken shows up at the last of the dark puper titles

### Solution - 2
- Open the `/lv6.js` file and copy the emojis at the bottom of the codes
![](https://i.imgur.com/oZ5vRpA.png)

- Use [Aadecode Online Decoder](https://cat-in-136.github.io/2010/12/aadecode-decode-encoded-as-aaencode.html) to decode the stuffs you just copied and you'll get your token
![](https://i.imgur.com/MivN20N.png)

<!-- ANSWER: https://r30challenge.herokuapp.com/lv7.php?token=emojicute -->


## Seventh Level
- Press the lock icon beside the URL and select "cookie"
- Open the Cookie package by clicking it and get your token `%7Bcookieyumyum%7D`
![](https://i.imgur.com/19XmGMM.png)
- But after using [URL Online Decoder](https://www.urldecoder.org/) your see this
![](https://i.imgur.com/P2bekn7.png)
- So the actual token is `cookieyumyum`

<!-- ANSWER: https://r30challenge.herokuapp.com/lv8.php?token=cookieyumyum -->

## Eighth Level
![](https://i.imgur.com/BD0HUL8.png)

- Open DevTools and select "Network" (at the top bar) and click "Headers" to find your token

<!-- ANSWER: https://r30challenge.herokuapp.com/lv9.php?token=headshot -->

## Ninth Level
![](https://i.imgur.com/Ngppxau.png)

- You'll get these rules after opening DevTools and press "Source" and click `/lv9.php?token=headshot` reading the php code in 
```cpp=
1. first_char_ASCII_number * second_char_ASCII_number % 1 = 0
2. third_char_ASCII_number * fourth_char_ASCII_number % 3 = 0
3. fifth_char_ASCII_number * sixth_char_ASCII_number % 5 = 0
4. seventh_char_ASCII_number * eighth_char_ASCII_number % 7 = 0
```
- Pass the string which follows the rules above by using [ASCII Code Table](https://www.wibibi.com/info.php?tid=ASCII_Code_Table)

<!-- ANSWER: https://r30challenge.herokuapp.com/lv10.php?token=aaccddii -->


## Tenth Level
![](https://i.imgur.com/fSo8W5R.png)
- Just tap open the api.php and the answer would pop up ...

<!-- ANSWER: https://r30challenge.herokuapp.com/lv11.php?token=sosdan -->

## Eleventh Level

#### Solution - 1
![](https://i.imgur.com/z9XqiMa.png)

- Enter the URL it gave and open the DevTools, select "Sources" and open the "news.js" file
![](https://i.imgur.com/RTDtwVP.png)
- Go to `http://r30challenge.herokuapp.com/news_api.php?id=888888` and grab your token
![](https://i.imgur.com/zIoZhZe.png)



#### Solution - 2
![](https://i.imgur.com/6x1ZnSh.png)

##### Ref
1. https://stackoverflow.com/questions/16482600/node-js-cannot-find-module-request
2. https://www.youtube.com/watch?v=qYwLOXjAiwM
- remember to add the address to your PATH!!!


<!-- ANSWER: https://r30challenge.herokuapp.com/lv12.php?token=fakeituntilyoumakeit -->

## Twelfth Level
![](https://i.imgur.com/pMO3OfQ.png)
- Open DevTools and press "Network", select "Headers" and you'll see the token in the response headers

<!-- ANSWER: https://r30challenge.herokuapp.com/lv13.php?token=you_are_cookie_master -->

## Thirteenth Level
![](https://i.imgur.com/O7hVhOO.png)
- Open the DevTools and select "Network"
- Pass some numbers in it and record the four number which website reacts longer than others(5371) 
- Kind of "Guessing number Game" (More time it reacts, more likely the answer is)

<!-- ANSWER: https://r30challenge.herokuapp.com/lv14.php?token=5371 -->

## Fourteenth Level
![](https://i.imgur.com/VVt6dVO.png)

- Open the DevTools, click "Sources" select "lv14.js" and you'll find these javascript codes
- Create a C++ code and after running it, you’ll get the token
```cpp=
//get the current time
#include <time.h>
#include <iostream>
#include <cstdlib>
using namespace std;
int main() {
    time_t t = time(NULL);
    struct tm *tm = localtime(&t);
    printf("%d-%d-%d %d:%d:%d\n", tm->tm_year + 1900, tm->tm_mon + 1, tm->tm_mday, tm->tm_hour, tm->tm_min, tm->tm_sec);
    int A = ((tm->tm_hour)*(tm->tm_min))+42;
    cout <<"The value of $a : " <<A << endl;

    // get the Acsii value of "z"
    int z = 'z'-65;
    //print the value of z
    cout << "The value of asii 'z' - 65 = " << z << endl;

    //print the largest prime factor of the value of n
    int isPrime = 1;
    int i;
    for(i = A;i>0;i--)
    {
        isPrime = 1;
        for(int j = 2; j<i;j++)
            if (i%j == 0 ) {
                isPrime = 0;
                continue;
            }
        if(isPrime == 1)
        {
            printf("%d",i);
            break;
        }
    }

    // Create a new variable and pass the rersult of the Integer C divided by the value of z
    int Z = A/z;// the int result
    int R = A%z;//the remainder
    cout << "The value of the result of the division "<<Z << endl;
    cout << "The value of the remainder of the division "<<R << endl;

    for ( int i = 0; i < Z ; i++)
    {
        cout << "z";
    }
    for ( int i = 0; i < 7-Z; i++){
        cout << "A";
    }
    cout << char(R+65) << endl;

    system("pause");
    return 0;
}
```

## Fifteenth Level
![](https://i.imgur.com/ZiACDLF.png)






