



3. ```javascript
    var breakfast = {
    name: 'The Lumberjack',
    price: '$9.95',
    ingredients: ['eggs', 'sausage', 'toast', 'hashbrowns', 'pancakes']
    }```




4. ```javascript
    var savingsAccount = {
    balance: 1000,
    interestRatePercent: 1,
    deposit: function addMoney(amount) {
        if (amount > 0) {
            savingsAccount.balance += amount;
        }
    },
    withdraw: function removeMoney(amount) {
        var verifyBalance = savingsAccount.balance - amount;
        if (amount > 0 && verifyBalance >= 0) {
            savingsAccount.balance -= amount;
        }
    },
    // your code goes here
    printAccountSummary: function() {
        console.log('Welcome!')
        return 'Your balance is currently $'+ this.balance+' and your interest rate is '+this.interestRatePercent+'%.'
    }
    };
    console.log(savingsAccount.printAccountSummary());
    ```

5. ```javascript
    var donuts = [
    { type: "Jelly", cost: 1.22 },
    { type: "Chocolate", cost: 2.45 },
    { type: "Cider", cost: 1.59 },
    { type: "Boston Cream", cost: 5.99 }
    ];

    // your code goes here
    donuts.forEach(function(donut){
       console.log(donut.type +' donuts cost $'+donut.cost+" each")
    });
    ```
