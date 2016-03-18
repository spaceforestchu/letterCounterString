    # letterCounterString
    function alphaCount (alphabet, text) {
      var results = '';
      alphabet = alphabet.toLowerCase().split('');
      text = text.toLowerCase().split('');
     var trueCounter = 0;
      alphabet.forEach(function(item){
          var counter = 0;
          text.forEach(function(i){
              
            if(item === i){
                counter++;
                trueCounter = counter;
                
            }
                 
          });
         
         if(counter > 0){
          
             results += item;
             results += ":";
             results += counter;
             results += ",";
         }
         
         
         
      });
    
        if(trueCounter > 0){
           
            return results.slice(0,-1);
        } else {
            return "no matches";
        }
    
    }
    
    
    alphaCount("i8gec","uoeu8382aeouhi488ap283.8");
