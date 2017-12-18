### _Stack Motion Effects_ 
             By   
        - Mary lou
        - Julian gurner
       
**MainJS**

   	this.DOM.columns.left.style.opacity= 0;
    this.DOM.columns.right.style.opacity = 0;
   		

----------


        anime({
            targets: this.DOM.stackItems,
            translateZ: [
                { 
                    value: function(target, index) {
                        return index * 10 + 10 - 8;
                    },
                    duration: 200 ,
                    easing: [0.42,0,1,1]
                },
                { 
                    value: 0,
                    duration: 900,
                    easing: [0.2,1,0.3,1]
                }
            ]
        	)};		