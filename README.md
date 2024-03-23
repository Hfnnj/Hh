* {
    margin: 0;
    padding: 0;
  }
  
  html,
  body {
    height: 100%;
    /* for touch screen */
    touch-action: none; 
  }
  
  body {
    overflow: hidden;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    background: #111;
    -webkit-perspective: 1000px;
            perspective: 1000px;
    -webkit-transform-style: preserve-3d;
            transform-style: preserve-3d;
  }
  
  #drag-container, #spin-container {
    position: relative;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    margin: auto;
    -webkit-transform-style: preserve-3d;
            transform-style: preserve-3d;
    -webkit-transform: rotateX(-10deg);
            transform: rotateX(-10deg);
            z-index: 100;
  }
  
  #drag-container img, #drag-container video {
    -webkit-transform-style: preserve-3d;
            transform-style: preserve-3d;
    position: absolute;
    left: 0;
    top: 0;
    max-width: 120%;
    max-height: 120%; 
    line-height: 200px;
    font-size: 50px;
    text-align: center;
    -webkit-box-shadow: 0 0 8px #fff;
            box-shadow: 0 0 8px #fff;
    -webkit-box-reflect: below 10px linear-gradient(transparent, transparent, #0005);
  }
  
  #drag-container img:hover, #drag-container video:hover {
    -webkit-box-shadow: 0 0 15px #fffd;
            box-shadow: 0 0 15px #fffd;
    -webkit-box-reflect: below 10px linear-gradient(transparent, transparent, #0007);
  }
  
  #drag-container p {
    
    position: absolute;
    top: 100%;
    left: 50%;
    -webkit-transform: translate(-50%,-50%) rotateX(90deg);
            transform: translate(-50%,-50%) rotateX(90deg);
    color: rgb(0, 195, 255);
    animation: fadein ease 15s;
  }

  @keyframes fadein {
      from {
          opacity:0;
          
      }
      to {
          opacity: 1;
          
      }
  }
  
  #ground {
    width: 900px;
    height: 900px;
    position: absolute;
    top: 100%;
    left: 50%;
    -webkit-transform: translate(-50%,-50%) rotateX(90deg);
            transform: translate(-50%,-50%) rotateX(90deg);
    background: -webkit-radial-gradient(center center, farthest-side , #9993, transparent);
  }
  
  #music-container {
    position: absolute;
    top: 0;
    left: 0;
    display: none;
  }
  
  @-webkit-keyframes spin {
    from{
      -webkit-transform: rotateY(0deg);
              transform: rotateY(0deg);
    } to{
      -webkit-transform: rotateY(360deg);
              transform: rotateY(360deg);
    }
  }
  
  @keyframes spin {
    from{
      -webkit-transform: rotateY(0deg);
              transform: rotateY(0deg);
    } to{
      -webkit-transform: rotateY(360deg);
              transform: rotateY(360deg);
    }
  }
  @-webkit-keyframes spinRevert {
    from{
      -webkit-transform: rotateY(360deg);
              transform: rotateY(360deg);
    } to{
      -webkit-transform: rotateY(0deg);
              transform: rotateY(0deg);
    }
  }
  @keyframes spinRevert {
    from{
      -webkit-transform: rotateY(360deg);
              transform: rotateY(360deg);
    } to{
      -webkit-transform: rotateY(0deg);
              transform: rotateY(0deg);
    }
  }

  #canvas {
    background-color:transparent;   
    color: transparent; 
    margin: 0;
    overflow: hidden;
    background-repeat: no-repeat;
    width: 100vw;
  }


#canva {
    position: absolute;
    top: 0px;
    right: 0px;
    overflow: hidden;
}

p {
    font-family: 'Dancing Script', cursive;
    font-family: 'Rampart One', cursive;
    font-size: 4vw;
    
}
