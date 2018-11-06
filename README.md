# js-callee
callee（谁调用了它）


   比如 写一个递归阶乘
   
      在这种有函数名的情况下可以这样写：
      
         function test(n){
           if(n==1){
           return 1
           }
           
           return n*test(n-1)
         }
    test(20)    //2432902008176640000
    
    
    但是还有一种情况，比如没有函数名，你怎么写阶乘？？？？
    
      有办法  这时候就用到了 callee，它是做啥的了？它是查看说调用了
      
        例如:
        
           var test=(functin (n){
               if(n==1){
                 return 1
                }
              return n*arguments.callee(n-1)
           }(20))
        
        
           test   //2432902008176640000
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
    
    
    
    
    
    
    
    
    
    
