# FORRJavascript
Javascript áfangi Verkefni 1

1. Null, er "Value of nothing" sem þýðir að það er gildi, en það gildir sem ekkert,
en þegar þú notar undefined þá er ''absence of value'' sem þýðir að það er meira að segja ekki gildi skráð.
notkun: 'var a = null;'
         'var a' fyrir undefined

2.Use strict lætur þig nota Strict Mode, sem gerir það léttara að troubleshoota
því þú getur séð villurnar í staðinn fyrir að sjá bara t.d. ''Bad Syntax''

3. Let er aðeins notað í 'Block' eða 'Scope' sem þú ert nú þegar staddur í,
en var er variable sem fer í gegnum allt,
hérna er dæmi um hvað ég meina https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/block
td ef þú setur var í einhverja for loop'u, þá mun það halda gildinu sem hún fékk í for loopinu fyrir utan loopuna,
en let hefur aðeins gildið inn í for loopuni 

4.       ```javascript
         1. function fall(a, b) {
                   return a + b;
                  }
         2. var fall = function(a, b) {
                   return a + b;
                  };
                  
          3. var fall = function abcfall(a, b) {
                     return a + b;      //fall og abcfall geta líka bæði heitið fall, eina ástæðan að nota er fyrir debugging
                  };
           ```
                  
                  
                  
                 

5. Býr til undefined function sem gerir alert('Hello World'), sviganir í enda kalla í functionið strax

6. 
         ```javascript
         2. function foo(){
         4. function bar() {
         5.   return 3;
             }
         3.     return bar();  
         6. function bar() { //Þetta overwrite'ar function bar og breytir því í 8 í staðinn fyrir 3.
         7.   return 8;
              }     
            }   
         1. alert(foo()); 
         ```
  
7. for og for-in hefur verið til lengi en for-of aðeins frá ECMAScript 6


8.
  ```javascript
  var test = [12, 929, 11, 3, 199, 1000, 7, 1, 24, 37, 4,
    19, 300, 3775, 299, 36, 209, 148, 169, 299,   
    6, 109, 20, 58, 139, 59, 3, 1, 139  
  ];
  
  // Write your code here
  test.forEach(function(tests)
  {
     if(tests % 3 === 0)    
     {
          tests = tests + 100
      }
     console.log(tests);
  });
  ```

9.
         ```javascript
    var bills = [50.23, 19.12, 34.01,
      100.11, 12.15, 9.90, 29.11, 12.99,
        10.00, 99.22, 102.20, 100.10, 6.77, 2.22
    ];

    var totals = bills.map(function(total) {
      total = total * 1.15;
      total = total.toFixed(2);
      console.log(total);
    });
         ```
10.
    ```javascript
          var numbers = [
          [243, 12, 23, 12, 45, 45, 78, 66, 223, 3],
          [34, 2, 1, 553, 23, 4, 66, 23, 4, 55],
         [67, 56, 45, 553, 44, 55, 5, 428, 452, 3],
         [12, 31, 55, 445, 79, 44, 674, 224, 4, 21],
         [4, 2, 3, 52, 13, 51, 44, 1, 67, 5],
          [5, 65, 4, 5, 5, 6, 5, 43, 23, 4424],
          [74, 532, 6, 7, 35, 17, 89, 43, 43, 66],
          [53, 6, 89, 10, 23, 52, 111, 44, 109, 80],
           [67, 6, 53, 537, 2, 168, 16, 2, 1, 8],
          [76, 7, 9, 6, 3, 73, 77, 100, 56, 100]
         ];

         // your code goes here
         for (var r = 0; r < numbers.length; r++) {
           for (var c = 0; c < numbers[r].length; c++) {
            if(numbers[r][c] % 2 === 0)
            {
             console.log("even");
            }
           else{
            console.log("odd");
          }
           }
          }
         ```
   
