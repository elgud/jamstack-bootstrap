---
layout: layouts/home.njk
title: Javascript Functions
templateClass: tmpl-home
---

<div class="container mt-5">
  <h1>Basic Javascript Function Tasks</h1>

  <p>Open the console to view the results</p>
</div>

<script>
    // function from task 1
    function outputMessage(){
        console.log("This is a message");
    }

    // function from task 2
    function createName(firstname, lastname) {
        fullName = firstname + ' ' + lastname;
        console.log(fullName);
    }

    // function from task 3
    function createFullName(firstname, lastname) {
        return firstname + ' ' + lastname;
    }

    // function from task 4
    function wearacoat(temp) {
        if (temp <10)
            return 'You should wear a coat when the temperature is '+temp;
        else
            return 'You should not wear a coat when the temperature is '+temp;
    }

    function wearACoatExtra(temp){
        strMessage = 'You don\'t need a coat';
        if (temp < 0) {
            strMessage  = 'Don\'t go outside';
        }
        else if (temp < 10) {
            strMessage = 'You need a coat and hat';
        }
        else if (temp < 15) {
            strMessage = 'You need a coat';
        }
        
        return strMessage;
    }

    function wearACoatExtraExtra(temp){
        var strMessage = '';
        if (temp < 0) {
            strMessage  = 'Don\'t go outside';
        }
        else if (temp < 10) {
            strMessage = 'You need a coat and hat';
        }
        else if (temp < 15) {
            strMessage = 'You need a coat';
        }
        if (!strMessage){
            strMessage = "You don't need to wear a coat";
        }
        
        return strMessage;
    }       
    console.log('Task 1 below');
    console.log('--------------');
    // calls the outputMessageFunction
    outputMessage();
    console.log('---------------');
    console.log('Task 1 above');
    console.log(' ');

    console.log('Task 2 below');
    console.log('--------------');
    // calls the createName function
    createName('Jim','Stott');
    var fname = 'Jane';
    var lname = 'Leaver'
    createName(fname,lname);
    console.log('---------------');
    console.log('Task 2 above');
    console.log(' ');

    console.log('Task 3 below');
    console.log('--------------');
    // calls the createFullName function which returns a string
    var fullName = createFullName(fname, lname);
    console.log(fullName);
    console.log(createFullName(fname, lname));
    console.log('---------------');
    console.log('Task 3 above');
    console.log(' ');

    console.log('Task 4 below');
    console.log('--------------');
    // calls the createFullName function which returns a string
    var temperature = 15;
    console.log(wearacoat(temperature));
    temperature = -5;
    console.log(wearacoat(temperature));
    console.log('---------------');
    console.log('Task 4 above');
    console.log(' ');

    console.log('--------Task 5 below ');
    console.log(wearACoatExtra(-4));
    console.log(wearACoatExtra(9));
    console.log(wearACoatExtra(14));
    console.log(wearACoatExtra(18));

    console.log('\n-------------Task 6 below ');
    console.log(wearACoatExtraExtra(-4));
    console.log(wearACoatExtraExtra(9));
    console.log(wearACoatExtraExtra(14));
    console.log(wearACoatExtraExtra(18));
   

</script>