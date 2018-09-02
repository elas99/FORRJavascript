# FORRJavascript
Javascript áfangi
1. Null, er "Value of nothing" sem þýðir að það er gildi, en það gildir sem ekkert, en þegar þú notar undefined þá er ''absence of value'' sem þýðir að það er meira að segja ekki gildi skráð.
notkun: 'var a = null;' og 'var a' fyrir undefined

2.Use strict lætur þig nota Strict Mode, sem gerir það léttara að troubleshoota því þú getur séð villurnar í staðinn fyrir að sjá bara t.d. ''Bad Syntax''

3. 


5. Býr til undefined function sem gerir alert('Hello World'), sviganir í enda kalla í functionið strax

6. 
 
  2. function foo(){
 
  4. function bar() {
  
  5.   return 3;
  
      }
      
  3.     return bar(); 
  
  6. function bar() { //Þetta overwrite'ar function bar og breytir því í 8 í staðinn fyrir 3.
  
  7.    return 8;
  
      }
      
    }
    
  1. alert(foo()); 
  

7.


8.
 <code>
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
  </code>

9.
