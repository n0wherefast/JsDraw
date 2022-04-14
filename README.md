# JsDraw

<body>
    <canvas width="600" height="600"></canvas>
  <script>
      let canvas = document.querySelector('canvas');
      let context = canvas.getContext('2d');

    
     context.lineWidth=4;
     
        let w = 60;
         let h = 60;
         let gap = 20;
         let x ,y ;
        
    
     for (let i =0; i<5; i++){
         for(let j=0; j<5; j++){
        
          x = 100 + (w+gap)*i;
          y = 100 +(w+gap)*j ;
         
         context.beginPath();
         context.rect(x,y,w,h)
         context.stroke()

        if(Math.random()>0.5){
         context.beginPath();
         context.rect(x+8,y+8,w-16,h-16)
         context.stroke();
        }
         
         
         

     }
    }

  </script>
  
</body>
