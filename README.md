body {
    background-color: #EDE9DE;
    font-family: 'Dancing Script', cursive;
    margin: 0;
    padding: 0;
    -webkit-backface-visibility: hidden;
    /* Chrome, Safari, Opera */
    backface-visibility: hidden;
}

.gift {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 300px;
    height: 300px;
    transform: translate3d(-50%, -50%, 0);
    cursor: pointer;
}

.gift-top {
    position: relative;
    width: 100%;
    height: 25%;
    background: #F54537;
    border-radius: 5px 5px 0 0;
    background-image: linear-gradient(to right, #f2adab 0%, #f2adab 44%, #faebc3 44%, #faebc3 56%, #f2adab 56%, #f2adab 100%);
}

.gift-top.hovered {
    animation: shake 3s infinite;
    -webkit-animation: shake 3s infinite;
    -moz-animation: shake 3s infinite;
    -ms-animation: shake 3s infinite;
    -o-animation: shake 3s infinite;
}

.gift-bottom.fadeout {
    -webkit-animation-name: fadeOutDown;
    animation-name: fadeOutDown;
    -webkit-animation-duration: 1s;
    animation-duration: 1s;
    -webkit-animation-fill-mode: both;
    animation-fill-mode: both;
}

.gift-top.fadeout {
    -webkit-animation-name: rotateOutUpRight;
    animation-name: rotateOutUpRight;
    -webkit-animation-duration: 1s;
    animation-duration: 1s;
    -webkit-animation-fill-mode: both;
    animation-fill-mode: both;
}

.gift-top::before,
.gift-top::after {
    content: "";
    width: 15px;
    height: 15px;
    border: 10px solid #faebc3;
    border-radius: 50% 50% 0 50%;
    position: absolute;
    top: 0;
    left: 50%;
    transform: translate3d(-100%, -100%, 0) skew(10deg, 10deg);
}

.gift-top::after {
    border-radius: 50% 50% 50% 0;
    transform: translate3d(0, -100%, 0) skew(-10deg, -10deg);
}

.gift-text {
    color: #333333;
    text-align: center;
}

.gift-final-text {
    text-align: center;
    font-size: 33px;
    display: none;
}

.gift-bottom {
    width: 95%;
    height: 75%;
    margin: 0 auto;
    background-image: linear-gradient(to right, #f2adab 0%, #f2adab 45%, #faebc3 45%, #faebc3 55%, #f2adab 55%, #f2adab 100%);
    border-radius: 0 0 5px 5px;
}

.gift-card-text {
    display: none;
    font-size: 33px;
    top: 50%;
    left: 50%;
    transform: translate3d(-50%, -50%, 0);
    position: absolute;
    width: 100%;
}

.lbWrapper {
    width: 100%;
    height: 100%;
    position: fixed;
    background: rgba(0, 0, 0, 0.8);
    padding: 0;
    z-index: 10;
    top: 0;
    left: 0;
    color: #fff;
    display: none;
}

.signupWrapper {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    -webkit-transform: translate(-50%, -50%);
    -moz-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    display: none;
}

.signupWrapper .error {
    display: none;
    color: #ff0000;
    text-align: center;
}

.signupWrapper .signUpTitle {
    text-align: center;
    font-size: 20px;
    text-transform: uppercase;
}

.signupWrapper .mlistWrapper {
    text-align: center;
    margin-top: 20px;
}

.signupWrapper input#email {
    width: 150px;
    border: none;
    box-shadow: none;
    padding: 5px;
}

.signupWrapper input.submit {
    padding: 4px 10px;
    cursor: pointer;
}

#snow {
    width: 100%;
}

@keyframes shake {
    0% {
        transform: rotate(0deg);
    }
    12% {
        transform: rotate(-10deg);
    }
    25% {
        transform: rotate(10deg);
    }
    37% {
        transform: rotate(0deg);
    }
    100% {
        transform: rotate(0deg);
    }
}

@-webkit-keyframes shake {
    0% {
        -webkit-transform: rotate(0deg);
    }
    12% {
        -webkit-transform: rotate(-10deg);
    }
    25% {
        -webkit-transform: rotate(10deg);
    }
    37% {
        -webkit-transform: rotate(0deg);
    }
    100% {
        -webkit-transform: rotate(0deg);
    }
}

@-moz-keyframes shake {
    0% {
        -moz-transform: rotate(0deg);
    }
    12% {
        -moz-transform: rotate(-10deg);
    }
    25% {
        -moz-transform: rotate(10deg);
    }
    37% {
        -moz-transform: rotate(0deg);
    }
    100% {
        -moz-transform: rotate(0deg);
    }
}

@-ms-keyframes shake {
    0% {
        -ms-transform: rotate(0deg);
    }
    12% {
        -ms-transform: rotate(0deg);
    }
    25% {
        -ms-transform: rotate(10deg);
    }
    37% {
        -ms-transform: rotate(0deg);
    }
    100% {
        -ms-transform: rotate(0deg);
    }
}

@-o-keyframes shake {
    0% {
        -o-transform: rotate(0deg);
    }
    12% {
        -o-transform: rotate(0deg);
    }
    25% {
        -o-transform: rotate(10deg);
    }
    37% {
        -o-transform: rotate(0deg);
    }
    100% {
        -o-transform: rotate(0deg);
    }
}

@-webkit-keyframes fadeOutDown {
    0% {
        opacity: 1;
    }
    100% {
        opacity: 0;
        -webkit-transform: translate3d(0, 100%, 0);
        transform: translate3d(0, 100%, 0);
    }
}

@keyframes fadeOutDown {
    0% {
        opacity: 1;
    }
    100% {
        opacity: 0;
        -webkit-transform: translate3d(0, 100%, 0);
        transform: translate3d(0, 100%, 0);
    }
}

@-webkit-keyframes rotateOutUpRight {
    0% {
        -webkit-transform-origin: right bottom;
        transform-origin: right bottom;
        opacity: 1;
    }
    100% {
        -webkit-transform-origin: right bottom;
        transform-origin: right bottom;
        -webkit-transform: rotate3d(0, 0, 1, 90deg);
        transform: rotate3d(0, 0, 1, 90deg);
        opacity: 0;
    }
}

@keyframes rotateOutUpRight {
    0% {
        -webkit-transform-origin: right bottom;
        transform-origin: right bottom;
        opacity: 1;
    }
    100% {
        -webkit-transform-origin: right bottom;
        transform-origin: right bottom;
        -webkit-transform: rotate3d(0, 0, 1, 90deg);
        transform: rotate3d(0, 0, 1, 90deg);
        opacity: 0;
    }
}


/*Santa CSS*/

.santa-wrapper {
    width: 280px;
    height: 280px;
    background: #a0d5d3;
    position: absolute;
    top: 50%;
    left: 50%;
    border-radius: 50%;
    margin-top: -60px;
    -webkit-transform: translate(-50%, -50%);
    -moz-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    -o-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    border: 10px solid #f8e7dc;
    overflow: hidden;
    display: none;
}

.santa {
    position: absolute;
    left: 50%;
    bottom: 0;
    -webkit-transform: translateX(-50%);
    -moz-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    -o-transform: translateX(-50%);
    transform: translateX(-50%);
}

.santa .body {
    width: 190px;
    height: 210px;
    background: #de2f32;
    position: relative;
    border-radius: 50%;
    top: 0;
    -webkit-animation: bodyLaugh 4s linear infinite;
    -moz-animation: bodyLaugh 4s linear infinite;
    -ms-animation: bodyLaugh 4s linear infinite;
    -o-animation: bodyLaugh 4s linear infinite;
    animation: bodyLaugh 4s linear infinite;
    -webkit-transform: translateY(50%);
    -moz-transform: translateY(50%);
    -ms-transform: translateY(50%);
    -o-transform: translateY(50%);
    transform: translateY(50%);
}

.santa .body:before {
    content: " ";
    width: 7px;
    height: 7px;
    background: #f7be10;
    border-radius: 50%;
    position: absolute;
    top: 35%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    -moz-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    -o-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    box-shadow: 0px -18px 0px #f7be10, 0px 18px 0px #f7be10;
}

.santa .head {
    z-index: 2;
    position: absolute;
    bottom: 90px;
    left: 50%;
    -webkit-animation: headLaugh 4s linear infinite;
    -moz-animation: headLaugh 4s linear infinite;
    -ms-animation: headLaugh 4s linear infinite;
    -o-animation: headLaugh 4s linear infinite;
    animation: headLaugh 4s linear infinite;
    -webkit-transform: translateX(-50%);
    -moz-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    -o-transform: translateX(-50%);
    transform: translateX(-50%);
}

.santa .head .face {
    width: 120px;
    height: 130px;
    background: #edcab0;
    background: radial-gradient(#edcab0, #e9a982);
    border-radius: 50%;
    border: 3px solid #f8e7dc;
}

.santa .head .face .redhat .whitepart {
    position: absolute;
    left: 50%;
    top: 0;
    -webkit-transform: translateX(-50%);
    -moz-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    -o-transform: translateX(-50%);
    transform: translateX(-50%);
    width: 90%;
    height: 32px;
    background: #f8e7dc;
    border-radius: 50px;
    z-index: 4;
    box-shadow: 0px 6px 0px -4px rgba(0, 0, 0, 0.1);
}

.santa .head .face .redhat .redpart {
    width: 120px;
    height: 120px;
    background: #de2f32;
    position: absolute;
    top: -50px;
    left: 15px;
    border-radius: 50%;
    z-index: -1;
}

.santa .head .face .redhat .redpart:before {
    content: " ";
    width: 95px;
    height: 95px;
    position: absolute;
    left: 0;
    top: 12px;
    border-radius: 50%;
    box-shadow: inset -8px -1px 0px -5px rgba(0, 0, 0, 0.05);
}

.santa .head .face .redhat .redpart:after {
    content: " ";
    position: absolute;
    right: 0;
    top: 60px;
    background: #de2f32;
    width: 20px;
    height: 50px;
}

.santa .head .face .redhat .hatball {
    width: 38px;
    height: 38px;
    background: #f8e7dc;
    border-radius: 50%;
    z-index: 5;
    position: absolute;
    right: -20px;
    top: 40px;
    box-shadow: 0px 6px 0px -4px rgba(0, 0, 0, 0.1);
}

.santa .head .face .eyes {
    position: absolute;
    left: 50%;
    -webkit-transform: translateX(-50%);
    -moz-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    -o-transform: translateX(-50%);
    transform: translateX(-50%);
    top: 57px;
}

.santa .head .face .eyes:before,
.santa .head .face .eyes:after {
    content: " ";
    position: absolute;
    width: 15px;
    height: 9px;
    top: 0;
    border: 5px solid #a8744f;
    border-width: 0;
    border-top-width: 5px;
    border-radius: 50%;
}

.santa .head .face .eyes:before {
    left: -28px;
}

.santa .head .face .eyes:after {
    right: -28px;
}

.santa .head .face .beard {
    width: 55px;
    height: 55px;
    background: #f8e7dc;
    border-radius: 50%;
    position: absolute;
    bottom: -30px;
    left: 50%;
    -webkit-animation: beardLaugh 4s linear infinite;
    -moz-animation: beardLaugh 4s linear infinite;
    -ms-animation: beardLaugh 4s linear infinite;
    -o-animation: beardLaugh 4s linear infinite;
    animation: beardLaugh 4s linear infinite;
    -webkit-transform: translateX(-50%);
    -moz-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    -o-transform: translateX(-50%);
    transform: translateX(-50%);
}

.santa .head .face .beard:before,
.santa .head .face .beard:after {
    content: " ";
    width: 80px;
    height: 80px;
    background: #f8e7dc;
    border-radius: 50%;
    position: absolute;
    bottom: 15px;
}

.santa .head .face .beard:before {
    left: -40px;
}

.santa .head .face .beard:after {
    right: -40px;
}

.santa .head .face .beard .nouse {
    width: 25px;
    height: 20px;
    border-radius: 50%;
    background: #edcab0;
    position: absolute;
    z-index: 3;
    box-shadow: inset -3px -3px 0px #e9a982;
    left: 50%;
    -webkit-transform: translateX(-50%);
    -moz-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    -o-transform: translateX(-50%);
    transform: translateX(-50%);
    top: -42px;
}

.santa .head .face .beard .mouth {
    background: #a8744f;
    z-index: 3;
    position: absolute;
    width: 15px;
    height: 5px;
    border-bottom-right-radius: 80px 50px;
    border-bottom-left-radius: 80px 50px;
    left: 50%;
    top: 0;
    -webkit-animation: mouthLaugh 4s linear infinite;
    -moz-animation: mouthLaugh 4s linear infinite;
    -ms-animation: mouthLaugh 4s linear infinite;
    -o-animation: mouthLaugh 4s linear infinite;
    animation: mouthLaugh 4s linear infinite;
    -webkit-transform: translateX(-50%);
    -moz-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    -o-transform: translateX(-50%);
    transform: translateX(-50%);
}

.santa .head .ears:before,
.santa .head .ears:after {
    content: " ";
    width: 20px;
    height: 30px;
    border-radius: 50%;
    background: radial-gradient(#e9a982, #edcab0);
    position: absolute;
    top: 50%;
    z-index: -1;
}

.santa .head .ears:before {
    left: -8px;
    -webkit-transform: rotate(-10deg);
    -moz-transform: rotate(-10deg);
    -ms-transform: rotate(-10deg);
    -o-transform: rotate(-10deg);
    transform: rotate(-10deg);
}

.santa .head .ears:after {
    right: -8px;
    -webkit-transform: rotate(10deg);
    -moz-transform: rotate(10deg);
    -ms-transform: rotate(10deg);
    -o-transform: rotate(10deg);
    transform: rotate(10deg);
}

@-webkit-keyframes bodyLaugh {
    0% {
        top: 0px;
    }
    2% {
        top: -3px;
    }
    4% {
        top: 0px;
    }
    8% {
        top: -3px;
    }
    10% {
        top: 0px;
    }
    12% {
        top: -3px;
    }
    14% {
        top: 0px;
    }
    18% {
        top: -3px;
    }
    20% {
        top: 0px;
    }
    22% {
        top: -3px;
    }
    24% {
        top: 0px;
    }
    28% {
        top: -3px;
    }
    30% {
        top: 0px;
    }
    100% {
        top: 0px;
    }
}

@-moz-keyframes bodyLaugh {
    0% {
        top: 0px;
    }
    2% {
        top: -3px;
    }
    4% {
        top: 0px;
    }
    8% {
        top: -3px;
    }
    10% {
        top: 0px;
    }
    12% {
        top: -3px;
    }
    14% {
        top: 0px;
    }
    18% {
        top: -3px;
    }
    20% {
        top: 0px;
    }
    22% {
        top: -3px;
    }
    24% {
        top: 0px;
    }
    28% {
        top: -3px;
    }
    30% {
        top: 0px;
    }
    100% {
        top: 0px;
    }
}

@-ms-keyframes bodyLaugh {
    0% {
        top: 0px;
    }
    2% {
        top: -3px;
    }
    4% {
        top: 0px;
    }
    8% {
        top: -3px;
    }
    10% {
        top: 0px;
    }
    12% {
        top: -3px;
    }
    14% {
        top: 0px;
    }
    18% {
        top: -3px;
    }
    20% {
        top: 0px;
    }
    22% {
        top: -3px;
    }
    24% {
        top: 0px;
    }
    28% {
        top: -3px;
    }
    30% {
        top: 0px;
    }
    100% {
        top: 0px;
    }
}

@keyframes bodyLaugh {
    0% {
        top: 0px;
    }
    2% {
        top: -3px;
    }
    4% {
        top: 0px;
    }
    8% {
        top: -3px;
    }
    10% {
        top: 0px;
    }
    12% {
        top: -3px;
    }
    14% {
        top: 0px;
    }
    18% {
        top: -3px;
    }
    20% {
        top: 0px;
    }
    22% {
        top: -3px;
    }
    24% {
        top: 0px;
    }
    28% {
        top: -3px;
    }
    30% {
        top: 0px;
    }
    100% {
        top: 0px;
    }
}

@-webkit-keyframes beardLaugh {
    0% {
        bottom: -28px;
    }
    2% {
        bottom: -30px;
    }
    4% {
        bottom: -28px;
    }
    8% {
        bottom: -30px;
    }
    10% {
        bottom: -28px;
    }
    12% {
        bottom: -30px;
    }
    14% {
        bottom: -28px;
    }
    18% {
        bottom: -30px;
    }
    20% {
        bottom: -28px;
    }
    22% {
        bottom: -30px;
    }
    24% {
        bottom: -28px;
    }
    28% {
        bottom: -30px;
    }
    30% {
        bottom: -28px;
    }
    100% {
        bottom: -28px;
    }
}

@-moz-keyframes beardLaugh {
    0% {
        bottom: -28px;
    }
    2% {
        bottom: -30px;
    }
    4% {
        bottom: -28px;
    }
    8% {
        bottom: -30px;
    }
    10% {
        bottom: -28px;
    }
    12% {
        bottom: -30px;
    }
    14% {
        bottom: -28px;
    }
    18% {
        bottom: -30px;
    }
    20% {
        bottom: -28px;
    }
    22% {
        bottom: -30px;
    }
    24% {
        bottom: -28px;
    }
    28% {
        bottom: -30px;
    }
    30% {
        bottom: -28px;
    }
    100% {
        bottom: -28px;
    }
}

@-ms-keyframes beardLaugh {
    0% {
        bottom: -28px;
    }
    2% {
        bottom: -30px;
    }
    4% {
        bottom: -28px;
    }
    8% {
        bottom: -30px;
    }
    10% {
        bottom: -28px;
    }
    12% {
        bottom: -30px;
    }
    14% {
        bottom: -28px;
    }
    18% {
        bottom: -30px;
    }
    20% {
        bottom: -28px;
    }
    22% {
        bottom: -30px;
    }
    24% {
        bottom: -28px;
    }
    28% {
        bottom: -30px;
    }
    30% {
        bottom: -28px;
    }
    100% {
        bottom: -28px;
    }
}

@keyframes beardLaugh {
    0% {
        bottom: -28px;
    }
    2% {
        bottom: -30px;
    }
    4% {
        bottom: -28px;
    }
    8% {
        bottom: -30px;
    }
    10% {
        bottom: -28px;
    }
    12% {
        bottom: -30px;
    }
    14% {
        bottom: -28px;
    }
    18% {
        bottom: -30px;
    }
    20% {
        bottom: -28px;
    }
    22% {
        bottom: -30px;
    }
    24% {
        bottom: -28px;
    }
    28% {
        bottom: -30px;
    }
    30% {
        bottom: -28px;
    }
    100% {
        bottom: -28px;
    }
}

@-webkit-keyframes headLaugh {
    0% {
        bottom: 83px;
    }
    45% {
        bottom: 83px;
    }
    50% {
        bottom: 90px;
    }
    92% {
        bottom: 90px;
    }
    98% {
        bottom: 83px;
    }
    100% {
        bottom: 83px;
    }
}

@-moz-keyframes headLaugh {
    0% {
        bottom: 83px;
    }
    45% {
        bottom: 83px;
    }
    50% {
        bottom: 90px;
    }
    92% {
        bottom: 90px;
    }
    98% {
        bottom: 83px;
    }
    100% {
        bottom: 83px;
    }
}

@-ms-keyframes headLaugh {
    0% {
        bottom: 83px;
    }
    45% {
        bottom: 83px;
    }
    50% {
        bottom: 90px;
    }
    92% {
        bottom: 90px;
    }
    98% {
        bottom: 83px;
    }
    100% {
        bottom: 83px;
    }
}

@keyframes headLaugh {
    0% {
        bottom: 83px;
    }
    45% {
        bottom: 83px;
    }
    50% {
        bottom: 90px;
    }
    92% {
        bottom: 90px;
    }
    98% {
        bottom: 83px;
    }
    100% {
        bottom: 83px;
    }
}

@-webkit-keyframes mouthLaugh {
    0% {
        width: 20px;
    }
    45% {
        width: 20px;
    }
    50% {
        width: 15px;
    }
    92% {
        width: 15px;
    }
    98% {
        width: 20px;
    }
    100% {
        width: 20px;
    }
}

@-moz-keyframes mouthLaugh {
    0% {
        width: 20px;
    }
    45% {
        width: 20px;
    }
    50% {
        width: 15px;
    }
    92% {
        width: 15px;
    }
    98% {
        width: 20px;
    }
    100% {
        width: 20px;
    }
}

@-ms-keyframes mouthLaugh {
    0% {
        width: 20px;
    }
    45% {
        width: 20px;
    }
    50% {
        width: 15px;
    }
    92% {
        width: 15px;
    }
    98% {
        width: 20px;
    }
    100% {
        width: 20px;
    }
}

@keyframes mouthLaugh {
    0% {
        width: 20px;
    }
    45% {
        width: 20px;
    }
    50% {
        width: 15px;
    }
    92% {
        width: 15px;
    }
    98% {
        width: 20px;
    }
    100% {
        width: 20px;
    }
}
html {
    height: 100%;
    width: 100%;
    overflow: hidden;
  }
  
  body {
    height: 100%;
    overflow: hidden;
    background-color: #f03033;
    filter: progid:DXImageTransform.Microsoft.gradient(gradientType=1, startColorstr='#FFF03033', endColorstr='#FF690000');
    background-image: url('data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4gPHN2ZyB2ZXJzaW9uPSIxLjEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGRlZnM+PHJhZGlhbEdyYWRpZW50IGlkPSJncmFkIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgY3g9IjUwJSIgY3k9IiIgcj0iMTAwJSI+PHN0b3Agb2Zmc2V0PSIwJSIgc3RvcC1jb2xvcj0iI2YwMzAzMyIvPjxzdG9wIG9mZnNldD0iMTAwJSIgc3RvcC1jb2xvcj0iIzY5MDAwMCIvPjwvcmFkaWFsR3JhZGllbnQ+PC9kZWZzPjxyZWN0IHg9IjAiIHk9IjAiIHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiIGZpbGw9InVybCgjZ3JhZCkiIC8+PC9zdmc+IA==');
    background-size: 100%;
    background-image: -moz-radial-gradient(center, ellipse cover, #f03033 0%, #690000 100%);
    background-image: -webkit-radial-gradient(center, ellipse cover, #f03033 0%, #690000 100%);
    background-image: radial-gradient(ellipse cover at center, #f03033 0%, #690000 100%);
  }
  body h1 {
    font-family: "Great Vibes", cursive;
    font-weight: 100;
    color: #ffffff;
    position: absolute;
    left: 7%;
    top: 2%;
    font-size: 14vw;
    opacity: 0.8;
    text-shadow: 1px 1px 20px rgba(255, 255, 255, 0.8);
    margin: 0;
  }
  body .container {
    position: absolute;
    padding: 0;
    top: calc(50% - (420px / 2));
    left: calc(50% - (380px / 2));
    min-width: 380px;
    height: 430px;
    margin: 50px auto 0;
  }
  body .container * {
    position: absolute;
  }
  body .container .star {
    top: 5px;
    left: calc(50% - 26px);
    display: block;
    color: red;
    width: 0px;
    height: 0px;
    border-right: 25px solid transparent;
    border-bottom: 17px solid #f8cd13;
    border-left: 25px solid transparent;
    -moz-transform: rotate(35deg);
    -webkit-transform: rotate(35deg);
    -ms-transform: rotate(35deg);
    -o-transform: rotate(35deg);
  }
  body .container .star:before {
    border-bottom: 20px solid #f8cd13;
    border-left: 7px solid transparent;
    border-right: 7px solid transparent;
    position: absolute;
    height: 0;
    width: 0;
    top: -14px;
    left: -16px;
    display: block;
    content: "";
    -webkit-transform: rotate(-35deg);
    -moz-transform: rotate(-35deg);
    -ms-transform: rotate(-35deg);
    -o-transform: rotate(-35deg);
  }
  body .container .star:after {
    position: absolute;
    display: block;
    color: red;
    top: 0px;
    left: -25px;
    width: 0px;
    height: 0px;
    border-right: 25px solid transparent;
    border-bottom: 17px solid #f8cd13;
    border-left: 25px solid transparent;
    -webkit-transform: rotate(-70deg);
    -moz-transform: rotate(-70deg);
    -ms-transform: rotate(-70deg);
    -o-transform: rotate(-70deg);
    content: "";
  }
  body .container .light {
    height: 5px;
    width: 3px;
    border-radius: 50% 50% 50% 50% / 70% 70% 30% 30%;
  }
  body .container .light:nth-of-type(1) {
    top: 40px;
    left: 194px;
  }
  body .container .light:nth-of-type(2) {
    top: 72px;
    left: 178px;
  }
  body .container .light:nth-of-type(3) {
    top: 88px;
    left: 148px;
  }
  body .container .light:nth-of-type(4) {
    top: 80px;
    left: 216px;
  }
  body .container .light:nth-of-type(5) {
    top: 120px;
    left: 220px;
  }
  body .container .light:nth-of-type(6) {
    top: 144px;
    left: 246px;
  }
  body .container .light:nth-of-type(7) {
    top: 120px;
    left: 170px;
  }
  body .container .light:nth-of-type(8) {
    top: 130px;
    left: 132px;
  }
  body .container .light:nth-of-type(9) {
    top: 146px;
    left: 190px;
  }
  body .container .light:nth-of-type(10) {
    top: 180px;
    left: 220px;
  }
  body .container .light:nth-of-type(11) {
    top: 196px;
    left: 262px;
  }
  body .container .light:nth-of-type(12) {
    top: 176px;
    left: 150px;
  }
  body .container .light:nth-of-type(13) {
    top: 196px;
    left: 110px;
  }
  body .container .light:nth-of-type(14) {
    top: 210px;
    left: 170px;
  }
  body .container .light:nth-of-type(15) {
    top: 218px;
    left: 220px;
  }
  body .container .light:nth-of-type(16) {
    top: 250px;
    left: 190px;
  }
  body .container .light:nth-of-type(17) {
    top: 240px;
    left: 260px;
  }
  body .container .light:nth-of-type(18) {
    top: 268px;
    left: 290px;
  }
  body .container .light:nth-of-type(19) {
    top: 270px;
    left: 230px;
  }
  body .container .light:nth-of-type(20) {
    top: 276px;
    left: 150px;
  }
  body .container .light:nth-of-type(21) {
    top: 240px;
    left: 120px;
  }
  body .container .light:nth-of-type(22) {
    top: 266px;
    left: 84px;
  }
  body .container .light:nth-of-type(23) {
    top: 316px;
    left: 60px;
  }
  body .container .light:nth-of-type(24) {
    top: 300px;
    left: 106px;
  }
  body .container .light:nth-of-type(25) {
    top: 334px;
    left: 130px;
  }
  body .container .light:nth-of-type(26) {
    top: 314px;
    left: 176px;
  }
  body .container .light:nth-of-type(27) {
    top: 336px;
    left: 216px;
  }
  body .container .light:nth-of-type(28) {
    top: 310px;
    left: 250px;
  }
  body .container .light:nth-of-type(29) {
    top: 310px;
    left: 300px;
  }
  body .container .light:nth-of-type(30) {
    top: 338px;
    left: 280px;
  }
  body .shadow {
    -moz-border-radius: 50%;
    -webkit-border-radius: 50%;
    border-radius: 50%;
    position: absolute;
    bottom: 20px;
    left: calc(50% - 80px);
    height: 0;
    z-index: -1;
    width: 160px;
    -moz-box-shadow: 0 0px 80px 30px rgba(0, 0, 0, 0.3);
    -webkit-box-shadow: 0 0px 80px 30px rgba(0, 0, 0, 0.3);
    box-shadow: 0 0px 80px 30px rgba(0, 0, 0, 0.3);
    background: transparent;
  }
  
  .star ~ .light {
    background: #eae486;
  }
  
  /* Number of lights */
  @-moz-keyframes lights-colors-1 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-1 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @keyframes lights-colors-1 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-1 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-1 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  @keyframes lights-glint-1 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  span.light:nth-child(10n + 1) {
    background: #7736d8;
    -moz-animation: lights-colors-1 3s infinite;
    -webkit-animation: lights-colors-1 3s infinite;
    animation: lights-colors-1 3s infinite;
  }
  span.light:nth-child(10n + 1):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-1 3s infinite;
    -webkit-animation: lights-glint-1 3s infinite;
    animation: lights-glint-1 3s infinite;
  }
  
  @-moz-keyframes lights-colors-2 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-2 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
  }
  @keyframes lights-colors-2 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
  }
  @-moz-keyframes lights-glint-2 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
  }
  @-webkit-keyframes lights-glint-2 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
  }
  @keyframes lights-glint-2 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
  }
  span.light:nth-child(10n + 2) {
    background: #36b8d8;
    -moz-animation: lights-colors-2 3s infinite;
    -webkit-animation: lights-colors-2 3s infinite;
    animation: lights-colors-2 3s infinite;
  }
  span.light:nth-child(10n + 2):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-2 3s infinite;
    -webkit-animation: lights-glint-2 3s infinite;
    animation: lights-glint-2 3s infinite;
  }
  
  @-moz-keyframes lights-colors-3 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-3 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @keyframes lights-colors-3 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-3 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-3 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @keyframes lights-glint-3 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  span.light:nth-child(10n + 3) {
    background: #d83636;
    -moz-animation: lights-colors-3 3s infinite;
    -webkit-animation: lights-colors-3 3s infinite;
    animation: lights-colors-3 3s infinite;
  }
  span.light:nth-child(10n + 3):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-3 3s infinite;
    -webkit-animation: lights-glint-3 3s infinite;
    animation: lights-glint-3 3s infinite;
  }
  
  @-moz-keyframes lights-colors-4 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-4 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @keyframes lights-colors-4 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-4 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-4 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @keyframes lights-glint-4 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  span.light:nth-child(10n + 4) {
    background: #4dd836;
    -moz-animation: lights-colors-4 3s infinite;
    -webkit-animation: lights-colors-4 3s infinite;
    animation: lights-colors-4 3s infinite;
  }
  span.light:nth-child(10n + 4):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-4 3s infinite;
    -webkit-animation: lights-glint-4 3s infinite;
    animation: lights-glint-4 3s infinite;
  }
  
  @-moz-keyframes lights-colors-5 {
    0%,
      32%,
      100% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-5 {
    0%,
      32%,
      100% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
  }
  @keyframes lights-colors-5 {
    0%,
      32%,
      100% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-5 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-5 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
  }
  @keyframes lights-glint-5 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
  }
  span.light:nth-child(10n + 5) {
    background: #4dd836;
    -moz-animation: lights-colors-5 3s infinite;
    -webkit-animation: lights-colors-5 3s infinite;
    animation: lights-colors-5 3s infinite;
  }
  span.light:nth-child(10n + 5):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-5 3s infinite;
    -webkit-animation: lights-glint-5 3s infinite;
    animation: lights-glint-5 3s infinite;
  }
  
  @-moz-keyframes lights-colors-6 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-6 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
  }
  @keyframes lights-colors-6 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-6 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-6 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
  }
  @keyframes lights-glint-6 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
  }
  span.light:nth-child(10n + 6) {
    background: #d87f36;
    -moz-animation: lights-colors-6 3s infinite;
    -webkit-animation: lights-colors-6 3s infinite;
    animation: lights-colors-6 3s infinite;
  }
  span.light:nth-child(10n + 6):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-6 3s infinite;
    -webkit-animation: lights-glint-6 3s infinite;
    animation: lights-glint-6 3s infinite;
  }
  
  @-moz-keyframes lights-colors-7 {
    0%,
      32%,
      100% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-7 {
    0%,
      32%,
      100% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
  }
  @keyframes lights-colors-7 {
    0%,
      32%,
      100% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
  }
  @-moz-keyframes lights-glint-7 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
  }
  @-webkit-keyframes lights-glint-7 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
  }
  @keyframes lights-glint-7 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
  }
  span.light:nth-child(10n + 7) {
    background: #d8368a;
    -moz-animation: lights-colors-7 3s infinite;
    -webkit-animation: lights-colors-7 3s infinite;
    animation: lights-colors-7 3s infinite;
  }
  span.light:nth-child(10n + 7):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-7 3s infinite;
    -webkit-animation: lights-glint-7 3s infinite;
    animation: lights-glint-7 3s infinite;
  }
  
  @-moz-keyframes lights-colors-8 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    66%,
      99% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-8 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    66%,
      99% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
  }
  @keyframes lights-colors-8 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    66%,
      99% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
  }
  @-moz-keyframes lights-glint-8 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
  }
  @-webkit-keyframes lights-glint-8 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
  }
  @keyframes lights-glint-8 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
  }
  span.light:nth-child(10n + 8) {
    background: #d8368a;
    -moz-animation: lights-colors-8 3s infinite;
    -webkit-animation: lights-colors-8 3s infinite;
    animation: lights-colors-8 3s infinite;
  }
  span.light:nth-child(10n + 8):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-8 3s infinite;
    -webkit-animation: lights-glint-8 3s infinite;
    animation: lights-glint-8 3s infinite;
  }
  
  @-moz-keyframes lights-colors-9 {
    0%,
      32%,
      100% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-9 {
    0%,
      32%,
      100% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @keyframes lights-colors-9 {
    0%,
      32%,
      100% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-9 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-9 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @keyframes lights-glint-9 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  span.light:nth-child(10n + 9) {
    background: #36d8c3;
    -moz-animation: lights-colors-9 3s infinite;
    -webkit-animation: lights-colors-9 3s infinite;
    animation: lights-colors-9 3s infinite;
  }
  span.light:nth-child(10n + 9):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-9 3s infinite;
    -webkit-animation: lights-glint-9 3s infinite;
    animation: lights-glint-9 3s infinite;
  }
  
  @-moz-keyframes lights-colors-10 {
    0%,
      32%,
      100% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    33%,
      65% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-10 {
    0%,
      32%,
      100% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    33%,
      65% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @keyframes lights-colors-10 {
    0%,
      32%,
      100% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    33%,
      65% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-10 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-10 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @keyframes lights-glint-10 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  span.light:nth-child(10n + 10) {
    background: #d8368a;
    -moz-animation: lights-colors-10 3s infinite;
    -webkit-animation: lights-colors-10 3s infinite;
    animation: lights-colors-10 3s infinite;
  }
  span.light:nth-child(10n + 10):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-10 3s infinite;
    -webkit-animation: lights-glint-10 3s infinite;
    animation: lights-glint-10 3s infinite;
  }
  
  @-moz-keyframes lights-colors-11 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-11 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @keyframes lights-colors-11 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-11 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-11 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @keyframes lights-glint-11 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  span.light:nth-child(10n + 11) {
    background: #c736d8;
    -moz-animation: lights-colors-11 3s infinite;
    -webkit-animation: lights-colors-11 3s infinite;
    animation: lights-colors-11 3s infinite;
  }
  span.light:nth-child(10n + 11):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-11 3s infinite;
    -webkit-animation: lights-glint-11 3s infinite;
    animation: lights-glint-11 3s infinite;
  }
  
  @-moz-keyframes lights-colors-12 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-12 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
  }
  @keyframes lights-colors-12 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
  }
  @-moz-keyframes lights-glint-12 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
  }
  @-webkit-keyframes lights-glint-12 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
  }
  @keyframes lights-glint-12 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
  }
  span.light:nth-child(10n + 12) {
    background: #c736d8;
    -moz-animation: lights-colors-12 3s infinite;
    -webkit-animation: lights-colors-12 3s infinite;
    animation: lights-colors-12 3s infinite;
  }
  span.light:nth-child(10n + 12):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-12 3s infinite;
    -webkit-animation: lights-glint-12 3s infinite;
    animation: lights-glint-12 3s infinite;
  }
  
  @-moz-keyframes lights-colors-13 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-13 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @keyframes lights-colors-13 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-13 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-13 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @keyframes lights-glint-13 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  span.light:nth-child(10n + 13) {
    background: #d83636;
    -moz-animation: lights-colors-13 3s infinite;
    -webkit-animation: lights-colors-13 3s infinite;
    animation: lights-colors-13 3s infinite;
  }
  span.light:nth-child(10n + 13):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-13 3s infinite;
    -webkit-animation: lights-glint-13 3s infinite;
    animation: lights-glint-13 3s infinite;
  }
  
  @-moz-keyframes lights-colors-14 {
    0%,
      32%,
      100% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-14 {
    0%,
      32%,
      100% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
  }
  @keyframes lights-colors-14 {
    0%,
      32%,
      100% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
  }
  @-moz-keyframes lights-glint-14 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
  }
  @-webkit-keyframes lights-glint-14 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
  }
  @keyframes lights-glint-14 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
  }
  span.light:nth-child(10n + 14) {
    background: #c736d8;
    -moz-animation: lights-colors-14 3s infinite;
    -webkit-animation: lights-colors-14 3s infinite;
    animation: lights-colors-14 3s infinite;
  }
  span.light:nth-child(10n + 14):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-14 3s infinite;
    -webkit-animation: lights-glint-14 3s infinite;
    animation: lights-glint-14 3s infinite;
  }
  
  @-moz-keyframes lights-colors-15 {
    0%,
      32%,
      100% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-15 {
    0%,
      32%,
      100% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
  }
  @keyframes lights-colors-15 {
    0%,
      32%,
      100% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-15 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-15 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
  }
  @keyframes lights-glint-15 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
  }
  span.light:nth-child(10n + 15) {
    background: #eae486;
    -moz-animation: lights-colors-15 3s infinite;
    -webkit-animation: lights-colors-15 3s infinite;
    animation: lights-colors-15 3s infinite;
  }
  span.light:nth-child(10n + 15):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-15 3s infinite;
    -webkit-animation: lights-glint-15 3s infinite;
    animation: lights-glint-15 3s infinite;
  }
  
  @-moz-keyframes lights-colors-16 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    66%,
      99% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-16 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    66%,
      99% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
  }
  @keyframes lights-colors-16 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    66%,
      99% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-16 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-16 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
  }
  @keyframes lights-glint-16 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
  }
  span.light:nth-child(10n + 16) {
    background: #d87f36;
    -moz-animation: lights-colors-16 3s infinite;
    -webkit-animation: lights-colors-16 3s infinite;
    animation: lights-colors-16 3s infinite;
  }
  span.light:nth-child(10n + 16):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-16 3s infinite;
    -webkit-animation: lights-glint-16 3s infinite;
    animation: lights-glint-16 3s infinite;
  }
  
  @-moz-keyframes lights-colors-17 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-17 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @keyframes lights-colors-17 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #eae486;
      box-shadow: 0 0 22px 5px rgba(234, 228, 134, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-17 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-17 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @keyframes lights-glint-17 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(234, 228, 134, 0), rgba(234, 228, 134, 0.3), rgba(234, 228, 134, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  span.light:nth-child(10n + 17) {
    background: #d83636;
    -moz-animation: lights-colors-17 3s infinite;
    -webkit-animation: lights-colors-17 3s infinite;
    animation: lights-colors-17 3s infinite;
  }
  span.light:nth-child(10n + 17):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-17 3s infinite;
    -webkit-animation: lights-glint-17 3s infinite;
    animation: lights-glint-17 3s infinite;
  }
  
  @-moz-keyframes lights-colors-18 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-18 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @keyframes lights-colors-18 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-18 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-18 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @keyframes lights-glint-18 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  span.light:nth-child(10n + 18) {
    background: #c736d8;
    -moz-animation: lights-colors-18 3s infinite;
    -webkit-animation: lights-colors-18 3s infinite;
    animation: lights-colors-18 3s infinite;
  }
  span.light:nth-child(10n + 18):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-18 3s infinite;
    -webkit-animation: lights-glint-18 3s infinite;
    animation: lights-glint-18 3s infinite;
  }
  
  @-moz-keyframes lights-colors-19 {
    0%,
      32%,
      100% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-19 {
    0%,
      32%,
      100% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
  }
  @keyframes lights-colors-19 {
    0%,
      32%,
      100% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
  }
  @-moz-keyframes lights-glint-19 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
  }
  @-webkit-keyframes lights-glint-19 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
  }
  @keyframes lights-glint-19 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
  }
  span.light:nth-child(10n + 19) {
    background: #d8368a;
    -moz-animation: lights-colors-19 3s infinite;
    -webkit-animation: lights-colors-19 3s infinite;
    animation: lights-colors-19 3s infinite;
  }
  span.light:nth-child(10n + 19):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-19 3s infinite;
    -webkit-animation: lights-glint-19 3s infinite;
    animation: lights-glint-19 3s infinite;
  }
  
  @-moz-keyframes lights-colors-20 {
    0%,
      32%,
      100% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-20 {
    0%,
      32%,
      100% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @keyframes lights-colors-20 {
    0%,
      32%,
      100% {
      background: #d87f36;
      box-shadow: 0 0 22px 5px rgba(216, 127, 54, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-20 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-20 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @keyframes lights-glint-20 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 127, 54, 0), rgba(216, 127, 54, 0.3), rgba(216, 127, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  span.light:nth-child(10n + 20) {
    background: #3658d8;
    -moz-animation: lights-colors-20 3s infinite;
    -webkit-animation: lights-colors-20 3s infinite;
    animation: lights-colors-20 3s infinite;
  }
  span.light:nth-child(10n + 20):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-20 3s infinite;
    -webkit-animation: lights-glint-20 3s infinite;
    animation: lights-glint-20 3s infinite;
  }
  
  @-moz-keyframes lights-colors-21 {
    0%,
      32%,
      100% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    33%,
      65% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-21 {
    0%,
      32%,
      100% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    33%,
      65% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @keyframes lights-colors-21 {
    0%,
      32%,
      100% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
    33%,
      65% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-21 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-21 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  @keyframes lights-glint-21 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  span.light:nth-child(10n + 21) {
    background: #36d8c3;
    -moz-animation: lights-colors-21 3s infinite;
    -webkit-animation: lights-colors-21 3s infinite;
    animation: lights-colors-21 3s infinite;
  }
  span.light:nth-child(10n + 21):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-21 3s infinite;
    -webkit-animation: lights-glint-21 3s infinite;
    animation: lights-glint-21 3s infinite;
  }
  
  @-moz-keyframes lights-colors-22 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
    66%,
      99% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-22 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
    66%,
      99% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
  }
  @keyframes lights-colors-22 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
    66%,
      99% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-22 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-22 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
  }
  @keyframes lights-glint-22 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
  }
  span.light:nth-child(10n + 22) {
    background: #36b8d8;
    -moz-animation: lights-colors-22 3s infinite;
    -webkit-animation: lights-colors-22 3s infinite;
    animation: lights-colors-22 3s infinite;
  }
  span.light:nth-child(10n + 22):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-22 3s infinite;
    -webkit-animation: lights-glint-22 3s infinite;
    animation: lights-glint-22 3s infinite;
  }
  
  @-moz-keyframes lights-colors-23 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-23 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @keyframes lights-colors-23 {
    0%,
      32%,
      100% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-23 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-23 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  @keyframes lights-glint-23 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  span.light:nth-child(10n + 23) {
    background: #c736d8;
    -moz-animation: lights-colors-23 3s infinite;
    -webkit-animation: lights-colors-23 3s infinite;
    animation: lights-colors-23 3s infinite;
  }
  span.light:nth-child(10n + 23):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-23 3s infinite;
    -webkit-animation: lights-glint-23 3s infinite;
    animation: lights-glint-23 3s infinite;
  }
  
  @-moz-keyframes lights-colors-24 {
    0%,
      32%,
      100% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-24 {
    0%,
      32%,
      100% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
  }
  @keyframes lights-colors-24 {
    0%,
      32%,
      100% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    33%,
      65% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    66%,
      99% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
  }
  @-moz-keyframes lights-glint-24 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
  }
  @-webkit-keyframes lights-glint-24 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
  }
  @keyframes lights-glint-24 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
  }
  span.light:nth-child(10n + 24) {
    background: #4dd836;
    -moz-animation: lights-colors-24 3s infinite;
    -webkit-animation: lights-colors-24 3s infinite;
    animation: lights-colors-24 3s infinite;
  }
  span.light:nth-child(10n + 24):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-24 3s infinite;
    -webkit-animation: lights-glint-24 3s infinite;
    animation: lights-glint-24 3s infinite;
  }
  
  @-moz-keyframes lights-colors-25 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-25 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @keyframes lights-colors-25 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-25 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-25 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @keyframes lights-glint-25 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  span.light:nth-child(10n + 25) {
    background: #7736d8;
    -moz-animation: lights-colors-25 3s infinite;
    -webkit-animation: lights-colors-25 3s infinite;
    animation: lights-colors-25 3s infinite;
  }
  span.light:nth-child(10n + 25):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-25 3s infinite;
    -webkit-animation: lights-glint-25 3s infinite;
    animation: lights-glint-25 3s infinite;
  }
  
  @-moz-keyframes lights-colors-26 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-26 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @keyframes lights-colors-26 {
    0%,
      32%,
      100% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    33%,
      65% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
    66%,
      99% {
      background: #d83636;
      box-shadow: 0 0 22px 5px rgba(216, 54, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-26 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-26 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  @keyframes lights-glint-26 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(216, 54, 54, 0), rgba(216, 54, 54, 0.3), rgba(216, 54, 54, 0));
    }
  }
  span.light:nth-child(10n + 26) {
    background: #d87f36;
    -moz-animation: lights-colors-26 3s infinite;
    -webkit-animation: lights-colors-26 3s infinite;
    animation: lights-colors-26 3s infinite;
  }
  span.light:nth-child(10n + 26):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-26 3s infinite;
    -webkit-animation: lights-glint-26 3s infinite;
    animation: lights-glint-26 3s infinite;
  }
  
  @-moz-keyframes lights-colors-27 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-27 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @keyframes lights-colors-27 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
  }
  @-moz-keyframes lights-glint-27 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  @-webkit-keyframes lights-glint-27 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  @keyframes lights-glint-27 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
  }
  span.light:nth-child(10n + 27) {
    background: #d87f36;
    -moz-animation: lights-colors-27 3s infinite;
    -webkit-animation: lights-colors-27 3s infinite;
    animation: lights-colors-27 3s infinite;
  }
  span.light:nth-child(10n + 27):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-27 3s infinite;
    -webkit-animation: lights-glint-27 3s infinite;
    animation: lights-glint-27 3s infinite;
  }
  
  @-moz-keyframes lights-colors-28 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-28 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @keyframes lights-colors-28 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #d8368a;
      box-shadow: 0 0 22px 5px rgba(216, 54, 138, 0.6);
    }
    66%,
      99% {
      background: #7736d8;
      box-shadow: 0 0 22px 5px rgba(119, 54, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-28 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-28 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  @keyframes lights-glint-28 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(216, 54, 138, 0), rgba(216, 54, 138, 0.3), rgba(216, 54, 138, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(119, 54, 216, 0), rgba(119, 54, 216, 0.3), rgba(119, 54, 216, 0));
    }
  }
  span.light:nth-child(10n + 28) {
    background: #c736d8;
    -moz-animation: lights-colors-28 3s infinite;
    -webkit-animation: lights-colors-28 3s infinite;
    animation: lights-colors-28 3s infinite;
  }
  span.light:nth-child(10n + 28):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-28 3s infinite;
    -webkit-animation: lights-glint-28 3s infinite;
    animation: lights-glint-28 3s infinite;
  }
  
  @-moz-keyframes lights-colors-29 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-29 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
  }
  @keyframes lights-colors-29 {
    0%,
      32%,
      100% {
      background: #4dd836;
      box-shadow: 0 0 22px 5px rgba(77, 216, 54, 0.6);
    }
    33%,
      65% {
      background: #36d8c3;
      box-shadow: 0 0 22px 5px rgba(54, 216, 195, 0.6);
    }
    66%,
      99% {
      background: #c736d8;
      box-shadow: 0 0 22px 5px rgba(199, 54, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-29 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-29 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
  }
  @keyframes lights-glint-29 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(77, 216, 54, 0), rgba(77, 216, 54, 0.3), rgba(77, 216, 54, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 216, 195, 0), rgba(54, 216, 195, 0.3), rgba(54, 216, 195, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(199, 54, 216, 0), rgba(199, 54, 216, 0.3), rgba(199, 54, 216, 0));
    }
  }
  span.light:nth-child(10n + 29) {
    background: #36d8c3;
    -moz-animation: lights-colors-29 3s infinite;
    -webkit-animation: lights-colors-29 3s infinite;
    animation: lights-colors-29 3s infinite;
  }
  span.light:nth-child(10n + 29):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-29 3s infinite;
    -webkit-animation: lights-glint-29 3s infinite;
    animation: lights-glint-29 3s infinite;
  }
  
  @-moz-keyframes lights-colors-30 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
  }
  @-webkit-keyframes lights-colors-30 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
  }
  @keyframes lights-colors-30 {
    0%,
      32%,
      100% {
      background: #36b8d8;
      box-shadow: 0 0 22px 5px rgba(54, 184, 216, 0.6);
    }
    33%,
      65% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
    66%,
      99% {
      background: #3658d8;
      box-shadow: 0 0 22px 5px rgba(54, 88, 216, 0.6);
    }
  }
  @-moz-keyframes lights-glint-30 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
  }
  @-webkit-keyframes lights-glint-30 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
  }
  @keyframes lights-glint-30 {
    0%,
      32%,
      100% {
      background-image: linear-gradient(to right, rgba(54, 184, 216, 0), rgba(54, 184, 216, 0.3), rgba(54, 184, 216, 0));
    }
    33%,
      65% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
    66%,
      99% {
      background-image: linear-gradient(to right, rgba(54, 88, 216, 0), rgba(54, 88, 216, 0.3), rgba(54, 88, 216, 0));
    }
  }
  span.light:nth-child(10n + 30) {
    background: #c736d8;
    -moz-animation: lights-colors-30 3s infinite;
    -webkit-animation: lights-colors-30 3s infinite;
    animation: lights-colors-30 3s infinite;
  }
  span.light:nth-child(10n + 30):before {
    content: "";
    position: absolute;
    top: -13px;
    left: 2px;
    height: 30px;
    width: 1px;
    -moz-transform: rotate(32deg);
    -ms-transform: rotate(32deg);
    -webkit-transform: rotate(32deg);
    transform: rotate(32deg);
    -moz-animation: lights-glint-30 3s infinite;
    -webkit-animation: lights-glint-30 3s infinite;
    animation: lights-glint-30 3s infinite;
  }
  
  /* -------- Glitter --------- */
  .glitter {
    position: absolute;
    width: 1px;
    height: 1px;
    background: transparent;
  }
  .glitter:before {
    content: "";
    position: absolute;
    top: 100px;
    width: 1px;
    height: 1px;
    background: transparent;
  }
  .glitter:after {
    content: "";
    position: absolute;
    left: 100px;
    width: 1px;
    height: 1px;
    background: transparent;
  }
  
  @-moz-keyframes glitter-1 {
    0%,
      100%,
      0%,
      10% {
      opacity: 0;
    }
    5% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-1 {
    0%,
      100%,
      0%,
      10% {
      opacity: 0;
    }
    5% {
      opacity: 1;
    }
  }
  @keyframes glitter-1 {
    0%,
      100%,
      0%,
      10% {
      opacity: 0;
    }
    5% {
      opacity: 1;
    }
  }
  .glitter_1 {
    -moz-animation: glitter-1 10s infinite;
    -webkit-animation: glitter-1 10s infinite;
    animation: glitter-1 10s infinite;
    box-shadow: 601px 513px #A1B8D0 , 927px 35px #A1B8D0 , 22px 959px #A1B8D0 , 108px 232px #A1B8D0 , 836px 793px #A1B8D0 , 705px 61px #A1B8D0 , 715px 865px #A1B8D0 , 224px 397px #A1B8D0 , 825px 56px #A1B8D0 , 178px 440px #A1B8D0 , 476px 741px #A1B8D0 , 871px 355px #A1B8D0 , 591px 364px #A1B8D0 , 434px 763px #A1B8D0 , 269px 682px #A1B8D0 , 404px 934px #A1B8D0 , 365px 591px #A1B8D0 , 412px 673px #A1B8D0 , 277px 221px #A1B8D0 , 763px 439px #A1B8D0 , 247px 461px #A1B8D0 , 379px 354px #A1B8D0 , 330px 958px #A1B8D0 , 708px 600px #A1B8D0 , 820px 917px #A1B8D0 , 985px 622px #A1B8D0 , 266px 435px #A1B8D0 , 132px 682px #A1B8D0 , 165px 433px #A1B8D0 , 865px 468px #A1B8D0 , 898px 150px #A1B8D0 , 724px 2px #A1B8D0 , 828px 749px #A1B8D0 , 55px 295px #A1B8D0 , 162px 950px #A1B8D0 , 896px 245px #A1B8D0 , 737px 937px #A1B8D0 , 995px 546px #A1B8D0 , 447px 833px #A1B8D0 , 441px 248px #A1B8D0 , 152px 933px #A1B8D0 , 779px 398px #A1B8D0 , 460px 52px #A1B8D0 , 158px 603px #A1B8D0 , 167px 766px #A1B8D0 , 993px 989px #A1B8D0 , 727px 3px #A1B8D0 , 259px 642px #A1B8D0 , 563px 156px #A1B8D0 , 482px 902px #A1B8D0 , 900px 197px #A1B8D0 , 496px 42px #A1B8D0 , 652px 38px #A1B8D0 , 558px 800px #A1B8D0 , 746px 987px #A1B8D0 , 199px 280px #A1B8D0 , 611px 784px #A1B8D0 , 552px 894px #A1B8D0 , 645px 613px #A1B8D0 , 847px 399px #A1B8D0 , 186px 84px #A1B8D0 , 176px 488px #A1B8D0 , 717px 312px #A1B8D0 , 230px 451px #A1B8D0 , 552px 617px #A1B8D0 , 237px 991px #A1B8D0 , 754px 725px #A1B8D0 , 843px 474px #A1B8D0 , 277px 749px #A1B8D0 , 180px 818px #A1B8D0 , 979px 573px #A1B8D0 , 524px 997px #A1B8D0 , 131px 27px #A1B8D0 , 1px 822px #A1B8D0 , 657px 602px #A1B8D0 , 1px 363px #A1B8D0 , 807px 533px #A1B8D0 , 250px 956px #A1B8D0 , 713px 633px #A1B8D0 , 694px 939px #A1B8D0 , 202px 867px #A1B8D0 , 511px 481px #A1B8D0 , 933px 831px #A1B8D0 , 123px 95px #A1B8D0 , 572px 823px #A1B8D0 , 442px 399px #A1B8D0 , 120px 577px #A1B8D0 , 122px 880px #A1B8D0 , 212px 72px #A1B8D0 , 482px 394px #A1B8D0 , 353px 527px #A1B8D0 , 729px 949px #A1B8D0 , 848px 544px #A1B8D0 , 550px 866px #A1B8D0 , 215px 51px #A1B8D0 , 252px 680px #A1B8D0 , 885px 74px #A1B8D0 , 211px 271px #A1B8D0 , 588px 810px #A1B8D0 , 967px 976px #A1B8D0 , 503px 984px #A1B8D0 , 489px 162px #A1B8D0 , 373px 88px #A1B8D0 , 211px 106px #A1B8D0 , 512px 711px #A1B8D0 , 758px 767px #A1B8D0 , 770px 691px #A1B8D0 , 47px 998px #A1B8D0 , 232px 563px #A1B8D0 , 123px 407px #A1B8D0 , 471px 762px #A1B8D0 , 275px 770px #A1B8D0 , 107px 584px #A1B8D0 , 355px 69px #A1B8D0 , 631px 444px #A1B8D0 , 240px 281px #A1B8D0 , 317px 637px #A1B8D0 , 577px 384px #A1B8D0 , 530px 833px #A1B8D0 , 516px 551px #A1B8D0 , 71px 56px #A1B8D0 , 906px 782px #A1B8D0 , 649px 998px #A1B8D0 , 84px 60px #A1B8D0 , 240px 563px #A1B8D0 , 32px 19px #A1B8D0 , 441px 778px #A1B8D0 , 544px 584px #A1B8D0 , 986px 317px #A1B8D0 , 116px 734px #A1B8D0 , 794px 839px #A1B8D0 , 112px 155px #A1B8D0 , 509px 292px #A1B8D0 , 163px 883px #A1B8D0 , 237px 861px #A1B8D0 , 441px 992px #A1B8D0 , 287px 274px #A1B8D0 , 466px 804px #A1B8D0 , 791px 443px #A1B8D0 , 778px 570px #A1B8D0 , 776px 183px #A1B8D0 , 831px 534px #A1B8D0 , 778px 235px #A1B8D0 , 268px 553px #A1B8D0 , 828px 366px #A1B8D0 , 46px 184px #A1B8D0 , 718px 685px #A1B8D0 , 461px 570px #A1B8D0 , 105px 821px #A1B8D0 , 121px 696px #A1B8D0 , 441px 279px #A1B8D0 , 252px 626px #A1B8D0 , 797px 50px #A1B8D0 , 895px 24px #A1B8D0 , 965px 368px #A1B8D0 , 764px 942px #A1B8D0 , 370px 343px #A1B8D0 , 726px 309px #A1B8D0 , 523px 680px #A1B8D0 , 12px 691px #A1B8D0 , 844px 598px #A1B8D0 , 439px 430px #A1B8D0 , 467px 740px #A1B8D0 , 263px 529px #A1B8D0 , 14px 248px #A1B8D0 , 753px 93px #A1B8D0 , 596px 422px #A1B8D0 , 469px 413px #A1B8D0 , 175px 555px #A1B8D0 , 29px 796px #A1B8D0 , 577px 887px #A1B8D0 , 918px 838px #A1B8D0 , 97px 62px #A1B8D0 , 765px 640px #A1B8D0 , 248px 897px #A1B8D0 , 812px 699px #A1B8D0 , 431px 472px #A1B8D0 , 751px 934px #A1B8D0 , 169px 206px #A1B8D0 , 19px 860px #A1B8D0 , 625px 164px #A1B8D0 , 578px 93px #A1B8D0 , 895px 297px #A1B8D0 , 744px 418px #A1B8D0 , 734px 854px #A1B8D0 , 626px 629px #A1B8D0 , 270px 468px #A1B8D0 , 769px 223px #A1B8D0 , 895px 772px #A1B8D0 , 721px 830px #A1B8D0 , 646px 75px #A1B8D0 , 718px 583px #A1B8D0 , 249px 558px #A1B8D0 , 106px 20px #A1B8D0 , 988px 623px #A1B8D0 , 907px 753px #A1B8D0 , 959px 235px #A1B8D0 , 821px 710px #A1B8D0 , 912px 827px #A1B8D0 , 143px 707px #A1B8D0;
  }
  .glitter_1:before {
    -moz-animation: glitter-1 8s infinite;
    -webkit-animation: glitter-1 8s infinite;
    animation: glitter-1 8s infinite;
    box-shadow: 601px 513px #A1B8D0 , 927px 35px #A1B8D0 , 22px 959px #A1B8D0 , 108px 232px #A1B8D0 , 836px 793px #A1B8D0 , 705px 61px #A1B8D0 , 715px 865px #A1B8D0 , 224px 397px #A1B8D0 , 825px 56px #A1B8D0 , 178px 440px #A1B8D0 , 476px 741px #A1B8D0 , 871px 355px #A1B8D0 , 591px 364px #A1B8D0 , 434px 763px #A1B8D0 , 269px 682px #A1B8D0 , 404px 934px #A1B8D0 , 365px 591px #A1B8D0 , 412px 673px #A1B8D0 , 277px 221px #A1B8D0 , 763px 439px #A1B8D0 , 247px 461px #A1B8D0 , 379px 354px #A1B8D0 , 330px 958px #A1B8D0 , 708px 600px #A1B8D0 , 820px 917px #A1B8D0 , 985px 622px #A1B8D0 , 266px 435px #A1B8D0 , 132px 682px #A1B8D0 , 165px 433px #A1B8D0 , 865px 468px #A1B8D0 , 898px 150px #A1B8D0 , 724px 2px #A1B8D0 , 828px 749px #A1B8D0 , 55px 295px #A1B8D0 , 162px 950px #A1B8D0 , 896px 245px #A1B8D0 , 737px 937px #A1B8D0 , 995px 546px #A1B8D0 , 447px 833px #A1B8D0 , 441px 248px #A1B8D0 , 152px 933px #A1B8D0 , 779px 398px #A1B8D0 , 460px 52px #A1B8D0 , 158px 603px #A1B8D0 , 167px 766px #A1B8D0 , 993px 989px #A1B8D0 , 727px 3px #A1B8D0 , 259px 642px #A1B8D0 , 563px 156px #A1B8D0 , 482px 902px #A1B8D0 , 900px 197px #A1B8D0 , 496px 42px #A1B8D0 , 652px 38px #A1B8D0 , 558px 800px #A1B8D0 , 746px 987px #A1B8D0 , 199px 280px #A1B8D0 , 611px 784px #A1B8D0 , 552px 894px #A1B8D0 , 645px 613px #A1B8D0 , 847px 399px #A1B8D0 , 186px 84px #A1B8D0 , 176px 488px #A1B8D0 , 717px 312px #A1B8D0 , 230px 451px #A1B8D0 , 552px 617px #A1B8D0 , 237px 991px #A1B8D0 , 754px 725px #A1B8D0 , 843px 474px #A1B8D0 , 277px 749px #A1B8D0 , 180px 818px #A1B8D0 , 979px 573px #A1B8D0 , 524px 997px #A1B8D0 , 131px 27px #A1B8D0 , 1px 822px #A1B8D0 , 657px 602px #A1B8D0 , 1px 363px #A1B8D0 , 807px 533px #A1B8D0 , 250px 956px #A1B8D0 , 713px 633px #A1B8D0 , 694px 939px #A1B8D0 , 202px 867px #A1B8D0 , 511px 481px #A1B8D0 , 933px 831px #A1B8D0 , 123px 95px #A1B8D0 , 572px 823px #A1B8D0 , 442px 399px #A1B8D0 , 120px 577px #A1B8D0 , 122px 880px #A1B8D0 , 212px 72px #A1B8D0 , 482px 394px #A1B8D0 , 353px 527px #A1B8D0 , 729px 949px #A1B8D0 , 848px 544px #A1B8D0 , 550px 866px #A1B8D0 , 215px 51px #A1B8D0 , 252px 680px #A1B8D0 , 885px 74px #A1B8D0 , 211px 271px #A1B8D0 , 588px 810px #A1B8D0 , 967px 976px #A1B8D0 , 503px 984px #A1B8D0 , 489px 162px #A1B8D0 , 373px 88px #A1B8D0 , 211px 106px #A1B8D0 , 512px 711px #A1B8D0 , 758px 767px #A1B8D0 , 770px 691px #A1B8D0 , 47px 998px #A1B8D0 , 232px 563px #A1B8D0 , 123px 407px #A1B8D0 , 471px 762px #A1B8D0 , 275px 770px #A1B8D0 , 107px 584px #A1B8D0 , 355px 69px #A1B8D0 , 631px 444px #A1B8D0 , 240px 281px #A1B8D0 , 317px 637px #A1B8D0 , 577px 384px #A1B8D0 , 530px 833px #A1B8D0 , 516px 551px #A1B8D0 , 71px 56px #A1B8D0 , 906px 782px #A1B8D0 , 649px 998px #A1B8D0 , 84px 60px #A1B8D0 , 240px 563px #A1B8D0 , 32px 19px #A1B8D0 , 441px 778px #A1B8D0 , 544px 584px #A1B8D0 , 986px 317px #A1B8D0 , 116px 734px #A1B8D0 , 794px 839px #A1B8D0 , 112px 155px #A1B8D0 , 509px 292px #A1B8D0 , 163px 883px #A1B8D0 , 237px 861px #A1B8D0 , 441px 992px #A1B8D0 , 287px 274px #A1B8D0 , 466px 804px #A1B8D0 , 791px 443px #A1B8D0 , 778px 570px #A1B8D0 , 776px 183px #A1B8D0 , 831px 534px #A1B8D0 , 778px 235px #A1B8D0 , 268px 553px #A1B8D0 , 828px 366px #A1B8D0 , 46px 184px #A1B8D0 , 718px 685px #A1B8D0 , 461px 570px #A1B8D0 , 105px 821px #A1B8D0 , 121px 696px #A1B8D0 , 441px 279px #A1B8D0 , 252px 626px #A1B8D0 , 797px 50px #A1B8D0 , 895px 24px #A1B8D0 , 965px 368px #A1B8D0 , 764px 942px #A1B8D0 , 370px 343px #A1B8D0 , 726px 309px #A1B8D0 , 523px 680px #A1B8D0 , 12px 691px #A1B8D0 , 844px 598px #A1B8D0 , 439px 430px #A1B8D0 , 467px 740px #A1B8D0 , 263px 529px #A1B8D0 , 14px 248px #A1B8D0 , 753px 93px #A1B8D0 , 596px 422px #A1B8D0 , 469px 413px #A1B8D0 , 175px 555px #A1B8D0 , 29px 796px #A1B8D0 , 577px 887px #A1B8D0 , 918px 838px #A1B8D0 , 97px 62px #A1B8D0 , 765px 640px #A1B8D0 , 248px 897px #A1B8D0 , 812px 699px #A1B8D0 , 431px 472px #A1B8D0 , 751px 934px #A1B8D0 , 169px 206px #A1B8D0 , 19px 860px #A1B8D0 , 625px 164px #A1B8D0 , 578px 93px #A1B8D0 , 895px 297px #A1B8D0 , 744px 418px #A1B8D0 , 734px 854px #A1B8D0 , 626px 629px #A1B8D0 , 270px 468px #A1B8D0 , 769px 223px #A1B8D0 , 895px 772px #A1B8D0 , 721px 830px #A1B8D0 , 646px 75px #A1B8D0 , 718px 583px #A1B8D0 , 249px 558px #A1B8D0 , 106px 20px #A1B8D0 , 988px 623px #A1B8D0 , 907px 753px #A1B8D0 , 959px 235px #A1B8D0 , 821px 710px #A1B8D0 , 912px 827px #A1B8D0 , 143px 707px #A1B8D0;
  }
  .glitter_1:after {
    -moz-animation: glitter-1 9s infinite;
    -webkit-animation: glitter-1 9s infinite;
    animation: glitter-1 9s infinite;
    box-shadow: 601px 513px #A1B8D0 , 927px 35px #A1B8D0 , 22px 959px #A1B8D0 , 108px 232px #A1B8D0 , 836px 793px #A1B8D0 , 705px 61px #A1B8D0 , 715px 865px #A1B8D0 , 224px 397px #A1B8D0 , 825px 56px #A1B8D0 , 178px 440px #A1B8D0 , 476px 741px #A1B8D0 , 871px 355px #A1B8D0 , 591px 364px #A1B8D0 , 434px 763px #A1B8D0 , 269px 682px #A1B8D0 , 404px 934px #A1B8D0 , 365px 591px #A1B8D0 , 412px 673px #A1B8D0 , 277px 221px #A1B8D0 , 763px 439px #A1B8D0 , 247px 461px #A1B8D0 , 379px 354px #A1B8D0 , 330px 958px #A1B8D0 , 708px 600px #A1B8D0 , 820px 917px #A1B8D0 , 985px 622px #A1B8D0 , 266px 435px #A1B8D0 , 132px 682px #A1B8D0 , 165px 433px #A1B8D0 , 865px 468px #A1B8D0 , 898px 150px #A1B8D0 , 724px 2px #A1B8D0 , 828px 749px #A1B8D0 , 55px 295px #A1B8D0 , 162px 950px #A1B8D0 , 896px 245px #A1B8D0 , 737px 937px #A1B8D0 , 995px 546px #A1B8D0 , 447px 833px #A1B8D0 , 441px 248px #A1B8D0 , 152px 933px #A1B8D0 , 779px 398px #A1B8D0 , 460px 52px #A1B8D0 , 158px 603px #A1B8D0 , 167px 766px #A1B8D0 , 993px 989px #A1B8D0 , 727px 3px #A1B8D0 , 259px 642px #A1B8D0 , 563px 156px #A1B8D0 , 482px 902px #A1B8D0 , 900px 197px #A1B8D0 , 496px 42px #A1B8D0 , 652px 38px #A1B8D0 , 558px 800px #A1B8D0 , 746px 987px #A1B8D0 , 199px 280px #A1B8D0 , 611px 784px #A1B8D0 , 552px 894px #A1B8D0 , 645px 613px #A1B8D0 , 847px 399px #A1B8D0 , 186px 84px #A1B8D0 , 176px 488px #A1B8D0 , 717px 312px #A1B8D0 , 230px 451px #A1B8D0 , 552px 617px #A1B8D0 , 237px 991px #A1B8D0 , 754px 725px #A1B8D0 , 843px 474px #A1B8D0 , 277px 749px #A1B8D0 , 180px 818px #A1B8D0 , 979px 573px #A1B8D0 , 524px 997px #A1B8D0 , 131px 27px #A1B8D0 , 1px 822px #A1B8D0 , 657px 602px #A1B8D0 , 1px 363px #A1B8D0 , 807px 533px #A1B8D0 , 250px 956px #A1B8D0 , 713px 633px #A1B8D0 , 694px 939px #A1B8D0 , 202px 867px #A1B8D0 , 511px 481px #A1B8D0 , 933px 831px #A1B8D0 , 123px 95px #A1B8D0 , 572px 823px #A1B8D0 , 442px 399px #A1B8D0 , 120px 577px #A1B8D0 , 122px 880px #A1B8D0 , 212px 72px #A1B8D0 , 482px 394px #A1B8D0 , 353px 527px #A1B8D0 , 729px 949px #A1B8D0 , 848px 544px #A1B8D0 , 550px 866px #A1B8D0 , 215px 51px #A1B8D0 , 252px 680px #A1B8D0 , 885px 74px #A1B8D0 , 211px 271px #A1B8D0 , 588px 810px #A1B8D0 , 967px 976px #A1B8D0 , 503px 984px #A1B8D0 , 489px 162px #A1B8D0 , 373px 88px #A1B8D0 , 211px 106px #A1B8D0 , 512px 711px #A1B8D0 , 758px 767px #A1B8D0 , 770px 691px #A1B8D0 , 47px 998px #A1B8D0 , 232px 563px #A1B8D0 , 123px 407px #A1B8D0 , 471px 762px #A1B8D0 , 275px 770px #A1B8D0 , 107px 584px #A1B8D0 , 355px 69px #A1B8D0 , 631px 444px #A1B8D0 , 240px 281px #A1B8D0 , 317px 637px #A1B8D0 , 577px 384px #A1B8D0 , 530px 833px #A1B8D0 , 516px 551px #A1B8D0 , 71px 56px #A1B8D0 , 906px 782px #A1B8D0 , 649px 998px #A1B8D0 , 84px 60px #A1B8D0 , 240px 563px #A1B8D0 , 32px 19px #A1B8D0 , 441px 778px #A1B8D0 , 544px 584px #A1B8D0 , 986px 317px #A1B8D0 , 116px 734px #A1B8D0 , 794px 839px #A1B8D0 , 112px 155px #A1B8D0 , 509px 292px #A1B8D0 , 163px 883px #A1B8D0 , 237px 861px #A1B8D0 , 441px 992px #A1B8D0 , 287px 274px #A1B8D0 , 466px 804px #A1B8D0 , 791px 443px #A1B8D0 , 778px 570px #A1B8D0 , 776px 183px #A1B8D0 , 831px 534px #A1B8D0 , 778px 235px #A1B8D0 , 268px 553px #A1B8D0 , 828px 366px #A1B8D0 , 46px 184px #A1B8D0 , 718px 685px #A1B8D0 , 461px 570px #A1B8D0 , 105px 821px #A1B8D0 , 121px 696px #A1B8D0 , 441px 279px #A1B8D0 , 252px 626px #A1B8D0 , 797px 50px #A1B8D0 , 895px 24px #A1B8D0 , 965px 368px #A1B8D0 , 764px 942px #A1B8D0 , 370px 343px #A1B8D0 , 726px 309px #A1B8D0 , 523px 680px #A1B8D0 , 12px 691px #A1B8D0 , 844px 598px #A1B8D0 , 439px 430px #A1B8D0 , 467px 740px #A1B8D0 , 263px 529px #A1B8D0 , 14px 248px #A1B8D0 , 753px 93px #A1B8D0 , 596px 422px #A1B8D0 , 469px 413px #A1B8D0 , 175px 555px #A1B8D0 , 29px 796px #A1B8D0 , 577px 887px #A1B8D0 , 918px 838px #A1B8D0 , 97px 62px #A1B8D0 , 765px 640px #A1B8D0 , 248px 897px #A1B8D0 , 812px 699px #A1B8D0 , 431px 472px #A1B8D0 , 751px 934px #A1B8D0 , 169px 206px #A1B8D0 , 19px 860px #A1B8D0 , 625px 164px #A1B8D0 , 578px 93px #A1B8D0 , 895px 297px #A1B8D0 , 744px 418px #A1B8D0 , 734px 854px #A1B8D0 , 626px 629px #A1B8D0 , 270px 468px #A1B8D0 , 769px 223px #A1B8D0 , 895px 772px #A1B8D0 , 721px 830px #A1B8D0 , 646px 75px #A1B8D0 , 718px 583px #A1B8D0 , 249px 558px #A1B8D0 , 106px 20px #A1B8D0 , 988px 623px #A1B8D0 , 907px 753px #A1B8D0 , 959px 235px #A1B8D0 , 821px 710px #A1B8D0 , 912px 827px #A1B8D0 , 143px 707px #A1B8D0;
  }
  
  @-moz-keyframes glitter-2 {
    0%,
      100%,
      2.90323%,
      12.90323% {
      opacity: 0;
    }
    7.90323% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-2 {
    0%,
      100%,
      2.90323%,
      12.90323% {
      opacity: 0;
    }
    7.90323% {
      opacity: 1;
    }
  }
  @keyframes glitter-2 {
    0%,
      100%,
      2.90323%,
      12.90323% {
      opacity: 0;
    }
    7.90323% {
      opacity: 1;
    }
  }
  .glitter_2 {
    -moz-animation: glitter-2 10s infinite;
    -webkit-animation: glitter-2 10s infinite;
    animation: glitter-2 10s infinite;
    box-shadow: 8px 52px #A1B8D0 , 734px 910px #A1B8D0 , 836px 596px #A1B8D0 , 884px 862px #A1B8D0 , 753px 877px #A1B8D0 , 871px 346px #A1B8D0 , 571px 600px #A1B8D0 , 592px 604px #A1B8D0 , 787px 240px #A1B8D0 , 758px 350px #A1B8D0 , 449px 165px #A1B8D0 , 857px 782px #A1B8D0 , 194px 785px #A1B8D0 , 985px 34px #A1B8D0 , 792px 320px #A1B8D0 , 530px 595px #A1B8D0 , 245px 745px #A1B8D0 , 531px 433px #A1B8D0 , 535px 849px #A1B8D0 , 260px 122px #A1B8D0 , 184px 47px #A1B8D0 , 733px 1000px #A1B8D0 , 111px 787px #A1B8D0 , 15px 592px #A1B8D0 , 617px 53px #A1B8D0 , 131px 814px #A1B8D0 , 769px 277px #A1B8D0 , 376px 733px #A1B8D0 , 162px 32px #A1B8D0 , 403px 795px #A1B8D0 , 275px 783px #A1B8D0 , 548px 844px #A1B8D0 , 275px 946px #A1B8D0 , 517px 690px #A1B8D0 , 61px 211px #A1B8D0 , 602px 900px #A1B8D0 , 461px 731px #A1B8D0 , 652px 946px #A1B8D0 , 537px 985px #A1B8D0 , 594px 496px #A1B8D0 , 569px 804px #A1B8D0 , 594px 793px #A1B8D0 , 827px 391px #A1B8D0 , 147px 241px #A1B8D0 , 167px 334px #A1B8D0 , 608px 891px #A1B8D0 , 478px 515px #A1B8D0 , 671px 115px #A1B8D0 , 60px 102px #A1B8D0 , 850px 579px #A1B8D0 , 817px 656px #A1B8D0 , 582px 182px #A1B8D0 , 615px 201px #A1B8D0 , 145px 428px #A1B8D0 , 549px 423px #A1B8D0 , 129px 364px #A1B8D0 , 36px 879px #A1B8D0 , 133px 86px #A1B8D0 , 935px 221px #A1B8D0 , 398px 991px #A1B8D0 , 866px 419px #A1B8D0 , 247px 385px #A1B8D0 , 746px 397px #A1B8D0 , 490px 769px #A1B8D0 , 710px 246px #A1B8D0 , 111px 258px #A1B8D0 , 331px 897px #A1B8D0 , 84px 282px #A1B8D0 , 278px 457px #A1B8D0 , 418px 331px #A1B8D0 , 574px 365px #A1B8D0 , 344px 579px #A1B8D0 , 826px 944px #A1B8D0 , 173px 744px #A1B8D0 , 217px 103px #A1B8D0 , 326px 528px #A1B8D0 , 604px 980px #A1B8D0 , 719px 724px #A1B8D0 , 824px 731px #A1B8D0 , 970px 224px #A1B8D0 , 243px 100px #A1B8D0 , 311px 968px #A1B8D0 , 90px 741px #A1B8D0 , 974px 674px #A1B8D0 , 291px 2px #A1B8D0 , 537px 744px #A1B8D0 , 997px 896px #A1B8D0 , 799px 566px #A1B8D0 , 562px 185px #A1B8D0 , 527px 982px #A1B8D0 , 852px 569px #A1B8D0 , 523px 591px #A1B8D0 , 240px 580px #A1B8D0 , 719px 789px #A1B8D0 , 325px 587px #A1B8D0 , 943px 216px #A1B8D0 , 507px 571px #A1B8D0 , 958px 167px #A1B8D0 , 684px 937px #A1B8D0 , 58px 673px #A1B8D0 , 463px 494px #A1B8D0 , 886px 722px #A1B8D0 , 511px 203px #A1B8D0 , 299px 72px #A1B8D0 , 662px 119px #A1B8D0 , 498px 735px #A1B8D0 , 546px 666px #A1B8D0 , 379px 542px #A1B8D0 , 702px 559px #A1B8D0 , 895px 493px #A1B8D0 , 812px 682px #A1B8D0 , 470px 29px #A1B8D0 , 28px 390px #A1B8D0 , 806px 396px #A1B8D0 , 477px 456px #A1B8D0 , 265px 453px #A1B8D0 , 723px 605px #A1B8D0 , 938px 950px #A1B8D0 , 359px 706px #A1B8D0 , 490px 204px #A1B8D0 , 400px 295px #A1B8D0 , 796px 899px #A1B8D0 , 628px 879px #A1B8D0 , 301px 563px #A1B8D0 , 793px 677px #A1B8D0 , 268px 67px #A1B8D0 , 478px 476px #A1B8D0 , 333px 805px #A1B8D0 , 866px 393px #A1B8D0 , 947px 742px #A1B8D0 , 967px 676px #A1B8D0 , 306px 128px #A1B8D0 , 701px 548px #A1B8D0 , 560px 829px #A1B8D0 , 899px 700px #A1B8D0 , 749px 675px #A1B8D0 , 608px 528px #A1B8D0 , 222px 380px #A1B8D0 , 863px 817px #A1B8D0 , 138px 759px #A1B8D0 , 34px 229px #A1B8D0 , 496px 867px #A1B8D0 , 646px 519px #A1B8D0 , 94px 476px #A1B8D0 , 38px 166px #A1B8D0 , 221px 692px #A1B8D0 , 73px 830px #A1B8D0 , 72px 180px #A1B8D0 , 726px 635px #A1B8D0 , 302px 263px #A1B8D0 , 786px 965px #A1B8D0 , 650px 137px #A1B8D0 , 616px 472px #A1B8D0 , 959px 526px #A1B8D0 , 278px 245px #A1B8D0 , 531px 213px #A1B8D0 , 824px 383px #A1B8D0 , 250px 288px #A1B8D0 , 100px 37px #A1B8D0 , 667px 34px #A1B8D0 , 301px 904px #A1B8D0 , 586px 255px #A1B8D0 , 20px 948px #A1B8D0 , 299px 593px #A1B8D0 , 870px 724px #A1B8D0 , 534px 484px #A1B8D0 , 130px 970px #A1B8D0 , 366px 817px #A1B8D0 , 691px 631px #A1B8D0 , 930px 307px #A1B8D0 , 504px 693px #A1B8D0 , 34px 83px #A1B8D0 , 689px 884px #A1B8D0 , 637px 276px #A1B8D0 , 354px 426px #A1B8D0 , 500px 566px #A1B8D0 , 622px 873px #A1B8D0 , 781px 549px #A1B8D0 , 292px 717px #A1B8D0 , 197px 1000px #A1B8D0 , 148px 494px #A1B8D0 , 763px 540px #A1B8D0 , 372px 618px #A1B8D0 , 978px 106px #A1B8D0 , 619px 564px #A1B8D0 , 799px 55px #A1B8D0 , 14px 289px #A1B8D0 , 697px 879px #A1B8D0 , 914px 927px #A1B8D0 , 579px 708px #A1B8D0 , 265px 71px #A1B8D0 , 979px 469px #A1B8D0 , 282px 491px #A1B8D0 , 829px 542px #A1B8D0 , 77px 727px #A1B8D0 , 557px 408px #A1B8D0 , 588px 681px #A1B8D0 , 371px 752px #A1B8D0 , 305px 722px #A1B8D0 , 745px 187px #A1B8D0;
  }
  .glitter_2:before {
    -moz-animation: glitter-2 8s infinite;
    -webkit-animation: glitter-2 8s infinite;
    animation: glitter-2 8s infinite;
    box-shadow: 8px 52px #A1B8D0 , 734px 910px #A1B8D0 , 836px 596px #A1B8D0 , 884px 862px #A1B8D0 , 753px 877px #A1B8D0 , 871px 346px #A1B8D0 , 571px 600px #A1B8D0 , 592px 604px #A1B8D0 , 787px 240px #A1B8D0 , 758px 350px #A1B8D0 , 449px 165px #A1B8D0 , 857px 782px #A1B8D0 , 194px 785px #A1B8D0 , 985px 34px #A1B8D0 , 792px 320px #A1B8D0 , 530px 595px #A1B8D0 , 245px 745px #A1B8D0 , 531px 433px #A1B8D0 , 535px 849px #A1B8D0 , 260px 122px #A1B8D0 , 184px 47px #A1B8D0 , 733px 1000px #A1B8D0 , 111px 787px #A1B8D0 , 15px 592px #A1B8D0 , 617px 53px #A1B8D0 , 131px 814px #A1B8D0 , 769px 277px #A1B8D0 , 376px 733px #A1B8D0 , 162px 32px #A1B8D0 , 403px 795px #A1B8D0 , 275px 783px #A1B8D0 , 548px 844px #A1B8D0 , 275px 946px #A1B8D0 , 517px 690px #A1B8D0 , 61px 211px #A1B8D0 , 602px 900px #A1B8D0 , 461px 731px #A1B8D0 , 652px 946px #A1B8D0 , 537px 985px #A1B8D0 , 594px 496px #A1B8D0 , 569px 804px #A1B8D0 , 594px 793px #A1B8D0 , 827px 391px #A1B8D0 , 147px 241px #A1B8D0 , 167px 334px #A1B8D0 , 608px 891px #A1B8D0 , 478px 515px #A1B8D0 , 671px 115px #A1B8D0 , 60px 102px #A1B8D0 , 850px 579px #A1B8D0 , 817px 656px #A1B8D0 , 582px 182px #A1B8D0 , 615px 201px #A1B8D0 , 145px 428px #A1B8D0 , 549px 423px #A1B8D0 , 129px 364px #A1B8D0 , 36px 879px #A1B8D0 , 133px 86px #A1B8D0 , 935px 221px #A1B8D0 , 398px 991px #A1B8D0 , 866px 419px #A1B8D0 , 247px 385px #A1B8D0 , 746px 397px #A1B8D0 , 490px 769px #A1B8D0 , 710px 246px #A1B8D0 , 111px 258px #A1B8D0 , 331px 897px #A1B8D0 , 84px 282px #A1B8D0 , 278px 457px #A1B8D0 , 418px 331px #A1B8D0 , 574px 365px #A1B8D0 , 344px 579px #A1B8D0 , 826px 944px #A1B8D0 , 173px 744px #A1B8D0 , 217px 103px #A1B8D0 , 326px 528px #A1B8D0 , 604px 980px #A1B8D0 , 719px 724px #A1B8D0 , 824px 731px #A1B8D0 , 970px 224px #A1B8D0 , 243px 100px #A1B8D0 , 311px 968px #A1B8D0 , 90px 741px #A1B8D0 , 974px 674px #A1B8D0 , 291px 2px #A1B8D0 , 537px 744px #A1B8D0 , 997px 896px #A1B8D0 , 799px 566px #A1B8D0 , 562px 185px #A1B8D0 , 527px 982px #A1B8D0 , 852px 569px #A1B8D0 , 523px 591px #A1B8D0 , 240px 580px #A1B8D0 , 719px 789px #A1B8D0 , 325px 587px #A1B8D0 , 943px 216px #A1B8D0 , 507px 571px #A1B8D0 , 958px 167px #A1B8D0 , 684px 937px #A1B8D0 , 58px 673px #A1B8D0 , 463px 494px #A1B8D0 , 886px 722px #A1B8D0 , 511px 203px #A1B8D0 , 299px 72px #A1B8D0 , 662px 119px #A1B8D0 , 498px 735px #A1B8D0 , 546px 666px #A1B8D0 , 379px 542px #A1B8D0 , 702px 559px #A1B8D0 , 895px 493px #A1B8D0 , 812px 682px #A1B8D0 , 470px 29px #A1B8D0 , 28px 390px #A1B8D0 , 806px 396px #A1B8D0 , 477px 456px #A1B8D0 , 265px 453px #A1B8D0 , 723px 605px #A1B8D0 , 938px 950px #A1B8D0 , 359px 706px #A1B8D0 , 490px 204px #A1B8D0 , 400px 295px #A1B8D0 , 796px 899px #A1B8D0 , 628px 879px #A1B8D0 , 301px 563px #A1B8D0 , 793px 677px #A1B8D0 , 268px 67px #A1B8D0 , 478px 476px #A1B8D0 , 333px 805px #A1B8D0 , 866px 393px #A1B8D0 , 947px 742px #A1B8D0 , 967px 676px #A1B8D0 , 306px 128px #A1B8D0 , 701px 548px #A1B8D0 , 560px 829px #A1B8D0 , 899px 700px #A1B8D0 , 749px 675px #A1B8D0 , 608px 528px #A1B8D0 , 222px 380px #A1B8D0 , 863px 817px #A1B8D0 , 138px 759px #A1B8D0 , 34px 229px #A1B8D0 , 496px 867px #A1B8D0 , 646px 519px #A1B8D0 , 94px 476px #A1B8D0 , 38px 166px #A1B8D0 , 221px 692px #A1B8D0 , 73px 830px #A1B8D0 , 72px 180px #A1B8D0 , 726px 635px #A1B8D0 , 302px 263px #A1B8D0 , 786px 965px #A1B8D0 , 650px 137px #A1B8D0 , 616px 472px #A1B8D0 , 959px 526px #A1B8D0 , 278px 245px #A1B8D0 , 531px 213px #A1B8D0 , 824px 383px #A1B8D0 , 250px 288px #A1B8D0 , 100px 37px #A1B8D0 , 667px 34px #A1B8D0 , 301px 904px #A1B8D0 , 586px 255px #A1B8D0 , 20px 948px #A1B8D0 , 299px 593px #A1B8D0 , 870px 724px #A1B8D0 , 534px 484px #A1B8D0 , 130px 970px #A1B8D0 , 366px 817px #A1B8D0 , 691px 631px #A1B8D0 , 930px 307px #A1B8D0 , 504px 693px #A1B8D0 , 34px 83px #A1B8D0 , 689px 884px #A1B8D0 , 637px 276px #A1B8D0 , 354px 426px #A1B8D0 , 500px 566px #A1B8D0 , 622px 873px #A1B8D0 , 781px 549px #A1B8D0 , 292px 717px #A1B8D0 , 197px 1000px #A1B8D0 , 148px 494px #A1B8D0 , 763px 540px #A1B8D0 , 372px 618px #A1B8D0 , 978px 106px #A1B8D0 , 619px 564px #A1B8D0 , 799px 55px #A1B8D0 , 14px 289px #A1B8D0 , 697px 879px #A1B8D0 , 914px 927px #A1B8D0 , 579px 708px #A1B8D0 , 265px 71px #A1B8D0 , 979px 469px #A1B8D0 , 282px 491px #A1B8D0 , 829px 542px #A1B8D0 , 77px 727px #A1B8D0 , 557px 408px #A1B8D0 , 588px 681px #A1B8D0 , 371px 752px #A1B8D0 , 305px 722px #A1B8D0 , 745px 187px #A1B8D0;
  }
  .glitter_2:after {
    -moz-animation: glitter-2 9s infinite;
    -webkit-animation: glitter-2 9s infinite;
    animation: glitter-2 9s infinite;
    box-shadow: 8px 52px #A1B8D0 , 734px 910px #A1B8D0 , 836px 596px #A1B8D0 , 884px 862px #A1B8D0 , 753px 877px #A1B8D0 , 871px 346px #A1B8D0 , 571px 600px #A1B8D0 , 592px 604px #A1B8D0 , 787px 240px #A1B8D0 , 758px 350px #A1B8D0 , 449px 165px #A1B8D0 , 857px 782px #A1B8D0 , 194px 785px #A1B8D0 , 985px 34px #A1B8D0 , 792px 320px #A1B8D0 , 530px 595px #A1B8D0 , 245px 745px #A1B8D0 , 531px 433px #A1B8D0 , 535px 849px #A1B8D0 , 260px 122px #A1B8D0 , 184px 47px #A1B8D0 , 733px 1000px #A1B8D0 , 111px 787px #A1B8D0 , 15px 592px #A1B8D0 , 617px 53px #A1B8D0 , 131px 814px #A1B8D0 , 769px 277px #A1B8D0 , 376px 733px #A1B8D0 , 162px 32px #A1B8D0 , 403px 795px #A1B8D0 , 275px 783px #A1B8D0 , 548px 844px #A1B8D0 , 275px 946px #A1B8D0 , 517px 690px #A1B8D0 , 61px 211px #A1B8D0 , 602px 900px #A1B8D0 , 461px 731px #A1B8D0 , 652px 946px #A1B8D0 , 537px 985px #A1B8D0 , 594px 496px #A1B8D0 , 569px 804px #A1B8D0 , 594px 793px #A1B8D0 , 827px 391px #A1B8D0 , 147px 241px #A1B8D0 , 167px 334px #A1B8D0 , 608px 891px #A1B8D0 , 478px 515px #A1B8D0 , 671px 115px #A1B8D0 , 60px 102px #A1B8D0 , 850px 579px #A1B8D0 , 817px 656px #A1B8D0 , 582px 182px #A1B8D0 , 615px 201px #A1B8D0 , 145px 428px #A1B8D0 , 549px 423px #A1B8D0 , 129px 364px #A1B8D0 , 36px 879px #A1B8D0 , 133px 86px #A1B8D0 , 935px 221px #A1B8D0 , 398px 991px #A1B8D0 , 866px 419px #A1B8D0 , 247px 385px #A1B8D0 , 746px 397px #A1B8D0 , 490px 769px #A1B8D0 , 710px 246px #A1B8D0 , 111px 258px #A1B8D0 , 331px 897px #A1B8D0 , 84px 282px #A1B8D0 , 278px 457px #A1B8D0 , 418px 331px #A1B8D0 , 574px 365px #A1B8D0 , 344px 579px #A1B8D0 , 826px 944px #A1B8D0 , 173px 744px #A1B8D0 , 217px 103px #A1B8D0 , 326px 528px #A1B8D0 , 604px 980px #A1B8D0 , 719px 724px #A1B8D0 , 824px 731px #A1B8D0 , 970px 224px #A1B8D0 , 243px 100px #A1B8D0 , 311px 968px #A1B8D0 , 90px 741px #A1B8D0 , 974px 674px #A1B8D0 , 291px 2px #A1B8D0 , 537px 744px #A1B8D0 , 997px 896px #A1B8D0 , 799px 566px #A1B8D0 , 562px 185px #A1B8D0 , 527px 982px #A1B8D0 , 852px 569px #A1B8D0 , 523px 591px #A1B8D0 , 240px 580px #A1B8D0 , 719px 789px #A1B8D0 , 325px 587px #A1B8D0 , 943px 216px #A1B8D0 , 507px 571px #A1B8D0 , 958px 167px #A1B8D0 , 684px 937px #A1B8D0 , 58px 673px #A1B8D0 , 463px 494px #A1B8D0 , 886px 722px #A1B8D0 , 511px 203px #A1B8D0 , 299px 72px #A1B8D0 , 662px 119px #A1B8D0 , 498px 735px #A1B8D0 , 546px 666px #A1B8D0 , 379px 542px #A1B8D0 , 702px 559px #A1B8D0 , 895px 493px #A1B8D0 , 812px 682px #A1B8D0 , 470px 29px #A1B8D0 , 28px 390px #A1B8D0 , 806px 396px #A1B8D0 , 477px 456px #A1B8D0 , 265px 453px #A1B8D0 , 723px 605px #A1B8D0 , 938px 950px #A1B8D0 , 359px 706px #A1B8D0 , 490px 204px #A1B8D0 , 400px 295px #A1B8D0 , 796px 899px #A1B8D0 , 628px 879px #A1B8D0 , 301px 563px #A1B8D0 , 793px 677px #A1B8D0 , 268px 67px #A1B8D0 , 478px 476px #A1B8D0 , 333px 805px #A1B8D0 , 866px 393px #A1B8D0 , 947px 742px #A1B8D0 , 967px 676px #A1B8D0 , 306px 128px #A1B8D0 , 701px 548px #A1B8D0 , 560px 829px #A1B8D0 , 899px 700px #A1B8D0 , 749px 675px #A1B8D0 , 608px 528px #A1B8D0 , 222px 380px #A1B8D0 , 863px 817px #A1B8D0 , 138px 759px #A1B8D0 , 34px 229px #A1B8D0 , 496px 867px #A1B8D0 , 646px 519px #A1B8D0 , 94px 476px #A1B8D0 , 38px 166px #A1B8D0 , 221px 692px #A1B8D0 , 73px 830px #A1B8D0 , 72px 180px #A1B8D0 , 726px 635px #A1B8D0 , 302px 263px #A1B8D0 , 786px 965px #A1B8D0 , 650px 137px #A1B8D0 , 616px 472px #A1B8D0 , 959px 526px #A1B8D0 , 278px 245px #A1B8D0 , 531px 213px #A1B8D0 , 824px 383px #A1B8D0 , 250px 288px #A1B8D0 , 100px 37px #A1B8D0 , 667px 34px #A1B8D0 , 301px 904px #A1B8D0 , 586px 255px #A1B8D0 , 20px 948px #A1B8D0 , 299px 593px #A1B8D0 , 870px 724px #A1B8D0 , 534px 484px #A1B8D0 , 130px 970px #A1B8D0 , 366px 817px #A1B8D0 , 691px 631px #A1B8D0 , 930px 307px #A1B8D0 , 504px 693px #A1B8D0 , 34px 83px #A1B8D0 , 689px 884px #A1B8D0 , 637px 276px #A1B8D0 , 354px 426px #A1B8D0 , 500px 566px #A1B8D0 , 622px 873px #A1B8D0 , 781px 549px #A1B8D0 , 292px 717px #A1B8D0 , 197px 1000px #A1B8D0 , 148px 494px #A1B8D0 , 763px 540px #A1B8D0 , 372px 618px #A1B8D0 , 978px 106px #A1B8D0 , 619px 564px #A1B8D0 , 799px 55px #A1B8D0 , 14px 289px #A1B8D0 , 697px 879px #A1B8D0 , 914px 927px #A1B8D0 , 579px 708px #A1B8D0 , 265px 71px #A1B8D0 , 979px 469px #A1B8D0 , 282px 491px #A1B8D0 , 829px 542px #A1B8D0 , 77px 727px #A1B8D0 , 557px 408px #A1B8D0 , 588px 681px #A1B8D0 , 371px 752px #A1B8D0 , 305px 722px #A1B8D0 , 745px 187px #A1B8D0;
  }
  
  @-moz-keyframes glitter-3 {
    0%,
      100%,
      5.80645%,
      15.80645% {
      opacity: 0;
    }
    10.80645% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-3 {
    0%,
      100%,
      5.80645%,
      15.80645% {
      opacity: 0;
    }
    10.80645% {
      opacity: 1;
    }
  }
  @keyframes glitter-3 {
    0%,
      100%,
      5.80645%,
      15.80645% {
      opacity: 0;
    }
    10.80645% {
      opacity: 1;
    }
  }
  .glitter_3 {
    -moz-animation: glitter-3 10s infinite;
    -webkit-animation: glitter-3 10s infinite;
    animation: glitter-3 10s infinite;
    box-shadow: 900px 227px #A1B8D0 , 445px 470px #A1B8D0 , 189px 137px #A1B8D0 , 420px 601px #A1B8D0 , 886px 884px #A1B8D0 , 867px 915px #A1B8D0 , 574px 623px #A1B8D0 , 82px 196px #A1B8D0 , 703px 230px #A1B8D0 , 521px 423px #A1B8D0 , 967px 355px #A1B8D0 , 28px 154px #A1B8D0 , 217px 288px #A1B8D0 , 311px 265px #A1B8D0 , 306px 275px #A1B8D0 , 346px 578px #A1B8D0 , 535px 626px #A1B8D0 , 650px 3px #A1B8D0 , 33px 277px #A1B8D0 , 61px 593px #A1B8D0 , 895px 650px #A1B8D0 , 649px 454px #A1B8D0 , 131px 943px #A1B8D0 , 533px 806px #A1B8D0 , 715px 10px #A1B8D0 , 884px 319px #A1B8D0 , 368px 110px #A1B8D0 , 688px 574px #A1B8D0 , 886px 368px #A1B8D0 , 928px 482px #A1B8D0 , 958px 514px #A1B8D0 , 281px 490px #A1B8D0 , 181px 755px #A1B8D0 , 755px 792px #A1B8D0 , 91px 523px #A1B8D0 , 792px 352px #A1B8D0 , 230px 53px #A1B8D0 , 472px 347px #A1B8D0 , 560px 677px #A1B8D0 , 263px 995px #A1B8D0 , 268px 768px #A1B8D0 , 261px 658px #A1B8D0 , 891px 154px #A1B8D0 , 618px 896px #A1B8D0 , 211px 256px #A1B8D0 , 655px 660px #A1B8D0 , 461px 164px #A1B8D0 , 913px 399px #A1B8D0 , 263px 503px #A1B8D0 , 669px 849px #A1B8D0 , 516px 877px #A1B8D0 , 401px 490px #A1B8D0 , 359px 407px #A1B8D0 , 265px 581px #A1B8D0 , 560px 708px #A1B8D0 , 832px 117px #A1B8D0 , 447px 981px #A1B8D0 , 579px 190px #A1B8D0 , 415px 390px #A1B8D0 , 154px 390px #A1B8D0 , 580px 477px #A1B8D0 , 193px 622px #A1B8D0 , 582px 55px #A1B8D0 , 542px 774px #A1B8D0 , 129px 544px #A1B8D0 , 988px 485px #A1B8D0 , 626px 332px #A1B8D0 , 603px 970px #A1B8D0 , 150px 574px #A1B8D0 , 969px 843px #A1B8D0 , 175px 286px #A1B8D0 , 376px 280px #A1B8D0 , 453px 680px #A1B8D0 , 850px 128px #A1B8D0 , 897px 374px #A1B8D0 , 27px 135px #A1B8D0 , 712px 577px #A1B8D0 , 44px 569px #A1B8D0 , 711px 110px #A1B8D0 , 908px 594px #A1B8D0 , 314px 245px #A1B8D0 , 515px 473px #A1B8D0 , 838px 57px #A1B8D0 , 98px 703px #A1B8D0 , 7px 489px #A1B8D0 , 916px 701px #A1B8D0 , 665px 792px #A1B8D0 , 657px 533px #A1B8D0 , 473px 28px #A1B8D0 , 801px 734px #A1B8D0 , 848px 917px #A1B8D0 , 37px 725px #A1B8D0 , 657px 182px #A1B8D0 , 550px 738px #A1B8D0 , 585px 316px #A1B8D0 , 14px 217px #A1B8D0 , 632px 291px #A1B8D0 , 352px 937px #A1B8D0 , 332px 932px #A1B8D0 , 413px 404px #A1B8D0 , 675px 408px #A1B8D0 , 767px 329px #A1B8D0 , 107px 470px #A1B8D0 , 270px 383px #A1B8D0 , 444px 200px #A1B8D0 , 844px 834px #A1B8D0 , 859px 810px #A1B8D0 , 201px 323px #A1B8D0 , 536px 945px #A1B8D0 , 882px 556px #A1B8D0 , 48px 226px #A1B8D0 , 430px 762px #A1B8D0 , 205px 213px #A1B8D0 , 136px 208px #A1B8D0 , 336px 799px #A1B8D0 , 687px 241px #A1B8D0 , 855px 107px #A1B8D0 , 467px 54px #A1B8D0 , 882px 556px #A1B8D0 , 992px 404px #A1B8D0 , 519px 452px #A1B8D0 , 895px 44px #A1B8D0 , 528px 233px #A1B8D0 , 92px 369px #A1B8D0 , 423px 666px #A1B8D0 , 819px 203px #A1B8D0 , 206px 641px #A1B8D0 , 158px 927px #A1B8D0 , 103px 351px #A1B8D0 , 147px 849px #A1B8D0 , 843px 11px #A1B8D0 , 807px 232px #A1B8D0 , 823px 108px #A1B8D0 , 911px 921px #A1B8D0 , 141px 270px #A1B8D0 , 902px 886px #A1B8D0 , 554px 41px #A1B8D0 , 344px 709px #A1B8D0 , 645px 226px #A1B8D0 , 220px 759px #A1B8D0 , 382px 972px #A1B8D0 , 549px 554px #A1B8D0 , 575px 606px #A1B8D0 , 344px 937px #A1B8D0 , 519px 967px #A1B8D0 , 983px 877px #A1B8D0 , 956px 624px #A1B8D0 , 583px 531px #A1B8D0 , 493px 986px #A1B8D0 , 571px 17px #A1B8D0 , 801px 966px #A1B8D0 , 870px 8px #A1B8D0 , 464px 34px #A1B8D0 , 212px 500px #A1B8D0 , 392px 713px #A1B8D0 , 582px 225px #A1B8D0 , 144px 891px #A1B8D0 , 536px 61px #A1B8D0 , 57px 471px #A1B8D0 , 299px 973px #A1B8D0 , 465px 807px #A1B8D0 , 144px 514px #A1B8D0 , 350px 298px #A1B8D0 , 393px 853px #A1B8D0 , 366px 58px #A1B8D0 , 996px 481px #A1B8D0 , 94px 743px #A1B8D0 , 975px 990px #A1B8D0 , 693px 360px #A1B8D0 , 879px 939px #A1B8D0 , 116px 57px #A1B8D0 , 434px 853px #A1B8D0 , 932px 854px #A1B8D0 , 441px 412px #A1B8D0 , 723px 96px #A1B8D0 , 286px 393px #A1B8D0 , 184px 294px #A1B8D0 , 203px 987px #A1B8D0 , 273px 778px #A1B8D0 , 218px 982px #A1B8D0 , 145px 789px #A1B8D0 , 222px 432px #A1B8D0 , 274px 476px #A1B8D0 , 190px 63px #A1B8D0 , 980px 495px #A1B8D0 , 827px 570px #A1B8D0 , 628px 132px #A1B8D0 , 135px 207px #A1B8D0 , 513px 415px #A1B8D0 , 888px 61px #A1B8D0 , 246px 770px #A1B8D0 , 414px 281px #A1B8D0 , 735px 627px #A1B8D0 , 471px 432px #A1B8D0 , 592px 625px #A1B8D0 , 938px 835px #A1B8D0 , 252px 824px #A1B8D0 , 221px 518px #A1B8D0 , 44px 966px #A1B8D0 , 327px 964px #A1B8D0;
  }
  .glitter_3:before {
    -moz-animation: glitter-3 8s infinite;
    -webkit-animation: glitter-3 8s infinite;
    animation: glitter-3 8s infinite;
    box-shadow: 900px 227px #A1B8D0 , 445px 470px #A1B8D0 , 189px 137px #A1B8D0 , 420px 601px #A1B8D0 , 886px 884px #A1B8D0 , 867px 915px #A1B8D0 , 574px 623px #A1B8D0 , 82px 196px #A1B8D0 , 703px 230px #A1B8D0 , 521px 423px #A1B8D0 , 967px 355px #A1B8D0 , 28px 154px #A1B8D0 , 217px 288px #A1B8D0 , 311px 265px #A1B8D0 , 306px 275px #A1B8D0 , 346px 578px #A1B8D0 , 535px 626px #A1B8D0 , 650px 3px #A1B8D0 , 33px 277px #A1B8D0 , 61px 593px #A1B8D0 , 895px 650px #A1B8D0 , 649px 454px #A1B8D0 , 131px 943px #A1B8D0 , 533px 806px #A1B8D0 , 715px 10px #A1B8D0 , 884px 319px #A1B8D0 , 368px 110px #A1B8D0 , 688px 574px #A1B8D0 , 886px 368px #A1B8D0 , 928px 482px #A1B8D0 , 958px 514px #A1B8D0 , 281px 490px #A1B8D0 , 181px 755px #A1B8D0 , 755px 792px #A1B8D0 , 91px 523px #A1B8D0 , 792px 352px #A1B8D0 , 230px 53px #A1B8D0 , 472px 347px #A1B8D0 , 560px 677px #A1B8D0 , 263px 995px #A1B8D0 , 268px 768px #A1B8D0 , 261px 658px #A1B8D0 , 891px 154px #A1B8D0 , 618px 896px #A1B8D0 , 211px 256px #A1B8D0 , 655px 660px #A1B8D0 , 461px 164px #A1B8D0 , 913px 399px #A1B8D0 , 263px 503px #A1B8D0 , 669px 849px #A1B8D0 , 516px 877px #A1B8D0 , 401px 490px #A1B8D0 , 359px 407px #A1B8D0 , 265px 581px #A1B8D0 , 560px 708px #A1B8D0 , 832px 117px #A1B8D0 , 447px 981px #A1B8D0 , 579px 190px #A1B8D0 , 415px 390px #A1B8D0 , 154px 390px #A1B8D0 , 580px 477px #A1B8D0 , 193px 622px #A1B8D0 , 582px 55px #A1B8D0 , 542px 774px #A1B8D0 , 129px 544px #A1B8D0 , 988px 485px #A1B8D0 , 626px 332px #A1B8D0 , 603px 970px #A1B8D0 , 150px 574px #A1B8D0 , 969px 843px #A1B8D0 , 175px 286px #A1B8D0 , 376px 280px #A1B8D0 , 453px 680px #A1B8D0 , 850px 128px #A1B8D0 , 897px 374px #A1B8D0 , 27px 135px #A1B8D0 , 712px 577px #A1B8D0 , 44px 569px #A1B8D0 , 711px 110px #A1B8D0 , 908px 594px #A1B8D0 , 314px 245px #A1B8D0 , 515px 473px #A1B8D0 , 838px 57px #A1B8D0 , 98px 703px #A1B8D0 , 7px 489px #A1B8D0 , 916px 701px #A1B8D0 , 665px 792px #A1B8D0 , 657px 533px #A1B8D0 , 473px 28px #A1B8D0 , 801px 734px #A1B8D0 , 848px 917px #A1B8D0 , 37px 725px #A1B8D0 , 657px 182px #A1B8D0 , 550px 738px #A1B8D0 , 585px 316px #A1B8D0 , 14px 217px #A1B8D0 , 632px 291px #A1B8D0 , 352px 937px #A1B8D0 , 332px 932px #A1B8D0 , 413px 404px #A1B8D0 , 675px 408px #A1B8D0 , 767px 329px #A1B8D0 , 107px 470px #A1B8D0 , 270px 383px #A1B8D0 , 444px 200px #A1B8D0 , 844px 834px #A1B8D0 , 859px 810px #A1B8D0 , 201px 323px #A1B8D0 , 536px 945px #A1B8D0 , 882px 556px #A1B8D0 , 48px 226px #A1B8D0 , 430px 762px #A1B8D0 , 205px 213px #A1B8D0 , 136px 208px #A1B8D0 , 336px 799px #A1B8D0 , 687px 241px #A1B8D0 , 855px 107px #A1B8D0 , 467px 54px #A1B8D0 , 882px 556px #A1B8D0 , 992px 404px #A1B8D0 , 519px 452px #A1B8D0 , 895px 44px #A1B8D0 , 528px 233px #A1B8D0 , 92px 369px #A1B8D0 , 423px 666px #A1B8D0 , 819px 203px #A1B8D0 , 206px 641px #A1B8D0 , 158px 927px #A1B8D0 , 103px 351px #A1B8D0 , 147px 849px #A1B8D0 , 843px 11px #A1B8D0 , 807px 232px #A1B8D0 , 823px 108px #A1B8D0 , 911px 921px #A1B8D0 , 141px 270px #A1B8D0 , 902px 886px #A1B8D0 , 554px 41px #A1B8D0 , 344px 709px #A1B8D0 , 645px 226px #A1B8D0 , 220px 759px #A1B8D0 , 382px 972px #A1B8D0 , 549px 554px #A1B8D0 , 575px 606px #A1B8D0 , 344px 937px #A1B8D0 , 519px 967px #A1B8D0 , 983px 877px #A1B8D0 , 956px 624px #A1B8D0 , 583px 531px #A1B8D0 , 493px 986px #A1B8D0 , 571px 17px #A1B8D0 , 801px 966px #A1B8D0 , 870px 8px #A1B8D0 , 464px 34px #A1B8D0 , 212px 500px #A1B8D0 , 392px 713px #A1B8D0 , 582px 225px #A1B8D0 , 144px 891px #A1B8D0 , 536px 61px #A1B8D0 , 57px 471px #A1B8D0 , 299px 973px #A1B8D0 , 465px 807px #A1B8D0 , 144px 514px #A1B8D0 , 350px 298px #A1B8D0 , 393px 853px #A1B8D0 , 366px 58px #A1B8D0 , 996px 481px #A1B8D0 , 94px 743px #A1B8D0 , 975px 990px #A1B8D0 , 693px 360px #A1B8D0 , 879px 939px #A1B8D0 , 116px 57px #A1B8D0 , 434px 853px #A1B8D0 , 932px 854px #A1B8D0 , 441px 412px #A1B8D0 , 723px 96px #A1B8D0 , 286px 393px #A1B8D0 , 184px 294px #A1B8D0 , 203px 987px #A1B8D0 , 273px 778px #A1B8D0 , 218px 982px #A1B8D0 , 145px 789px #A1B8D0 , 222px 432px #A1B8D0 , 274px 476px #A1B8D0 , 190px 63px #A1B8D0 , 980px 495px #A1B8D0 , 827px 570px #A1B8D0 , 628px 132px #A1B8D0 , 135px 207px #A1B8D0 , 513px 415px #A1B8D0 , 888px 61px #A1B8D0 , 246px 770px #A1B8D0 , 414px 281px #A1B8D0 , 735px 627px #A1B8D0 , 471px 432px #A1B8D0 , 592px 625px #A1B8D0 , 938px 835px #A1B8D0 , 252px 824px #A1B8D0 , 221px 518px #A1B8D0 , 44px 966px #A1B8D0 , 327px 964px #A1B8D0;
  }
  .glitter_3:after {
    -moz-animation: glitter-3 9s infinite;
    -webkit-animation: glitter-3 9s infinite;
    animation: glitter-3 9s infinite;
    box-shadow: 900px 227px #A1B8D0 , 445px 470px #A1B8D0 , 189px 137px #A1B8D0 , 420px 601px #A1B8D0 , 886px 884px #A1B8D0 , 867px 915px #A1B8D0 , 574px 623px #A1B8D0 , 82px 196px #A1B8D0 , 703px 230px #A1B8D0 , 521px 423px #A1B8D0 , 967px 355px #A1B8D0 , 28px 154px #A1B8D0 , 217px 288px #A1B8D0 , 311px 265px #A1B8D0 , 306px 275px #A1B8D0 , 346px 578px #A1B8D0 , 535px 626px #A1B8D0 , 650px 3px #A1B8D0 , 33px 277px #A1B8D0 , 61px 593px #A1B8D0 , 895px 650px #A1B8D0 , 649px 454px #A1B8D0 , 131px 943px #A1B8D0 , 533px 806px #A1B8D0 , 715px 10px #A1B8D0 , 884px 319px #A1B8D0 , 368px 110px #A1B8D0 , 688px 574px #A1B8D0 , 886px 368px #A1B8D0 , 928px 482px #A1B8D0 , 958px 514px #A1B8D0 , 281px 490px #A1B8D0 , 181px 755px #A1B8D0 , 755px 792px #A1B8D0 , 91px 523px #A1B8D0 , 792px 352px #A1B8D0 , 230px 53px #A1B8D0 , 472px 347px #A1B8D0 , 560px 677px #A1B8D0 , 263px 995px #A1B8D0 , 268px 768px #A1B8D0 , 261px 658px #A1B8D0 , 891px 154px #A1B8D0 , 618px 896px #A1B8D0 , 211px 256px #A1B8D0 , 655px 660px #A1B8D0 , 461px 164px #A1B8D0 , 913px 399px #A1B8D0 , 263px 503px #A1B8D0 , 669px 849px #A1B8D0 , 516px 877px #A1B8D0 , 401px 490px #A1B8D0 , 359px 407px #A1B8D0 , 265px 581px #A1B8D0 , 560px 708px #A1B8D0 , 832px 117px #A1B8D0 , 447px 981px #A1B8D0 , 579px 190px #A1B8D0 , 415px 390px #A1B8D0 , 154px 390px #A1B8D0 , 580px 477px #A1B8D0 , 193px 622px #A1B8D0 , 582px 55px #A1B8D0 , 542px 774px #A1B8D0 , 129px 544px #A1B8D0 , 988px 485px #A1B8D0 , 626px 332px #A1B8D0 , 603px 970px #A1B8D0 , 150px 574px #A1B8D0 , 969px 843px #A1B8D0 , 175px 286px #A1B8D0 , 376px 280px #A1B8D0 , 453px 680px #A1B8D0 , 850px 128px #A1B8D0 , 897px 374px #A1B8D0 , 27px 135px #A1B8D0 , 712px 577px #A1B8D0 , 44px 569px #A1B8D0 , 711px 110px #A1B8D0 , 908px 594px #A1B8D0 , 314px 245px #A1B8D0 , 515px 473px #A1B8D0 , 838px 57px #A1B8D0 , 98px 703px #A1B8D0 , 7px 489px #A1B8D0 , 916px 701px #A1B8D0 , 665px 792px #A1B8D0 , 657px 533px #A1B8D0 , 473px 28px #A1B8D0 , 801px 734px #A1B8D0 , 848px 917px #A1B8D0 , 37px 725px #A1B8D0 , 657px 182px #A1B8D0 , 550px 738px #A1B8D0 , 585px 316px #A1B8D0 , 14px 217px #A1B8D0 , 632px 291px #A1B8D0 , 352px 937px #A1B8D0 , 332px 932px #A1B8D0 , 413px 404px #A1B8D0 , 675px 408px #A1B8D0 , 767px 329px #A1B8D0 , 107px 470px #A1B8D0 , 270px 383px #A1B8D0 , 444px 200px #A1B8D0 , 844px 834px #A1B8D0 , 859px 810px #A1B8D0 , 201px 323px #A1B8D0 , 536px 945px #A1B8D0 , 882px 556px #A1B8D0 , 48px 226px #A1B8D0 , 430px 762px #A1B8D0 , 205px 213px #A1B8D0 , 136px 208px #A1B8D0 , 336px 799px #A1B8D0 , 687px 241px #A1B8D0 , 855px 107px #A1B8D0 , 467px 54px #A1B8D0 , 882px 556px #A1B8D0 , 992px 404px #A1B8D0 , 519px 452px #A1B8D0 , 895px 44px #A1B8D0 , 528px 233px #A1B8D0 , 92px 369px #A1B8D0 , 423px 666px #A1B8D0 , 819px 203px #A1B8D0 , 206px 641px #A1B8D0 , 158px 927px #A1B8D0 , 103px 351px #A1B8D0 , 147px 849px #A1B8D0 , 843px 11px #A1B8D0 , 807px 232px #A1B8D0 , 823px 108px #A1B8D0 , 911px 921px #A1B8D0 , 141px 270px #A1B8D0 , 902px 886px #A1B8D0 , 554px 41px #A1B8D0 , 344px 709px #A1B8D0 , 645px 226px #A1B8D0 , 220px 759px #A1B8D0 , 382px 972px #A1B8D0 , 549px 554px #A1B8D0 , 575px 606px #A1B8D0 , 344px 937px #A1B8D0 , 519px 967px #A1B8D0 , 983px 877px #A1B8D0 , 956px 624px #A1B8D0 , 583px 531px #A1B8D0 , 493px 986px #A1B8D0 , 571px 17px #A1B8D0 , 801px 966px #A1B8D0 , 870px 8px #A1B8D0 , 464px 34px #A1B8D0 , 212px 500px #A1B8D0 , 392px 713px #A1B8D0 , 582px 225px #A1B8D0 , 144px 891px #A1B8D0 , 536px 61px #A1B8D0 , 57px 471px #A1B8D0 , 299px 973px #A1B8D0 , 465px 807px #A1B8D0 , 144px 514px #A1B8D0 , 350px 298px #A1B8D0 , 393px 853px #A1B8D0 , 366px 58px #A1B8D0 , 996px 481px #A1B8D0 , 94px 743px #A1B8D0 , 975px 990px #A1B8D0 , 693px 360px #A1B8D0 , 879px 939px #A1B8D0 , 116px 57px #A1B8D0 , 434px 853px #A1B8D0 , 932px 854px #A1B8D0 , 441px 412px #A1B8D0 , 723px 96px #A1B8D0 , 286px 393px #A1B8D0 , 184px 294px #A1B8D0 , 203px 987px #A1B8D0 , 273px 778px #A1B8D0 , 218px 982px #A1B8D0 , 145px 789px #A1B8D0 , 222px 432px #A1B8D0 , 274px 476px #A1B8D0 , 190px 63px #A1B8D0 , 980px 495px #A1B8D0 , 827px 570px #A1B8D0 , 628px 132px #A1B8D0 , 135px 207px #A1B8D0 , 513px 415px #A1B8D0 , 888px 61px #A1B8D0 , 246px 770px #A1B8D0 , 414px 281px #A1B8D0 , 735px 627px #A1B8D0 , 471px 432px #A1B8D0 , 592px 625px #A1B8D0 , 938px 835px #A1B8D0 , 252px 824px #A1B8D0 , 221px 518px #A1B8D0 , 44px 966px #A1B8D0 , 327px 964px #A1B8D0;
  }
  
  @-moz-keyframes glitter-4 {
    0%,
      100%,
      8.70968%,
      18.70968% {
      opacity: 0;
    }
    13.70968% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-4 {
    0%,
      100%,
      8.70968%,
      18.70968% {
      opacity: 0;
    }
    13.70968% {
      opacity: 1;
    }
  }
  @keyframes glitter-4 {
    0%,
      100%,
      8.70968%,
      18.70968% {
      opacity: 0;
    }
    13.70968% {
      opacity: 1;
    }
  }
  .glitter_4 {
    -moz-animation: glitter-4 10s infinite;
    -webkit-animation: glitter-4 10s infinite;
    animation: glitter-4 10s infinite;
    box-shadow: 961px 397px #A1B8D0 , 634px 979px #A1B8D0 , 772px 90px #A1B8D0 , 630px 232px #A1B8D0 , 855px 195px #A1B8D0 , 592px 558px #A1B8D0 , 867px 172px #A1B8D0 , 557px 557px #A1B8D0 , 763px 765px #A1B8D0 , 707px 835px #A1B8D0 , 886px 194px #A1B8D0 , 39px 540px #A1B8D0 , 830px 376px #A1B8D0 , 487px 473px #A1B8D0 , 156px 756px #A1B8D0 , 224px 322px #A1B8D0 , 448px 324px #A1B8D0 , 511px 180px #A1B8D0 , 977px 234px #A1B8D0 , 4px 768px #A1B8D0 , 29px 675px #A1B8D0 , 156px 58px #A1B8D0 , 364px 635px #A1B8D0 , 1px 683px #A1B8D0 , 136px 544px #A1B8D0 , 121px 602px #A1B8D0 , 509px 235px #A1B8D0 , 997px 789px #A1B8D0 , 782px 213px #A1B8D0 , 965px 937px #A1B8D0 , 651px 928px #A1B8D0 , 363px 89px #A1B8D0 , 124px 809px #A1B8D0 , 463px 188px #A1B8D0 , 111px 960px #A1B8D0 , 539px 25px #A1B8D0 , 611px 426px #A1B8D0 , 352px 853px #A1B8D0 , 753px 768px #A1B8D0 , 266px 908px #A1B8D0 , 572px 567px #A1B8D0 , 32px 543px #A1B8D0 , 413px 74px #A1B8D0 , 412px 694px #A1B8D0 , 385px 939px #A1B8D0 , 466px 489px #A1B8D0 , 70px 786px #A1B8D0 , 298px 116px #A1B8D0 , 702px 627px #A1B8D0 , 949px 347px #A1B8D0 , 710px 154px #A1B8D0 , 375px 868px #A1B8D0 , 911px 458px #A1B8D0 , 574px 998px #A1B8D0 , 569px 785px #A1B8D0 , 750px 1px #A1B8D0 , 248px 979px #A1B8D0 , 157px 779px #A1B8D0 , 534px 191px #A1B8D0 , 985px 18px #A1B8D0 , 707px 238px #A1B8D0 , 263px 870px #A1B8D0 , 52px 733px #A1B8D0 , 263px 152px #A1B8D0 , 40px 960px #A1B8D0 , 998px 576px #A1B8D0 , 173px 775px #A1B8D0 , 259px 683px #A1B8D0 , 959px 792px #A1B8D0 , 941px 94px #A1B8D0 , 486px 888px #A1B8D0 , 905px 183px #A1B8D0 , 307px 921px #A1B8D0 , 292px 947px #A1B8D0 , 534px 479px #A1B8D0 , 535px 774px #A1B8D0 , 136px 216px #A1B8D0 , 192px 911px #A1B8D0 , 265px 458px #A1B8D0 , 317px 169px #A1B8D0 , 764px 985px #A1B8D0 , 997px 544px #A1B8D0 , 284px 432px #A1B8D0 , 12px 502px #A1B8D0 , 350px 859px #A1B8D0 , 729px 966px #A1B8D0 , 679px 76px #A1B8D0 , 153px 577px #A1B8D0 , 297px 329px #A1B8D0 , 20px 642px #A1B8D0 , 154px 521px #A1B8D0 , 458px 579px #A1B8D0 , 116px 468px #A1B8D0 , 109px 346px #A1B8D0 , 182px 472px #A1B8D0 , 575px 119px #A1B8D0 , 882px 904px #A1B8D0 , 463px 172px #A1B8D0 , 379px 638px #A1B8D0 , 155px 319px #A1B8D0 , 810px 451px #A1B8D0 , 553px 623px #A1B8D0 , 388px 355px #A1B8D0 , 883px 542px #A1B8D0 , 713px 806px #A1B8D0 , 143px 279px #A1B8D0 , 672px 626px #A1B8D0 , 995px 710px #A1B8D0 , 303px 862px #A1B8D0 , 851px 966px #A1B8D0 , 257px 286px #A1B8D0 , 939px 55px #A1B8D0 , 503px 37px #A1B8D0 , 528px 595px #A1B8D0 , 867px 149px #A1B8D0 , 214px 560px #A1B8D0 , 755px 248px #A1B8D0 , 5px 698px #A1B8D0 , 808px 867px #A1B8D0 , 827px 188px #A1B8D0 , 503px 853px #A1B8D0 , 541px 318px #A1B8D0 , 384px 255px #A1B8D0 , 542px 211px #A1B8D0 , 317px 462px #A1B8D0 , 706px 929px #A1B8D0 , 380px 442px #A1B8D0 , 337px 466px #A1B8D0 , 134px 32px #A1B8D0 , 679px 605px #A1B8D0 , 681px 341px #A1B8D0 , 394px 757px #A1B8D0 , 615px 631px #A1B8D0 , 551px 907px #A1B8D0 , 878px 601px #A1B8D0 , 773px 847px #A1B8D0 , 755px 828px #A1B8D0 , 696px 584px #A1B8D0 , 227px 989px #A1B8D0 , 366px 41px #A1B8D0 , 428px 892px #A1B8D0 , 281px 661px #A1B8D0 , 259px 663px #A1B8D0 , 150px 847px #A1B8D0 , 487px 858px #A1B8D0 , 566px 696px #A1B8D0 , 968px 536px #A1B8D0 , 829px 212px #A1B8D0 , 328px 337px #A1B8D0 , 201px 745px #A1B8D0 , 469px 845px #A1B8D0 , 749px 878px #A1B8D0 , 993px 919px #A1B8D0 , 189px 592px #A1B8D0 , 649px 185px #A1B8D0 , 696px 936px #A1B8D0 , 517px 117px #A1B8D0 , 376px 923px #A1B8D0 , 220px 157px #A1B8D0 , 511px 682px #A1B8D0 , 83px 41px #A1B8D0 , 526px 33px #A1B8D0 , 772px 578px #A1B8D0 , 405px 965px #A1B8D0 , 421px 983px #A1B8D0 , 723px 25px #A1B8D0 , 380px 594px #A1B8D0 , 62px 848px #A1B8D0 , 708px 245px #A1B8D0 , 750px 294px #A1B8D0 , 91px 402px #A1B8D0 , 417px 751px #A1B8D0 , 658px 947px #A1B8D0 , 933px 478px #A1B8D0 , 991px 673px #A1B8D0 , 304px 661px #A1B8D0 , 716px 85px #A1B8D0 , 595px 757px #A1B8D0 , 177px 127px #A1B8D0 , 297px 351px #A1B8D0 , 273px 521px #A1B8D0 , 96px 88px #A1B8D0 , 416px 571px #A1B8D0 , 16px 130px #A1B8D0 , 515px 534px #A1B8D0 , 118px 789px #A1B8D0 , 961px 771px #A1B8D0 , 123px 509px #A1B8D0 , 818px 740px #A1B8D0 , 213px 584px #A1B8D0 , 583px 773px #A1B8D0 , 255px 599px #A1B8D0 , 12px 123px #A1B8D0 , 819px 686px #A1B8D0 , 792px 484px #A1B8D0 , 450px 847px #A1B8D0 , 3px 910px #A1B8D0 , 28px 54px #A1B8D0 , 9px 909px #A1B8D0 , 143px 507px #A1B8D0;
  }
  .glitter_4:before {
    -moz-animation: glitter-4 8s infinite;
    -webkit-animation: glitter-4 8s infinite;
    animation: glitter-4 8s infinite;
    box-shadow: 961px 397px #A1B8D0 , 634px 979px #A1B8D0 , 772px 90px #A1B8D0 , 630px 232px #A1B8D0 , 855px 195px #A1B8D0 , 592px 558px #A1B8D0 , 867px 172px #A1B8D0 , 557px 557px #A1B8D0 , 763px 765px #A1B8D0 , 707px 835px #A1B8D0 , 886px 194px #A1B8D0 , 39px 540px #A1B8D0 , 830px 376px #A1B8D0 , 487px 473px #A1B8D0 , 156px 756px #A1B8D0 , 224px 322px #A1B8D0 , 448px 324px #A1B8D0 , 511px 180px #A1B8D0 , 977px 234px #A1B8D0 , 4px 768px #A1B8D0 , 29px 675px #A1B8D0 , 156px 58px #A1B8D0 , 364px 635px #A1B8D0 , 1px 683px #A1B8D0 , 136px 544px #A1B8D0 , 121px 602px #A1B8D0 , 509px 235px #A1B8D0 , 997px 789px #A1B8D0 , 782px 213px #A1B8D0 , 965px 937px #A1B8D0 , 651px 928px #A1B8D0 , 363px 89px #A1B8D0 , 124px 809px #A1B8D0 , 463px 188px #A1B8D0 , 111px 960px #A1B8D0 , 539px 25px #A1B8D0 , 611px 426px #A1B8D0 , 352px 853px #A1B8D0 , 753px 768px #A1B8D0 , 266px 908px #A1B8D0 , 572px 567px #A1B8D0 , 32px 543px #A1B8D0 , 413px 74px #A1B8D0 , 412px 694px #A1B8D0 , 385px 939px #A1B8D0 , 466px 489px #A1B8D0 , 70px 786px #A1B8D0 , 298px 116px #A1B8D0 , 702px 627px #A1B8D0 , 949px 347px #A1B8D0 , 710px 154px #A1B8D0 , 375px 868px #A1B8D0 , 911px 458px #A1B8D0 , 574px 998px #A1B8D0 , 569px 785px #A1B8D0 , 750px 1px #A1B8D0 , 248px 979px #A1B8D0 , 157px 779px #A1B8D0 , 534px 191px #A1B8D0 , 985px 18px #A1B8D0 , 707px 238px #A1B8D0 , 263px 870px #A1B8D0 , 52px 733px #A1B8D0 , 263px 152px #A1B8D0 , 40px 960px #A1B8D0 , 998px 576px #A1B8D0 , 173px 775px #A1B8D0 , 259px 683px #A1B8D0 , 959px 792px #A1B8D0 , 941px 94px #A1B8D0 , 486px 888px #A1B8D0 , 905px 183px #A1B8D0 , 307px 921px #A1B8D0 , 292px 947px #A1B8D0 , 534px 479px #A1B8D0 , 535px 774px #A1B8D0 , 136px 216px #A1B8D0 , 192px 911px #A1B8D0 , 265px 458px #A1B8D0 , 317px 169px #A1B8D0 , 764px 985px #A1B8D0 , 997px 544px #A1B8D0 , 284px 432px #A1B8D0 , 12px 502px #A1B8D0 , 350px 859px #A1B8D0 , 729px 966px #A1B8D0 , 679px 76px #A1B8D0 , 153px 577px #A1B8D0 , 297px 329px #A1B8D0 , 20px 642px #A1B8D0 , 154px 521px #A1B8D0 , 458px 579px #A1B8D0 , 116px 468px #A1B8D0 , 109px 346px #A1B8D0 , 182px 472px #A1B8D0 , 575px 119px #A1B8D0 , 882px 904px #A1B8D0 , 463px 172px #A1B8D0 , 379px 638px #A1B8D0 , 155px 319px #A1B8D0 , 810px 451px #A1B8D0 , 553px 623px #A1B8D0 , 388px 355px #A1B8D0 , 883px 542px #A1B8D0 , 713px 806px #A1B8D0 , 143px 279px #A1B8D0 , 672px 626px #A1B8D0 , 995px 710px #A1B8D0 , 303px 862px #A1B8D0 , 851px 966px #A1B8D0 , 257px 286px #A1B8D0 , 939px 55px #A1B8D0 , 503px 37px #A1B8D0 , 528px 595px #A1B8D0 , 867px 149px #A1B8D0 , 214px 560px #A1B8D0 , 755px 248px #A1B8D0 , 5px 698px #A1B8D0 , 808px 867px #A1B8D0 , 827px 188px #A1B8D0 , 503px 853px #A1B8D0 , 541px 318px #A1B8D0 , 384px 255px #A1B8D0 , 542px 211px #A1B8D0 , 317px 462px #A1B8D0 , 706px 929px #A1B8D0 , 380px 442px #A1B8D0 , 337px 466px #A1B8D0 , 134px 32px #A1B8D0 , 679px 605px #A1B8D0 , 681px 341px #A1B8D0 , 394px 757px #A1B8D0 , 615px 631px #A1B8D0 , 551px 907px #A1B8D0 , 878px 601px #A1B8D0 , 773px 847px #A1B8D0 , 755px 828px #A1B8D0 , 696px 584px #A1B8D0 , 227px 989px #A1B8D0 , 366px 41px #A1B8D0 , 428px 892px #A1B8D0 , 281px 661px #A1B8D0 , 259px 663px #A1B8D0 , 150px 847px #A1B8D0 , 487px 858px #A1B8D0 , 566px 696px #A1B8D0 , 968px 536px #A1B8D0 , 829px 212px #A1B8D0 , 328px 337px #A1B8D0 , 201px 745px #A1B8D0 , 469px 845px #A1B8D0 , 749px 878px #A1B8D0 , 993px 919px #A1B8D0 , 189px 592px #A1B8D0 , 649px 185px #A1B8D0 , 696px 936px #A1B8D0 , 517px 117px #A1B8D0 , 376px 923px #A1B8D0 , 220px 157px #A1B8D0 , 511px 682px #A1B8D0 , 83px 41px #A1B8D0 , 526px 33px #A1B8D0 , 772px 578px #A1B8D0 , 405px 965px #A1B8D0 , 421px 983px #A1B8D0 , 723px 25px #A1B8D0 , 380px 594px #A1B8D0 , 62px 848px #A1B8D0 , 708px 245px #A1B8D0 , 750px 294px #A1B8D0 , 91px 402px #A1B8D0 , 417px 751px #A1B8D0 , 658px 947px #A1B8D0 , 933px 478px #A1B8D0 , 991px 673px #A1B8D0 , 304px 661px #A1B8D0 , 716px 85px #A1B8D0 , 595px 757px #A1B8D0 , 177px 127px #A1B8D0 , 297px 351px #A1B8D0 , 273px 521px #A1B8D0 , 96px 88px #A1B8D0 , 416px 571px #A1B8D0 , 16px 130px #A1B8D0 , 515px 534px #A1B8D0 , 118px 789px #A1B8D0 , 961px 771px #A1B8D0 , 123px 509px #A1B8D0 , 818px 740px #A1B8D0 , 213px 584px #A1B8D0 , 583px 773px #A1B8D0 , 255px 599px #A1B8D0 , 12px 123px #A1B8D0 , 819px 686px #A1B8D0 , 792px 484px #A1B8D0 , 450px 847px #A1B8D0 , 3px 910px #A1B8D0 , 28px 54px #A1B8D0 , 9px 909px #A1B8D0 , 143px 507px #A1B8D0;
  }
  .glitter_4:after {
    -moz-animation: glitter-4 9s infinite;
    -webkit-animation: glitter-4 9s infinite;
    animation: glitter-4 9s infinite;
    box-shadow: 961px 397px #A1B8D0 , 634px 979px #A1B8D0 , 772px 90px #A1B8D0 , 630px 232px #A1B8D0 , 855px 195px #A1B8D0 , 592px 558px #A1B8D0 , 867px 172px #A1B8D0 , 557px 557px #A1B8D0 , 763px 765px #A1B8D0 , 707px 835px #A1B8D0 , 886px 194px #A1B8D0 , 39px 540px #A1B8D0 , 830px 376px #A1B8D0 , 487px 473px #A1B8D0 , 156px 756px #A1B8D0 , 224px 322px #A1B8D0 , 448px 324px #A1B8D0 , 511px 180px #A1B8D0 , 977px 234px #A1B8D0 , 4px 768px #A1B8D0 , 29px 675px #A1B8D0 , 156px 58px #A1B8D0 , 364px 635px #A1B8D0 , 1px 683px #A1B8D0 , 136px 544px #A1B8D0 , 121px 602px #A1B8D0 , 509px 235px #A1B8D0 , 997px 789px #A1B8D0 , 782px 213px #A1B8D0 , 965px 937px #A1B8D0 , 651px 928px #A1B8D0 , 363px 89px #A1B8D0 , 124px 809px #A1B8D0 , 463px 188px #A1B8D0 , 111px 960px #A1B8D0 , 539px 25px #A1B8D0 , 611px 426px #A1B8D0 , 352px 853px #A1B8D0 , 753px 768px #A1B8D0 , 266px 908px #A1B8D0 , 572px 567px #A1B8D0 , 32px 543px #A1B8D0 , 413px 74px #A1B8D0 , 412px 694px #A1B8D0 , 385px 939px #A1B8D0 , 466px 489px #A1B8D0 , 70px 786px #A1B8D0 , 298px 116px #A1B8D0 , 702px 627px #A1B8D0 , 949px 347px #A1B8D0 , 710px 154px #A1B8D0 , 375px 868px #A1B8D0 , 911px 458px #A1B8D0 , 574px 998px #A1B8D0 , 569px 785px #A1B8D0 , 750px 1px #A1B8D0 , 248px 979px #A1B8D0 , 157px 779px #A1B8D0 , 534px 191px #A1B8D0 , 985px 18px #A1B8D0 , 707px 238px #A1B8D0 , 263px 870px #A1B8D0 , 52px 733px #A1B8D0 , 263px 152px #A1B8D0 , 40px 960px #A1B8D0 , 998px 576px #A1B8D0 , 173px 775px #A1B8D0 , 259px 683px #A1B8D0 , 959px 792px #A1B8D0 , 941px 94px #A1B8D0 , 486px 888px #A1B8D0 , 905px 183px #A1B8D0 , 307px 921px #A1B8D0 , 292px 947px #A1B8D0 , 534px 479px #A1B8D0 , 535px 774px #A1B8D0 , 136px 216px #A1B8D0 , 192px 911px #A1B8D0 , 265px 458px #A1B8D0 , 317px 169px #A1B8D0 , 764px 985px #A1B8D0 , 997px 544px #A1B8D0 , 284px 432px #A1B8D0 , 12px 502px #A1B8D0 , 350px 859px #A1B8D0 , 729px 966px #A1B8D0 , 679px 76px #A1B8D0 , 153px 577px #A1B8D0 , 297px 329px #A1B8D0 , 20px 642px #A1B8D0 , 154px 521px #A1B8D0 , 458px 579px #A1B8D0 , 116px 468px #A1B8D0 , 109px 346px #A1B8D0 , 182px 472px #A1B8D0 , 575px 119px #A1B8D0 , 882px 904px #A1B8D0 , 463px 172px #A1B8D0 , 379px 638px #A1B8D0 , 155px 319px #A1B8D0 , 810px 451px #A1B8D0 , 553px 623px #A1B8D0 , 388px 355px #A1B8D0 , 883px 542px #A1B8D0 , 713px 806px #A1B8D0 , 143px 279px #A1B8D0 , 672px 626px #A1B8D0 , 995px 710px #A1B8D0 , 303px 862px #A1B8D0 , 851px 966px #A1B8D0 , 257px 286px #A1B8D0 , 939px 55px #A1B8D0 , 503px 37px #A1B8D0 , 528px 595px #A1B8D0 , 867px 149px #A1B8D0 , 214px 560px #A1B8D0 , 755px 248px #A1B8D0 , 5px 698px #A1B8D0 , 808px 867px #A1B8D0 , 827px 188px #A1B8D0 , 503px 853px #A1B8D0 , 541px 318px #A1B8D0 , 384px 255px #A1B8D0 , 542px 211px #A1B8D0 , 317px 462px #A1B8D0 , 706px 929px #A1B8D0 , 380px 442px #A1B8D0 , 337px 466px #A1B8D0 , 134px 32px #A1B8D0 , 679px 605px #A1B8D0 , 681px 341px #A1B8D0 , 394px 757px #A1B8D0 , 615px 631px #A1B8D0 , 551px 907px #A1B8D0 , 878px 601px #A1B8D0 , 773px 847px #A1B8D0 , 755px 828px #A1B8D0 , 696px 584px #A1B8D0 , 227px 989px #A1B8D0 , 366px 41px #A1B8D0 , 428px 892px #A1B8D0 , 281px 661px #A1B8D0 , 259px 663px #A1B8D0 , 150px 847px #A1B8D0 , 487px 858px #A1B8D0 , 566px 696px #A1B8D0 , 968px 536px #A1B8D0 , 829px 212px #A1B8D0 , 328px 337px #A1B8D0 , 201px 745px #A1B8D0 , 469px 845px #A1B8D0 , 749px 878px #A1B8D0 , 993px 919px #A1B8D0 , 189px 592px #A1B8D0 , 649px 185px #A1B8D0 , 696px 936px #A1B8D0 , 517px 117px #A1B8D0 , 376px 923px #A1B8D0 , 220px 157px #A1B8D0 , 511px 682px #A1B8D0 , 83px 41px #A1B8D0 , 526px 33px #A1B8D0 , 772px 578px #A1B8D0 , 405px 965px #A1B8D0 , 421px 983px #A1B8D0 , 723px 25px #A1B8D0 , 380px 594px #A1B8D0 , 62px 848px #A1B8D0 , 708px 245px #A1B8D0 , 750px 294px #A1B8D0 , 91px 402px #A1B8D0 , 417px 751px #A1B8D0 , 658px 947px #A1B8D0 , 933px 478px #A1B8D0 , 991px 673px #A1B8D0 , 304px 661px #A1B8D0 , 716px 85px #A1B8D0 , 595px 757px #A1B8D0 , 177px 127px #A1B8D0 , 297px 351px #A1B8D0 , 273px 521px #A1B8D0 , 96px 88px #A1B8D0 , 416px 571px #A1B8D0 , 16px 130px #A1B8D0 , 515px 534px #A1B8D0 , 118px 789px #A1B8D0 , 961px 771px #A1B8D0 , 123px 509px #A1B8D0 , 818px 740px #A1B8D0 , 213px 584px #A1B8D0 , 583px 773px #A1B8D0 , 255px 599px #A1B8D0 , 12px 123px #A1B8D0 , 819px 686px #A1B8D0 , 792px 484px #A1B8D0 , 450px 847px #A1B8D0 , 3px 910px #A1B8D0 , 28px 54px #A1B8D0 , 9px 909px #A1B8D0 , 143px 507px #A1B8D0;
  }
  
  @-moz-keyframes glitter-5 {
    0%,
      100%,
      11.6129%,
      21.6129% {
      opacity: 0;
    }
    16.6129% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-5 {
    0%,
      100%,
      11.6129%,
      21.6129% {
      opacity: 0;
    }
    16.6129% {
      opacity: 1;
    }
  }
  @keyframes glitter-5 {
    0%,
      100%,
      11.6129%,
      21.6129% {
      opacity: 0;
    }
    16.6129% {
      opacity: 1;
    }
  }
  .glitter_5 {
    -moz-animation: glitter-5 10s infinite;
    -webkit-animation: glitter-5 10s infinite;
    animation: glitter-5 10s infinite;
    box-shadow: 326px 581px #A1B8D0 , 119px 471px #A1B8D0 , 488px 196px #A1B8D0 , 197px 991px #A1B8D0 , 991px 89px #A1B8D0 , 305px 858px #A1B8D0 , 347px 463px #A1B8D0 , 985px 583px #A1B8D0 , 289px 57px #A1B8D0 , 452px 727px #A1B8D0 , 177px 483px #A1B8D0 , 517px 560px #A1B8D0 , 250px 471px #A1B8D0 , 749px 72px #A1B8D0 , 114px 52px #A1B8D0 , 947px 348px #A1B8D0 , 371px 377px #A1B8D0 , 936px 426px #A1B8D0 , 800px 969px #A1B8D0 , 75px 34px #A1B8D0 , 160px 807px #A1B8D0 , 626px 694px #A1B8D0 , 575px 890px #A1B8D0 , 274px 787px #A1B8D0 , 297px 742px #A1B8D0 , 628px 864px #A1B8D0 , 27px 790px #A1B8D0 , 883px 471px #A1B8D0 , 988px 179px #A1B8D0 , 837px 11px #A1B8D0 , 961px 293px #A1B8D0 , 838px 634px #A1B8D0 , 75px 687px #A1B8D0 , 211px 581px #A1B8D0 , 854px 120px #A1B8D0 , 498px 895px #A1B8D0 , 679px 153px #A1B8D0 , 231px 534px #A1B8D0 , 2px 759px #A1B8D0 , 663px 720px #A1B8D0 , 247px 120px #A1B8D0 , 134px 231px #A1B8D0 , 148px 35px #A1B8D0 , 625px 603px #A1B8D0 , 411px 138px #A1B8D0 , 409px 855px #A1B8D0 , 474px 818px #A1B8D0 , 192px 884px #A1B8D0 , 14px 744px #A1B8D0 , 331px 647px #A1B8D0 , 185px 139px #A1B8D0 , 298px 690px #A1B8D0 , 356px 775px #A1B8D0 , 269px 381px #A1B8D0 , 182px 542px #A1B8D0 , 501px 410px #A1B8D0 , 153px 968px #A1B8D0 , 411px 104px #A1B8D0 , 286px 746px #A1B8D0 , 614px 559px #A1B8D0 , 477px 703px #A1B8D0 , 214px 776px #A1B8D0 , 436px 895px #A1B8D0 , 217px 971px #A1B8D0 , 156px 624px #A1B8D0 , 908px 298px #A1B8D0 , 460px 701px #A1B8D0 , 667px 716px #A1B8D0 , 499px 377px #A1B8D0 , 204px 692px #A1B8D0 , 256px 548px #A1B8D0 , 154px 943px #A1B8D0 , 185px 943px #A1B8D0 , 477px 515px #A1B8D0 , 168px 585px #A1B8D0 , 185px 280px #A1B8D0 , 491px 508px #A1B8D0 , 505px 642px #A1B8D0 , 684px 496px #A1B8D0 , 639px 809px #A1B8D0 , 457px 827px #A1B8D0 , 16px 1px #A1B8D0 , 428px 3px #A1B8D0 , 154px 492px #A1B8D0 , 559px 869px #A1B8D0 , 47px 69px #A1B8D0 , 643px 602px #A1B8D0 , 965px 247px #A1B8D0 , 261px 872px #A1B8D0 , 53px 704px #A1B8D0 , 442px 725px #A1B8D0 , 559px 601px #A1B8D0 , 420px 213px #A1B8D0 , 698px 434px #A1B8D0 , 642px 121px #A1B8D0 , 855px 734px #A1B8D0 , 180px 81px #A1B8D0 , 513px 981px #A1B8D0 , 515px 221px #A1B8D0 , 608px 883px #A1B8D0 , 415px 288px #A1B8D0 , 946px 976px #A1B8D0 , 498px 711px #A1B8D0 , 620px 151px #A1B8D0 , 369px 391px #A1B8D0 , 381px 198px #A1B8D0 , 66px 475px #A1B8D0 , 409px 393px #A1B8D0 , 606px 117px #A1B8D0 , 307px 3px #A1B8D0 , 605px 170px #A1B8D0 , 531px 955px #A1B8D0 , 542px 156px #A1B8D0 , 731px 224px #A1B8D0 , 360px 980px #A1B8D0 , 359px 171px #A1B8D0 , 802px 576px #A1B8D0 , 706px 916px #A1B8D0 , 787px 680px #A1B8D0 , 419px 428px #A1B8D0 , 571px 195px #A1B8D0 , 833px 557px #A1B8D0 , 244px 39px #A1B8D0 , 151px 817px #A1B8D0 , 538px 652px #A1B8D0 , 6px 141px #A1B8D0 , 508px 495px #A1B8D0 , 789px 949px #A1B8D0 , 321px 5px #A1B8D0 , 155px 581px #A1B8D0 , 921px 858px #A1B8D0 , 811px 351px #A1B8D0 , 486px 737px #A1B8D0 , 983px 449px #A1B8D0 , 24px 602px #A1B8D0 , 640px 592px #A1B8D0 , 868px 256px #A1B8D0 , 663px 699px #A1B8D0 , 103px 137px #A1B8D0 , 588px 37px #A1B8D0 , 841px 285px #A1B8D0 , 573px 766px #A1B8D0 , 171px 228px #A1B8D0 , 92px 820px #A1B8D0 , 752px 341px #A1B8D0 , 206px 285px #A1B8D0 , 305px 853px #A1B8D0 , 140px 928px #A1B8D0 , 824px 526px #A1B8D0 , 956px 559px #A1B8D0 , 249px 164px #A1B8D0 , 596px 972px #A1B8D0 , 642px 605px #A1B8D0 , 443px 636px #A1B8D0 , 251px 832px #A1B8D0 , 537px 511px #A1B8D0 , 947px 324px #A1B8D0 , 47px 354px #A1B8D0 , 77px 763px #A1B8D0 , 355px 210px #A1B8D0 , 45px 724px #A1B8D0 , 916px 934px #A1B8D0 , 135px 974px #A1B8D0 , 460px 897px #A1B8D0 , 348px 614px #A1B8D0 , 354px 9px #A1B8D0 , 325px 350px #A1B8D0 , 32px 375px #A1B8D0 , 297px 47px #A1B8D0 , 565px 762px #A1B8D0 , 117px 161px #A1B8D0 , 347px 707px #A1B8D0 , 946px 391px #A1B8D0 , 466px 197px #A1B8D0 , 113px 13px #A1B8D0 , 456px 334px #A1B8D0 , 560px 38px #A1B8D0 , 202px 101px #A1B8D0 , 229px 986px #A1B8D0 , 449px 612px #A1B8D0 , 162px 122px #A1B8D0 , 965px 566px #A1B8D0 , 54px 21px #A1B8D0 , 626px 195px #A1B8D0 , 860px 798px #A1B8D0 , 229px 234px #A1B8D0 , 304px 974px #A1B8D0 , 814px 963px #A1B8D0 , 474px 151px #A1B8D0 , 12px 423px #A1B8D0 , 435px 417px #A1B8D0 , 232px 468px #A1B8D0 , 757px 998px #A1B8D0 , 557px 458px #A1B8D0 , 129px 538px #A1B8D0 , 893px 302px #A1B8D0 , 117px 831px #A1B8D0 , 523px 399px #A1B8D0 , 121px 395px #A1B8D0 , 211px 162px #A1B8D0;
  }
  .glitter_5:before {
    -moz-animation: glitter-5 8s infinite;
    -webkit-animation: glitter-5 8s infinite;
    animation: glitter-5 8s infinite;
    box-shadow: 326px 581px #A1B8D0 , 119px 471px #A1B8D0 , 488px 196px #A1B8D0 , 197px 991px #A1B8D0 , 991px 89px #A1B8D0 , 305px 858px #A1B8D0 , 347px 463px #A1B8D0 , 985px 583px #A1B8D0 , 289px 57px #A1B8D0 , 452px 727px #A1B8D0 , 177px 483px #A1B8D0 , 517px 560px #A1B8D0 , 250px 471px #A1B8D0 , 749px 72px #A1B8D0 , 114px 52px #A1B8D0 , 947px 348px #A1B8D0 , 371px 377px #A1B8D0 , 936px 426px #A1B8D0 , 800px 969px #A1B8D0 , 75px 34px #A1B8D0 , 160px 807px #A1B8D0 , 626px 694px #A1B8D0 , 575px 890px #A1B8D0 , 274px 787px #A1B8D0 , 297px 742px #A1B8D0 , 628px 864px #A1B8D0 , 27px 790px #A1B8D0 , 883px 471px #A1B8D0 , 988px 179px #A1B8D0 , 837px 11px #A1B8D0 , 961px 293px #A1B8D0 , 838px 634px #A1B8D0 , 75px 687px #A1B8D0 , 211px 581px #A1B8D0 , 854px 120px #A1B8D0 , 498px 895px #A1B8D0 , 679px 153px #A1B8D0 , 231px 534px #A1B8D0 , 2px 759px #A1B8D0 , 663px 720px #A1B8D0 , 247px 120px #A1B8D0 , 134px 231px #A1B8D0 , 148px 35px #A1B8D0 , 625px 603px #A1B8D0 , 411px 138px #A1B8D0 , 409px 855px #A1B8D0 , 474px 818px #A1B8D0 , 192px 884px #A1B8D0 , 14px 744px #A1B8D0 , 331px 647px #A1B8D0 , 185px 139px #A1B8D0 , 298px 690px #A1B8D0 , 356px 775px #A1B8D0 , 269px 381px #A1B8D0 , 182px 542px #A1B8D0 , 501px 410px #A1B8D0 , 153px 968px #A1B8D0 , 411px 104px #A1B8D0 , 286px 746px #A1B8D0 , 614px 559px #A1B8D0 , 477px 703px #A1B8D0 , 214px 776px #A1B8D0 , 436px 895px #A1B8D0 , 217px 971px #A1B8D0 , 156px 624px #A1B8D0 , 908px 298px #A1B8D0 , 460px 701px #A1B8D0 , 667px 716px #A1B8D0 , 499px 377px #A1B8D0 , 204px 692px #A1B8D0 , 256px 548px #A1B8D0 , 154px 943px #A1B8D0 , 185px 943px #A1B8D0 , 477px 515px #A1B8D0 , 168px 585px #A1B8D0 , 185px 280px #A1B8D0 , 491px 508px #A1B8D0 , 505px 642px #A1B8D0 , 684px 496px #A1B8D0 , 639px 809px #A1B8D0 , 457px 827px #A1B8D0 , 16px 1px #A1B8D0 , 428px 3px #A1B8D0 , 154px 492px #A1B8D0 , 559px 869px #A1B8D0 , 47px 69px #A1B8D0 , 643px 602px #A1B8D0 , 965px 247px #A1B8D0 , 261px 872px #A1B8D0 , 53px 704px #A1B8D0 , 442px 725px #A1B8D0 , 559px 601px #A1B8D0 , 420px 213px #A1B8D0 , 698px 434px #A1B8D0 , 642px 121px #A1B8D0 , 855px 734px #A1B8D0 , 180px 81px #A1B8D0 , 513px 981px #A1B8D0 , 515px 221px #A1B8D0 , 608px 883px #A1B8D0 , 415px 288px #A1B8D0 , 946px 976px #A1B8D0 , 498px 711px #A1B8D0 , 620px 151px #A1B8D0 , 369px 391px #A1B8D0 , 381px 198px #A1B8D0 , 66px 475px #A1B8D0 , 409px 393px #A1B8D0 , 606px 117px #A1B8D0 , 307px 3px #A1B8D0 , 605px 170px #A1B8D0 , 531px 955px #A1B8D0 , 542px 156px #A1B8D0 , 731px 224px #A1B8D0 , 360px 980px #A1B8D0 , 359px 171px #A1B8D0 , 802px 576px #A1B8D0 , 706px 916px #A1B8D0 , 787px 680px #A1B8D0 , 419px 428px #A1B8D0 , 571px 195px #A1B8D0 , 833px 557px #A1B8D0 , 244px 39px #A1B8D0 , 151px 817px #A1B8D0 , 538px 652px #A1B8D0 , 6px 141px #A1B8D0 , 508px 495px #A1B8D0 , 789px 949px #A1B8D0 , 321px 5px #A1B8D0 , 155px 581px #A1B8D0 , 921px 858px #A1B8D0 , 811px 351px #A1B8D0 , 486px 737px #A1B8D0 , 983px 449px #A1B8D0 , 24px 602px #A1B8D0 , 640px 592px #A1B8D0 , 868px 256px #A1B8D0 , 663px 699px #A1B8D0 , 103px 137px #A1B8D0 , 588px 37px #A1B8D0 , 841px 285px #A1B8D0 , 573px 766px #A1B8D0 , 171px 228px #A1B8D0 , 92px 820px #A1B8D0 , 752px 341px #A1B8D0 , 206px 285px #A1B8D0 , 305px 853px #A1B8D0 , 140px 928px #A1B8D0 , 824px 526px #A1B8D0 , 956px 559px #A1B8D0 , 249px 164px #A1B8D0 , 596px 972px #A1B8D0 , 642px 605px #A1B8D0 , 443px 636px #A1B8D0 , 251px 832px #A1B8D0 , 537px 511px #A1B8D0 , 947px 324px #A1B8D0 , 47px 354px #A1B8D0 , 77px 763px #A1B8D0 , 355px 210px #A1B8D0 , 45px 724px #A1B8D0 , 916px 934px #A1B8D0 , 135px 974px #A1B8D0 , 460px 897px #A1B8D0 , 348px 614px #A1B8D0 , 354px 9px #A1B8D0 , 325px 350px #A1B8D0 , 32px 375px #A1B8D0 , 297px 47px #A1B8D0 , 565px 762px #A1B8D0 , 117px 161px #A1B8D0 , 347px 707px #A1B8D0 , 946px 391px #A1B8D0 , 466px 197px #A1B8D0 , 113px 13px #A1B8D0 , 456px 334px #A1B8D0 , 560px 38px #A1B8D0 , 202px 101px #A1B8D0 , 229px 986px #A1B8D0 , 449px 612px #A1B8D0 , 162px 122px #A1B8D0 , 965px 566px #A1B8D0 , 54px 21px #A1B8D0 , 626px 195px #A1B8D0 , 860px 798px #A1B8D0 , 229px 234px #A1B8D0 , 304px 974px #A1B8D0 , 814px 963px #A1B8D0 , 474px 151px #A1B8D0 , 12px 423px #A1B8D0 , 435px 417px #A1B8D0 , 232px 468px #A1B8D0 , 757px 998px #A1B8D0 , 557px 458px #A1B8D0 , 129px 538px #A1B8D0 , 893px 302px #A1B8D0 , 117px 831px #A1B8D0 , 523px 399px #A1B8D0 , 121px 395px #A1B8D0 , 211px 162px #A1B8D0;
  }
  .glitter_5:after {
    -moz-animation: glitter-5 9s infinite;
    -webkit-animation: glitter-5 9s infinite;
    animation: glitter-5 9s infinite;
    box-shadow: 326px 581px #A1B8D0 , 119px 471px #A1B8D0 , 488px 196px #A1B8D0 , 197px 991px #A1B8D0 , 991px 89px #A1B8D0 , 305px 858px #A1B8D0 , 347px 463px #A1B8D0 , 985px 583px #A1B8D0 , 289px 57px #A1B8D0 , 452px 727px #A1B8D0 , 177px 483px #A1B8D0 , 517px 560px #A1B8D0 , 250px 471px #A1B8D0 , 749px 72px #A1B8D0 , 114px 52px #A1B8D0 , 947px 348px #A1B8D0 , 371px 377px #A1B8D0 , 936px 426px #A1B8D0 , 800px 969px #A1B8D0 , 75px 34px #A1B8D0 , 160px 807px #A1B8D0 , 626px 694px #A1B8D0 , 575px 890px #A1B8D0 , 274px 787px #A1B8D0 , 297px 742px #A1B8D0 , 628px 864px #A1B8D0 , 27px 790px #A1B8D0 , 883px 471px #A1B8D0 , 988px 179px #A1B8D0 , 837px 11px #A1B8D0 , 961px 293px #A1B8D0 , 838px 634px #A1B8D0 , 75px 687px #A1B8D0 , 211px 581px #A1B8D0 , 854px 120px #A1B8D0 , 498px 895px #A1B8D0 , 679px 153px #A1B8D0 , 231px 534px #A1B8D0 , 2px 759px #A1B8D0 , 663px 720px #A1B8D0 , 247px 120px #A1B8D0 , 134px 231px #A1B8D0 , 148px 35px #A1B8D0 , 625px 603px #A1B8D0 , 411px 138px #A1B8D0 , 409px 855px #A1B8D0 , 474px 818px #A1B8D0 , 192px 884px #A1B8D0 , 14px 744px #A1B8D0 , 331px 647px #A1B8D0 , 185px 139px #A1B8D0 , 298px 690px #A1B8D0 , 356px 775px #A1B8D0 , 269px 381px #A1B8D0 , 182px 542px #A1B8D0 , 501px 410px #A1B8D0 , 153px 968px #A1B8D0 , 411px 104px #A1B8D0 , 286px 746px #A1B8D0 , 614px 559px #A1B8D0 , 477px 703px #A1B8D0 , 214px 776px #A1B8D0 , 436px 895px #A1B8D0 , 217px 971px #A1B8D0 , 156px 624px #A1B8D0 , 908px 298px #A1B8D0 , 460px 701px #A1B8D0 , 667px 716px #A1B8D0 , 499px 377px #A1B8D0 , 204px 692px #A1B8D0 , 256px 548px #A1B8D0 , 154px 943px #A1B8D0 , 185px 943px #A1B8D0 , 477px 515px #A1B8D0 , 168px 585px #A1B8D0 , 185px 280px #A1B8D0 , 491px 508px #A1B8D0 , 505px 642px #A1B8D0 , 684px 496px #A1B8D0 , 639px 809px #A1B8D0 , 457px 827px #A1B8D0 , 16px 1px #A1B8D0 , 428px 3px #A1B8D0 , 154px 492px #A1B8D0 , 559px 869px #A1B8D0 , 47px 69px #A1B8D0 , 643px 602px #A1B8D0 , 965px 247px #A1B8D0 , 261px 872px #A1B8D0 , 53px 704px #A1B8D0 , 442px 725px #A1B8D0 , 559px 601px #A1B8D0 , 420px 213px #A1B8D0 , 698px 434px #A1B8D0 , 642px 121px #A1B8D0 , 855px 734px #A1B8D0 , 180px 81px #A1B8D0 , 513px 981px #A1B8D0 , 515px 221px #A1B8D0 , 608px 883px #A1B8D0 , 415px 288px #A1B8D0 , 946px 976px #A1B8D0 , 498px 711px #A1B8D0 , 620px 151px #A1B8D0 , 369px 391px #A1B8D0 , 381px 198px #A1B8D0 , 66px 475px #A1B8D0 , 409px 393px #A1B8D0 , 606px 117px #A1B8D0 , 307px 3px #A1B8D0 , 605px 170px #A1B8D0 , 531px 955px #A1B8D0 , 542px 156px #A1B8D0 , 731px 224px #A1B8D0 , 360px 980px #A1B8D0 , 359px 171px #A1B8D0 , 802px 576px #A1B8D0 , 706px 916px #A1B8D0 , 787px 680px #A1B8D0 , 419px 428px #A1B8D0 , 571px 195px #A1B8D0 , 833px 557px #A1B8D0 , 244px 39px #A1B8D0 , 151px 817px #A1B8D0 , 538px 652px #A1B8D0 , 6px 141px #A1B8D0 , 508px 495px #A1B8D0 , 789px 949px #A1B8D0 , 321px 5px #A1B8D0 , 155px 581px #A1B8D0 , 921px 858px #A1B8D0 , 811px 351px #A1B8D0 , 486px 737px #A1B8D0 , 983px 449px #A1B8D0 , 24px 602px #A1B8D0 , 640px 592px #A1B8D0 , 868px 256px #A1B8D0 , 663px 699px #A1B8D0 , 103px 137px #A1B8D0 , 588px 37px #A1B8D0 , 841px 285px #A1B8D0 , 573px 766px #A1B8D0 , 171px 228px #A1B8D0 , 92px 820px #A1B8D0 , 752px 341px #A1B8D0 , 206px 285px #A1B8D0 , 305px 853px #A1B8D0 , 140px 928px #A1B8D0 , 824px 526px #A1B8D0 , 956px 559px #A1B8D0 , 249px 164px #A1B8D0 , 596px 972px #A1B8D0 , 642px 605px #A1B8D0 , 443px 636px #A1B8D0 , 251px 832px #A1B8D0 , 537px 511px #A1B8D0 , 947px 324px #A1B8D0 , 47px 354px #A1B8D0 , 77px 763px #A1B8D0 , 355px 210px #A1B8D0 , 45px 724px #A1B8D0 , 916px 934px #A1B8D0 , 135px 974px #A1B8D0 , 460px 897px #A1B8D0 , 348px 614px #A1B8D0 , 354px 9px #A1B8D0 , 325px 350px #A1B8D0 , 32px 375px #A1B8D0 , 297px 47px #A1B8D0 , 565px 762px #A1B8D0 , 117px 161px #A1B8D0 , 347px 707px #A1B8D0 , 946px 391px #A1B8D0 , 466px 197px #A1B8D0 , 113px 13px #A1B8D0 , 456px 334px #A1B8D0 , 560px 38px #A1B8D0 , 202px 101px #A1B8D0 , 229px 986px #A1B8D0 , 449px 612px #A1B8D0 , 162px 122px #A1B8D0 , 965px 566px #A1B8D0 , 54px 21px #A1B8D0 , 626px 195px #A1B8D0 , 860px 798px #A1B8D0 , 229px 234px #A1B8D0 , 304px 974px #A1B8D0 , 814px 963px #A1B8D0 , 474px 151px #A1B8D0 , 12px 423px #A1B8D0 , 435px 417px #A1B8D0 , 232px 468px #A1B8D0 , 757px 998px #A1B8D0 , 557px 458px #A1B8D0 , 129px 538px #A1B8D0 , 893px 302px #A1B8D0 , 117px 831px #A1B8D0 , 523px 399px #A1B8D0 , 121px 395px #A1B8D0 , 211px 162px #A1B8D0;
  }
  
  @-moz-keyframes glitter-6 {
    0%,
      100%,
      14.51613%,
      24.51613% {
      opacity: 0;
    }
    19.51613% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-6 {
    0%,
      100%,
      14.51613%,
      24.51613% {
      opacity: 0;
    }
    19.51613% {
      opacity: 1;
    }
  }
  @keyframes glitter-6 {
    0%,
      100%,
      14.51613%,
      24.51613% {
      opacity: 0;
    }
    19.51613% {
      opacity: 1;
    }
  }
  .glitter_6 {
    -moz-animation: glitter-6 10s infinite;
    -webkit-animation: glitter-6 10s infinite;
    animation: glitter-6 10s infinite;
    box-shadow: 496px 999px #A1B8D0 , 177px 59px #A1B8D0 , 807px 825px #A1B8D0 , 113px 424px #A1B8D0 , 436px 834px #A1B8D0 , 16px 656px #A1B8D0 , 885px 833px #A1B8D0 , 778px 379px #A1B8D0 , 680px 448px #A1B8D0 , 296px 898px #A1B8D0 , 433px 351px #A1B8D0 , 706px 352px #A1B8D0 , 39px 654px #A1B8D0 , 739px 534px #A1B8D0 , 961px 912px #A1B8D0 , 391px 837px #A1B8D0 , 309px 534px #A1B8D0 , 994px 703px #A1B8D0 , 646px 778px #A1B8D0 , 609px 753px #A1B8D0 , 745px 96px #A1B8D0 , 140px 20px #A1B8D0 , 55px 531px #A1B8D0 , 818px 97px #A1B8D0 , 923px 585px #A1B8D0 , 378px 443px #A1B8D0 , 626px 790px #A1B8D0 , 594px 813px #A1B8D0 , 237px 415px #A1B8D0 , 660px 974px #A1B8D0 , 645px 502px #A1B8D0 , 955px 403px #A1B8D0 , 597px 292px #A1B8D0 , 384px 71px #A1B8D0 , 896px 265px #A1B8D0 , 419px 691px #A1B8D0 , 1000px 852px #A1B8D0 , 817px 21px #A1B8D0 , 27px 688px #A1B8D0 , 191px 341px #A1B8D0 , 949px 147px #A1B8D0 , 739px 880px #A1B8D0 , 779px 307px #A1B8D0 , 188px 752px #A1B8D0 , 507px 732px #A1B8D0 , 284px 761px #A1B8D0 , 76px 666px #A1B8D0 , 468px 159px #A1B8D0 , 789px 156px #A1B8D0 , 639px 226px #A1B8D0 , 854px 746px #A1B8D0 , 565px 220px #A1B8D0 , 741px 226px #A1B8D0 , 975px 867px #A1B8D0 , 505px 205px #A1B8D0 , 653px 318px #A1B8D0 , 325px 317px #A1B8D0 , 858px 965px #A1B8D0 , 72px 341px #A1B8D0 , 176px 286px #A1B8D0 , 828px 582px #A1B8D0 , 684px 846px #A1B8D0 , 211px 973px #A1B8D0 , 394px 550px #A1B8D0 , 136px 716px #A1B8D0 , 3px 37px #A1B8D0 , 4px 160px #A1B8D0 , 125px 774px #A1B8D0 , 551px 990px #A1B8D0 , 379px 6px #A1B8D0 , 981px 674px #A1B8D0 , 418px 543px #A1B8D0 , 758px 626px #A1B8D0 , 92px 178px #A1B8D0 , 300px 410px #A1B8D0 , 746px 759px #A1B8D0 , 443px 840px #A1B8D0 , 596px 532px #A1B8D0 , 905px 193px #A1B8D0 , 998px 326px #A1B8D0 , 123px 622px #A1B8D0 , 117px 976px #A1B8D0 , 382px 605px #A1B8D0 , 74px 267px #A1B8D0 , 362px 890px #A1B8D0 , 222px 207px #A1B8D0 , 716px 156px #A1B8D0 , 477px 419px #A1B8D0 , 724px 989px #A1B8D0 , 394px 854px #A1B8D0 , 605px 845px #A1B8D0 , 761px 619px #A1B8D0 , 8px 534px #A1B8D0 , 551px 818px #A1B8D0 , 54px 750px #A1B8D0 , 724px 736px #A1B8D0 , 783px 670px #A1B8D0 , 689px 71px #A1B8D0 , 724px 269px #A1B8D0 , 618px 134px #A1B8D0 , 334px 637px #A1B8D0 , 192px 647px #A1B8D0 , 379px 757px #A1B8D0 , 140px 126px #A1B8D0 , 996px 786px #A1B8D0 , 146px 722px #A1B8D0 , 883px 753px #A1B8D0 , 10px 619px #A1B8D0 , 728px 809px #A1B8D0 , 448px 102px #A1B8D0 , 708px 184px #A1B8D0 , 492px 354px #A1B8D0 , 745px 658px #A1B8D0 , 502px 500px #A1B8D0 , 836px 692px #A1B8D0 , 503px 244px #A1B8D0 , 842px 204px #A1B8D0 , 781px 595px #A1B8D0 , 723px 331px #A1B8D0 , 390px 466px #A1B8D0 , 531px 705px #A1B8D0 , 261px 353px #A1B8D0 , 902px 637px #A1B8D0 , 897px 657px #A1B8D0 , 726px 583px #A1B8D0 , 685px 908px #A1B8D0 , 660px 395px #A1B8D0 , 477px 564px #A1B8D0 , 514px 697px #A1B8D0 , 111px 750px #A1B8D0 , 351px 639px #A1B8D0 , 913px 671px #A1B8D0 , 439px 891px #A1B8D0 , 681px 479px #A1B8D0 , 487px 477px #A1B8D0 , 389px 416px #A1B8D0 , 145px 866px #A1B8D0 , 339px 994px #A1B8D0 , 497px 248px #A1B8D0 , 396px 817px #A1B8D0 , 408px 233px #A1B8D0 , 143px 403px #A1B8D0 , 326px 984px #A1B8D0 , 574px 493px #A1B8D0 , 814px 674px #A1B8D0 , 332px 960px #A1B8D0 , 250px 635px #A1B8D0 , 296px 17px #A1B8D0 , 982px 114px #A1B8D0 , 635px 149px #A1B8D0 , 62px 177px #A1B8D0 , 400px 728px #A1B8D0 , 762px 777px #A1B8D0 , 238px 696px #A1B8D0 , 600px 127px #A1B8D0 , 141px 866px #A1B8D0 , 942px 502px #A1B8D0 , 600px 408px #A1B8D0 , 963px 490px #A1B8D0 , 77px 334px #A1B8D0 , 659px 255px #A1B8D0 , 343px 325px #A1B8D0 , 937px 639px #A1B8D0 , 916px 1px #A1B8D0 , 247px 413px #A1B8D0 , 885px 739px #A1B8D0 , 343px 613px #A1B8D0 , 457px 105px #A1B8D0 , 737px 623px #A1B8D0 , 325px 842px #A1B8D0 , 552px 846px #A1B8D0 , 617px 724px #A1B8D0 , 712px 483px #A1B8D0 , 535px 389px #A1B8D0 , 65px 793px #A1B8D0 , 994px 502px #A1B8D0 , 158px 947px #A1B8D0 , 163px 993px #A1B8D0 , 160px 482px #A1B8D0 , 89px 85px #A1B8D0 , 337px 591px #A1B8D0 , 205px 587px #A1B8D0 , 690px 181px #A1B8D0 , 818px 918px #A1B8D0 , 647px 66px #A1B8D0 , 349px 929px #A1B8D0 , 11px 91px #A1B8D0 , 583px 515px #A1B8D0 , 864px 832px #A1B8D0 , 28px 694px #A1B8D0 , 129px 723px #A1B8D0 , 329px 580px #A1B8D0 , 267px 741px #A1B8D0 , 291px 119px #A1B8D0 , 926px 827px #A1B8D0 , 152px 523px #A1B8D0 , 574px 560px #A1B8D0 , 890px 216px #A1B8D0 , 811px 417px #A1B8D0 , 373px 708px #A1B8D0;
  }
  .glitter_6:before {
    -moz-animation: glitter-6 8s infinite;
    -webkit-animation: glitter-6 8s infinite;
    animation: glitter-6 8s infinite;
    box-shadow: 496px 999px #A1B8D0 , 177px 59px #A1B8D0 , 807px 825px #A1B8D0 , 113px 424px #A1B8D0 , 436px 834px #A1B8D0 , 16px 656px #A1B8D0 , 885px 833px #A1B8D0 , 778px 379px #A1B8D0 , 680px 448px #A1B8D0 , 296px 898px #A1B8D0 , 433px 351px #A1B8D0 , 706px 352px #A1B8D0 , 39px 654px #A1B8D0 , 739px 534px #A1B8D0 , 961px 912px #A1B8D0 , 391px 837px #A1B8D0 , 309px 534px #A1B8D0 , 994px 703px #A1B8D0 , 646px 778px #A1B8D0 , 609px 753px #A1B8D0 , 745px 96px #A1B8D0 , 140px 20px #A1B8D0 , 55px 531px #A1B8D0 , 818px 97px #A1B8D0 , 923px 585px #A1B8D0 , 378px 443px #A1B8D0 , 626px 790px #A1B8D0 , 594px 813px #A1B8D0 , 237px 415px #A1B8D0 , 660px 974px #A1B8D0 , 645px 502px #A1B8D0 , 955px 403px #A1B8D0 , 597px 292px #A1B8D0 , 384px 71px #A1B8D0 , 896px 265px #A1B8D0 , 419px 691px #A1B8D0 , 1000px 852px #A1B8D0 , 817px 21px #A1B8D0 , 27px 688px #A1B8D0 , 191px 341px #A1B8D0 , 949px 147px #A1B8D0 , 739px 880px #A1B8D0 , 779px 307px #A1B8D0 , 188px 752px #A1B8D0 , 507px 732px #A1B8D0 , 284px 761px #A1B8D0 , 76px 666px #A1B8D0 , 468px 159px #A1B8D0 , 789px 156px #A1B8D0 , 639px 226px #A1B8D0 , 854px 746px #A1B8D0 , 565px 220px #A1B8D0 , 741px 226px #A1B8D0 , 975px 867px #A1B8D0 , 505px 205px #A1B8D0 , 653px 318px #A1B8D0 , 325px 317px #A1B8D0 , 858px 965px #A1B8D0 , 72px 341px #A1B8D0 , 176px 286px #A1B8D0 , 828px 582px #A1B8D0 , 684px 846px #A1B8D0 , 211px 973px #A1B8D0 , 394px 550px #A1B8D0 , 136px 716px #A1B8D0 , 3px 37px #A1B8D0 , 4px 160px #A1B8D0 , 125px 774px #A1B8D0 , 551px 990px #A1B8D0 , 379px 6px #A1B8D0 , 981px 674px #A1B8D0 , 418px 543px #A1B8D0 , 758px 626px #A1B8D0 , 92px 178px #A1B8D0 , 300px 410px #A1B8D0 , 746px 759px #A1B8D0 , 443px 840px #A1B8D0 , 596px 532px #A1B8D0 , 905px 193px #A1B8D0 , 998px 326px #A1B8D0 , 123px 622px #A1B8D0 , 117px 976px #A1B8D0 , 382px 605px #A1B8D0 , 74px 267px #A1B8D0 , 362px 890px #A1B8D0 , 222px 207px #A1B8D0 , 716px 156px #A1B8D0 , 477px 419px #A1B8D0 , 724px 989px #A1B8D0 , 394px 854px #A1B8D0 , 605px 845px #A1B8D0 , 761px 619px #A1B8D0 , 8px 534px #A1B8D0 , 551px 818px #A1B8D0 , 54px 750px #A1B8D0 , 724px 736px #A1B8D0 , 783px 670px #A1B8D0 , 689px 71px #A1B8D0 , 724px 269px #A1B8D0 , 618px 134px #A1B8D0 , 334px 637px #A1B8D0 , 192px 647px #A1B8D0 , 379px 757px #A1B8D0 , 140px 126px #A1B8D0 , 996px 786px #A1B8D0 , 146px 722px #A1B8D0 , 883px 753px #A1B8D0 , 10px 619px #A1B8D0 , 728px 809px #A1B8D0 , 448px 102px #A1B8D0 , 708px 184px #A1B8D0 , 492px 354px #A1B8D0 , 745px 658px #A1B8D0 , 502px 500px #A1B8D0 , 836px 692px #A1B8D0 , 503px 244px #A1B8D0 , 842px 204px #A1B8D0 , 781px 595px #A1B8D0 , 723px 331px #A1B8D0 , 390px 466px #A1B8D0 , 531px 705px #A1B8D0 , 261px 353px #A1B8D0 , 902px 637px #A1B8D0 , 897px 657px #A1B8D0 , 726px 583px #A1B8D0 , 685px 908px #A1B8D0 , 660px 395px #A1B8D0 , 477px 564px #A1B8D0 , 514px 697px #A1B8D0 , 111px 750px #A1B8D0 , 351px 639px #A1B8D0 , 913px 671px #A1B8D0 , 439px 891px #A1B8D0 , 681px 479px #A1B8D0 , 487px 477px #A1B8D0 , 389px 416px #A1B8D0 , 145px 866px #A1B8D0 , 339px 994px #A1B8D0 , 497px 248px #A1B8D0 , 396px 817px #A1B8D0 , 408px 233px #A1B8D0 , 143px 403px #A1B8D0 , 326px 984px #A1B8D0 , 574px 493px #A1B8D0 , 814px 674px #A1B8D0 , 332px 960px #A1B8D0 , 250px 635px #A1B8D0 , 296px 17px #A1B8D0 , 982px 114px #A1B8D0 , 635px 149px #A1B8D0 , 62px 177px #A1B8D0 , 400px 728px #A1B8D0 , 762px 777px #A1B8D0 , 238px 696px #A1B8D0 , 600px 127px #A1B8D0 , 141px 866px #A1B8D0 , 942px 502px #A1B8D0 , 600px 408px #A1B8D0 , 963px 490px #A1B8D0 , 77px 334px #A1B8D0 , 659px 255px #A1B8D0 , 343px 325px #A1B8D0 , 937px 639px #A1B8D0 , 916px 1px #A1B8D0 , 247px 413px #A1B8D0 , 885px 739px #A1B8D0 , 343px 613px #A1B8D0 , 457px 105px #A1B8D0 , 737px 623px #A1B8D0 , 325px 842px #A1B8D0 , 552px 846px #A1B8D0 , 617px 724px #A1B8D0 , 712px 483px #A1B8D0 , 535px 389px #A1B8D0 , 65px 793px #A1B8D0 , 994px 502px #A1B8D0 , 158px 947px #A1B8D0 , 163px 993px #A1B8D0 , 160px 482px #A1B8D0 , 89px 85px #A1B8D0 , 337px 591px #A1B8D0 , 205px 587px #A1B8D0 , 690px 181px #A1B8D0 , 818px 918px #A1B8D0 , 647px 66px #A1B8D0 , 349px 929px #A1B8D0 , 11px 91px #A1B8D0 , 583px 515px #A1B8D0 , 864px 832px #A1B8D0 , 28px 694px #A1B8D0 , 129px 723px #A1B8D0 , 329px 580px #A1B8D0 , 267px 741px #A1B8D0 , 291px 119px #A1B8D0 , 926px 827px #A1B8D0 , 152px 523px #A1B8D0 , 574px 560px #A1B8D0 , 890px 216px #A1B8D0 , 811px 417px #A1B8D0 , 373px 708px #A1B8D0;
  }
  .glitter_6:after {
    -moz-animation: glitter-6 9s infinite;
    -webkit-animation: glitter-6 9s infinite;
    animation: glitter-6 9s infinite;
    box-shadow: 496px 999px #A1B8D0 , 177px 59px #A1B8D0 , 807px 825px #A1B8D0 , 113px 424px #A1B8D0 , 436px 834px #A1B8D0 , 16px 656px #A1B8D0 , 885px 833px #A1B8D0 , 778px 379px #A1B8D0 , 680px 448px #A1B8D0 , 296px 898px #A1B8D0 , 433px 351px #A1B8D0 , 706px 352px #A1B8D0 , 39px 654px #A1B8D0 , 739px 534px #A1B8D0 , 961px 912px #A1B8D0 , 391px 837px #A1B8D0 , 309px 534px #A1B8D0 , 994px 703px #A1B8D0 , 646px 778px #A1B8D0 , 609px 753px #A1B8D0 , 745px 96px #A1B8D0 , 140px 20px #A1B8D0 , 55px 531px #A1B8D0 , 818px 97px #A1B8D0 , 923px 585px #A1B8D0 , 378px 443px #A1B8D0 , 626px 790px #A1B8D0 , 594px 813px #A1B8D0 , 237px 415px #A1B8D0 , 660px 974px #A1B8D0 , 645px 502px #A1B8D0 , 955px 403px #A1B8D0 , 597px 292px #A1B8D0 , 384px 71px #A1B8D0 , 896px 265px #A1B8D0 , 419px 691px #A1B8D0 , 1000px 852px #A1B8D0 , 817px 21px #A1B8D0 , 27px 688px #A1B8D0 , 191px 341px #A1B8D0 , 949px 147px #A1B8D0 , 739px 880px #A1B8D0 , 779px 307px #A1B8D0 , 188px 752px #A1B8D0 , 507px 732px #A1B8D0 , 284px 761px #A1B8D0 , 76px 666px #A1B8D0 , 468px 159px #A1B8D0 , 789px 156px #A1B8D0 , 639px 226px #A1B8D0 , 854px 746px #A1B8D0 , 565px 220px #A1B8D0 , 741px 226px #A1B8D0 , 975px 867px #A1B8D0 , 505px 205px #A1B8D0 , 653px 318px #A1B8D0 , 325px 317px #A1B8D0 , 858px 965px #A1B8D0 , 72px 341px #A1B8D0 , 176px 286px #A1B8D0 , 828px 582px #A1B8D0 , 684px 846px #A1B8D0 , 211px 973px #A1B8D0 , 394px 550px #A1B8D0 , 136px 716px #A1B8D0 , 3px 37px #A1B8D0 , 4px 160px #A1B8D0 , 125px 774px #A1B8D0 , 551px 990px #A1B8D0 , 379px 6px #A1B8D0 , 981px 674px #A1B8D0 , 418px 543px #A1B8D0 , 758px 626px #A1B8D0 , 92px 178px #A1B8D0 , 300px 410px #A1B8D0 , 746px 759px #A1B8D0 , 443px 840px #A1B8D0 , 596px 532px #A1B8D0 , 905px 193px #A1B8D0 , 998px 326px #A1B8D0 , 123px 622px #A1B8D0 , 117px 976px #A1B8D0 , 382px 605px #A1B8D0 , 74px 267px #A1B8D0 , 362px 890px #A1B8D0 , 222px 207px #A1B8D0 , 716px 156px #A1B8D0 , 477px 419px #A1B8D0 , 724px 989px #A1B8D0 , 394px 854px #A1B8D0 , 605px 845px #A1B8D0 , 761px 619px #A1B8D0 , 8px 534px #A1B8D0 , 551px 818px #A1B8D0 , 54px 750px #A1B8D0 , 724px 736px #A1B8D0 , 783px 670px #A1B8D0 , 689px 71px #A1B8D0 , 724px 269px #A1B8D0 , 618px 134px #A1B8D0 , 334px 637px #A1B8D0 , 192px 647px #A1B8D0 , 379px 757px #A1B8D0 , 140px 126px #A1B8D0 , 996px 786px #A1B8D0 , 146px 722px #A1B8D0 , 883px 753px #A1B8D0 , 10px 619px #A1B8D0 , 728px 809px #A1B8D0 , 448px 102px #A1B8D0 , 708px 184px #A1B8D0 , 492px 354px #A1B8D0 , 745px 658px #A1B8D0 , 502px 500px #A1B8D0 , 836px 692px #A1B8D0 , 503px 244px #A1B8D0 , 842px 204px #A1B8D0 , 781px 595px #A1B8D0 , 723px 331px #A1B8D0 , 390px 466px #A1B8D0 , 531px 705px #A1B8D0 , 261px 353px #A1B8D0 , 902px 637px #A1B8D0 , 897px 657px #A1B8D0 , 726px 583px #A1B8D0 , 685px 908px #A1B8D0 , 660px 395px #A1B8D0 , 477px 564px #A1B8D0 , 514px 697px #A1B8D0 , 111px 750px #A1B8D0 , 351px 639px #A1B8D0 , 913px 671px #A1B8D0 , 439px 891px #A1B8D0 , 681px 479px #A1B8D0 , 487px 477px #A1B8D0 , 389px 416px #A1B8D0 , 145px 866px #A1B8D0 , 339px 994px #A1B8D0 , 497px 248px #A1B8D0 , 396px 817px #A1B8D0 , 408px 233px #A1B8D0 , 143px 403px #A1B8D0 , 326px 984px #A1B8D0 , 574px 493px #A1B8D0 , 814px 674px #A1B8D0 , 332px 960px #A1B8D0 , 250px 635px #A1B8D0 , 296px 17px #A1B8D0 , 982px 114px #A1B8D0 , 635px 149px #A1B8D0 , 62px 177px #A1B8D0 , 400px 728px #A1B8D0 , 762px 777px #A1B8D0 , 238px 696px #A1B8D0 , 600px 127px #A1B8D0 , 141px 866px #A1B8D0 , 942px 502px #A1B8D0 , 600px 408px #A1B8D0 , 963px 490px #A1B8D0 , 77px 334px #A1B8D0 , 659px 255px #A1B8D0 , 343px 325px #A1B8D0 , 937px 639px #A1B8D0 , 916px 1px #A1B8D0 , 247px 413px #A1B8D0 , 885px 739px #A1B8D0 , 343px 613px #A1B8D0 , 457px 105px #A1B8D0 , 737px 623px #A1B8D0 , 325px 842px #A1B8D0 , 552px 846px #A1B8D0 , 617px 724px #A1B8D0 , 712px 483px #A1B8D0 , 535px 389px #A1B8D0 , 65px 793px #A1B8D0 , 994px 502px #A1B8D0 , 158px 947px #A1B8D0 , 163px 993px #A1B8D0 , 160px 482px #A1B8D0 , 89px 85px #A1B8D0 , 337px 591px #A1B8D0 , 205px 587px #A1B8D0 , 690px 181px #A1B8D0 , 818px 918px #A1B8D0 , 647px 66px #A1B8D0 , 349px 929px #A1B8D0 , 11px 91px #A1B8D0 , 583px 515px #A1B8D0 , 864px 832px #A1B8D0 , 28px 694px #A1B8D0 , 129px 723px #A1B8D0 , 329px 580px #A1B8D0 , 267px 741px #A1B8D0 , 291px 119px #A1B8D0 , 926px 827px #A1B8D0 , 152px 523px #A1B8D0 , 574px 560px #A1B8D0 , 890px 216px #A1B8D0 , 811px 417px #A1B8D0 , 373px 708px #A1B8D0;
  }
  
  @-moz-keyframes glitter-7 {
    0%,
      100%,
      17.41935%,
      27.41935% {
      opacity: 0;
    }
    22.41935% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-7 {
    0%,
      100%,
      17.41935%,
      27.41935% {
      opacity: 0;
    }
    22.41935% {
      opacity: 1;
    }
  }
  @keyframes glitter-7 {
    0%,
      100%,
      17.41935%,
      27.41935% {
      opacity: 0;
    }
    22.41935% {
      opacity: 1;
    }
  }
  .glitter_7 {
    -moz-animation: glitter-7 10s infinite;
    -webkit-animation: glitter-7 10s infinite;
    animation: glitter-7 10s infinite;
    box-shadow: 547px 782px #A1B8D0 , 625px 11px #A1B8D0 , 895px 997px #A1B8D0 , 357px 687px #A1B8D0 , 689px 271px #A1B8D0 , 938px 298px #A1B8D0 , 392px 116px #A1B8D0 , 627px 778px #A1B8D0 , 472px 186px #A1B8D0 , 983px 665px #A1B8D0 , 545px 136px #A1B8D0 , 306px 817px #A1B8D0 , 974px 154px #A1B8D0 , 739px 905px #A1B8D0 , 273px 288px #A1B8D0 , 101px 759px #A1B8D0 , 42px 43px #A1B8D0 , 226px 821px #A1B8D0 , 464px 401px #A1B8D0 , 408px 976px #A1B8D0 , 505px 679px #A1B8D0 , 451px 925px #A1B8D0 , 406px 48px #A1B8D0 , 900px 320px #A1B8D0 , 464px 471px #A1B8D0 , 639px 790px #A1B8D0 , 227px 623px #A1B8D0 , 372px 185px #A1B8D0 , 680px 981px #A1B8D0 , 666px 565px #A1B8D0 , 429px 150px #A1B8D0 , 972px 962px #A1B8D0 , 872px 174px #A1B8D0 , 891px 772px #A1B8D0 , 119px 470px #A1B8D0 , 143px 354px #A1B8D0 , 866px 838px #A1B8D0 , 795px 450px #A1B8D0 , 260px 152px #A1B8D0 , 316px 392px #A1B8D0 , 103px 511px #A1B8D0 , 292px 884px #A1B8D0 , 398px 45px #A1B8D0 , 180px 376px #A1B8D0 , 156px 613px #A1B8D0 , 404px 407px #A1B8D0 , 437px 536px #A1B8D0 , 768px 288px #A1B8D0 , 467px 233px #A1B8D0 , 675px 349px #A1B8D0 , 361px 501px #A1B8D0 , 501px 518px #A1B8D0 , 206px 895px #A1B8D0 , 437px 497px #A1B8D0 , 218px 586px #A1B8D0 , 409px 582px #A1B8D0 , 541px 503px #A1B8D0 , 283px 50px #A1B8D0 , 336px 165px #A1B8D0 , 342px 136px #A1B8D0 , 858px 329px #A1B8D0 , 451px 316px #A1B8D0 , 710px 680px #A1B8D0 , 409px 801px #A1B8D0 , 930px 793px #A1B8D0 , 560px 340px #A1B8D0 , 822px 905px #A1B8D0 , 68px 907px #A1B8D0 , 168px 165px #A1B8D0 , 39px 926px #A1B8D0 , 241px 133px #A1B8D0 , 217px 998px #A1B8D0 , 466px 660px #A1B8D0 , 380px 583px #A1B8D0 , 994px 760px #A1B8D0 , 829px 743px #A1B8D0 , 815px 109px #A1B8D0 , 437px 170px #A1B8D0 , 160px 658px #A1B8D0 , 461px 950px #A1B8D0 , 682px 355px #A1B8D0 , 221px 932px #A1B8D0 , 479px 1000px #A1B8D0 , 474px 454px #A1B8D0 , 78px 953px #A1B8D0 , 749px 68px #A1B8D0 , 140px 23px #A1B8D0 , 313px 639px #A1B8D0 , 243px 896px #A1B8D0 , 643px 62px #A1B8D0 , 9px 438px #A1B8D0 , 297px 335px #A1B8D0 , 624px 172px #A1B8D0 , 926px 977px #A1B8D0 , 761px 230px #A1B8D0 , 105px 681px #A1B8D0 , 814px 795px #A1B8D0 , 973px 326px #A1B8D0 , 695px 404px #A1B8D0 , 731px 278px #A1B8D0 , 341px 446px #A1B8D0 , 224px 691px #A1B8D0 , 491px 593px #A1B8D0 , 126px 49px #A1B8D0 , 356px 298px #A1B8D0 , 613px 342px #A1B8D0 , 919px 409px #A1B8D0 , 829px 155px #A1B8D0 , 198px 540px #A1B8D0 , 423px 803px #A1B8D0 , 766px 369px #A1B8D0 , 27px 225px #A1B8D0 , 291px 569px #A1B8D0 , 843px 735px #A1B8D0 , 461px 793px #A1B8D0 , 36px 700px #A1B8D0 , 658px 412px #A1B8D0 , 373px 192px #A1B8D0 , 141px 326px #A1B8D0 , 814px 408px #A1B8D0 , 719px 888px #A1B8D0 , 42px 88px #A1B8D0 , 928px 538px #A1B8D0 , 620px 518px #A1B8D0 , 836px 790px #A1B8D0 , 855px 845px #A1B8D0 , 713px 368px #A1B8D0 , 11px 741px #A1B8D0 , 982px 668px #A1B8D0 , 181px 840px #A1B8D0 , 801px 582px #A1B8D0 , 505px 570px #A1B8D0 , 531px 536px #A1B8D0 , 59px 949px #A1B8D0 , 450px 855px #A1B8D0 , 621px 219px #A1B8D0 , 721px 459px #A1B8D0 , 410px 333px #A1B8D0 , 849px 246px #A1B8D0 , 762px 449px #A1B8D0 , 780px 847px #A1B8D0 , 318px 366px #A1B8D0 , 988px 628px #A1B8D0 , 910px 524px #A1B8D0 , 279px 963px #A1B8D0 , 562px 238px #A1B8D0 , 69px 451px #A1B8D0 , 452px 928px #A1B8D0 , 337px 948px #A1B8D0 , 470px 615px #A1B8D0 , 473px 880px #A1B8D0 , 293px 2px #A1B8D0 , 653px 468px #A1B8D0 , 784px 352px #A1B8D0 , 535px 428px #A1B8D0 , 983px 167px #A1B8D0 , 520px 690px #A1B8D0 , 334px 369px #A1B8D0 , 663px 723px #A1B8D0 , 95px 215px #A1B8D0 , 876px 189px #A1B8D0 , 971px 729px #A1B8D0 , 594px 387px #A1B8D0 , 610px 277px #A1B8D0 , 667px 112px #A1B8D0 , 898px 737px #A1B8D0 , 61px 359px #A1B8D0 , 848px 772px #A1B8D0 , 695px 367px #A1B8D0 , 227px 793px #A1B8D0 , 421px 935px #A1B8D0 , 664px 982px #A1B8D0 , 635px 329px #A1B8D0 , 227px 486px #A1B8D0 , 534px 796px #A1B8D0 , 445px 655px #A1B8D0 , 327px 951px #A1B8D0 , 5px 206px #A1B8D0 , 63px 938px #A1B8D0 , 147px 340px #A1B8D0 , 294px 913px #A1B8D0 , 157px 773px #A1B8D0 , 871px 641px #A1B8D0 , 870px 776px #A1B8D0 , 935px 707px #A1B8D0 , 743px 979px #A1B8D0 , 978px 396px #A1B8D0 , 431px 212px #A1B8D0 , 117px 733px #A1B8D0 , 621px 842px #A1B8D0 , 593px 575px #A1B8D0 , 566px 970px #A1B8D0 , 526px 175px #A1B8D0 , 468px 434px #A1B8D0 , 288px 40px #A1B8D0 , 139px 711px #A1B8D0 , 994px 177px #A1B8D0 , 999px 474px #A1B8D0 , 858px 898px #A1B8D0 , 269px 612px #A1B8D0;
  }
  .glitter_7:before {
    -moz-animation: glitter-7 8s infinite;
    -webkit-animation: glitter-7 8s infinite;
    animation: glitter-7 8s infinite;
    box-shadow: 547px 782px #A1B8D0 , 625px 11px #A1B8D0 , 895px 997px #A1B8D0 , 357px 687px #A1B8D0 , 689px 271px #A1B8D0 , 938px 298px #A1B8D0 , 392px 116px #A1B8D0 , 627px 778px #A1B8D0 , 472px 186px #A1B8D0 , 983px 665px #A1B8D0 , 545px 136px #A1B8D0 , 306px 817px #A1B8D0 , 974px 154px #A1B8D0 , 739px 905px #A1B8D0 , 273px 288px #A1B8D0 , 101px 759px #A1B8D0 , 42px 43px #A1B8D0 , 226px 821px #A1B8D0 , 464px 401px #A1B8D0 , 408px 976px #A1B8D0 , 505px 679px #A1B8D0 , 451px 925px #A1B8D0 , 406px 48px #A1B8D0 , 900px 320px #A1B8D0 , 464px 471px #A1B8D0 , 639px 790px #A1B8D0 , 227px 623px #A1B8D0 , 372px 185px #A1B8D0 , 680px 981px #A1B8D0 , 666px 565px #A1B8D0 , 429px 150px #A1B8D0 , 972px 962px #A1B8D0 , 872px 174px #A1B8D0 , 891px 772px #A1B8D0 , 119px 470px #A1B8D0 , 143px 354px #A1B8D0 , 866px 838px #A1B8D0 , 795px 450px #A1B8D0 , 260px 152px #A1B8D0 , 316px 392px #A1B8D0 , 103px 511px #A1B8D0 , 292px 884px #A1B8D0 , 398px 45px #A1B8D0 , 180px 376px #A1B8D0 , 156px 613px #A1B8D0 , 404px 407px #A1B8D0 , 437px 536px #A1B8D0 , 768px 288px #A1B8D0 , 467px 233px #A1B8D0 , 675px 349px #A1B8D0 , 361px 501px #A1B8D0 , 501px 518px #A1B8D0 , 206px 895px #A1B8D0 , 437px 497px #A1B8D0 , 218px 586px #A1B8D0 , 409px 582px #A1B8D0 , 541px 503px #A1B8D0 , 283px 50px #A1B8D0 , 336px 165px #A1B8D0 , 342px 136px #A1B8D0 , 858px 329px #A1B8D0 , 451px 316px #A1B8D0 , 710px 680px #A1B8D0 , 409px 801px #A1B8D0 , 930px 793px #A1B8D0 , 560px 340px #A1B8D0 , 822px 905px #A1B8D0 , 68px 907px #A1B8D0 , 168px 165px #A1B8D0 , 39px 926px #A1B8D0 , 241px 133px #A1B8D0 , 217px 998px #A1B8D0 , 466px 660px #A1B8D0 , 380px 583px #A1B8D0 , 994px 760px #A1B8D0 , 829px 743px #A1B8D0 , 815px 109px #A1B8D0 , 437px 170px #A1B8D0 , 160px 658px #A1B8D0 , 461px 950px #A1B8D0 , 682px 355px #A1B8D0 , 221px 932px #A1B8D0 , 479px 1000px #A1B8D0 , 474px 454px #A1B8D0 , 78px 953px #A1B8D0 , 749px 68px #A1B8D0 , 140px 23px #A1B8D0 , 313px 639px #A1B8D0 , 243px 896px #A1B8D0 , 643px 62px #A1B8D0 , 9px 438px #A1B8D0 , 297px 335px #A1B8D0 , 624px 172px #A1B8D0 , 926px 977px #A1B8D0 , 761px 230px #A1B8D0 , 105px 681px #A1B8D0 , 814px 795px #A1B8D0 , 973px 326px #A1B8D0 , 695px 404px #A1B8D0 , 731px 278px #A1B8D0 , 341px 446px #A1B8D0 , 224px 691px #A1B8D0 , 491px 593px #A1B8D0 , 126px 49px #A1B8D0 , 356px 298px #A1B8D0 , 613px 342px #A1B8D0 , 919px 409px #A1B8D0 , 829px 155px #A1B8D0 , 198px 540px #A1B8D0 , 423px 803px #A1B8D0 , 766px 369px #A1B8D0 , 27px 225px #A1B8D0 , 291px 569px #A1B8D0 , 843px 735px #A1B8D0 , 461px 793px #A1B8D0 , 36px 700px #A1B8D0 , 658px 412px #A1B8D0 , 373px 192px #A1B8D0 , 141px 326px #A1B8D0 , 814px 408px #A1B8D0 , 719px 888px #A1B8D0 , 42px 88px #A1B8D0 , 928px 538px #A1B8D0 , 620px 518px #A1B8D0 , 836px 790px #A1B8D0 , 855px 845px #A1B8D0 , 713px 368px #A1B8D0 , 11px 741px #A1B8D0 , 982px 668px #A1B8D0 , 181px 840px #A1B8D0 , 801px 582px #A1B8D0 , 505px 570px #A1B8D0 , 531px 536px #A1B8D0 , 59px 949px #A1B8D0 , 450px 855px #A1B8D0 , 621px 219px #A1B8D0 , 721px 459px #A1B8D0 , 410px 333px #A1B8D0 , 849px 246px #A1B8D0 , 762px 449px #A1B8D0 , 780px 847px #A1B8D0 , 318px 366px #A1B8D0 , 988px 628px #A1B8D0 , 910px 524px #A1B8D0 , 279px 963px #A1B8D0 , 562px 238px #A1B8D0 , 69px 451px #A1B8D0 , 452px 928px #A1B8D0 , 337px 948px #A1B8D0 , 470px 615px #A1B8D0 , 473px 880px #A1B8D0 , 293px 2px #A1B8D0 , 653px 468px #A1B8D0 , 784px 352px #A1B8D0 , 535px 428px #A1B8D0 , 983px 167px #A1B8D0 , 520px 690px #A1B8D0 , 334px 369px #A1B8D0 , 663px 723px #A1B8D0 , 95px 215px #A1B8D0 , 876px 189px #A1B8D0 , 971px 729px #A1B8D0 , 594px 387px #A1B8D0 , 610px 277px #A1B8D0 , 667px 112px #A1B8D0 , 898px 737px #A1B8D0 , 61px 359px #A1B8D0 , 848px 772px #A1B8D0 , 695px 367px #A1B8D0 , 227px 793px #A1B8D0 , 421px 935px #A1B8D0 , 664px 982px #A1B8D0 , 635px 329px #A1B8D0 , 227px 486px #A1B8D0 , 534px 796px #A1B8D0 , 445px 655px #A1B8D0 , 327px 951px #A1B8D0 , 5px 206px #A1B8D0 , 63px 938px #A1B8D0 , 147px 340px #A1B8D0 , 294px 913px #A1B8D0 , 157px 773px #A1B8D0 , 871px 641px #A1B8D0 , 870px 776px #A1B8D0 , 935px 707px #A1B8D0 , 743px 979px #A1B8D0 , 978px 396px #A1B8D0 , 431px 212px #A1B8D0 , 117px 733px #A1B8D0 , 621px 842px #A1B8D0 , 593px 575px #A1B8D0 , 566px 970px #A1B8D0 , 526px 175px #A1B8D0 , 468px 434px #A1B8D0 , 288px 40px #A1B8D0 , 139px 711px #A1B8D0 , 994px 177px #A1B8D0 , 999px 474px #A1B8D0 , 858px 898px #A1B8D0 , 269px 612px #A1B8D0;
  }
  .glitter_7:after {
    -moz-animation: glitter-7 9s infinite;
    -webkit-animation: glitter-7 9s infinite;
    animation: glitter-7 9s infinite;
    box-shadow: 547px 782px #A1B8D0 , 625px 11px #A1B8D0 , 895px 997px #A1B8D0 , 357px 687px #A1B8D0 , 689px 271px #A1B8D0 , 938px 298px #A1B8D0 , 392px 116px #A1B8D0 , 627px 778px #A1B8D0 , 472px 186px #A1B8D0 , 983px 665px #A1B8D0 , 545px 136px #A1B8D0 , 306px 817px #A1B8D0 , 974px 154px #A1B8D0 , 739px 905px #A1B8D0 , 273px 288px #A1B8D0 , 101px 759px #A1B8D0 , 42px 43px #A1B8D0 , 226px 821px #A1B8D0 , 464px 401px #A1B8D0 , 408px 976px #A1B8D0 , 505px 679px #A1B8D0 , 451px 925px #A1B8D0 , 406px 48px #A1B8D0 , 900px 320px #A1B8D0 , 464px 471px #A1B8D0 , 639px 790px #A1B8D0 , 227px 623px #A1B8D0 , 372px 185px #A1B8D0 , 680px 981px #A1B8D0 , 666px 565px #A1B8D0 , 429px 150px #A1B8D0 , 972px 962px #A1B8D0 , 872px 174px #A1B8D0 , 891px 772px #A1B8D0 , 119px 470px #A1B8D0 , 143px 354px #A1B8D0 , 866px 838px #A1B8D0 , 795px 450px #A1B8D0 , 260px 152px #A1B8D0 , 316px 392px #A1B8D0 , 103px 511px #A1B8D0 , 292px 884px #A1B8D0 , 398px 45px #A1B8D0 , 180px 376px #A1B8D0 , 156px 613px #A1B8D0 , 404px 407px #A1B8D0 , 437px 536px #A1B8D0 , 768px 288px #A1B8D0 , 467px 233px #A1B8D0 , 675px 349px #A1B8D0 , 361px 501px #A1B8D0 , 501px 518px #A1B8D0 , 206px 895px #A1B8D0 , 437px 497px #A1B8D0 , 218px 586px #A1B8D0 , 409px 582px #A1B8D0 , 541px 503px #A1B8D0 , 283px 50px #A1B8D0 , 336px 165px #A1B8D0 , 342px 136px #A1B8D0 , 858px 329px #A1B8D0 , 451px 316px #A1B8D0 , 710px 680px #A1B8D0 , 409px 801px #A1B8D0 , 930px 793px #A1B8D0 , 560px 340px #A1B8D0 , 822px 905px #A1B8D0 , 68px 907px #A1B8D0 , 168px 165px #A1B8D0 , 39px 926px #A1B8D0 , 241px 133px #A1B8D0 , 217px 998px #A1B8D0 , 466px 660px #A1B8D0 , 380px 583px #A1B8D0 , 994px 760px #A1B8D0 , 829px 743px #A1B8D0 , 815px 109px #A1B8D0 , 437px 170px #A1B8D0 , 160px 658px #A1B8D0 , 461px 950px #A1B8D0 , 682px 355px #A1B8D0 , 221px 932px #A1B8D0 , 479px 1000px #A1B8D0 , 474px 454px #A1B8D0 , 78px 953px #A1B8D0 , 749px 68px #A1B8D0 , 140px 23px #A1B8D0 , 313px 639px #A1B8D0 , 243px 896px #A1B8D0 , 643px 62px #A1B8D0 , 9px 438px #A1B8D0 , 297px 335px #A1B8D0 , 624px 172px #A1B8D0 , 926px 977px #A1B8D0 , 761px 230px #A1B8D0 , 105px 681px #A1B8D0 , 814px 795px #A1B8D0 , 973px 326px #A1B8D0 , 695px 404px #A1B8D0 , 731px 278px #A1B8D0 , 341px 446px #A1B8D0 , 224px 691px #A1B8D0 , 491px 593px #A1B8D0 , 126px 49px #A1B8D0 , 356px 298px #A1B8D0 , 613px 342px #A1B8D0 , 919px 409px #A1B8D0 , 829px 155px #A1B8D0 , 198px 540px #A1B8D0 , 423px 803px #A1B8D0 , 766px 369px #A1B8D0 , 27px 225px #A1B8D0 , 291px 569px #A1B8D0 , 843px 735px #A1B8D0 , 461px 793px #A1B8D0 , 36px 700px #A1B8D0 , 658px 412px #A1B8D0 , 373px 192px #A1B8D0 , 141px 326px #A1B8D0 , 814px 408px #A1B8D0 , 719px 888px #A1B8D0 , 42px 88px #A1B8D0 , 928px 538px #A1B8D0 , 620px 518px #A1B8D0 , 836px 790px #A1B8D0 , 855px 845px #A1B8D0 , 713px 368px #A1B8D0 , 11px 741px #A1B8D0 , 982px 668px #A1B8D0 , 181px 840px #A1B8D0 , 801px 582px #A1B8D0 , 505px 570px #A1B8D0 , 531px 536px #A1B8D0 , 59px 949px #A1B8D0 , 450px 855px #A1B8D0 , 621px 219px #A1B8D0 , 721px 459px #A1B8D0 , 410px 333px #A1B8D0 , 849px 246px #A1B8D0 , 762px 449px #A1B8D0 , 780px 847px #A1B8D0 , 318px 366px #A1B8D0 , 988px 628px #A1B8D0 , 910px 524px #A1B8D0 , 279px 963px #A1B8D0 , 562px 238px #A1B8D0 , 69px 451px #A1B8D0 , 452px 928px #A1B8D0 , 337px 948px #A1B8D0 , 470px 615px #A1B8D0 , 473px 880px #A1B8D0 , 293px 2px #A1B8D0 , 653px 468px #A1B8D0 , 784px 352px #A1B8D0 , 535px 428px #A1B8D0 , 983px 167px #A1B8D0 , 520px 690px #A1B8D0 , 334px 369px #A1B8D0 , 663px 723px #A1B8D0 , 95px 215px #A1B8D0 , 876px 189px #A1B8D0 , 971px 729px #A1B8D0 , 594px 387px #A1B8D0 , 610px 277px #A1B8D0 , 667px 112px #A1B8D0 , 898px 737px #A1B8D0 , 61px 359px #A1B8D0 , 848px 772px #A1B8D0 , 695px 367px #A1B8D0 , 227px 793px #A1B8D0 , 421px 935px #A1B8D0 , 664px 982px #A1B8D0 , 635px 329px #A1B8D0 , 227px 486px #A1B8D0 , 534px 796px #A1B8D0 , 445px 655px #A1B8D0 , 327px 951px #A1B8D0 , 5px 206px #A1B8D0 , 63px 938px #A1B8D0 , 147px 340px #A1B8D0 , 294px 913px #A1B8D0 , 157px 773px #A1B8D0 , 871px 641px #A1B8D0 , 870px 776px #A1B8D0 , 935px 707px #A1B8D0 , 743px 979px #A1B8D0 , 978px 396px #A1B8D0 , 431px 212px #A1B8D0 , 117px 733px #A1B8D0 , 621px 842px #A1B8D0 , 593px 575px #A1B8D0 , 566px 970px #A1B8D0 , 526px 175px #A1B8D0 , 468px 434px #A1B8D0 , 288px 40px #A1B8D0 , 139px 711px #A1B8D0 , 994px 177px #A1B8D0 , 999px 474px #A1B8D0 , 858px 898px #A1B8D0 , 269px 612px #A1B8D0;
  }
  
  @-moz-keyframes glitter-8 {
    0%,
      100%,
      20.32258%,
      30.32258% {
      opacity: 0;
    }
    25.32258% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-8 {
    0%,
      100%,
      20.32258%,
      30.32258% {
      opacity: 0;
    }
    25.32258% {
      opacity: 1;
    }
  }
  @keyframes glitter-8 {
    0%,
      100%,
      20.32258%,
      30.32258% {
      opacity: 0;
    }
    25.32258% {
      opacity: 1;
    }
  }
  .glitter_8 {
    -moz-animation: glitter-8 10s infinite;
    -webkit-animation: glitter-8 10s infinite;
    animation: glitter-8 10s infinite;
    box-shadow: 736px 447px #A1B8D0 , 554px 982px #A1B8D0 , 584px 54px #A1B8D0 , 472px 574px #A1B8D0 , 586px 985px #A1B8D0 , 961px 357px #A1B8D0 , 574px 743px #A1B8D0 , 465px 210px #A1B8D0 , 372px 157px #A1B8D0 , 856px 38px #A1B8D0 , 366px 552px #A1B8D0 , 428px 272px #A1B8D0 , 425px 849px #A1B8D0 , 362px 458px #A1B8D0 , 166px 728px #A1B8D0 , 865px 444px #A1B8D0 , 92px 150px #A1B8D0 , 714px 759px #A1B8D0 , 154px 157px #A1B8D0 , 850px 508px #A1B8D0 , 203px 590px #A1B8D0 , 350px 48px #A1B8D0 , 909px 187px #A1B8D0 , 187px 504px #A1B8D0 , 187px 9px #A1B8D0 , 567px 205px #A1B8D0 , 610px 305px #A1B8D0 , 757px 620px #A1B8D0 , 258px 747px #A1B8D0 , 872px 779px #A1B8D0 , 981px 352px #A1B8D0 , 343px 335px #A1B8D0 , 771px 284px #A1B8D0 , 829px 210px #A1B8D0 , 874px 837px #A1B8D0 , 298px 902px #A1B8D0 , 931px 357px #A1B8D0 , 594px 317px #A1B8D0 , 660px 853px #A1B8D0 , 70px 160px #A1B8D0 , 157px 688px #A1B8D0 , 74px 968px #A1B8D0 , 712px 665px #A1B8D0 , 195px 188px #A1B8D0 , 359px 129px #A1B8D0 , 549px 524px #A1B8D0 , 701px 956px #A1B8D0 , 721px 335px #A1B8D0 , 899px 184px #A1B8D0 , 696px 238px #A1B8D0 , 32px 440px #A1B8D0 , 693px 975px #A1B8D0 , 455px 87px #A1B8D0 , 605px 548px #A1B8D0 , 466px 387px #A1B8D0 , 458px 540px #A1B8D0 , 533px 524px #A1B8D0 , 935px 176px #A1B8D0 , 730px 945px #A1B8D0 , 575px 919px #A1B8D0 , 349px 775px #A1B8D0 , 170px 685px #A1B8D0 , 572px 413px #A1B8D0 , 405px 221px #A1B8D0 , 322px 555px #A1B8D0 , 531px 115px #A1B8D0 , 545px 731px #A1B8D0 , 115px 492px #A1B8D0 , 927px 142px #A1B8D0 , 109px 842px #A1B8D0 , 851px 197px #A1B8D0 , 512px 708px #A1B8D0 , 493px 472px #A1B8D0 , 289px 730px #A1B8D0 , 125px 850px #A1B8D0 , 20px 272px #A1B8D0 , 480px 561px #A1B8D0 , 692px 888px #A1B8D0 , 31px 894px #A1B8D0 , 430px 300px #A1B8D0 , 136px 658px #A1B8D0 , 861px 769px #A1B8D0 , 649px 371px #A1B8D0 , 379px 532px #A1B8D0 , 637px 761px #A1B8D0 , 410px 535px #A1B8D0 , 332px 409px #A1B8D0 , 148px 733px #A1B8D0 , 250px 402px #A1B8D0 , 32px 352px #A1B8D0 , 294px 172px #A1B8D0 , 982px 863px #A1B8D0 , 750px 995px #A1B8D0 , 237px 215px #A1B8D0 , 331px 666px #A1B8D0 , 746px 73px #A1B8D0 , 899px 35px #A1B8D0 , 813px 866px #A1B8D0 , 661px 328px #A1B8D0 , 390px 389px #A1B8D0 , 738px 468px #A1B8D0 , 985px 308px #A1B8D0 , 716px 902px #A1B8D0 , 189px 32px #A1B8D0 , 794px 508px #A1B8D0 , 871px 272px #A1B8D0 , 878px 122px #A1B8D0 , 865px 138px #A1B8D0 , 469px 476px #A1B8D0 , 403px 373px #A1B8D0 , 667px 366px #A1B8D0 , 771px 196px #A1B8D0 , 262px 244px #A1B8D0 , 391px 91px #A1B8D0 , 791px 384px #A1B8D0 , 935px 236px #A1B8D0 , 412px 184px #A1B8D0 , 470px 140px #A1B8D0 , 123px 652px #A1B8D0 , 631px 15px #A1B8D0 , 242px 682px #A1B8D0 , 447px 541px #A1B8D0 , 571px 649px #A1B8D0 , 970px 913px #A1B8D0 , 849px 681px #A1B8D0 , 68px 8px #A1B8D0 , 860px 692px #A1B8D0 , 563px 741px #A1B8D0 , 708px 107px #A1B8D0 , 72px 923px #A1B8D0 , 383px 538px #A1B8D0 , 421px 373px #A1B8D0 , 550px 140px #A1B8D0 , 79px 165px #A1B8D0 , 322px 914px #A1B8D0 , 915px 183px #A1B8D0 , 234px 969px #A1B8D0 , 698px 960px #A1B8D0 , 185px 65px #A1B8D0 , 548px 771px #A1B8D0 , 442px 535px #A1B8D0 , 739px 286px #A1B8D0 , 697px 294px #A1B8D0 , 362px 676px #A1B8D0 , 980px 601px #A1B8D0 , 226px 448px #A1B8D0 , 37px 883px #A1B8D0 , 769px 668px #A1B8D0 , 250px 561px #A1B8D0 , 24px 342px #A1B8D0 , 326px 981px #A1B8D0 , 119px 960px #A1B8D0 , 670px 88px #A1B8D0 , 244px 344px #A1B8D0 , 162px 900px #A1B8D0 , 784px 243px #A1B8D0 , 885px 860px #A1B8D0 , 64px 463px #A1B8D0 , 745px 370px #A1B8D0 , 214px 163px #A1B8D0 , 58px 830px #A1B8D0 , 351px 254px #A1B8D0 , 388px 797px #A1B8D0 , 359px 563px #A1B8D0 , 946px 473px #A1B8D0 , 324px 822px #A1B8D0 , 783px 451px #A1B8D0 , 223px 44px #A1B8D0 , 136px 71px #A1B8D0 , 294px 799px #A1B8D0 , 147px 108px #A1B8D0 , 87px 814px #A1B8D0 , 695px 255px #A1B8D0 , 496px 64px #A1B8D0 , 802px 489px #A1B8D0 , 795px 446px #A1B8D0 , 761px 148px #A1B8D0 , 709px 222px #A1B8D0 , 739px 318px #A1B8D0 , 408px 673px #A1B8D0 , 892px 509px #A1B8D0 , 381px 997px #A1B8D0 , 210px 527px #A1B8D0 , 433px 957px #A1B8D0 , 541px 561px #A1B8D0 , 91px 140px #A1B8D0 , 866px 327px #A1B8D0 , 141px 456px #A1B8D0 , 236px 712px #A1B8D0 , 38px 308px #A1B8D0 , 110px 152px #A1B8D0 , 523px 48px #A1B8D0 , 840px 471px #A1B8D0 , 415px 93px #A1B8D0 , 2px 271px #A1B8D0 , 979px 405px #A1B8D0 , 97px 108px #A1B8D0 , 944px 214px #A1B8D0 , 855px 334px #A1B8D0 , 321px 744px #A1B8D0;
  }
  .glitter_8:before {
    -moz-animation: glitter-8 8s infinite;
    -webkit-animation: glitter-8 8s infinite;
    animation: glitter-8 8s infinite;
    box-shadow: 736px 447px #A1B8D0 , 554px 982px #A1B8D0 , 584px 54px #A1B8D0 , 472px 574px #A1B8D0 , 586px 985px #A1B8D0 , 961px 357px #A1B8D0 , 574px 743px #A1B8D0 , 465px 210px #A1B8D0 , 372px 157px #A1B8D0 , 856px 38px #A1B8D0 , 366px 552px #A1B8D0 , 428px 272px #A1B8D0 , 425px 849px #A1B8D0 , 362px 458px #A1B8D0 , 166px 728px #A1B8D0 , 865px 444px #A1B8D0 , 92px 150px #A1B8D0 , 714px 759px #A1B8D0 , 154px 157px #A1B8D0 , 850px 508px #A1B8D0 , 203px 590px #A1B8D0 , 350px 48px #A1B8D0 , 909px 187px #A1B8D0 , 187px 504px #A1B8D0 , 187px 9px #A1B8D0 , 567px 205px #A1B8D0 , 610px 305px #A1B8D0 , 757px 620px #A1B8D0 , 258px 747px #A1B8D0 , 872px 779px #A1B8D0 , 981px 352px #A1B8D0 , 343px 335px #A1B8D0 , 771px 284px #A1B8D0 , 829px 210px #A1B8D0 , 874px 837px #A1B8D0 , 298px 902px #A1B8D0 , 931px 357px #A1B8D0 , 594px 317px #A1B8D0 , 660px 853px #A1B8D0 , 70px 160px #A1B8D0 , 157px 688px #A1B8D0 , 74px 968px #A1B8D0 , 712px 665px #A1B8D0 , 195px 188px #A1B8D0 , 359px 129px #A1B8D0 , 549px 524px #A1B8D0 , 701px 956px #A1B8D0 , 721px 335px #A1B8D0 , 899px 184px #A1B8D0 , 696px 238px #A1B8D0 , 32px 440px #A1B8D0 , 693px 975px #A1B8D0 , 455px 87px #A1B8D0 , 605px 548px #A1B8D0 , 466px 387px #A1B8D0 , 458px 540px #A1B8D0 , 533px 524px #A1B8D0 , 935px 176px #A1B8D0 , 730px 945px #A1B8D0 , 575px 919px #A1B8D0 , 349px 775px #A1B8D0 , 170px 685px #A1B8D0 , 572px 413px #A1B8D0 , 405px 221px #A1B8D0 , 322px 555px #A1B8D0 , 531px 115px #A1B8D0 , 545px 731px #A1B8D0 , 115px 492px #A1B8D0 , 927px 142px #A1B8D0 , 109px 842px #A1B8D0 , 851px 197px #A1B8D0 , 512px 708px #A1B8D0 , 493px 472px #A1B8D0 , 289px 730px #A1B8D0 , 125px 850px #A1B8D0 , 20px 272px #A1B8D0 , 480px 561px #A1B8D0 , 692px 888px #A1B8D0 , 31px 894px #A1B8D0 , 430px 300px #A1B8D0 , 136px 658px #A1B8D0 , 861px 769px #A1B8D0 , 649px 371px #A1B8D0 , 379px 532px #A1B8D0 , 637px 761px #A1B8D0 , 410px 535px #A1B8D0 , 332px 409px #A1B8D0 , 148px 733px #A1B8D0 , 250px 402px #A1B8D0 , 32px 352px #A1B8D0 , 294px 172px #A1B8D0 , 982px 863px #A1B8D0 , 750px 995px #A1B8D0 , 237px 215px #A1B8D0 , 331px 666px #A1B8D0 , 746px 73px #A1B8D0 , 899px 35px #A1B8D0 , 813px 866px #A1B8D0 , 661px 328px #A1B8D0 , 390px 389px #A1B8D0 , 738px 468px #A1B8D0 , 985px 308px #A1B8D0 , 716px 902px #A1B8D0 , 189px 32px #A1B8D0 , 794px 508px #A1B8D0 , 871px 272px #A1B8D0 , 878px 122px #A1B8D0 , 865px 138px #A1B8D0 , 469px 476px #A1B8D0 , 403px 373px #A1B8D0 , 667px 366px #A1B8D0 , 771px 196px #A1B8D0 , 262px 244px #A1B8D0 , 391px 91px #A1B8D0 , 791px 384px #A1B8D0 , 935px 236px #A1B8D0 , 412px 184px #A1B8D0 , 470px 140px #A1B8D0 , 123px 652px #A1B8D0 , 631px 15px #A1B8D0 , 242px 682px #A1B8D0 , 447px 541px #A1B8D0 , 571px 649px #A1B8D0 , 970px 913px #A1B8D0 , 849px 681px #A1B8D0 , 68px 8px #A1B8D0 , 860px 692px #A1B8D0 , 563px 741px #A1B8D0 , 708px 107px #A1B8D0 , 72px 923px #A1B8D0 , 383px 538px #A1B8D0 , 421px 373px #A1B8D0 , 550px 140px #A1B8D0 , 79px 165px #A1B8D0 , 322px 914px #A1B8D0 , 915px 183px #A1B8D0 , 234px 969px #A1B8D0 , 698px 960px #A1B8D0 , 185px 65px #A1B8D0 , 548px 771px #A1B8D0 , 442px 535px #A1B8D0 , 739px 286px #A1B8D0 , 697px 294px #A1B8D0 , 362px 676px #A1B8D0 , 980px 601px #A1B8D0 , 226px 448px #A1B8D0 , 37px 883px #A1B8D0 , 769px 668px #A1B8D0 , 250px 561px #A1B8D0 , 24px 342px #A1B8D0 , 326px 981px #A1B8D0 , 119px 960px #A1B8D0 , 670px 88px #A1B8D0 , 244px 344px #A1B8D0 , 162px 900px #A1B8D0 , 784px 243px #A1B8D0 , 885px 860px #A1B8D0 , 64px 463px #A1B8D0 , 745px 370px #A1B8D0 , 214px 163px #A1B8D0 , 58px 830px #A1B8D0 , 351px 254px #A1B8D0 , 388px 797px #A1B8D0 , 359px 563px #A1B8D0 , 946px 473px #A1B8D0 , 324px 822px #A1B8D0 , 783px 451px #A1B8D0 , 223px 44px #A1B8D0 , 136px 71px #A1B8D0 , 294px 799px #A1B8D0 , 147px 108px #A1B8D0 , 87px 814px #A1B8D0 , 695px 255px #A1B8D0 , 496px 64px #A1B8D0 , 802px 489px #A1B8D0 , 795px 446px #A1B8D0 , 761px 148px #A1B8D0 , 709px 222px #A1B8D0 , 739px 318px #A1B8D0 , 408px 673px #A1B8D0 , 892px 509px #A1B8D0 , 381px 997px #A1B8D0 , 210px 527px #A1B8D0 , 433px 957px #A1B8D0 , 541px 561px #A1B8D0 , 91px 140px #A1B8D0 , 866px 327px #A1B8D0 , 141px 456px #A1B8D0 , 236px 712px #A1B8D0 , 38px 308px #A1B8D0 , 110px 152px #A1B8D0 , 523px 48px #A1B8D0 , 840px 471px #A1B8D0 , 415px 93px #A1B8D0 , 2px 271px #A1B8D0 , 979px 405px #A1B8D0 , 97px 108px #A1B8D0 , 944px 214px #A1B8D0 , 855px 334px #A1B8D0 , 321px 744px #A1B8D0;
  }
  .glitter_8:after {
    -moz-animation: glitter-8 9s infinite;
    -webkit-animation: glitter-8 9s infinite;
    animation: glitter-8 9s infinite;
    box-shadow: 736px 447px #A1B8D0 , 554px 982px #A1B8D0 , 584px 54px #A1B8D0 , 472px 574px #A1B8D0 , 586px 985px #A1B8D0 , 961px 357px #A1B8D0 , 574px 743px #A1B8D0 , 465px 210px #A1B8D0 , 372px 157px #A1B8D0 , 856px 38px #A1B8D0 , 366px 552px #A1B8D0 , 428px 272px #A1B8D0 , 425px 849px #A1B8D0 , 362px 458px #A1B8D0 , 166px 728px #A1B8D0 , 865px 444px #A1B8D0 , 92px 150px #A1B8D0 , 714px 759px #A1B8D0 , 154px 157px #A1B8D0 , 850px 508px #A1B8D0 , 203px 590px #A1B8D0 , 350px 48px #A1B8D0 , 909px 187px #A1B8D0 , 187px 504px #A1B8D0 , 187px 9px #A1B8D0 , 567px 205px #A1B8D0 , 610px 305px #A1B8D0 , 757px 620px #A1B8D0 , 258px 747px #A1B8D0 , 872px 779px #A1B8D0 , 981px 352px #A1B8D0 , 343px 335px #A1B8D0 , 771px 284px #A1B8D0 , 829px 210px #A1B8D0 , 874px 837px #A1B8D0 , 298px 902px #A1B8D0 , 931px 357px #A1B8D0 , 594px 317px #A1B8D0 , 660px 853px #A1B8D0 , 70px 160px #A1B8D0 , 157px 688px #A1B8D0 , 74px 968px #A1B8D0 , 712px 665px #A1B8D0 , 195px 188px #A1B8D0 , 359px 129px #A1B8D0 , 549px 524px #A1B8D0 , 701px 956px #A1B8D0 , 721px 335px #A1B8D0 , 899px 184px #A1B8D0 , 696px 238px #A1B8D0 , 32px 440px #A1B8D0 , 693px 975px #A1B8D0 , 455px 87px #A1B8D0 , 605px 548px #A1B8D0 , 466px 387px #A1B8D0 , 458px 540px #A1B8D0 , 533px 524px #A1B8D0 , 935px 176px #A1B8D0 , 730px 945px #A1B8D0 , 575px 919px #A1B8D0 , 349px 775px #A1B8D0 , 170px 685px #A1B8D0 , 572px 413px #A1B8D0 , 405px 221px #A1B8D0 , 322px 555px #A1B8D0 , 531px 115px #A1B8D0 , 545px 731px #A1B8D0 , 115px 492px #A1B8D0 , 927px 142px #A1B8D0 , 109px 842px #A1B8D0 , 851px 197px #A1B8D0 , 512px 708px #A1B8D0 , 493px 472px #A1B8D0 , 289px 730px #A1B8D0 , 125px 850px #A1B8D0 , 20px 272px #A1B8D0 , 480px 561px #A1B8D0 , 692px 888px #A1B8D0 , 31px 894px #A1B8D0 , 430px 300px #A1B8D0 , 136px 658px #A1B8D0 , 861px 769px #A1B8D0 , 649px 371px #A1B8D0 , 379px 532px #A1B8D0 , 637px 761px #A1B8D0 , 410px 535px #A1B8D0 , 332px 409px #A1B8D0 , 148px 733px #A1B8D0 , 250px 402px #A1B8D0 , 32px 352px #A1B8D0 , 294px 172px #A1B8D0 , 982px 863px #A1B8D0 , 750px 995px #A1B8D0 , 237px 215px #A1B8D0 , 331px 666px #A1B8D0 , 746px 73px #A1B8D0 , 899px 35px #A1B8D0 , 813px 866px #A1B8D0 , 661px 328px #A1B8D0 , 390px 389px #A1B8D0 , 738px 468px #A1B8D0 , 985px 308px #A1B8D0 , 716px 902px #A1B8D0 , 189px 32px #A1B8D0 , 794px 508px #A1B8D0 , 871px 272px #A1B8D0 , 878px 122px #A1B8D0 , 865px 138px #A1B8D0 , 469px 476px #A1B8D0 , 403px 373px #A1B8D0 , 667px 366px #A1B8D0 , 771px 196px #A1B8D0 , 262px 244px #A1B8D0 , 391px 91px #A1B8D0 , 791px 384px #A1B8D0 , 935px 236px #A1B8D0 , 412px 184px #A1B8D0 , 470px 140px #A1B8D0 , 123px 652px #A1B8D0 , 631px 15px #A1B8D0 , 242px 682px #A1B8D0 , 447px 541px #A1B8D0 , 571px 649px #A1B8D0 , 970px 913px #A1B8D0 , 849px 681px #A1B8D0 , 68px 8px #A1B8D0 , 860px 692px #A1B8D0 , 563px 741px #A1B8D0 , 708px 107px #A1B8D0 , 72px 923px #A1B8D0 , 383px 538px #A1B8D0 , 421px 373px #A1B8D0 , 550px 140px #A1B8D0 , 79px 165px #A1B8D0 , 322px 914px #A1B8D0 , 915px 183px #A1B8D0 , 234px 969px #A1B8D0 , 698px 960px #A1B8D0 , 185px 65px #A1B8D0 , 548px 771px #A1B8D0 , 442px 535px #A1B8D0 , 739px 286px #A1B8D0 , 697px 294px #A1B8D0 , 362px 676px #A1B8D0 , 980px 601px #A1B8D0 , 226px 448px #A1B8D0 , 37px 883px #A1B8D0 , 769px 668px #A1B8D0 , 250px 561px #A1B8D0 , 24px 342px #A1B8D0 , 326px 981px #A1B8D0 , 119px 960px #A1B8D0 , 670px 88px #A1B8D0 , 244px 344px #A1B8D0 , 162px 900px #A1B8D0 , 784px 243px #A1B8D0 , 885px 860px #A1B8D0 , 64px 463px #A1B8D0 , 745px 370px #A1B8D0 , 214px 163px #A1B8D0 , 58px 830px #A1B8D0 , 351px 254px #A1B8D0 , 388px 797px #A1B8D0 , 359px 563px #A1B8D0 , 946px 473px #A1B8D0 , 324px 822px #A1B8D0 , 783px 451px #A1B8D0 , 223px 44px #A1B8D0 , 136px 71px #A1B8D0 , 294px 799px #A1B8D0 , 147px 108px #A1B8D0 , 87px 814px #A1B8D0 , 695px 255px #A1B8D0 , 496px 64px #A1B8D0 , 802px 489px #A1B8D0 , 795px 446px #A1B8D0 , 761px 148px #A1B8D0 , 709px 222px #A1B8D0 , 739px 318px #A1B8D0 , 408px 673px #A1B8D0 , 892px 509px #A1B8D0 , 381px 997px #A1B8D0 , 210px 527px #A1B8D0 , 433px 957px #A1B8D0 , 541px 561px #A1B8D0 , 91px 140px #A1B8D0 , 866px 327px #A1B8D0 , 141px 456px #A1B8D0 , 236px 712px #A1B8D0 , 38px 308px #A1B8D0 , 110px 152px #A1B8D0 , 523px 48px #A1B8D0 , 840px 471px #A1B8D0 , 415px 93px #A1B8D0 , 2px 271px #A1B8D0 , 979px 405px #A1B8D0 , 97px 108px #A1B8D0 , 944px 214px #A1B8D0 , 855px 334px #A1B8D0 , 321px 744px #A1B8D0;
  }
  
  @-moz-keyframes glitter-9 {
    0%,
      100%,
      23.22581%,
      33.22581% {
      opacity: 0;
    }
    28.22581% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-9 {
    0%,
      100%,
      23.22581%,
      33.22581% {
      opacity: 0;
    }
    28.22581% {
      opacity: 1;
    }
  }
  @keyframes glitter-9 {
    0%,
      100%,
      23.22581%,
      33.22581% {
      opacity: 0;
    }
    28.22581% {
      opacity: 1;
    }
  }
  .glitter_9 {
    -moz-animation: glitter-9 10s infinite;
    -webkit-animation: glitter-9 10s infinite;
    animation: glitter-9 10s infinite;
    box-shadow: 194px 725px #A1B8D0 , 274px 132px #A1B8D0 , 193px 544px #A1B8D0 , 44px 917px #A1B8D0 , 609px 715px #A1B8D0 , 268px 999px #A1B8D0 , 309px 755px #A1B8D0 , 785px 606px #A1B8D0 , 585px 473px #A1B8D0 , 883px 239px #A1B8D0 , 846px 454px #A1B8D0 , 291px 754px #A1B8D0 , 496px 224px #A1B8D0 , 409px 780px #A1B8D0 , 962px 990px #A1B8D0 , 640px 554px #A1B8D0 , 881px 226px #A1B8D0 , 551px 637px #A1B8D0 , 430px 565px #A1B8D0 , 239px 278px #A1B8D0 , 59px 576px #A1B8D0 , 150px 473px #A1B8D0 , 446px 768px #A1B8D0 , 248px 430px #A1B8D0 , 784px 468px #A1B8D0 , 363px 370px #A1B8D0 , 902px 993px #A1B8D0 , 754px 841px #A1B8D0 , 990px 166px #A1B8D0 , 467px 770px #A1B8D0 , 249px 302px #A1B8D0 , 970px 775px #A1B8D0 , 391px 160px #A1B8D0 , 251px 145px #A1B8D0 , 891px 320px #A1B8D0 , 186px 690px #A1B8D0 , 311px 952px #A1B8D0 , 946px 205px #A1B8D0 , 262px 307px #A1B8D0 , 487px 152px #A1B8D0 , 222px 262px #A1B8D0 , 247px 114px #A1B8D0 , 234px 461px #A1B8D0 , 59px 647px #A1B8D0 , 622px 824px #A1B8D0 , 945px 494px #A1B8D0 , 244px 653px #A1B8D0 , 119px 860px #A1B8D0 , 794px 758px #A1B8D0 , 158px 517px #A1B8D0 , 671px 732px #A1B8D0 , 617px 807px #A1B8D0 , 727px 387px #A1B8D0 , 498px 648px #A1B8D0 , 142px 893px #A1B8D0 , 451px 798px #A1B8D0 , 71px 387px #A1B8D0 , 705px 686px #A1B8D0 , 591px 466px #A1B8D0 , 118px 617px #A1B8D0 , 216px 70px #A1B8D0 , 457px 661px #A1B8D0 , 816px 443px #A1B8D0 , 961px 100px #A1B8D0 , 971px 61px #A1B8D0 , 944px 709px #A1B8D0 , 797px 93px #A1B8D0 , 808px 400px #A1B8D0 , 205px 605px #A1B8D0 , 740px 678px #A1B8D0 , 286px 60px #A1B8D0 , 821px 707px #A1B8D0 , 834px 909px #A1B8D0 , 207px 481px #A1B8D0 , 916px 167px #A1B8D0 , 276px 528px #A1B8D0 , 645px 658px #A1B8D0 , 964px 400px #A1B8D0 , 636px 359px #A1B8D0 , 327px 611px #A1B8D0 , 890px 71px #A1B8D0 , 431px 565px #A1B8D0 , 530px 894px #A1B8D0 , 173px 279px #A1B8D0 , 684px 457px #A1B8D0 , 342px 282px #A1B8D0 , 209px 121px #A1B8D0 , 846px 695px #A1B8D0 , 516px 138px #A1B8D0 , 710px 742px #A1B8D0 , 965px 829px #A1B8D0 , 270px 508px #A1B8D0 , 746px 99px #A1B8D0 , 517px 589px #A1B8D0 , 885px 121px #A1B8D0 , 645px 719px #A1B8D0 , 872px 781px #A1B8D0 , 194px 459px #A1B8D0 , 680px 131px #A1B8D0 , 84px 451px #A1B8D0 , 691px 773px #A1B8D0 , 453px 29px #A1B8D0 , 649px 490px #A1B8D0 , 545px 274px #A1B8D0 , 752px 335px #A1B8D0 , 568px 995px #A1B8D0 , 470px 597px #A1B8D0 , 862px 980px #A1B8D0 , 158px 386px #A1B8D0 , 429px 941px #A1B8D0 , 125px 12px #A1B8D0 , 759px 547px #A1B8D0 , 868px 160px #A1B8D0 , 475px 71px #A1B8D0 , 578px 755px #A1B8D0 , 248px 729px #A1B8D0 , 85px 130px #A1B8D0 , 74px 459px #A1B8D0 , 458px 471px #A1B8D0 , 319px 636px #A1B8D0 , 113px 581px #A1B8D0 , 965px 642px #A1B8D0 , 744px 951px #A1B8D0 , 681px 123px #A1B8D0 , 492px 730px #A1B8D0 , 332px 49px #A1B8D0 , 418px 178px #A1B8D0 , 684px 885px #A1B8D0 , 477px 938px #A1B8D0 , 881px 564px #A1B8D0 , 535px 892px #A1B8D0 , 580px 326px #A1B8D0 , 209px 729px #A1B8D0 , 629px 682px #A1B8D0 , 823px 371px #A1B8D0 , 860px 338px #A1B8D0 , 893px 121px #A1B8D0 , 409px 197px #A1B8D0 , 707px 8px #A1B8D0 , 276px 532px #A1B8D0 , 906px 647px #A1B8D0 , 727px 820px #A1B8D0 , 40px 297px #A1B8D0 , 793px 598px #A1B8D0 , 981px 4px #A1B8D0 , 731px 871px #A1B8D0 , 330px 514px #A1B8D0 , 55px 349px #A1B8D0 , 744px 861px #A1B8D0 , 766px 271px #A1B8D0 , 40px 878px #A1B8D0 , 333px 628px #A1B8D0 , 233px 567px #A1B8D0 , 977px 352px #A1B8D0 , 620px 788px #A1B8D0 , 872px 192px #A1B8D0 , 7px 828px #A1B8D0 , 963px 709px #A1B8D0 , 810px 728px #A1B8D0 , 75px 125px #A1B8D0 , 356px 57px #A1B8D0 , 650px 824px #A1B8D0 , 202px 646px #A1B8D0 , 709px 410px #A1B8D0 , 616px 171px #A1B8D0 , 665px 409px #A1B8D0 , 188px 395px #A1B8D0 , 216px 212px #A1B8D0 , 397px 219px #A1B8D0 , 267px 717px #A1B8D0 , 459px 539px #A1B8D0 , 802px 483px #A1B8D0 , 211px 343px #A1B8D0 , 716px 147px #A1B8D0 , 714px 242px #A1B8D0 , 511px 750px #A1B8D0 , 392px 564px #A1B8D0 , 395px 400px #A1B8D0 , 812px 991px #A1B8D0 , 32px 94px #A1B8D0 , 451px 532px #A1B8D0 , 265px 498px #A1B8D0 , 828px 558px #A1B8D0 , 412px 522px #A1B8D0 , 208px 239px #A1B8D0 , 465px 83px #A1B8D0 , 907px 95px #A1B8D0 , 831px 458px #A1B8D0 , 972px 334px #A1B8D0 , 928px 431px #A1B8D0 , 794px 360px #A1B8D0 , 749px 765px #A1B8D0 , 449px 560px #A1B8D0 , 525px 448px #A1B8D0 , 119px 945px #A1B8D0 , 392px 789px #A1B8D0 , 778px 434px #A1B8D0 , 21px 48px #A1B8D0 , 104px 308px #A1B8D0 , 846px 960px #A1B8D0;
  }
  .glitter_9:before {
    -moz-animation: glitter-9 8s infinite;
    -webkit-animation: glitter-9 8s infinite;
    animation: glitter-9 8s infinite;
    box-shadow: 194px 725px #A1B8D0 , 274px 132px #A1B8D0 , 193px 544px #A1B8D0 , 44px 917px #A1B8D0 , 609px 715px #A1B8D0 , 268px 999px #A1B8D0 , 309px 755px #A1B8D0 , 785px 606px #A1B8D0 , 585px 473px #A1B8D0 , 883px 239px #A1B8D0 , 846px 454px #A1B8D0 , 291px 754px #A1B8D0 , 496px 224px #A1B8D0 , 409px 780px #A1B8D0 , 962px 990px #A1B8D0 , 640px 554px #A1B8D0 , 881px 226px #A1B8D0 , 551px 637px #A1B8D0 , 430px 565px #A1B8D0 , 239px 278px #A1B8D0 , 59px 576px #A1B8D0 , 150px 473px #A1B8D0 , 446px 768px #A1B8D0 , 248px 430px #A1B8D0 , 784px 468px #A1B8D0 , 363px 370px #A1B8D0 , 902px 993px #A1B8D0 , 754px 841px #A1B8D0 , 990px 166px #A1B8D0 , 467px 770px #A1B8D0 , 249px 302px #A1B8D0 , 970px 775px #A1B8D0 , 391px 160px #A1B8D0 , 251px 145px #A1B8D0 , 891px 320px #A1B8D0 , 186px 690px #A1B8D0 , 311px 952px #A1B8D0 , 946px 205px #A1B8D0 , 262px 307px #A1B8D0 , 487px 152px #A1B8D0 , 222px 262px #A1B8D0 , 247px 114px #A1B8D0 , 234px 461px #A1B8D0 , 59px 647px #A1B8D0 , 622px 824px #A1B8D0 , 945px 494px #A1B8D0 , 244px 653px #A1B8D0 , 119px 860px #A1B8D0 , 794px 758px #A1B8D0 , 158px 517px #A1B8D0 , 671px 732px #A1B8D0 , 617px 807px #A1B8D0 , 727px 387px #A1B8D0 , 498px 648px #A1B8D0 , 142px 893px #A1B8D0 , 451px 798px #A1B8D0 , 71px 387px #A1B8D0 , 705px 686px #A1B8D0 , 591px 466px #A1B8D0 , 118px 617px #A1B8D0 , 216px 70px #A1B8D0 , 457px 661px #A1B8D0 , 816px 443px #A1B8D0 , 961px 100px #A1B8D0 , 971px 61px #A1B8D0 , 944px 709px #A1B8D0 , 797px 93px #A1B8D0 , 808px 400px #A1B8D0 , 205px 605px #A1B8D0 , 740px 678px #A1B8D0 , 286px 60px #A1B8D0 , 821px 707px #A1B8D0 , 834px 909px #A1B8D0 , 207px 481px #A1B8D0 , 916px 167px #A1B8D0 , 276px 528px #A1B8D0 , 645px 658px #A1B8D0 , 964px 400px #A1B8D0 , 636px 359px #A1B8D0 , 327px 611px #A1B8D0 , 890px 71px #A1B8D0 , 431px 565px #A1B8D0 , 530px 894px #A1B8D0 , 173px 279px #A1B8D0 , 684px 457px #A1B8D0 , 342px 282px #A1B8D0 , 209px 121px #A1B8D0 , 846px 695px #A1B8D0 , 516px 138px #A1B8D0 , 710px 742px #A1B8D0 , 965px 829px #A1B8D0 , 270px 508px #A1B8D0 , 746px 99px #A1B8D0 , 517px 589px #A1B8D0 , 885px 121px #A1B8D0 , 645px 719px #A1B8D0 , 872px 781px #A1B8D0 , 194px 459px #A1B8D0 , 680px 131px #A1B8D0 , 84px 451px #A1B8D0 , 691px 773px #A1B8D0 , 453px 29px #A1B8D0 , 649px 490px #A1B8D0 , 545px 274px #A1B8D0 , 752px 335px #A1B8D0 , 568px 995px #A1B8D0 , 470px 597px #A1B8D0 , 862px 980px #A1B8D0 , 158px 386px #A1B8D0 , 429px 941px #A1B8D0 , 125px 12px #A1B8D0 , 759px 547px #A1B8D0 , 868px 160px #A1B8D0 , 475px 71px #A1B8D0 , 578px 755px #A1B8D0 , 248px 729px #A1B8D0 , 85px 130px #A1B8D0 , 74px 459px #A1B8D0 , 458px 471px #A1B8D0 , 319px 636px #A1B8D0 , 113px 581px #A1B8D0 , 965px 642px #A1B8D0 , 744px 951px #A1B8D0 , 681px 123px #A1B8D0 , 492px 730px #A1B8D0 , 332px 49px #A1B8D0 , 418px 178px #A1B8D0 , 684px 885px #A1B8D0 , 477px 938px #A1B8D0 , 881px 564px #A1B8D0 , 535px 892px #A1B8D0 , 580px 326px #A1B8D0 , 209px 729px #A1B8D0 , 629px 682px #A1B8D0 , 823px 371px #A1B8D0 , 860px 338px #A1B8D0 , 893px 121px #A1B8D0 , 409px 197px #A1B8D0 , 707px 8px #A1B8D0 , 276px 532px #A1B8D0 , 906px 647px #A1B8D0 , 727px 820px #A1B8D0 , 40px 297px #A1B8D0 , 793px 598px #A1B8D0 , 981px 4px #A1B8D0 , 731px 871px #A1B8D0 , 330px 514px #A1B8D0 , 55px 349px #A1B8D0 , 744px 861px #A1B8D0 , 766px 271px #A1B8D0 , 40px 878px #A1B8D0 , 333px 628px #A1B8D0 , 233px 567px #A1B8D0 , 977px 352px #A1B8D0 , 620px 788px #A1B8D0 , 872px 192px #A1B8D0 , 7px 828px #A1B8D0 , 963px 709px #A1B8D0 , 810px 728px #A1B8D0 , 75px 125px #A1B8D0 , 356px 57px #A1B8D0 , 650px 824px #A1B8D0 , 202px 646px #A1B8D0 , 709px 410px #A1B8D0 , 616px 171px #A1B8D0 , 665px 409px #A1B8D0 , 188px 395px #A1B8D0 , 216px 212px #A1B8D0 , 397px 219px #A1B8D0 , 267px 717px #A1B8D0 , 459px 539px #A1B8D0 , 802px 483px #A1B8D0 , 211px 343px #A1B8D0 , 716px 147px #A1B8D0 , 714px 242px #A1B8D0 , 511px 750px #A1B8D0 , 392px 564px #A1B8D0 , 395px 400px #A1B8D0 , 812px 991px #A1B8D0 , 32px 94px #A1B8D0 , 451px 532px #A1B8D0 , 265px 498px #A1B8D0 , 828px 558px #A1B8D0 , 412px 522px #A1B8D0 , 208px 239px #A1B8D0 , 465px 83px #A1B8D0 , 907px 95px #A1B8D0 , 831px 458px #A1B8D0 , 972px 334px #A1B8D0 , 928px 431px #A1B8D0 , 794px 360px #A1B8D0 , 749px 765px #A1B8D0 , 449px 560px #A1B8D0 , 525px 448px #A1B8D0 , 119px 945px #A1B8D0 , 392px 789px #A1B8D0 , 778px 434px #A1B8D0 , 21px 48px #A1B8D0 , 104px 308px #A1B8D0 , 846px 960px #A1B8D0;
  }
  .glitter_9:after {
    -moz-animation: glitter-9 9s infinite;
    -webkit-animation: glitter-9 9s infinite;
    animation: glitter-9 9s infinite;
    box-shadow: 194px 725px #A1B8D0 , 274px 132px #A1B8D0 , 193px 544px #A1B8D0 , 44px 917px #A1B8D0 , 609px 715px #A1B8D0 , 268px 999px #A1B8D0 , 309px 755px #A1B8D0 , 785px 606px #A1B8D0 , 585px 473px #A1B8D0 , 883px 239px #A1B8D0 , 846px 454px #A1B8D0 , 291px 754px #A1B8D0 , 496px 224px #A1B8D0 , 409px 780px #A1B8D0 , 962px 990px #A1B8D0 , 640px 554px #A1B8D0 , 881px 226px #A1B8D0 , 551px 637px #A1B8D0 , 430px 565px #A1B8D0 , 239px 278px #A1B8D0 , 59px 576px #A1B8D0 , 150px 473px #A1B8D0 , 446px 768px #A1B8D0 , 248px 430px #A1B8D0 , 784px 468px #A1B8D0 , 363px 370px #A1B8D0 , 902px 993px #A1B8D0 , 754px 841px #A1B8D0 , 990px 166px #A1B8D0 , 467px 770px #A1B8D0 , 249px 302px #A1B8D0 , 970px 775px #A1B8D0 , 391px 160px #A1B8D0 , 251px 145px #A1B8D0 , 891px 320px #A1B8D0 , 186px 690px #A1B8D0 , 311px 952px #A1B8D0 , 946px 205px #A1B8D0 , 262px 307px #A1B8D0 , 487px 152px #A1B8D0 , 222px 262px #A1B8D0 , 247px 114px #A1B8D0 , 234px 461px #A1B8D0 , 59px 647px #A1B8D0 , 622px 824px #A1B8D0 , 945px 494px #A1B8D0 , 244px 653px #A1B8D0 , 119px 860px #A1B8D0 , 794px 758px #A1B8D0 , 158px 517px #A1B8D0 , 671px 732px #A1B8D0 , 617px 807px #A1B8D0 , 727px 387px #A1B8D0 , 498px 648px #A1B8D0 , 142px 893px #A1B8D0 , 451px 798px #A1B8D0 , 71px 387px #A1B8D0 , 705px 686px #A1B8D0 , 591px 466px #A1B8D0 , 118px 617px #A1B8D0 , 216px 70px #A1B8D0 , 457px 661px #A1B8D0 , 816px 443px #A1B8D0 , 961px 100px #A1B8D0 , 971px 61px #A1B8D0 , 944px 709px #A1B8D0 , 797px 93px #A1B8D0 , 808px 400px #A1B8D0 , 205px 605px #A1B8D0 , 740px 678px #A1B8D0 , 286px 60px #A1B8D0 , 821px 707px #A1B8D0 , 834px 909px #A1B8D0 , 207px 481px #A1B8D0 , 916px 167px #A1B8D0 , 276px 528px #A1B8D0 , 645px 658px #A1B8D0 , 964px 400px #A1B8D0 , 636px 359px #A1B8D0 , 327px 611px #A1B8D0 , 890px 71px #A1B8D0 , 431px 565px #A1B8D0 , 530px 894px #A1B8D0 , 173px 279px #A1B8D0 , 684px 457px #A1B8D0 , 342px 282px #A1B8D0 , 209px 121px #A1B8D0 , 846px 695px #A1B8D0 , 516px 138px #A1B8D0 , 710px 742px #A1B8D0 , 965px 829px #A1B8D0 , 270px 508px #A1B8D0 , 746px 99px #A1B8D0 , 517px 589px #A1B8D0 , 885px 121px #A1B8D0 , 645px 719px #A1B8D0 , 872px 781px #A1B8D0 , 194px 459px #A1B8D0 , 680px 131px #A1B8D0 , 84px 451px #A1B8D0 , 691px 773px #A1B8D0 , 453px 29px #A1B8D0 , 649px 490px #A1B8D0 , 545px 274px #A1B8D0 , 752px 335px #A1B8D0 , 568px 995px #A1B8D0 , 470px 597px #A1B8D0 , 862px 980px #A1B8D0 , 158px 386px #A1B8D0 , 429px 941px #A1B8D0 , 125px 12px #A1B8D0 , 759px 547px #A1B8D0 , 868px 160px #A1B8D0 , 475px 71px #A1B8D0 , 578px 755px #A1B8D0 , 248px 729px #A1B8D0 , 85px 130px #A1B8D0 , 74px 459px #A1B8D0 , 458px 471px #A1B8D0 , 319px 636px #A1B8D0 , 113px 581px #A1B8D0 , 965px 642px #A1B8D0 , 744px 951px #A1B8D0 , 681px 123px #A1B8D0 , 492px 730px #A1B8D0 , 332px 49px #A1B8D0 , 418px 178px #A1B8D0 , 684px 885px #A1B8D0 , 477px 938px #A1B8D0 , 881px 564px #A1B8D0 , 535px 892px #A1B8D0 , 580px 326px #A1B8D0 , 209px 729px #A1B8D0 , 629px 682px #A1B8D0 , 823px 371px #A1B8D0 , 860px 338px #A1B8D0 , 893px 121px #A1B8D0 , 409px 197px #A1B8D0 , 707px 8px #A1B8D0 , 276px 532px #A1B8D0 , 906px 647px #A1B8D0 , 727px 820px #A1B8D0 , 40px 297px #A1B8D0 , 793px 598px #A1B8D0 , 981px 4px #A1B8D0 , 731px 871px #A1B8D0 , 330px 514px #A1B8D0 , 55px 349px #A1B8D0 , 744px 861px #A1B8D0 , 766px 271px #A1B8D0 , 40px 878px #A1B8D0 , 333px 628px #A1B8D0 , 233px 567px #A1B8D0 , 977px 352px #A1B8D0 , 620px 788px #A1B8D0 , 872px 192px #A1B8D0 , 7px 828px #A1B8D0 , 963px 709px #A1B8D0 , 810px 728px #A1B8D0 , 75px 125px #A1B8D0 , 356px 57px #A1B8D0 , 650px 824px #A1B8D0 , 202px 646px #A1B8D0 , 709px 410px #A1B8D0 , 616px 171px #A1B8D0 , 665px 409px #A1B8D0 , 188px 395px #A1B8D0 , 216px 212px #A1B8D0 , 397px 219px #A1B8D0 , 267px 717px #A1B8D0 , 459px 539px #A1B8D0 , 802px 483px #A1B8D0 , 211px 343px #A1B8D0 , 716px 147px #A1B8D0 , 714px 242px #A1B8D0 , 511px 750px #A1B8D0 , 392px 564px #A1B8D0 , 395px 400px #A1B8D0 , 812px 991px #A1B8D0 , 32px 94px #A1B8D0 , 451px 532px #A1B8D0 , 265px 498px #A1B8D0 , 828px 558px #A1B8D0 , 412px 522px #A1B8D0 , 208px 239px #A1B8D0 , 465px 83px #A1B8D0 , 907px 95px #A1B8D0 , 831px 458px #A1B8D0 , 972px 334px #A1B8D0 , 928px 431px #A1B8D0 , 794px 360px #A1B8D0 , 749px 765px #A1B8D0 , 449px 560px #A1B8D0 , 525px 448px #A1B8D0 , 119px 945px #A1B8D0 , 392px 789px #A1B8D0 , 778px 434px #A1B8D0 , 21px 48px #A1B8D0 , 104px 308px #A1B8D0 , 846px 960px #A1B8D0;
  }
  
  @-moz-keyframes glitter-10 {
    0%,
      100%,
      26.12903%,
      36.12903% {
      opacity: 0;
    }
    31.12903% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-10 {
    0%,
      100%,
      26.12903%,
      36.12903% {
      opacity: 0;
    }
    31.12903% {
      opacity: 1;
    }
  }
  @keyframes glitter-10 {
    0%,
      100%,
      26.12903%,
      36.12903% {
      opacity: 0;
    }
    31.12903% {
      opacity: 1;
    }
  }
  .glitter_10 {
    -moz-animation: glitter-10 10s infinite;
    -webkit-animation: glitter-10 10s infinite;
    animation: glitter-10 10s infinite;
    box-shadow: 724px 170px #A1B8D0 , 500px 182px #A1B8D0 , 427px 488px #A1B8D0 , 139px 697px #A1B8D0 , 911px 634px #A1B8D0 , 589px 906px #A1B8D0 , 332px 46px #A1B8D0 , 969px 271px #A1B8D0 , 555px 587px #A1B8D0 , 616px 46px #A1B8D0 , 432px 883px #A1B8D0 , 796px 117px #A1B8D0 , 987px 560px #A1B8D0 , 24px 952px #A1B8D0 , 621px 689px #A1B8D0 , 786px 549px #A1B8D0 , 793px 723px #A1B8D0 , 791px 221px #A1B8D0 , 991px 489px #A1B8D0 , 421px 133px #A1B8D0 , 147px 582px #A1B8D0 , 425px 901px #A1B8D0 , 659px 995px #A1B8D0 , 728px 351px #A1B8D0 , 530px 122px #A1B8D0 , 640px 360px #A1B8D0 , 74px 876px #A1B8D0 , 232px 329px #A1B8D0 , 330px 349px #A1B8D0 , 817px 586px #A1B8D0 , 326px 403px #A1B8D0 , 819px 753px #A1B8D0 , 480px 127px #A1B8D0 , 892px 409px #A1B8D0 , 734px 262px #A1B8D0 , 252px 333px #A1B8D0 , 779px 773px #A1B8D0 , 272px 884px #A1B8D0 , 933px 818px #A1B8D0 , 944px 824px #A1B8D0 , 465px 743px #A1B8D0 , 909px 942px #A1B8D0 , 758px 24px #A1B8D0 , 973px 795px #A1B8D0 , 238px 79px #A1B8D0 , 872px 395px #A1B8D0 , 18px 897px #A1B8D0 , 623px 756px #A1B8D0 , 282px 445px #A1B8D0 , 347px 421px #A1B8D0 , 316px 693px #A1B8D0 , 92px 741px #A1B8D0 , 407px 833px #A1B8D0 , 878px 865px #A1B8D0 , 958px 174px #A1B8D0 , 340px 50px #A1B8D0 , 832px 726px #A1B8D0 , 720px 790px #A1B8D0 , 938px 21px #A1B8D0 , 573px 238px #A1B8D0 , 22px 615px #A1B8D0 , 361px 246px #A1B8D0 , 976px 599px #A1B8D0 , 844px 743px #A1B8D0 , 253px 976px #A1B8D0 , 711px 184px #A1B8D0 , 896px 440px #A1B8D0 , 664px 982px #A1B8D0 , 793px 124px #A1B8D0 , 384px 849px #A1B8D0 , 302px 782px #A1B8D0 , 550px 238px #A1B8D0 , 740px 329px #A1B8D0 , 173px 282px #A1B8D0 , 148px 692px #A1B8D0 , 674px 388px #A1B8D0 , 478px 39px #A1B8D0 , 499px 739px #A1B8D0 , 924px 474px #A1B8D0 , 696px 988px #A1B8D0 , 282px 835px #A1B8D0 , 843px 728px #A1B8D0 , 216px 469px #A1B8D0 , 391px 372px #A1B8D0 , 866px 421px #A1B8D0 , 708px 9px #A1B8D0 , 471px 759px #A1B8D0 , 223px 967px #A1B8D0 , 815px 383px #A1B8D0 , 563px 985px #A1B8D0 , 783px 388px #A1B8D0 , 962px 459px #A1B8D0 , 156px 830px #A1B8D0 , 722px 698px #A1B8D0 , 122px 868px #A1B8D0 , 609px 376px #A1B8D0 , 878px 445px #A1B8D0 , 536px 369px #A1B8D0 , 985px 559px #A1B8D0 , 237px 720px #A1B8D0 , 240px 633px #A1B8D0 , 705px 281px #A1B8D0 , 68px 627px #A1B8D0 , 724px 128px #A1B8D0 , 114px 498px #A1B8D0 , 136px 687px #A1B8D0 , 5px 485px #A1B8D0 , 492px 778px #A1B8D0 , 676px 382px #A1B8D0 , 316px 487px #A1B8D0 , 967px 378px #A1B8D0 , 443px 152px #A1B8D0 , 919px 764px #A1B8D0 , 403px 446px #A1B8D0 , 820px 356px #A1B8D0 , 366px 733px #A1B8D0 , 348px 584px #A1B8D0 , 998px 469px #A1B8D0 , 13px 387px #A1B8D0 , 343px 799px #A1B8D0 , 330px 846px #A1B8D0 , 282px 188px #A1B8D0 , 45px 38px #A1B8D0 , 916px 6px #A1B8D0 , 681px 269px #A1B8D0 , 369px 100px #A1B8D0 , 342px 45px #A1B8D0 , 380px 494px #A1B8D0 , 72px 278px #A1B8D0 , 151px 347px #A1B8D0 , 519px 819px #A1B8D0 , 747px 66px #A1B8D0 , 584px 132px #A1B8D0 , 236px 943px #A1B8D0 , 92px 492px #A1B8D0 , 172px 987px #A1B8D0 , 33px 978px #A1B8D0 , 183px 316px #A1B8D0 , 149px 133px #A1B8D0 , 367px 291px #A1B8D0 , 331px 834px #A1B8D0 , 588px 767px #A1B8D0 , 927px 76px #A1B8D0 , 527px 706px #A1B8D0 , 636px 631px #A1B8D0 , 873px 381px #A1B8D0 , 102px 133px #A1B8D0 , 671px 152px #A1B8D0 , 549px 396px #A1B8D0 , 813px 180px #A1B8D0 , 790px 864px #A1B8D0 , 880px 857px #A1B8D0 , 167px 188px #A1B8D0 , 746px 185px #A1B8D0 , 243px 2px #A1B8D0 , 69px 714px #A1B8D0 , 587px 937px #A1B8D0 , 204px 428px #A1B8D0 , 979px 670px #A1B8D0 , 402px 759px #A1B8D0 , 730px 620px #A1B8D0 , 970px 633px #A1B8D0 , 145px 600px #A1B8D0 , 65px 261px #A1B8D0 , 471px 252px #A1B8D0 , 323px 949px #A1B8D0 , 105px 834px #A1B8D0 , 935px 722px #A1B8D0 , 60px 960px #A1B8D0 , 218px 82px #A1B8D0 , 444px 2px #A1B8D0 , 522px 590px #A1B8D0 , 741px 298px #A1B8D0 , 33px 588px #A1B8D0 , 831px 310px #A1B8D0 , 734px 100px #A1B8D0 , 8px 376px #A1B8D0 , 591px 882px #A1B8D0 , 530px 656px #A1B8D0 , 201px 267px #A1B8D0 , 443px 979px #A1B8D0 , 298px 993px #A1B8D0 , 614px 489px #A1B8D0 , 322px 591px #A1B8D0 , 844px 257px #A1B8D0 , 515px 322px #A1B8D0 , 616px 238px #A1B8D0 , 515px 439px #A1B8D0 , 437px 368px #A1B8D0 , 803px 959px #A1B8D0 , 182px 614px #A1B8D0 , 422px 285px #A1B8D0 , 266px 338px #A1B8D0 , 299px 716px #A1B8D0 , 85px 359px #A1B8D0 , 291px 621px #A1B8D0 , 411px 869px #A1B8D0 , 713px 752px #A1B8D0 , 695px 729px #A1B8D0 , 892px 292px #A1B8D0;
  }
  .glitter_10:before {
    -moz-animation: glitter-10 8s infinite;
    -webkit-animation: glitter-10 8s infinite;
    animation: glitter-10 8s infinite;
    box-shadow: 724px 170px #A1B8D0 , 500px 182px #A1B8D0 , 427px 488px #A1B8D0 , 139px 697px #A1B8D0 , 911px 634px #A1B8D0 , 589px 906px #A1B8D0 , 332px 46px #A1B8D0 , 969px 271px #A1B8D0 , 555px 587px #A1B8D0 , 616px 46px #A1B8D0 , 432px 883px #A1B8D0 , 796px 117px #A1B8D0 , 987px 560px #A1B8D0 , 24px 952px #A1B8D0 , 621px 689px #A1B8D0 , 786px 549px #A1B8D0 , 793px 723px #A1B8D0 , 791px 221px #A1B8D0 , 991px 489px #A1B8D0 , 421px 133px #A1B8D0 , 147px 582px #A1B8D0 , 425px 901px #A1B8D0 , 659px 995px #A1B8D0 , 728px 351px #A1B8D0 , 530px 122px #A1B8D0 , 640px 360px #A1B8D0 , 74px 876px #A1B8D0 , 232px 329px #A1B8D0 , 330px 349px #A1B8D0 , 817px 586px #A1B8D0 , 326px 403px #A1B8D0 , 819px 753px #A1B8D0 , 480px 127px #A1B8D0 , 892px 409px #A1B8D0 , 734px 262px #A1B8D0 , 252px 333px #A1B8D0 , 779px 773px #A1B8D0 , 272px 884px #A1B8D0 , 933px 818px #A1B8D0 , 944px 824px #A1B8D0 , 465px 743px #A1B8D0 , 909px 942px #A1B8D0 , 758px 24px #A1B8D0 , 973px 795px #A1B8D0 , 238px 79px #A1B8D0 , 872px 395px #A1B8D0 , 18px 897px #A1B8D0 , 623px 756px #A1B8D0 , 282px 445px #A1B8D0 , 347px 421px #A1B8D0 , 316px 693px #A1B8D0 , 92px 741px #A1B8D0 , 407px 833px #A1B8D0 , 878px 865px #A1B8D0 , 958px 174px #A1B8D0 , 340px 50px #A1B8D0 , 832px 726px #A1B8D0 , 720px 790px #A1B8D0 , 938px 21px #A1B8D0 , 573px 238px #A1B8D0 , 22px 615px #A1B8D0 , 361px 246px #A1B8D0 , 976px 599px #A1B8D0 , 844px 743px #A1B8D0 , 253px 976px #A1B8D0 , 711px 184px #A1B8D0 , 896px 440px #A1B8D0 , 664px 982px #A1B8D0 , 793px 124px #A1B8D0 , 384px 849px #A1B8D0 , 302px 782px #A1B8D0 , 550px 238px #A1B8D0 , 740px 329px #A1B8D0 , 173px 282px #A1B8D0 , 148px 692px #A1B8D0 , 674px 388px #A1B8D0 , 478px 39px #A1B8D0 , 499px 739px #A1B8D0 , 924px 474px #A1B8D0 , 696px 988px #A1B8D0 , 282px 835px #A1B8D0 , 843px 728px #A1B8D0 , 216px 469px #A1B8D0 , 391px 372px #A1B8D0 , 866px 421px #A1B8D0 , 708px 9px #A1B8D0 , 471px 759px #A1B8D0 , 223px 967px #A1B8D0 , 815px 383px #A1B8D0 , 563px 985px #A1B8D0 , 783px 388px #A1B8D0 , 962px 459px #A1B8D0 , 156px 830px #A1B8D0 , 722px 698px #A1B8D0 , 122px 868px #A1B8D0 , 609px 376px #A1B8D0 , 878px 445px #A1B8D0 , 536px 369px #A1B8D0 , 985px 559px #A1B8D0 , 237px 720px #A1B8D0 , 240px 633px #A1B8D0 , 705px 281px #A1B8D0 , 68px 627px #A1B8D0 , 724px 128px #A1B8D0 , 114px 498px #A1B8D0 , 136px 687px #A1B8D0 , 5px 485px #A1B8D0 , 492px 778px #A1B8D0 , 676px 382px #A1B8D0 , 316px 487px #A1B8D0 , 967px 378px #A1B8D0 , 443px 152px #A1B8D0 , 919px 764px #A1B8D0 , 403px 446px #A1B8D0 , 820px 356px #A1B8D0 , 366px 733px #A1B8D0 , 348px 584px #A1B8D0 , 998px 469px #A1B8D0 , 13px 387px #A1B8D0 , 343px 799px #A1B8D0 , 330px 846px #A1B8D0 , 282px 188px #A1B8D0 , 45px 38px #A1B8D0 , 916px 6px #A1B8D0 , 681px 269px #A1B8D0 , 369px 100px #A1B8D0 , 342px 45px #A1B8D0 , 380px 494px #A1B8D0 , 72px 278px #A1B8D0 , 151px 347px #A1B8D0 , 519px 819px #A1B8D0 , 747px 66px #A1B8D0 , 584px 132px #A1B8D0 , 236px 943px #A1B8D0 , 92px 492px #A1B8D0 , 172px 987px #A1B8D0 , 33px 978px #A1B8D0 , 183px 316px #A1B8D0 , 149px 133px #A1B8D0 , 367px 291px #A1B8D0 , 331px 834px #A1B8D0 , 588px 767px #A1B8D0 , 927px 76px #A1B8D0 , 527px 706px #A1B8D0 , 636px 631px #A1B8D0 , 873px 381px #A1B8D0 , 102px 133px #A1B8D0 , 671px 152px #A1B8D0 , 549px 396px #A1B8D0 , 813px 180px #A1B8D0 , 790px 864px #A1B8D0 , 880px 857px #A1B8D0 , 167px 188px #A1B8D0 , 746px 185px #A1B8D0 , 243px 2px #A1B8D0 , 69px 714px #A1B8D0 , 587px 937px #A1B8D0 , 204px 428px #A1B8D0 , 979px 670px #A1B8D0 , 402px 759px #A1B8D0 , 730px 620px #A1B8D0 , 970px 633px #A1B8D0 , 145px 600px #A1B8D0 , 65px 261px #A1B8D0 , 471px 252px #A1B8D0 , 323px 949px #A1B8D0 , 105px 834px #A1B8D0 , 935px 722px #A1B8D0 , 60px 960px #A1B8D0 , 218px 82px #A1B8D0 , 444px 2px #A1B8D0 , 522px 590px #A1B8D0 , 741px 298px #A1B8D0 , 33px 588px #A1B8D0 , 831px 310px #A1B8D0 , 734px 100px #A1B8D0 , 8px 376px #A1B8D0 , 591px 882px #A1B8D0 , 530px 656px #A1B8D0 , 201px 267px #A1B8D0 , 443px 979px #A1B8D0 , 298px 993px #A1B8D0 , 614px 489px #A1B8D0 , 322px 591px #A1B8D0 , 844px 257px #A1B8D0 , 515px 322px #A1B8D0 , 616px 238px #A1B8D0 , 515px 439px #A1B8D0 , 437px 368px #A1B8D0 , 803px 959px #A1B8D0 , 182px 614px #A1B8D0 , 422px 285px #A1B8D0 , 266px 338px #A1B8D0 , 299px 716px #A1B8D0 , 85px 359px #A1B8D0 , 291px 621px #A1B8D0 , 411px 869px #A1B8D0 , 713px 752px #A1B8D0 , 695px 729px #A1B8D0 , 892px 292px #A1B8D0;
  }
  .glitter_10:after {
    -moz-animation: glitter-10 9s infinite;
    -webkit-animation: glitter-10 9s infinite;
    animation: glitter-10 9s infinite;
    box-shadow: 724px 170px #A1B8D0 , 500px 182px #A1B8D0 , 427px 488px #A1B8D0 , 139px 697px #A1B8D0 , 911px 634px #A1B8D0 , 589px 906px #A1B8D0 , 332px 46px #A1B8D0 , 969px 271px #A1B8D0 , 555px 587px #A1B8D0 , 616px 46px #A1B8D0 , 432px 883px #A1B8D0 , 796px 117px #A1B8D0 , 987px 560px #A1B8D0 , 24px 952px #A1B8D0 , 621px 689px #A1B8D0 , 786px 549px #A1B8D0 , 793px 723px #A1B8D0 , 791px 221px #A1B8D0 , 991px 489px #A1B8D0 , 421px 133px #A1B8D0 , 147px 582px #A1B8D0 , 425px 901px #A1B8D0 , 659px 995px #A1B8D0 , 728px 351px #A1B8D0 , 530px 122px #A1B8D0 , 640px 360px #A1B8D0 , 74px 876px #A1B8D0 , 232px 329px #A1B8D0 , 330px 349px #A1B8D0 , 817px 586px #A1B8D0 , 326px 403px #A1B8D0 , 819px 753px #A1B8D0 , 480px 127px #A1B8D0 , 892px 409px #A1B8D0 , 734px 262px #A1B8D0 , 252px 333px #A1B8D0 , 779px 773px #A1B8D0 , 272px 884px #A1B8D0 , 933px 818px #A1B8D0 , 944px 824px #A1B8D0 , 465px 743px #A1B8D0 , 909px 942px #A1B8D0 , 758px 24px #A1B8D0 , 973px 795px #A1B8D0 , 238px 79px #A1B8D0 , 872px 395px #A1B8D0 , 18px 897px #A1B8D0 , 623px 756px #A1B8D0 , 282px 445px #A1B8D0 , 347px 421px #A1B8D0 , 316px 693px #A1B8D0 , 92px 741px #A1B8D0 , 407px 833px #A1B8D0 , 878px 865px #A1B8D0 , 958px 174px #A1B8D0 , 340px 50px #A1B8D0 , 832px 726px #A1B8D0 , 720px 790px #A1B8D0 , 938px 21px #A1B8D0 , 573px 238px #A1B8D0 , 22px 615px #A1B8D0 , 361px 246px #A1B8D0 , 976px 599px #A1B8D0 , 844px 743px #A1B8D0 , 253px 976px #A1B8D0 , 711px 184px #A1B8D0 , 896px 440px #A1B8D0 , 664px 982px #A1B8D0 , 793px 124px #A1B8D0 , 384px 849px #A1B8D0 , 302px 782px #A1B8D0 , 550px 238px #A1B8D0 , 740px 329px #A1B8D0 , 173px 282px #A1B8D0 , 148px 692px #A1B8D0 , 674px 388px #A1B8D0 , 478px 39px #A1B8D0 , 499px 739px #A1B8D0 , 924px 474px #A1B8D0 , 696px 988px #A1B8D0 , 282px 835px #A1B8D0 , 843px 728px #A1B8D0 , 216px 469px #A1B8D0 , 391px 372px #A1B8D0 , 866px 421px #A1B8D0 , 708px 9px #A1B8D0 , 471px 759px #A1B8D0 , 223px 967px #A1B8D0 , 815px 383px #A1B8D0 , 563px 985px #A1B8D0 , 783px 388px #A1B8D0 , 962px 459px #A1B8D0 , 156px 830px #A1B8D0 , 722px 698px #A1B8D0 , 122px 868px #A1B8D0 , 609px 376px #A1B8D0 , 878px 445px #A1B8D0 , 536px 369px #A1B8D0 , 985px 559px #A1B8D0 , 237px 720px #A1B8D0 , 240px 633px #A1B8D0 , 705px 281px #A1B8D0 , 68px 627px #A1B8D0 , 724px 128px #A1B8D0 , 114px 498px #A1B8D0 , 136px 687px #A1B8D0 , 5px 485px #A1B8D0 , 492px 778px #A1B8D0 , 676px 382px #A1B8D0 , 316px 487px #A1B8D0 , 967px 378px #A1B8D0 , 443px 152px #A1B8D0 , 919px 764px #A1B8D0 , 403px 446px #A1B8D0 , 820px 356px #A1B8D0 , 366px 733px #A1B8D0 , 348px 584px #A1B8D0 , 998px 469px #A1B8D0 , 13px 387px #A1B8D0 , 343px 799px #A1B8D0 , 330px 846px #A1B8D0 , 282px 188px #A1B8D0 , 45px 38px #A1B8D0 , 916px 6px #A1B8D0 , 681px 269px #A1B8D0 , 369px 100px #A1B8D0 , 342px 45px #A1B8D0 , 380px 494px #A1B8D0 , 72px 278px #A1B8D0 , 151px 347px #A1B8D0 , 519px 819px #A1B8D0 , 747px 66px #A1B8D0 , 584px 132px #A1B8D0 , 236px 943px #A1B8D0 , 92px 492px #A1B8D0 , 172px 987px #A1B8D0 , 33px 978px #A1B8D0 , 183px 316px #A1B8D0 , 149px 133px #A1B8D0 , 367px 291px #A1B8D0 , 331px 834px #A1B8D0 , 588px 767px #A1B8D0 , 927px 76px #A1B8D0 , 527px 706px #A1B8D0 , 636px 631px #A1B8D0 , 873px 381px #A1B8D0 , 102px 133px #A1B8D0 , 671px 152px #A1B8D0 , 549px 396px #A1B8D0 , 813px 180px #A1B8D0 , 790px 864px #A1B8D0 , 880px 857px #A1B8D0 , 167px 188px #A1B8D0 , 746px 185px #A1B8D0 , 243px 2px #A1B8D0 , 69px 714px #A1B8D0 , 587px 937px #A1B8D0 , 204px 428px #A1B8D0 , 979px 670px #A1B8D0 , 402px 759px #A1B8D0 , 730px 620px #A1B8D0 , 970px 633px #A1B8D0 , 145px 600px #A1B8D0 , 65px 261px #A1B8D0 , 471px 252px #A1B8D0 , 323px 949px #A1B8D0 , 105px 834px #A1B8D0 , 935px 722px #A1B8D0 , 60px 960px #A1B8D0 , 218px 82px #A1B8D0 , 444px 2px #A1B8D0 , 522px 590px #A1B8D0 , 741px 298px #A1B8D0 , 33px 588px #A1B8D0 , 831px 310px #A1B8D0 , 734px 100px #A1B8D0 , 8px 376px #A1B8D0 , 591px 882px #A1B8D0 , 530px 656px #A1B8D0 , 201px 267px #A1B8D0 , 443px 979px #A1B8D0 , 298px 993px #A1B8D0 , 614px 489px #A1B8D0 , 322px 591px #A1B8D0 , 844px 257px #A1B8D0 , 515px 322px #A1B8D0 , 616px 238px #A1B8D0 , 515px 439px #A1B8D0 , 437px 368px #A1B8D0 , 803px 959px #A1B8D0 , 182px 614px #A1B8D0 , 422px 285px #A1B8D0 , 266px 338px #A1B8D0 , 299px 716px #A1B8D0 , 85px 359px #A1B8D0 , 291px 621px #A1B8D0 , 411px 869px #A1B8D0 , 713px 752px #A1B8D0 , 695px 729px #A1B8D0 , 892px 292px #A1B8D0;
  }
  
  @-moz-keyframes glitter-11 {
    0%,
      100%,
      29.03226%,
      39.03226% {
      opacity: 0;
    }
    34.03226% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-11 {
    0%,
      100%,
      29.03226%,
      39.03226% {
      opacity: 0;
    }
    34.03226% {
      opacity: 1;
    }
  }
  @keyframes glitter-11 {
    0%,
      100%,
      29.03226%,
      39.03226% {
      opacity: 0;
    }
    34.03226% {
      opacity: 1;
    }
  }
  .glitter_11 {
    -moz-animation: glitter-11 10s infinite;
    -webkit-animation: glitter-11 10s infinite;
    animation: glitter-11 10s infinite;
    box-shadow: 767px 326px #A1B8D0 , 751px 617px #A1B8D0 , 409px 846px #A1B8D0 , 325px 27px #A1B8D0 , 601px 164px #A1B8D0 , 223px 759px #A1B8D0 , 138px 23px #A1B8D0 , 73px 759px #A1B8D0 , 33px 377px #A1B8D0 , 302px 291px #A1B8D0 , 370px 666px #A1B8D0 , 573px 880px #A1B8D0 , 358px 802px #A1B8D0 , 333px 986px #A1B8D0 , 622px 718px #A1B8D0 , 737px 3px #A1B8D0 , 135px 227px #A1B8D0 , 198px 889px #A1B8D0 , 16px 162px #A1B8D0 , 251px 376px #A1B8D0 , 332px 127px #A1B8D0 , 237px 112px #A1B8D0 , 778px 407px #A1B8D0 , 933px 797px #A1B8D0 , 241px 912px #A1B8D0 , 637px 548px #A1B8D0 , 852px 907px #A1B8D0 , 908px 255px #A1B8D0 , 663px 826px #A1B8D0 , 796px 449px #A1B8D0 , 627px 295px #A1B8D0 , 434px 394px #A1B8D0 , 514px 925px #A1B8D0 , 435px 383px #A1B8D0 , 643px 946px #A1B8D0 , 74px 181px #A1B8D0 , 262px 500px #A1B8D0 , 730px 971px #A1B8D0 , 707px 819px #A1B8D0 , 866px 883px #A1B8D0 , 345px 135px #A1B8D0 , 383px 684px #A1B8D0 , 99px 291px #A1B8D0 , 663px 155px #A1B8D0 , 837px 377px #A1B8D0 , 842px 532px #A1B8D0 , 457px 631px #A1B8D0 , 280px 225px #A1B8D0 , 546px 964px #A1B8D0 , 161px 343px #A1B8D0 , 98px 950px #A1B8D0 , 846px 578px #A1B8D0 , 513px 949px #A1B8D0 , 764px 948px #A1B8D0 , 10px 19px #A1B8D0 , 106px 289px #A1B8D0 , 833px 389px #A1B8D0 , 663px 115px #A1B8D0 , 347px 724px #A1B8D0 , 312px 373px #A1B8D0 , 238px 92px #A1B8D0 , 403px 310px #A1B8D0 , 57px 805px #A1B8D0 , 738px 782px #A1B8D0 , 604px 926px #A1B8D0 , 992px 638px #A1B8D0 , 367px 892px #A1B8D0 , 57px 256px #A1B8D0 , 265px 47px #A1B8D0 , 105px 95px #A1B8D0 , 13px 638px #A1B8D0 , 853px 268px #A1B8D0 , 305px 59px #A1B8D0 , 922px 132px #A1B8D0 , 297px 381px #A1B8D0 , 219px 209px #A1B8D0 , 503px 152px #A1B8D0 , 202px 324px #A1B8D0 , 996px 265px #A1B8D0 , 244px 511px #A1B8D0 , 402px 485px #A1B8D0 , 994px 753px #A1B8D0 , 941px 901px #A1B8D0 , 102px 995px #A1B8D0 , 735px 909px #A1B8D0 , 79px 267px #A1B8D0 , 540px 589px #A1B8D0 , 83px 971px #A1B8D0 , 990px 712px #A1B8D0 , 761px 742px #A1B8D0 , 294px 861px #A1B8D0 , 65px 986px #A1B8D0 , 50px 12px #A1B8D0 , 130px 469px #A1B8D0 , 530px 301px #A1B8D0 , 621px 555px #A1B8D0 , 764px 31px #A1B8D0 , 997px 441px #A1B8D0 , 299px 456px #A1B8D0 , 400px 471px #A1B8D0 , 557px 63px #A1B8D0 , 74px 174px #A1B8D0 , 244px 528px #A1B8D0 , 361px 382px #A1B8D0 , 630px 432px #A1B8D0 , 136px 595px #A1B8D0 , 204px 291px #A1B8D0 , 314px 35px #A1B8D0 , 69px 621px #A1B8D0 , 676px 86px #A1B8D0 , 217px 509px #A1B8D0 , 173px 381px #A1B8D0 , 886px 87px #A1B8D0 , 31px 875px #A1B8D0 , 933px 248px #A1B8D0 , 846px 784px #A1B8D0 , 192px 798px #A1B8D0 , 306px 178px #A1B8D0 , 116px 516px #A1B8D0 , 663px 553px #A1B8D0 , 412px 327px #A1B8D0 , 782px 712px #A1B8D0 , 300px 315px #A1B8D0 , 945px 318px #A1B8D0 , 95px 192px #A1B8D0 , 669px 637px #A1B8D0 , 311px 302px #A1B8D0 , 70px 503px #A1B8D0 , 120px 920px #A1B8D0 , 402px 727px #A1B8D0 , 954px 130px #A1B8D0 , 847px 121px #A1B8D0 , 603px 302px #A1B8D0 , 913px 93px #A1B8D0 , 24px 179px #A1B8D0 , 297px 572px #A1B8D0 , 34px 704px #A1B8D0 , 198px 761px #A1B8D0 , 680px 95px #A1B8D0 , 617px 367px #A1B8D0 , 830px 82px #A1B8D0 , 331px 573px #A1B8D0 , 917px 633px #A1B8D0 , 193px 922px #A1B8D0 , 62px 740px #A1B8D0 , 679px 264px #A1B8D0 , 727px 563px #A1B8D0 , 113px 25px #A1B8D0 , 285px 171px #A1B8D0 , 366px 455px #A1B8D0 , 683px 962px #A1B8D0 , 465px 992px #A1B8D0 , 578px 485px #A1B8D0 , 822px 541px #A1B8D0 , 21px 793px #A1B8D0 , 826px 278px #A1B8D0 , 89px 608px #A1B8D0 , 374px 263px #A1B8D0 , 319px 346px #A1B8D0 , 129px 338px #A1B8D0 , 652px 486px #A1B8D0 , 151px 593px #A1B8D0 , 658px 22px #A1B8D0 , 717px 52px #A1B8D0 , 993px 420px #A1B8D0 , 249px 27px #A1B8D0 , 182px 910px #A1B8D0 , 867px 112px #A1B8D0 , 887px 30px #A1B8D0 , 633px 300px #A1B8D0 , 47px 665px #A1B8D0 , 750px 551px #A1B8D0 , 698px 858px #A1B8D0 , 811px 911px #A1B8D0 , 327px 940px #A1B8D0 , 111px 614px #A1B8D0 , 766px 481px #A1B8D0 , 710px 947px #A1B8D0 , 614px 368px #A1B8D0 , 825px 668px #A1B8D0 , 358px 588px #A1B8D0 , 753px 801px #A1B8D0 , 184px 102px #A1B8D0 , 765px 804px #A1B8D0 , 106px 107px #A1B8D0 , 112px 75px #A1B8D0 , 399px 775px #A1B8D0 , 525px 596px #A1B8D0 , 910px 424px #A1B8D0 , 871px 88px #A1B8D0 , 855px 111px #A1B8D0 , 774px 683px #A1B8D0 , 13px 55px #A1B8D0 , 120px 496px #A1B8D0 , 559px 723px #A1B8D0 , 695px 376px #A1B8D0 , 649px 35px #A1B8D0 , 566px 30px #A1B8D0 , 852px 586px #A1B8D0 , 52px 157px #A1B8D0;
  }
  .glitter_11:before {
    -moz-animation: glitter-11 8s infinite;
    -webkit-animation: glitter-11 8s infinite;
    animation: glitter-11 8s infinite;
    box-shadow: 767px 326px #A1B8D0 , 751px 617px #A1B8D0 , 409px 846px #A1B8D0 , 325px 27px #A1B8D0 , 601px 164px #A1B8D0 , 223px 759px #A1B8D0 , 138px 23px #A1B8D0 , 73px 759px #A1B8D0 , 33px 377px #A1B8D0 , 302px 291px #A1B8D0 , 370px 666px #A1B8D0 , 573px 880px #A1B8D0 , 358px 802px #A1B8D0 , 333px 986px #A1B8D0 , 622px 718px #A1B8D0 , 737px 3px #A1B8D0 , 135px 227px #A1B8D0 , 198px 889px #A1B8D0 , 16px 162px #A1B8D0 , 251px 376px #A1B8D0 , 332px 127px #A1B8D0 , 237px 112px #A1B8D0 , 778px 407px #A1B8D0 , 933px 797px #A1B8D0 , 241px 912px #A1B8D0 , 637px 548px #A1B8D0 , 852px 907px #A1B8D0 , 908px 255px #A1B8D0 , 663px 826px #A1B8D0 , 796px 449px #A1B8D0 , 627px 295px #A1B8D0 , 434px 394px #A1B8D0 , 514px 925px #A1B8D0 , 435px 383px #A1B8D0 , 643px 946px #A1B8D0 , 74px 181px #A1B8D0 , 262px 500px #A1B8D0 , 730px 971px #A1B8D0 , 707px 819px #A1B8D0 , 866px 883px #A1B8D0 , 345px 135px #A1B8D0 , 383px 684px #A1B8D0 , 99px 291px #A1B8D0 , 663px 155px #A1B8D0 , 837px 377px #A1B8D0 , 842px 532px #A1B8D0 , 457px 631px #A1B8D0 , 280px 225px #A1B8D0 , 546px 964px #A1B8D0 , 161px 343px #A1B8D0 , 98px 950px #A1B8D0 , 846px 578px #A1B8D0 , 513px 949px #A1B8D0 , 764px 948px #A1B8D0 , 10px 19px #A1B8D0 , 106px 289px #A1B8D0 , 833px 389px #A1B8D0 , 663px 115px #A1B8D0 , 347px 724px #A1B8D0 , 312px 373px #A1B8D0 , 238px 92px #A1B8D0 , 403px 310px #A1B8D0 , 57px 805px #A1B8D0 , 738px 782px #A1B8D0 , 604px 926px #A1B8D0 , 992px 638px #A1B8D0 , 367px 892px #A1B8D0 , 57px 256px #A1B8D0 , 265px 47px #A1B8D0 , 105px 95px #A1B8D0 , 13px 638px #A1B8D0 , 853px 268px #A1B8D0 , 305px 59px #A1B8D0 , 922px 132px #A1B8D0 , 297px 381px #A1B8D0 , 219px 209px #A1B8D0 , 503px 152px #A1B8D0 , 202px 324px #A1B8D0 , 996px 265px #A1B8D0 , 244px 511px #A1B8D0 , 402px 485px #A1B8D0 , 994px 753px #A1B8D0 , 941px 901px #A1B8D0 , 102px 995px #A1B8D0 , 735px 909px #A1B8D0 , 79px 267px #A1B8D0 , 540px 589px #A1B8D0 , 83px 971px #A1B8D0 , 990px 712px #A1B8D0 , 761px 742px #A1B8D0 , 294px 861px #A1B8D0 , 65px 986px #A1B8D0 , 50px 12px #A1B8D0 , 130px 469px #A1B8D0 , 530px 301px #A1B8D0 , 621px 555px #A1B8D0 , 764px 31px #A1B8D0 , 997px 441px #A1B8D0 , 299px 456px #A1B8D0 , 400px 471px #A1B8D0 , 557px 63px #A1B8D0 , 74px 174px #A1B8D0 , 244px 528px #A1B8D0 , 361px 382px #A1B8D0 , 630px 432px #A1B8D0 , 136px 595px #A1B8D0 , 204px 291px #A1B8D0 , 314px 35px #A1B8D0 , 69px 621px #A1B8D0 , 676px 86px #A1B8D0 , 217px 509px #A1B8D0 , 173px 381px #A1B8D0 , 886px 87px #A1B8D0 , 31px 875px #A1B8D0 , 933px 248px #A1B8D0 , 846px 784px #A1B8D0 , 192px 798px #A1B8D0 , 306px 178px #A1B8D0 , 116px 516px #A1B8D0 , 663px 553px #A1B8D0 , 412px 327px #A1B8D0 , 782px 712px #A1B8D0 , 300px 315px #A1B8D0 , 945px 318px #A1B8D0 , 95px 192px #A1B8D0 , 669px 637px #A1B8D0 , 311px 302px #A1B8D0 , 70px 503px #A1B8D0 , 120px 920px #A1B8D0 , 402px 727px #A1B8D0 , 954px 130px #A1B8D0 , 847px 121px #A1B8D0 , 603px 302px #A1B8D0 , 913px 93px #A1B8D0 , 24px 179px #A1B8D0 , 297px 572px #A1B8D0 , 34px 704px #A1B8D0 , 198px 761px #A1B8D0 , 680px 95px #A1B8D0 , 617px 367px #A1B8D0 , 830px 82px #A1B8D0 , 331px 573px #A1B8D0 , 917px 633px #A1B8D0 , 193px 922px #A1B8D0 , 62px 740px #A1B8D0 , 679px 264px #A1B8D0 , 727px 563px #A1B8D0 , 113px 25px #A1B8D0 , 285px 171px #A1B8D0 , 366px 455px #A1B8D0 , 683px 962px #A1B8D0 , 465px 992px #A1B8D0 , 578px 485px #A1B8D0 , 822px 541px #A1B8D0 , 21px 793px #A1B8D0 , 826px 278px #A1B8D0 , 89px 608px #A1B8D0 , 374px 263px #A1B8D0 , 319px 346px #A1B8D0 , 129px 338px #A1B8D0 , 652px 486px #A1B8D0 , 151px 593px #A1B8D0 , 658px 22px #A1B8D0 , 717px 52px #A1B8D0 , 993px 420px #A1B8D0 , 249px 27px #A1B8D0 , 182px 910px #A1B8D0 , 867px 112px #A1B8D0 , 887px 30px #A1B8D0 , 633px 300px #A1B8D0 , 47px 665px #A1B8D0 , 750px 551px #A1B8D0 , 698px 858px #A1B8D0 , 811px 911px #A1B8D0 , 327px 940px #A1B8D0 , 111px 614px #A1B8D0 , 766px 481px #A1B8D0 , 710px 947px #A1B8D0 , 614px 368px #A1B8D0 , 825px 668px #A1B8D0 , 358px 588px #A1B8D0 , 753px 801px #A1B8D0 , 184px 102px #A1B8D0 , 765px 804px #A1B8D0 , 106px 107px #A1B8D0 , 112px 75px #A1B8D0 , 399px 775px #A1B8D0 , 525px 596px #A1B8D0 , 910px 424px #A1B8D0 , 871px 88px #A1B8D0 , 855px 111px #A1B8D0 , 774px 683px #A1B8D0 , 13px 55px #A1B8D0 , 120px 496px #A1B8D0 , 559px 723px #A1B8D0 , 695px 376px #A1B8D0 , 649px 35px #A1B8D0 , 566px 30px #A1B8D0 , 852px 586px #A1B8D0 , 52px 157px #A1B8D0;
  }
  .glitter_11:after {
    -moz-animation: glitter-11 9s infinite;
    -webkit-animation: glitter-11 9s infinite;
    animation: glitter-11 9s infinite;
    box-shadow: 767px 326px #A1B8D0 , 751px 617px #A1B8D0 , 409px 846px #A1B8D0 , 325px 27px #A1B8D0 , 601px 164px #A1B8D0 , 223px 759px #A1B8D0 , 138px 23px #A1B8D0 , 73px 759px #A1B8D0 , 33px 377px #A1B8D0 , 302px 291px #A1B8D0 , 370px 666px #A1B8D0 , 573px 880px #A1B8D0 , 358px 802px #A1B8D0 , 333px 986px #A1B8D0 , 622px 718px #A1B8D0 , 737px 3px #A1B8D0 , 135px 227px #A1B8D0 , 198px 889px #A1B8D0 , 16px 162px #A1B8D0 , 251px 376px #A1B8D0 , 332px 127px #A1B8D0 , 237px 112px #A1B8D0 , 778px 407px #A1B8D0 , 933px 797px #A1B8D0 , 241px 912px #A1B8D0 , 637px 548px #A1B8D0 , 852px 907px #A1B8D0 , 908px 255px #A1B8D0 , 663px 826px #A1B8D0 , 796px 449px #A1B8D0 , 627px 295px #A1B8D0 , 434px 394px #A1B8D0 , 514px 925px #A1B8D0 , 435px 383px #A1B8D0 , 643px 946px #A1B8D0 , 74px 181px #A1B8D0 , 262px 500px #A1B8D0 , 730px 971px #A1B8D0 , 707px 819px #A1B8D0 , 866px 883px #A1B8D0 , 345px 135px #A1B8D0 , 383px 684px #A1B8D0 , 99px 291px #A1B8D0 , 663px 155px #A1B8D0 , 837px 377px #A1B8D0 , 842px 532px #A1B8D0 , 457px 631px #A1B8D0 , 280px 225px #A1B8D0 , 546px 964px #A1B8D0 , 161px 343px #A1B8D0 , 98px 950px #A1B8D0 , 846px 578px #A1B8D0 , 513px 949px #A1B8D0 , 764px 948px #A1B8D0 , 10px 19px #A1B8D0 , 106px 289px #A1B8D0 , 833px 389px #A1B8D0 , 663px 115px #A1B8D0 , 347px 724px #A1B8D0 , 312px 373px #A1B8D0 , 238px 92px #A1B8D0 , 403px 310px #A1B8D0 , 57px 805px #A1B8D0 , 738px 782px #A1B8D0 , 604px 926px #A1B8D0 , 992px 638px #A1B8D0 , 367px 892px #A1B8D0 , 57px 256px #A1B8D0 , 265px 47px #A1B8D0 , 105px 95px #A1B8D0 , 13px 638px #A1B8D0 , 853px 268px #A1B8D0 , 305px 59px #A1B8D0 , 922px 132px #A1B8D0 , 297px 381px #A1B8D0 , 219px 209px #A1B8D0 , 503px 152px #A1B8D0 , 202px 324px #A1B8D0 , 996px 265px #A1B8D0 , 244px 511px #A1B8D0 , 402px 485px #A1B8D0 , 994px 753px #A1B8D0 , 941px 901px #A1B8D0 , 102px 995px #A1B8D0 , 735px 909px #A1B8D0 , 79px 267px #A1B8D0 , 540px 589px #A1B8D0 , 83px 971px #A1B8D0 , 990px 712px #A1B8D0 , 761px 742px #A1B8D0 , 294px 861px #A1B8D0 , 65px 986px #A1B8D0 , 50px 12px #A1B8D0 , 130px 469px #A1B8D0 , 530px 301px #A1B8D0 , 621px 555px #A1B8D0 , 764px 31px #A1B8D0 , 997px 441px #A1B8D0 , 299px 456px #A1B8D0 , 400px 471px #A1B8D0 , 557px 63px #A1B8D0 , 74px 174px #A1B8D0 , 244px 528px #A1B8D0 , 361px 382px #A1B8D0 , 630px 432px #A1B8D0 , 136px 595px #A1B8D0 , 204px 291px #A1B8D0 , 314px 35px #A1B8D0 , 69px 621px #A1B8D0 , 676px 86px #A1B8D0 , 217px 509px #A1B8D0 , 173px 381px #A1B8D0 , 886px 87px #A1B8D0 , 31px 875px #A1B8D0 , 933px 248px #A1B8D0 , 846px 784px #A1B8D0 , 192px 798px #A1B8D0 , 306px 178px #A1B8D0 , 116px 516px #A1B8D0 , 663px 553px #A1B8D0 , 412px 327px #A1B8D0 , 782px 712px #A1B8D0 , 300px 315px #A1B8D0 , 945px 318px #A1B8D0 , 95px 192px #A1B8D0 , 669px 637px #A1B8D0 , 311px 302px #A1B8D0 , 70px 503px #A1B8D0 , 120px 920px #A1B8D0 , 402px 727px #A1B8D0 , 954px 130px #A1B8D0 , 847px 121px #A1B8D0 , 603px 302px #A1B8D0 , 913px 93px #A1B8D0 , 24px 179px #A1B8D0 , 297px 572px #A1B8D0 , 34px 704px #A1B8D0 , 198px 761px #A1B8D0 , 680px 95px #A1B8D0 , 617px 367px #A1B8D0 , 830px 82px #A1B8D0 , 331px 573px #A1B8D0 , 917px 633px #A1B8D0 , 193px 922px #A1B8D0 , 62px 740px #A1B8D0 , 679px 264px #A1B8D0 , 727px 563px #A1B8D0 , 113px 25px #A1B8D0 , 285px 171px #A1B8D0 , 366px 455px #A1B8D0 , 683px 962px #A1B8D0 , 465px 992px #A1B8D0 , 578px 485px #A1B8D0 , 822px 541px #A1B8D0 , 21px 793px #A1B8D0 , 826px 278px #A1B8D0 , 89px 608px #A1B8D0 , 374px 263px #A1B8D0 , 319px 346px #A1B8D0 , 129px 338px #A1B8D0 , 652px 486px #A1B8D0 , 151px 593px #A1B8D0 , 658px 22px #A1B8D0 , 717px 52px #A1B8D0 , 993px 420px #A1B8D0 , 249px 27px #A1B8D0 , 182px 910px #A1B8D0 , 867px 112px #A1B8D0 , 887px 30px #A1B8D0 , 633px 300px #A1B8D0 , 47px 665px #A1B8D0 , 750px 551px #A1B8D0 , 698px 858px #A1B8D0 , 811px 911px #A1B8D0 , 327px 940px #A1B8D0 , 111px 614px #A1B8D0 , 766px 481px #A1B8D0 , 710px 947px #A1B8D0 , 614px 368px #A1B8D0 , 825px 668px #A1B8D0 , 358px 588px #A1B8D0 , 753px 801px #A1B8D0 , 184px 102px #A1B8D0 , 765px 804px #A1B8D0 , 106px 107px #A1B8D0 , 112px 75px #A1B8D0 , 399px 775px #A1B8D0 , 525px 596px #A1B8D0 , 910px 424px #A1B8D0 , 871px 88px #A1B8D0 , 855px 111px #A1B8D0 , 774px 683px #A1B8D0 , 13px 55px #A1B8D0 , 120px 496px #A1B8D0 , 559px 723px #A1B8D0 , 695px 376px #A1B8D0 , 649px 35px #A1B8D0 , 566px 30px #A1B8D0 , 852px 586px #A1B8D0 , 52px 157px #A1B8D0;
  }
  
  @-moz-keyframes glitter-12 {
    0%,
      100%,
      31.93548%,
      41.93548% {
      opacity: 0;
    }
    36.93548% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-12 {
    0%,
      100%,
      31.93548%,
      41.93548% {
      opacity: 0;
    }
    36.93548% {
      opacity: 1;
    }
  }
  @keyframes glitter-12 {
    0%,
      100%,
      31.93548%,
      41.93548% {
      opacity: 0;
    }
    36.93548% {
      opacity: 1;
    }
  }
  .glitter_12 {
    -moz-animation: glitter-12 10s infinite;
    -webkit-animation: glitter-12 10s infinite;
    animation: glitter-12 10s infinite;
    box-shadow: 843px 592px #A1B8D0 , 87px 18px #A1B8D0 , 976px 869px #A1B8D0 , 984px 806px #A1B8D0 , 817px 680px #A1B8D0 , 643px 119px #A1B8D0 , 404px 438px #A1B8D0 , 205px 139px #A1B8D0 , 594px 20px #A1B8D0 , 971px 583px #A1B8D0 , 618px 40px #A1B8D0 , 25px 864px #A1B8D0 , 820px 290px #A1B8D0 , 793px 811px #A1B8D0 , 883px 290px #A1B8D0 , 583px 61px #A1B8D0 , 43px 251px #A1B8D0 , 154px 235px #A1B8D0 , 701px 203px #A1B8D0 , 633px 184px #A1B8D0 , 741px 868px #A1B8D0 , 504px 842px #A1B8D0 , 714px 543px #A1B8D0 , 795px 620px #A1B8D0 , 973px 814px #A1B8D0 , 621px 7px #A1B8D0 , 973px 672px #A1B8D0 , 932px 167px #A1B8D0 , 464px 886px #A1B8D0 , 514px 298px #A1B8D0 , 966px 302px #A1B8D0 , 655px 851px #A1B8D0 , 454px 154px #A1B8D0 , 245px 252px #A1B8D0 , 758px 290px #A1B8D0 , 681px 731px #A1B8D0 , 348px 689px #A1B8D0 , 697px 144px #A1B8D0 , 336px 35px #A1B8D0 , 110px 314px #A1B8D0 , 997px 235px #A1B8D0 , 27px 627px #A1B8D0 , 145px 398px #A1B8D0 , 771px 313px #A1B8D0 , 358px 86px #A1B8D0 , 919px 532px #A1B8D0 , 144px 634px #A1B8D0 , 622px 453px #A1B8D0 , 543px 474px #A1B8D0 , 174px 203px #A1B8D0 , 111px 316px #A1B8D0 , 104px 962px #A1B8D0 , 11px 7px #A1B8D0 , 164px 567px #A1B8D0 , 507px 592px #A1B8D0 , 805px 297px #A1B8D0 , 112px 731px #A1B8D0 , 227px 151px #A1B8D0 , 192px 442px #A1B8D0 , 849px 96px #A1B8D0 , 374px 624px #A1B8D0 , 271px 691px #A1B8D0 , 121px 69px #A1B8D0 , 950px 897px #A1B8D0 , 390px 794px #A1B8D0 , 317px 251px #A1B8D0 , 241px 490px #A1B8D0 , 68px 865px #A1B8D0 , 991px 70px #A1B8D0 , 107px 754px #A1B8D0 , 713px 691px #A1B8D0 , 756px 572px #A1B8D0 , 686px 420px #A1B8D0 , 431px 810px #A1B8D0 , 223px 576px #A1B8D0 , 640px 69px #A1B8D0 , 383px 538px #A1B8D0 , 873px 931px #A1B8D0 , 152px 862px #A1B8D0 , 959px 313px #A1B8D0 , 277px 373px #A1B8D0 , 153px 624px #A1B8D0 , 251px 525px #A1B8D0 , 441px 596px #A1B8D0 , 437px 499px #A1B8D0 , 619px 203px #A1B8D0 , 701px 109px #A1B8D0 , 583px 924px #A1B8D0 , 871px 232px #A1B8D0 , 909px 622px #A1B8D0 , 337px 993px #A1B8D0 , 672px 474px #A1B8D0 , 861px 255px #A1B8D0 , 358px 588px #A1B8D0 , 955px 81px #A1B8D0 , 21px 311px #A1B8D0 , 387px 693px #A1B8D0 , 183px 789px #A1B8D0 , 702px 739px #A1B8D0 , 961px 448px #A1B8D0 , 464px 546px #A1B8D0 , 521px 638px #A1B8D0 , 871px 668px #A1B8D0 , 103px 37px #A1B8D0 , 815px 925px #A1B8D0 , 891px 367px #A1B8D0 , 421px 806px #A1B8D0 , 214px 63px #A1B8D0 , 394px 515px #A1B8D0 , 861px 93px #A1B8D0 , 834px 877px #A1B8D0 , 215px 928px #A1B8D0 , 543px 819px #A1B8D0 , 734px 452px #A1B8D0 , 520px 949px #A1B8D0 , 927px 578px #A1B8D0 , 400px 808px #A1B8D0 , 657px 855px #A1B8D0 , 713px 256px #A1B8D0 , 817px 426px #A1B8D0 , 537px 568px #A1B8D0 , 927px 617px #A1B8D0 , 837px 735px #A1B8D0 , 290px 53px #A1B8D0 , 99px 345px #A1B8D0 , 521px 666px #A1B8D0 , 373px 590px #A1B8D0 , 51px 338px #A1B8D0 , 541px 39px #A1B8D0 , 769px 529px #A1B8D0 , 692px 237px #A1B8D0 , 867px 666px #A1B8D0 , 315px 849px #A1B8D0 , 945px 24px #A1B8D0 , 503px 848px #A1B8D0 , 920px 345px #A1B8D0 , 245px 262px #A1B8D0 , 310px 242px #A1B8D0 , 776px 655px #A1B8D0 , 529px 235px #A1B8D0 , 56px 771px #A1B8D0 , 946px 95px #A1B8D0 , 449px 503px #A1B8D0 , 33px 240px #A1B8D0 , 271px 637px #A1B8D0 , 420px 946px #A1B8D0 , 208px 359px #A1B8D0 , 294px 359px #A1B8D0 , 110px 25px #A1B8D0 , 79px 199px #A1B8D0 , 927px 31px #A1B8D0 , 889px 411px #A1B8D0 , 400px 188px #A1B8D0 , 871px 542px #A1B8D0 , 13px 967px #A1B8D0 , 784px 167px #A1B8D0 , 654px 576px #A1B8D0 , 796px 897px #A1B8D0 , 485px 92px #A1B8D0 , 837px 848px #A1B8D0 , 268px 642px #A1B8D0 , 203px 417px #A1B8D0 , 377px 646px #A1B8D0 , 940px 400px #A1B8D0 , 133px 55px #A1B8D0 , 400px 40px #A1B8D0 , 230px 818px #A1B8D0 , 844px 769px #A1B8D0 , 505px 723px #A1B8D0 , 970px 364px #A1B8D0 , 152px 796px #A1B8D0 , 950px 95px #A1B8D0 , 105px 465px #A1B8D0 , 81px 650px #A1B8D0 , 359px 931px #A1B8D0 , 513px 283px #A1B8D0 , 14px 136px #A1B8D0 , 354px 863px #A1B8D0 , 159px 337px #A1B8D0 , 262px 161px #A1B8D0 , 949px 959px #A1B8D0 , 992px 711px #A1B8D0 , 436px 5px #A1B8D0 , 565px 32px #A1B8D0 , 321px 961px #A1B8D0 , 370px 219px #A1B8D0 , 836px 689px #A1B8D0 , 839px 760px #A1B8D0 , 746px 744px #A1B8D0 , 724px 963px #A1B8D0 , 824px 354px #A1B8D0 , 361px 808px #A1B8D0 , 464px 280px #A1B8D0 , 427px 559px #A1B8D0 , 863px 1px #A1B8D0 , 484px 751px #A1B8D0 , 659px 471px #A1B8D0 , 940px 927px #A1B8D0 , 983px 731px #A1B8D0 , 19px 303px #A1B8D0;
  }
  .glitter_12:before {
    -moz-animation: glitter-12 8s infinite;
    -webkit-animation: glitter-12 8s infinite;
    animation: glitter-12 8s infinite;
    box-shadow: 843px 592px #A1B8D0 , 87px 18px #A1B8D0 , 976px 869px #A1B8D0 , 984px 806px #A1B8D0 , 817px 680px #A1B8D0 , 643px 119px #A1B8D0 , 404px 438px #A1B8D0 , 205px 139px #A1B8D0 , 594px 20px #A1B8D0 , 971px 583px #A1B8D0 , 618px 40px #A1B8D0 , 25px 864px #A1B8D0 , 820px 290px #A1B8D0 , 793px 811px #A1B8D0 , 883px 290px #A1B8D0 , 583px 61px #A1B8D0 , 43px 251px #A1B8D0 , 154px 235px #A1B8D0 , 701px 203px #A1B8D0 , 633px 184px #A1B8D0 , 741px 868px #A1B8D0 , 504px 842px #A1B8D0 , 714px 543px #A1B8D0 , 795px 620px #A1B8D0 , 973px 814px #A1B8D0 , 621px 7px #A1B8D0 , 973px 672px #A1B8D0 , 932px 167px #A1B8D0 , 464px 886px #A1B8D0 , 514px 298px #A1B8D0 , 966px 302px #A1B8D0 , 655px 851px #A1B8D0 , 454px 154px #A1B8D0 , 245px 252px #A1B8D0 , 758px 290px #A1B8D0 , 681px 731px #A1B8D0 , 348px 689px #A1B8D0 , 697px 144px #A1B8D0 , 336px 35px #A1B8D0 , 110px 314px #A1B8D0 , 997px 235px #A1B8D0 , 27px 627px #A1B8D0 , 145px 398px #A1B8D0 , 771px 313px #A1B8D0 , 358px 86px #A1B8D0 , 919px 532px #A1B8D0 , 144px 634px #A1B8D0 , 622px 453px #A1B8D0 , 543px 474px #A1B8D0 , 174px 203px #A1B8D0 , 111px 316px #A1B8D0 , 104px 962px #A1B8D0 , 11px 7px #A1B8D0 , 164px 567px #A1B8D0 , 507px 592px #A1B8D0 , 805px 297px #A1B8D0 , 112px 731px #A1B8D0 , 227px 151px #A1B8D0 , 192px 442px #A1B8D0 , 849px 96px #A1B8D0 , 374px 624px #A1B8D0 , 271px 691px #A1B8D0 , 121px 69px #A1B8D0 , 950px 897px #A1B8D0 , 390px 794px #A1B8D0 , 317px 251px #A1B8D0 , 241px 490px #A1B8D0 , 68px 865px #A1B8D0 , 991px 70px #A1B8D0 , 107px 754px #A1B8D0 , 713px 691px #A1B8D0 , 756px 572px #A1B8D0 , 686px 420px #A1B8D0 , 431px 810px #A1B8D0 , 223px 576px #A1B8D0 , 640px 69px #A1B8D0 , 383px 538px #A1B8D0 , 873px 931px #A1B8D0 , 152px 862px #A1B8D0 , 959px 313px #A1B8D0 , 277px 373px #A1B8D0 , 153px 624px #A1B8D0 , 251px 525px #A1B8D0 , 441px 596px #A1B8D0 , 437px 499px #A1B8D0 , 619px 203px #A1B8D0 , 701px 109px #A1B8D0 , 583px 924px #A1B8D0 , 871px 232px #A1B8D0 , 909px 622px #A1B8D0 , 337px 993px #A1B8D0 , 672px 474px #A1B8D0 , 861px 255px #A1B8D0 , 358px 588px #A1B8D0 , 955px 81px #A1B8D0 , 21px 311px #A1B8D0 , 387px 693px #A1B8D0 , 183px 789px #A1B8D0 , 702px 739px #A1B8D0 , 961px 448px #A1B8D0 , 464px 546px #A1B8D0 , 521px 638px #A1B8D0 , 871px 668px #A1B8D0 , 103px 37px #A1B8D0 , 815px 925px #A1B8D0 , 891px 367px #A1B8D0 , 421px 806px #A1B8D0 , 214px 63px #A1B8D0 , 394px 515px #A1B8D0 , 861px 93px #A1B8D0 , 834px 877px #A1B8D0 , 215px 928px #A1B8D0 , 543px 819px #A1B8D0 , 734px 452px #A1B8D0 , 520px 949px #A1B8D0 , 927px 578px #A1B8D0 , 400px 808px #A1B8D0 , 657px 855px #A1B8D0 , 713px 256px #A1B8D0 , 817px 426px #A1B8D0 , 537px 568px #A1B8D0 , 927px 617px #A1B8D0 , 837px 735px #A1B8D0 , 290px 53px #A1B8D0 , 99px 345px #A1B8D0 , 521px 666px #A1B8D0 , 373px 590px #A1B8D0 , 51px 338px #A1B8D0 , 541px 39px #A1B8D0 , 769px 529px #A1B8D0 , 692px 237px #A1B8D0 , 867px 666px #A1B8D0 , 315px 849px #A1B8D0 , 945px 24px #A1B8D0 , 503px 848px #A1B8D0 , 920px 345px #A1B8D0 , 245px 262px #A1B8D0 , 310px 242px #A1B8D0 , 776px 655px #A1B8D0 , 529px 235px #A1B8D0 , 56px 771px #A1B8D0 , 946px 95px #A1B8D0 , 449px 503px #A1B8D0 , 33px 240px #A1B8D0 , 271px 637px #A1B8D0 , 420px 946px #A1B8D0 , 208px 359px #A1B8D0 , 294px 359px #A1B8D0 , 110px 25px #A1B8D0 , 79px 199px #A1B8D0 , 927px 31px #A1B8D0 , 889px 411px #A1B8D0 , 400px 188px #A1B8D0 , 871px 542px #A1B8D0 , 13px 967px #A1B8D0 , 784px 167px #A1B8D0 , 654px 576px #A1B8D0 , 796px 897px #A1B8D0 , 485px 92px #A1B8D0 , 837px 848px #A1B8D0 , 268px 642px #A1B8D0 , 203px 417px #A1B8D0 , 377px 646px #A1B8D0 , 940px 400px #A1B8D0 , 133px 55px #A1B8D0 , 400px 40px #A1B8D0 , 230px 818px #A1B8D0 , 844px 769px #A1B8D0 , 505px 723px #A1B8D0 , 970px 364px #A1B8D0 , 152px 796px #A1B8D0 , 950px 95px #A1B8D0 , 105px 465px #A1B8D0 , 81px 650px #A1B8D0 , 359px 931px #A1B8D0 , 513px 283px #A1B8D0 , 14px 136px #A1B8D0 , 354px 863px #A1B8D0 , 159px 337px #A1B8D0 , 262px 161px #A1B8D0 , 949px 959px #A1B8D0 , 992px 711px #A1B8D0 , 436px 5px #A1B8D0 , 565px 32px #A1B8D0 , 321px 961px #A1B8D0 , 370px 219px #A1B8D0 , 836px 689px #A1B8D0 , 839px 760px #A1B8D0 , 746px 744px #A1B8D0 , 724px 963px #A1B8D0 , 824px 354px #A1B8D0 , 361px 808px #A1B8D0 , 464px 280px #A1B8D0 , 427px 559px #A1B8D0 , 863px 1px #A1B8D0 , 484px 751px #A1B8D0 , 659px 471px #A1B8D0 , 940px 927px #A1B8D0 , 983px 731px #A1B8D0 , 19px 303px #A1B8D0;
  }
  .glitter_12:after {
    -moz-animation: glitter-12 9s infinite;
    -webkit-animation: glitter-12 9s infinite;
    animation: glitter-12 9s infinite;
    box-shadow: 843px 592px #A1B8D0 , 87px 18px #A1B8D0 , 976px 869px #A1B8D0 , 984px 806px #A1B8D0 , 817px 680px #A1B8D0 , 643px 119px #A1B8D0 , 404px 438px #A1B8D0 , 205px 139px #A1B8D0 , 594px 20px #A1B8D0 , 971px 583px #A1B8D0 , 618px 40px #A1B8D0 , 25px 864px #A1B8D0 , 820px 290px #A1B8D0 , 793px 811px #A1B8D0 , 883px 290px #A1B8D0 , 583px 61px #A1B8D0 , 43px 251px #A1B8D0 , 154px 235px #A1B8D0 , 701px 203px #A1B8D0 , 633px 184px #A1B8D0 , 741px 868px #A1B8D0 , 504px 842px #A1B8D0 , 714px 543px #A1B8D0 , 795px 620px #A1B8D0 , 973px 814px #A1B8D0 , 621px 7px #A1B8D0 , 973px 672px #A1B8D0 , 932px 167px #A1B8D0 , 464px 886px #A1B8D0 , 514px 298px #A1B8D0 , 966px 302px #A1B8D0 , 655px 851px #A1B8D0 , 454px 154px #A1B8D0 , 245px 252px #A1B8D0 , 758px 290px #A1B8D0 , 681px 731px #A1B8D0 , 348px 689px #A1B8D0 , 697px 144px #A1B8D0 , 336px 35px #A1B8D0 , 110px 314px #A1B8D0 , 997px 235px #A1B8D0 , 27px 627px #A1B8D0 , 145px 398px #A1B8D0 , 771px 313px #A1B8D0 , 358px 86px #A1B8D0 , 919px 532px #A1B8D0 , 144px 634px #A1B8D0 , 622px 453px #A1B8D0 , 543px 474px #A1B8D0 , 174px 203px #A1B8D0 , 111px 316px #A1B8D0 , 104px 962px #A1B8D0 , 11px 7px #A1B8D0 , 164px 567px #A1B8D0 , 507px 592px #A1B8D0 , 805px 297px #A1B8D0 , 112px 731px #A1B8D0 , 227px 151px #A1B8D0 , 192px 442px #A1B8D0 , 849px 96px #A1B8D0 , 374px 624px #A1B8D0 , 271px 691px #A1B8D0 , 121px 69px #A1B8D0 , 950px 897px #A1B8D0 , 390px 794px #A1B8D0 , 317px 251px #A1B8D0 , 241px 490px #A1B8D0 , 68px 865px #A1B8D0 , 991px 70px #A1B8D0 , 107px 754px #A1B8D0 , 713px 691px #A1B8D0 , 756px 572px #A1B8D0 , 686px 420px #A1B8D0 , 431px 810px #A1B8D0 , 223px 576px #A1B8D0 , 640px 69px #A1B8D0 , 383px 538px #A1B8D0 , 873px 931px #A1B8D0 , 152px 862px #A1B8D0 , 959px 313px #A1B8D0 , 277px 373px #A1B8D0 , 153px 624px #A1B8D0 , 251px 525px #A1B8D0 , 441px 596px #A1B8D0 , 437px 499px #A1B8D0 , 619px 203px #A1B8D0 , 701px 109px #A1B8D0 , 583px 924px #A1B8D0 , 871px 232px #A1B8D0 , 909px 622px #A1B8D0 , 337px 993px #A1B8D0 , 672px 474px #A1B8D0 , 861px 255px #A1B8D0 , 358px 588px #A1B8D0 , 955px 81px #A1B8D0 , 21px 311px #A1B8D0 , 387px 693px #A1B8D0 , 183px 789px #A1B8D0 , 702px 739px #A1B8D0 , 961px 448px #A1B8D0 , 464px 546px #A1B8D0 , 521px 638px #A1B8D0 , 871px 668px #A1B8D0 , 103px 37px #A1B8D0 , 815px 925px #A1B8D0 , 891px 367px #A1B8D0 , 421px 806px #A1B8D0 , 214px 63px #A1B8D0 , 394px 515px #A1B8D0 , 861px 93px #A1B8D0 , 834px 877px #A1B8D0 , 215px 928px #A1B8D0 , 543px 819px #A1B8D0 , 734px 452px #A1B8D0 , 520px 949px #A1B8D0 , 927px 578px #A1B8D0 , 400px 808px #A1B8D0 , 657px 855px #A1B8D0 , 713px 256px #A1B8D0 , 817px 426px #A1B8D0 , 537px 568px #A1B8D0 , 927px 617px #A1B8D0 , 837px 735px #A1B8D0 , 290px 53px #A1B8D0 , 99px 345px #A1B8D0 , 521px 666px #A1B8D0 , 373px 590px #A1B8D0 , 51px 338px #A1B8D0 , 541px 39px #A1B8D0 , 769px 529px #A1B8D0 , 692px 237px #A1B8D0 , 867px 666px #A1B8D0 , 315px 849px #A1B8D0 , 945px 24px #A1B8D0 , 503px 848px #A1B8D0 , 920px 345px #A1B8D0 , 245px 262px #A1B8D0 , 310px 242px #A1B8D0 , 776px 655px #A1B8D0 , 529px 235px #A1B8D0 , 56px 771px #A1B8D0 , 946px 95px #A1B8D0 , 449px 503px #A1B8D0 , 33px 240px #A1B8D0 , 271px 637px #A1B8D0 , 420px 946px #A1B8D0 , 208px 359px #A1B8D0 , 294px 359px #A1B8D0 , 110px 25px #A1B8D0 , 79px 199px #A1B8D0 , 927px 31px #A1B8D0 , 889px 411px #A1B8D0 , 400px 188px #A1B8D0 , 871px 542px #A1B8D0 , 13px 967px #A1B8D0 , 784px 167px #A1B8D0 , 654px 576px #A1B8D0 , 796px 897px #A1B8D0 , 485px 92px #A1B8D0 , 837px 848px #A1B8D0 , 268px 642px #A1B8D0 , 203px 417px #A1B8D0 , 377px 646px #A1B8D0 , 940px 400px #A1B8D0 , 133px 55px #A1B8D0 , 400px 40px #A1B8D0 , 230px 818px #A1B8D0 , 844px 769px #A1B8D0 , 505px 723px #A1B8D0 , 970px 364px #A1B8D0 , 152px 796px #A1B8D0 , 950px 95px #A1B8D0 , 105px 465px #A1B8D0 , 81px 650px #A1B8D0 , 359px 931px #A1B8D0 , 513px 283px #A1B8D0 , 14px 136px #A1B8D0 , 354px 863px #A1B8D0 , 159px 337px #A1B8D0 , 262px 161px #A1B8D0 , 949px 959px #A1B8D0 , 992px 711px #A1B8D0 , 436px 5px #A1B8D0 , 565px 32px #A1B8D0 , 321px 961px #A1B8D0 , 370px 219px #A1B8D0 , 836px 689px #A1B8D0 , 839px 760px #A1B8D0 , 746px 744px #A1B8D0 , 724px 963px #A1B8D0 , 824px 354px #A1B8D0 , 361px 808px #A1B8D0 , 464px 280px #A1B8D0 , 427px 559px #A1B8D0 , 863px 1px #A1B8D0 , 484px 751px #A1B8D0 , 659px 471px #A1B8D0 , 940px 927px #A1B8D0 , 983px 731px #A1B8D0 , 19px 303px #A1B8D0;
  }
  
  @-moz-keyframes glitter-13 {
    0%,
      100%,
      34.83871%,
      44.83871% {
      opacity: 0;
    }
    39.83871% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-13 {
    0%,
      100%,
      34.83871%,
      44.83871% {
      opacity: 0;
    }
    39.83871% {
      opacity: 1;
    }
  }
  @keyframes glitter-13 {
    0%,
      100%,
      34.83871%,
      44.83871% {
      opacity: 0;
    }
    39.83871% {
      opacity: 1;
    }
  }
  .glitter_13 {
    -moz-animation: glitter-13 10s infinite;
    -webkit-animation: glitter-13 10s infinite;
    animation: glitter-13 10s infinite;
    box-shadow: 630px 171px #A1B8D0 , 151px 590px #A1B8D0 , 615px 617px #A1B8D0 , 54px 984px #A1B8D0 , 765px 726px #A1B8D0 , 977px 702px #A1B8D0 , 734px 263px #A1B8D0 , 543px 112px #A1B8D0 , 733px 190px #A1B8D0 , 107px 877px #A1B8D0 , 831px 110px #A1B8D0 , 346px 519px #A1B8D0 , 631px 220px #A1B8D0 , 301px 569px #A1B8D0 , 393px 219px #A1B8D0 , 487px 39px #A1B8D0 , 376px 51px #A1B8D0 , 689px 20px #A1B8D0 , 791px 178px #A1B8D0 , 616px 17px #A1B8D0 , 478px 601px #A1B8D0 , 761px 1000px #A1B8D0 , 323px 85px #A1B8D0 , 236px 550px #A1B8D0 , 909px 22px #A1B8D0 , 109px 116px #A1B8D0 , 854px 9px #A1B8D0 , 526px 676px #A1B8D0 , 501px 388px #A1B8D0 , 995px 490px #A1B8D0 , 221px 282px #A1B8D0 , 505px 117px #A1B8D0 , 415px 610px #A1B8D0 , 951px 197px #A1B8D0 , 970px 941px #A1B8D0 , 40px 164px #A1B8D0 , 683px 968px #A1B8D0 , 495px 725px #A1B8D0 , 136px 209px #A1B8D0 , 461px 386px #A1B8D0 , 280px 734px #A1B8D0 , 957px 906px #A1B8D0 , 484px 472px #A1B8D0 , 706px 36px #A1B8D0 , 999px 702px #A1B8D0 , 512px 293px #A1B8D0 , 585px 950px #A1B8D0 , 548px 67px #A1B8D0 , 344px 511px #A1B8D0 , 428px 779px #A1B8D0 , 277px 561px #A1B8D0 , 887px 380px #A1B8D0 , 413px 895px #A1B8D0 , 916px 950px #A1B8D0 , 260px 685px #A1B8D0 , 192px 271px #A1B8D0 , 90px 139px #A1B8D0 , 823px 900px #A1B8D0 , 56px 176px #A1B8D0 , 536px 617px #A1B8D0 , 359px 901px #A1B8D0 , 698px 794px #A1B8D0 , 351px 781px #A1B8D0 , 873px 965px #A1B8D0 , 270px 473px #A1B8D0 , 769px 402px #A1B8D0 , 828px 340px #A1B8D0 , 785px 261px #A1B8D0 , 851px 769px #A1B8D0 , 872px 301px #A1B8D0 , 546px 125px #A1B8D0 , 394px 184px #A1B8D0 , 584px 337px #A1B8D0 , 869px 147px #A1B8D0 , 608px 264px #A1B8D0 , 55px 448px #A1B8D0 , 165px 572px #A1B8D0 , 99px 561px #A1B8D0 , 178px 508px #A1B8D0 , 53px 953px #A1B8D0 , 309px 668px #A1B8D0 , 782px 492px #A1B8D0 , 32px 532px #A1B8D0 , 160px 886px #A1B8D0 , 943px 870px #A1B8D0 , 916px 6px #A1B8D0 , 631px 450px #A1B8D0 , 665px 908px #A1B8D0 , 689px 703px #A1B8D0 , 574px 907px #A1B8D0 , 990px 180px #A1B8D0 , 208px 934px #A1B8D0 , 737px 38px #A1B8D0 , 512px 162px #A1B8D0 , 899px 800px #A1B8D0 , 533px 784px #A1B8D0 , 161px 706px #A1B8D0 , 377px 580px #A1B8D0 , 460px 49px #A1B8D0 , 243px 311px #A1B8D0 , 395px 904px #A1B8D0 , 986px 442px #A1B8D0 , 96px 342px #A1B8D0 , 196px 710px #A1B8D0 , 14px 406px #A1B8D0 , 558px 899px #A1B8D0 , 191px 191px #A1B8D0 , 145px 246px #A1B8D0 , 998px 790px #A1B8D0 , 877px 722px #A1B8D0 , 875px 469px #A1B8D0 , 208px 769px #A1B8D0 , 348px 875px #A1B8D0 , 640px 960px #A1B8D0 , 528px 176px #A1B8D0 , 11px 733px #A1B8D0 , 717px 394px #A1B8D0 , 809px 122px #A1B8D0 , 958px 503px #A1B8D0 , 333px 992px #A1B8D0 , 477px 416px #A1B8D0 , 942px 330px #A1B8D0 , 567px 956px #A1B8D0 , 839px 45px #A1B8D0 , 515px 347px #A1B8D0 , 472px 98px #A1B8D0 , 297px 259px #A1B8D0 , 334px 206px #A1B8D0 , 866px 601px #A1B8D0 , 227px 828px #A1B8D0 , 422px 467px #A1B8D0 , 683px 839px #A1B8D0 , 85px 912px #A1B8D0 , 67px 251px #A1B8D0 , 475px 918px #A1B8D0 , 626px 40px #A1B8D0 , 719px 533px #A1B8D0 , 580px 815px #A1B8D0 , 708px 796px #A1B8D0 , 826px 788px #A1B8D0 , 696px 78px #A1B8D0 , 7px 349px #A1B8D0 , 249px 279px #A1B8D0 , 881px 516px #A1B8D0 , 575px 573px #A1B8D0 , 971px 431px #A1B8D0 , 326px 3px #A1B8D0 , 732px 849px #A1B8D0 , 945px 152px #A1B8D0 , 302px 647px #A1B8D0 , 294px 785px #A1B8D0 , 361px 26px #A1B8D0 , 189px 190px #A1B8D0 , 988px 639px #A1B8D0 , 123px 288px #A1B8D0 , 877px 26px #A1B8D0 , 841px 144px #A1B8D0 , 790px 259px #A1B8D0 , 271px 234px #A1B8D0 , 589px 610px #A1B8D0 , 33px 2px #A1B8D0 , 222px 98px #A1B8D0 , 181px 549px #A1B8D0 , 586px 895px #A1B8D0 , 404px 930px #A1B8D0 , 881px 149px #A1B8D0 , 12px 639px #A1B8D0 , 700px 672px #A1B8D0 , 475px 366px #A1B8D0 , 992px 60px #A1B8D0 , 361px 112px #A1B8D0 , 488px 66px #A1B8D0 , 395px 173px #A1B8D0 , 19px 981px #A1B8D0 , 621px 538px #A1B8D0 , 597px 430px #A1B8D0 , 571px 894px #A1B8D0 , 13px 109px #A1B8D0 , 924px 363px #A1B8D0 , 123px 881px #A1B8D0 , 394px 611px #A1B8D0 , 40px 88px #A1B8D0 , 232px 494px #A1B8D0 , 872px 205px #A1B8D0 , 577px 339px #A1B8D0 , 654px 276px #A1B8D0 , 979px 642px #A1B8D0 , 153px 546px #A1B8D0 , 63px 436px #A1B8D0 , 779px 840px #A1B8D0 , 192px 76px #A1B8D0 , 642px 806px #A1B8D0 , 154px 597px #A1B8D0 , 67px 114px #A1B8D0 , 848px 651px #A1B8D0 , 557px 54px #A1B8D0 , 35px 125px #A1B8D0 , 443px 122px #A1B8D0 , 288px 156px #A1B8D0 , 936px 61px #A1B8D0;
  }
  .glitter_13:before {
    -moz-animation: glitter-13 8s infinite;
    -webkit-animation: glitter-13 8s infinite;
    animation: glitter-13 8s infinite;
    box-shadow: 630px 171px #A1B8D0 , 151px 590px #A1B8D0 , 615px 617px #A1B8D0 , 54px 984px #A1B8D0 , 765px 726px #A1B8D0 , 977px 702px #A1B8D0 , 734px 263px #A1B8D0 , 543px 112px #A1B8D0 , 733px 190px #A1B8D0 , 107px 877px #A1B8D0 , 831px 110px #A1B8D0 , 346px 519px #A1B8D0 , 631px 220px #A1B8D0 , 301px 569px #A1B8D0 , 393px 219px #A1B8D0 , 487px 39px #A1B8D0 , 376px 51px #A1B8D0 , 689px 20px #A1B8D0 , 791px 178px #A1B8D0 , 616px 17px #A1B8D0 , 478px 601px #A1B8D0 , 761px 1000px #A1B8D0 , 323px 85px #A1B8D0 , 236px 550px #A1B8D0 , 909px 22px #A1B8D0 , 109px 116px #A1B8D0 , 854px 9px #A1B8D0 , 526px 676px #A1B8D0 , 501px 388px #A1B8D0 , 995px 490px #A1B8D0 , 221px 282px #A1B8D0 , 505px 117px #A1B8D0 , 415px 610px #A1B8D0 , 951px 197px #A1B8D0 , 970px 941px #A1B8D0 , 40px 164px #A1B8D0 , 683px 968px #A1B8D0 , 495px 725px #A1B8D0 , 136px 209px #A1B8D0 , 461px 386px #A1B8D0 , 280px 734px #A1B8D0 , 957px 906px #A1B8D0 , 484px 472px #A1B8D0 , 706px 36px #A1B8D0 , 999px 702px #A1B8D0 , 512px 293px #A1B8D0 , 585px 950px #A1B8D0 , 548px 67px #A1B8D0 , 344px 511px #A1B8D0 , 428px 779px #A1B8D0 , 277px 561px #A1B8D0 , 887px 380px #A1B8D0 , 413px 895px #A1B8D0 , 916px 950px #A1B8D0 , 260px 685px #A1B8D0 , 192px 271px #A1B8D0 , 90px 139px #A1B8D0 , 823px 900px #A1B8D0 , 56px 176px #A1B8D0 , 536px 617px #A1B8D0 , 359px 901px #A1B8D0 , 698px 794px #A1B8D0 , 351px 781px #A1B8D0 , 873px 965px #A1B8D0 , 270px 473px #A1B8D0 , 769px 402px #A1B8D0 , 828px 340px #A1B8D0 , 785px 261px #A1B8D0 , 851px 769px #A1B8D0 , 872px 301px #A1B8D0 , 546px 125px #A1B8D0 , 394px 184px #A1B8D0 , 584px 337px #A1B8D0 , 869px 147px #A1B8D0 , 608px 264px #A1B8D0 , 55px 448px #A1B8D0 , 165px 572px #A1B8D0 , 99px 561px #A1B8D0 , 178px 508px #A1B8D0 , 53px 953px #A1B8D0 , 309px 668px #A1B8D0 , 782px 492px #A1B8D0 , 32px 532px #A1B8D0 , 160px 886px #A1B8D0 , 943px 870px #A1B8D0 , 916px 6px #A1B8D0 , 631px 450px #A1B8D0 , 665px 908px #A1B8D0 , 689px 703px #A1B8D0 , 574px 907px #A1B8D0 , 990px 180px #A1B8D0 , 208px 934px #A1B8D0 , 737px 38px #A1B8D0 , 512px 162px #A1B8D0 , 899px 800px #A1B8D0 , 533px 784px #A1B8D0 , 161px 706px #A1B8D0 , 377px 580px #A1B8D0 , 460px 49px #A1B8D0 , 243px 311px #A1B8D0 , 395px 904px #A1B8D0 , 986px 442px #A1B8D0 , 96px 342px #A1B8D0 , 196px 710px #A1B8D0 , 14px 406px #A1B8D0 , 558px 899px #A1B8D0 , 191px 191px #A1B8D0 , 145px 246px #A1B8D0 , 998px 790px #A1B8D0 , 877px 722px #A1B8D0 , 875px 469px #A1B8D0 , 208px 769px #A1B8D0 , 348px 875px #A1B8D0 , 640px 960px #A1B8D0 , 528px 176px #A1B8D0 , 11px 733px #A1B8D0 , 717px 394px #A1B8D0 , 809px 122px #A1B8D0 , 958px 503px #A1B8D0 , 333px 992px #A1B8D0 , 477px 416px #A1B8D0 , 942px 330px #A1B8D0 , 567px 956px #A1B8D0 , 839px 45px #A1B8D0 , 515px 347px #A1B8D0 , 472px 98px #A1B8D0 , 297px 259px #A1B8D0 , 334px 206px #A1B8D0 , 866px 601px #A1B8D0 , 227px 828px #A1B8D0 , 422px 467px #A1B8D0 , 683px 839px #A1B8D0 , 85px 912px #A1B8D0 , 67px 251px #A1B8D0 , 475px 918px #A1B8D0 , 626px 40px #A1B8D0 , 719px 533px #A1B8D0 , 580px 815px #A1B8D0 , 708px 796px #A1B8D0 , 826px 788px #A1B8D0 , 696px 78px #A1B8D0 , 7px 349px #A1B8D0 , 249px 279px #A1B8D0 , 881px 516px #A1B8D0 , 575px 573px #A1B8D0 , 971px 431px #A1B8D0 , 326px 3px #A1B8D0 , 732px 849px #A1B8D0 , 945px 152px #A1B8D0 , 302px 647px #A1B8D0 , 294px 785px #A1B8D0 , 361px 26px #A1B8D0 , 189px 190px #A1B8D0 , 988px 639px #A1B8D0 , 123px 288px #A1B8D0 , 877px 26px #A1B8D0 , 841px 144px #A1B8D0 , 790px 259px #A1B8D0 , 271px 234px #A1B8D0 , 589px 610px #A1B8D0 , 33px 2px #A1B8D0 , 222px 98px #A1B8D0 , 181px 549px #A1B8D0 , 586px 895px #A1B8D0 , 404px 930px #A1B8D0 , 881px 149px #A1B8D0 , 12px 639px #A1B8D0 , 700px 672px #A1B8D0 , 475px 366px #A1B8D0 , 992px 60px #A1B8D0 , 361px 112px #A1B8D0 , 488px 66px #A1B8D0 , 395px 173px #A1B8D0 , 19px 981px #A1B8D0 , 621px 538px #A1B8D0 , 597px 430px #A1B8D0 , 571px 894px #A1B8D0 , 13px 109px #A1B8D0 , 924px 363px #A1B8D0 , 123px 881px #A1B8D0 , 394px 611px #A1B8D0 , 40px 88px #A1B8D0 , 232px 494px #A1B8D0 , 872px 205px #A1B8D0 , 577px 339px #A1B8D0 , 654px 276px #A1B8D0 , 979px 642px #A1B8D0 , 153px 546px #A1B8D0 , 63px 436px #A1B8D0 , 779px 840px #A1B8D0 , 192px 76px #A1B8D0 , 642px 806px #A1B8D0 , 154px 597px #A1B8D0 , 67px 114px #A1B8D0 , 848px 651px #A1B8D0 , 557px 54px #A1B8D0 , 35px 125px #A1B8D0 , 443px 122px #A1B8D0 , 288px 156px #A1B8D0 , 936px 61px #A1B8D0;
  }
  .glitter_13:after {
    -moz-animation: glitter-13 9s infinite;
    -webkit-animation: glitter-13 9s infinite;
    animation: glitter-13 9s infinite;
    box-shadow: 630px 171px #A1B8D0 , 151px 590px #A1B8D0 , 615px 617px #A1B8D0 , 54px 984px #A1B8D0 , 765px 726px #A1B8D0 , 977px 702px #A1B8D0 , 734px 263px #A1B8D0 , 543px 112px #A1B8D0 , 733px 190px #A1B8D0 , 107px 877px #A1B8D0 , 831px 110px #A1B8D0 , 346px 519px #A1B8D0 , 631px 220px #A1B8D0 , 301px 569px #A1B8D0 , 393px 219px #A1B8D0 , 487px 39px #A1B8D0 , 376px 51px #A1B8D0 , 689px 20px #A1B8D0 , 791px 178px #A1B8D0 , 616px 17px #A1B8D0 , 478px 601px #A1B8D0 , 761px 1000px #A1B8D0 , 323px 85px #A1B8D0 , 236px 550px #A1B8D0 , 909px 22px #A1B8D0 , 109px 116px #A1B8D0 , 854px 9px #A1B8D0 , 526px 676px #A1B8D0 , 501px 388px #A1B8D0 , 995px 490px #A1B8D0 , 221px 282px #A1B8D0 , 505px 117px #A1B8D0 , 415px 610px #A1B8D0 , 951px 197px #A1B8D0 , 970px 941px #A1B8D0 , 40px 164px #A1B8D0 , 683px 968px #A1B8D0 , 495px 725px #A1B8D0 , 136px 209px #A1B8D0 , 461px 386px #A1B8D0 , 280px 734px #A1B8D0 , 957px 906px #A1B8D0 , 484px 472px #A1B8D0 , 706px 36px #A1B8D0 , 999px 702px #A1B8D0 , 512px 293px #A1B8D0 , 585px 950px #A1B8D0 , 548px 67px #A1B8D0 , 344px 511px #A1B8D0 , 428px 779px #A1B8D0 , 277px 561px #A1B8D0 , 887px 380px #A1B8D0 , 413px 895px #A1B8D0 , 916px 950px #A1B8D0 , 260px 685px #A1B8D0 , 192px 271px #A1B8D0 , 90px 139px #A1B8D0 , 823px 900px #A1B8D0 , 56px 176px #A1B8D0 , 536px 617px #A1B8D0 , 359px 901px #A1B8D0 , 698px 794px #A1B8D0 , 351px 781px #A1B8D0 , 873px 965px #A1B8D0 , 270px 473px #A1B8D0 , 769px 402px #A1B8D0 , 828px 340px #A1B8D0 , 785px 261px #A1B8D0 , 851px 769px #A1B8D0 , 872px 301px #A1B8D0 , 546px 125px #A1B8D0 , 394px 184px #A1B8D0 , 584px 337px #A1B8D0 , 869px 147px #A1B8D0 , 608px 264px #A1B8D0 , 55px 448px #A1B8D0 , 165px 572px #A1B8D0 , 99px 561px #A1B8D0 , 178px 508px #A1B8D0 , 53px 953px #A1B8D0 , 309px 668px #A1B8D0 , 782px 492px #A1B8D0 , 32px 532px #A1B8D0 , 160px 886px #A1B8D0 , 943px 870px #A1B8D0 , 916px 6px #A1B8D0 , 631px 450px #A1B8D0 , 665px 908px #A1B8D0 , 689px 703px #A1B8D0 , 574px 907px #A1B8D0 , 990px 180px #A1B8D0 , 208px 934px #A1B8D0 , 737px 38px #A1B8D0 , 512px 162px #A1B8D0 , 899px 800px #A1B8D0 , 533px 784px #A1B8D0 , 161px 706px #A1B8D0 , 377px 580px #A1B8D0 , 460px 49px #A1B8D0 , 243px 311px #A1B8D0 , 395px 904px #A1B8D0 , 986px 442px #A1B8D0 , 96px 342px #A1B8D0 , 196px 710px #A1B8D0 , 14px 406px #A1B8D0 , 558px 899px #A1B8D0 , 191px 191px #A1B8D0 , 145px 246px #A1B8D0 , 998px 790px #A1B8D0 , 877px 722px #A1B8D0 , 875px 469px #A1B8D0 , 208px 769px #A1B8D0 , 348px 875px #A1B8D0 , 640px 960px #A1B8D0 , 528px 176px #A1B8D0 , 11px 733px #A1B8D0 , 717px 394px #A1B8D0 , 809px 122px #A1B8D0 , 958px 503px #A1B8D0 , 333px 992px #A1B8D0 , 477px 416px #A1B8D0 , 942px 330px #A1B8D0 , 567px 956px #A1B8D0 , 839px 45px #A1B8D0 , 515px 347px #A1B8D0 , 472px 98px #A1B8D0 , 297px 259px #A1B8D0 , 334px 206px #A1B8D0 , 866px 601px #A1B8D0 , 227px 828px #A1B8D0 , 422px 467px #A1B8D0 , 683px 839px #A1B8D0 , 85px 912px #A1B8D0 , 67px 251px #A1B8D0 , 475px 918px #A1B8D0 , 626px 40px #A1B8D0 , 719px 533px #A1B8D0 , 580px 815px #A1B8D0 , 708px 796px #A1B8D0 , 826px 788px #A1B8D0 , 696px 78px #A1B8D0 , 7px 349px #A1B8D0 , 249px 279px #A1B8D0 , 881px 516px #A1B8D0 , 575px 573px #A1B8D0 , 971px 431px #A1B8D0 , 326px 3px #A1B8D0 , 732px 849px #A1B8D0 , 945px 152px #A1B8D0 , 302px 647px #A1B8D0 , 294px 785px #A1B8D0 , 361px 26px #A1B8D0 , 189px 190px #A1B8D0 , 988px 639px #A1B8D0 , 123px 288px #A1B8D0 , 877px 26px #A1B8D0 , 841px 144px #A1B8D0 , 790px 259px #A1B8D0 , 271px 234px #A1B8D0 , 589px 610px #A1B8D0 , 33px 2px #A1B8D0 , 222px 98px #A1B8D0 , 181px 549px #A1B8D0 , 586px 895px #A1B8D0 , 404px 930px #A1B8D0 , 881px 149px #A1B8D0 , 12px 639px #A1B8D0 , 700px 672px #A1B8D0 , 475px 366px #A1B8D0 , 992px 60px #A1B8D0 , 361px 112px #A1B8D0 , 488px 66px #A1B8D0 , 395px 173px #A1B8D0 , 19px 981px #A1B8D0 , 621px 538px #A1B8D0 , 597px 430px #A1B8D0 , 571px 894px #A1B8D0 , 13px 109px #A1B8D0 , 924px 363px #A1B8D0 , 123px 881px #A1B8D0 , 394px 611px #A1B8D0 , 40px 88px #A1B8D0 , 232px 494px #A1B8D0 , 872px 205px #A1B8D0 , 577px 339px #A1B8D0 , 654px 276px #A1B8D0 , 979px 642px #A1B8D0 , 153px 546px #A1B8D0 , 63px 436px #A1B8D0 , 779px 840px #A1B8D0 , 192px 76px #A1B8D0 , 642px 806px #A1B8D0 , 154px 597px #A1B8D0 , 67px 114px #A1B8D0 , 848px 651px #A1B8D0 , 557px 54px #A1B8D0 , 35px 125px #A1B8D0 , 443px 122px #A1B8D0 , 288px 156px #A1B8D0 , 936px 61px #A1B8D0;
  }
  
  @-moz-keyframes glitter-14 {
    0%,
      100%,
      37.74194%,
      47.74194% {
      opacity: 0;
    }
    42.74194% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-14 {
    0%,
      100%,
      37.74194%,
      47.74194% {
      opacity: 0;
    }
    42.74194% {
      opacity: 1;
    }
  }
  @keyframes glitter-14 {
    0%,
      100%,
      37.74194%,
      47.74194% {
      opacity: 0;
    }
    42.74194% {
      opacity: 1;
    }
  }
  .glitter_14 {
    -moz-animation: glitter-14 10s infinite;
    -webkit-animation: glitter-14 10s infinite;
    animation: glitter-14 10s infinite;
    box-shadow: 740px 893px #A1B8D0 , 398px 481px #A1B8D0 , 629px 553px #A1B8D0 , 763px 769px #A1B8D0 , 2px 950px #A1B8D0 , 738px 274px #A1B8D0 , 411px 368px #A1B8D0 , 344px 114px #A1B8D0 , 638px 800px #A1B8D0 , 539px 443px #A1B8D0 , 629px 858px #A1B8D0 , 350px 749px #A1B8D0 , 597px 641px #A1B8D0 , 860px 85px #A1B8D0 , 65px 867px #A1B8D0 , 389px 168px #A1B8D0 , 634px 302px #A1B8D0 , 157px 759px #A1B8D0 , 192px 848px #A1B8D0 , 527px 472px #A1B8D0 , 37px 87px #A1B8D0 , 945px 490px #A1B8D0 , 234px 988px #A1B8D0 , 659px 628px #A1B8D0 , 396px 425px #A1B8D0 , 895px 488px #A1B8D0 , 109px 607px #A1B8D0 , 913px 989px #A1B8D0 , 677px 79px #A1B8D0 , 533px 847px #A1B8D0 , 420px 804px #A1B8D0 , 483px 683px #A1B8D0 , 12px 839px #A1B8D0 , 990px 148px #A1B8D0 , 466px 71px #A1B8D0 , 172px 632px #A1B8D0 , 854px 840px #A1B8D0 , 930px 646px #A1B8D0 , 31px 569px #A1B8D0 , 322px 417px #A1B8D0 , 626px 141px #A1B8D0 , 38px 917px #A1B8D0 , 518px 452px #A1B8D0 , 581px 791px #A1B8D0 , 318px 941px #A1B8D0 , 236px 510px #A1B8D0 , 750px 691px #A1B8D0 , 231px 333px #A1B8D0 , 232px 338px #A1B8D0 , 349px 897px #A1B8D0 , 610px 942px #A1B8D0 , 393px 903px #A1B8D0 , 599px 688px #A1B8D0 , 839px 968px #A1B8D0 , 875px 34px #A1B8D0 , 750px 7px #A1B8D0 , 731px 655px #A1B8D0 , 685px 246px #A1B8D0 , 764px 182px #A1B8D0 , 403px 12px #A1B8D0 , 662px 677px #A1B8D0 , 901px 711px #A1B8D0 , 981px 275px #A1B8D0 , 44px 203px #A1B8D0 , 88px 326px #A1B8D0 , 42px 645px #A1B8D0 , 671px 731px #A1B8D0 , 889px 107px #A1B8D0 , 404px 178px #A1B8D0 , 749px 169px #A1B8D0 , 501px 595px #A1B8D0 , 796px 442px #A1B8D0 , 545px 807px #A1B8D0 , 144px 430px #A1B8D0 , 635px 396px #A1B8D0 , 710px 183px #A1B8D0 , 652px 394px #A1B8D0 , 986px 876px #A1B8D0 , 1000px 578px #A1B8D0 , 956px 664px #A1B8D0 , 503px 852px #A1B8D0 , 184px 507px #A1B8D0 , 121px 946px #A1B8D0 , 613px 558px #A1B8D0 , 715px 760px #A1B8D0 , 461px 104px #A1B8D0 , 154px 133px #A1B8D0 , 353px 289px #A1B8D0 , 13px 639px #A1B8D0 , 101px 157px #A1B8D0 , 722px 492px #A1B8D0 , 604px 102px #A1B8D0 , 392px 638px #A1B8D0 , 512px 841px #A1B8D0 , 737px 910px #A1B8D0 , 387px 276px #A1B8D0 , 253px 673px #A1B8D0 , 181px 330px #A1B8D0 , 598px 809px #A1B8D0 , 795px 178px #A1B8D0 , 913px 125px #A1B8D0 , 167px 787px #A1B8D0 , 952px 56px #A1B8D0 , 583px 489px #A1B8D0 , 363px 574px #A1B8D0 , 349px 43px #A1B8D0 , 826px 691px #A1B8D0 , 13px 825px #A1B8D0 , 318px 933px #A1B8D0 , 759px 42px #A1B8D0 , 149px 500px #A1B8D0 , 411px 601px #A1B8D0 , 488px 164px #A1B8D0 , 261px 740px #A1B8D0 , 912px 974px #A1B8D0 , 301px 455px #A1B8D0 , 961px 974px #A1B8D0 , 268px 330px #A1B8D0 , 961px 832px #A1B8D0 , 630px 649px #A1B8D0 , 868px 332px #A1B8D0 , 711px 74px #A1B8D0 , 262px 409px #A1B8D0 , 425px 772px #A1B8D0 , 878px 203px #A1B8D0 , 468px 385px #A1B8D0 , 653px 52px #A1B8D0 , 940px 146px #A1B8D0 , 928px 581px #A1B8D0 , 505px 989px #A1B8D0 , 675px 852px #A1B8D0 , 189px 938px #A1B8D0 , 998px 797px #A1B8D0 , 988px 54px #A1B8D0 , 922px 405px #A1B8D0 , 976px 563px #A1B8D0 , 418px 678px #A1B8D0 , 213px 695px #A1B8D0 , 460px 213px #A1B8D0 , 351px 761px #A1B8D0 , 680px 619px #A1B8D0 , 461px 717px #A1B8D0 , 452px 336px #A1B8D0 , 483px 496px #A1B8D0 , 547px 652px #A1B8D0 , 92px 152px #A1B8D0 , 854px 818px #A1B8D0 , 532px 452px #A1B8D0 , 541px 870px #A1B8D0 , 725px 572px #A1B8D0 , 301px 672px #A1B8D0 , 31px 699px #A1B8D0 , 403px 314px #A1B8D0 , 83px 387px #A1B8D0 , 291px 678px #A1B8D0 , 704px 956px #A1B8D0 , 181px 832px #A1B8D0 , 472px 831px #A1B8D0 , 926px 765px #A1B8D0 , 181px 806px #A1B8D0 , 418px 407px #A1B8D0 , 762px 416px #A1B8D0 , 507px 415px #A1B8D0 , 907px 744px #A1B8D0 , 627px 816px #A1B8D0 , 83px 21px #A1B8D0 , 845px 158px #A1B8D0 , 119px 282px #A1B8D0 , 51px 285px #A1B8D0 , 635px 627px #A1B8D0 , 212px 366px #A1B8D0 , 316px 355px #A1B8D0 , 932px 175px #A1B8D0 , 671px 663px #A1B8D0 , 613px 771px #A1B8D0 , 887px 530px #A1B8D0 , 735px 29px #A1B8D0 , 589px 929px #A1B8D0 , 384px 218px #A1B8D0 , 737px 555px #A1B8D0 , 448px 410px #A1B8D0 , 426px 599px #A1B8D0 , 442px 598px #A1B8D0 , 778px 262px #A1B8D0 , 259px 124px #A1B8D0 , 877px 109px #A1B8D0 , 74px 981px #A1B8D0 , 185px 793px #A1B8D0 , 574px 187px #A1B8D0 , 992px 868px #A1B8D0 , 58px 470px #A1B8D0 , 355px 589px #A1B8D0 , 925px 830px #A1B8D0 , 767px 78px #A1B8D0 , 145px 842px #A1B8D0 , 455px 502px #A1B8D0 , 627px 244px #A1B8D0 , 260px 630px #A1B8D0 , 634px 654px #A1B8D0 , 858px 888px #A1B8D0;
  }
  .glitter_14:before {
    -moz-animation: glitter-14 8s infinite;
    -webkit-animation: glitter-14 8s infinite;
    animation: glitter-14 8s infinite;
    box-shadow: 740px 893px #A1B8D0 , 398px 481px #A1B8D0 , 629px 553px #A1B8D0 , 763px 769px #A1B8D0 , 2px 950px #A1B8D0 , 738px 274px #A1B8D0 , 411px 368px #A1B8D0 , 344px 114px #A1B8D0 , 638px 800px #A1B8D0 , 539px 443px #A1B8D0 , 629px 858px #A1B8D0 , 350px 749px #A1B8D0 , 597px 641px #A1B8D0 , 860px 85px #A1B8D0 , 65px 867px #A1B8D0 , 389px 168px #A1B8D0 , 634px 302px #A1B8D0 , 157px 759px #A1B8D0 , 192px 848px #A1B8D0 , 527px 472px #A1B8D0 , 37px 87px #A1B8D0 , 945px 490px #A1B8D0 , 234px 988px #A1B8D0 , 659px 628px #A1B8D0 , 396px 425px #A1B8D0 , 895px 488px #A1B8D0 , 109px 607px #A1B8D0 , 913px 989px #A1B8D0 , 677px 79px #A1B8D0 , 533px 847px #A1B8D0 , 420px 804px #A1B8D0 , 483px 683px #A1B8D0 , 12px 839px #A1B8D0 , 990px 148px #A1B8D0 , 466px 71px #A1B8D0 , 172px 632px #A1B8D0 , 854px 840px #A1B8D0 , 930px 646px #A1B8D0 , 31px 569px #A1B8D0 , 322px 417px #A1B8D0 , 626px 141px #A1B8D0 , 38px 917px #A1B8D0 , 518px 452px #A1B8D0 , 581px 791px #A1B8D0 , 318px 941px #A1B8D0 , 236px 510px #A1B8D0 , 750px 691px #A1B8D0 , 231px 333px #A1B8D0 , 232px 338px #A1B8D0 , 349px 897px #A1B8D0 , 610px 942px #A1B8D0 , 393px 903px #A1B8D0 , 599px 688px #A1B8D0 , 839px 968px #A1B8D0 , 875px 34px #A1B8D0 , 750px 7px #A1B8D0 , 731px 655px #A1B8D0 , 685px 246px #A1B8D0 , 764px 182px #A1B8D0 , 403px 12px #A1B8D0 , 662px 677px #A1B8D0 , 901px 711px #A1B8D0 , 981px 275px #A1B8D0 , 44px 203px #A1B8D0 , 88px 326px #A1B8D0 , 42px 645px #A1B8D0 , 671px 731px #A1B8D0 , 889px 107px #A1B8D0 , 404px 178px #A1B8D0 , 749px 169px #A1B8D0 , 501px 595px #A1B8D0 , 796px 442px #A1B8D0 , 545px 807px #A1B8D0 , 144px 430px #A1B8D0 , 635px 396px #A1B8D0 , 710px 183px #A1B8D0 , 652px 394px #A1B8D0 , 986px 876px #A1B8D0 , 1000px 578px #A1B8D0 , 956px 664px #A1B8D0 , 503px 852px #A1B8D0 , 184px 507px #A1B8D0 , 121px 946px #A1B8D0 , 613px 558px #A1B8D0 , 715px 760px #A1B8D0 , 461px 104px #A1B8D0 , 154px 133px #A1B8D0 , 353px 289px #A1B8D0 , 13px 639px #A1B8D0 , 101px 157px #A1B8D0 , 722px 492px #A1B8D0 , 604px 102px #A1B8D0 , 392px 638px #A1B8D0 , 512px 841px #A1B8D0 , 737px 910px #A1B8D0 , 387px 276px #A1B8D0 , 253px 673px #A1B8D0 , 181px 330px #A1B8D0 , 598px 809px #A1B8D0 , 795px 178px #A1B8D0 , 913px 125px #A1B8D0 , 167px 787px #A1B8D0 , 952px 56px #A1B8D0 , 583px 489px #A1B8D0 , 363px 574px #A1B8D0 , 349px 43px #A1B8D0 , 826px 691px #A1B8D0 , 13px 825px #A1B8D0 , 318px 933px #A1B8D0 , 759px 42px #A1B8D0 , 149px 500px #A1B8D0 , 411px 601px #A1B8D0 , 488px 164px #A1B8D0 , 261px 740px #A1B8D0 , 912px 974px #A1B8D0 , 301px 455px #A1B8D0 , 961px 974px #A1B8D0 , 268px 330px #A1B8D0 , 961px 832px #A1B8D0 , 630px 649px #A1B8D0 , 868px 332px #A1B8D0 , 711px 74px #A1B8D0 , 262px 409px #A1B8D0 , 425px 772px #A1B8D0 , 878px 203px #A1B8D0 , 468px 385px #A1B8D0 , 653px 52px #A1B8D0 , 940px 146px #A1B8D0 , 928px 581px #A1B8D0 , 505px 989px #A1B8D0 , 675px 852px #A1B8D0 , 189px 938px #A1B8D0 , 998px 797px #A1B8D0 , 988px 54px #A1B8D0 , 922px 405px #A1B8D0 , 976px 563px #A1B8D0 , 418px 678px #A1B8D0 , 213px 695px #A1B8D0 , 460px 213px #A1B8D0 , 351px 761px #A1B8D0 , 680px 619px #A1B8D0 , 461px 717px #A1B8D0 , 452px 336px #A1B8D0 , 483px 496px #A1B8D0 , 547px 652px #A1B8D0 , 92px 152px #A1B8D0 , 854px 818px #A1B8D0 , 532px 452px #A1B8D0 , 541px 870px #A1B8D0 , 725px 572px #A1B8D0 , 301px 672px #A1B8D0 , 31px 699px #A1B8D0 , 403px 314px #A1B8D0 , 83px 387px #A1B8D0 , 291px 678px #A1B8D0 , 704px 956px #A1B8D0 , 181px 832px #A1B8D0 , 472px 831px #A1B8D0 , 926px 765px #A1B8D0 , 181px 806px #A1B8D0 , 418px 407px #A1B8D0 , 762px 416px #A1B8D0 , 507px 415px #A1B8D0 , 907px 744px #A1B8D0 , 627px 816px #A1B8D0 , 83px 21px #A1B8D0 , 845px 158px #A1B8D0 , 119px 282px #A1B8D0 , 51px 285px #A1B8D0 , 635px 627px #A1B8D0 , 212px 366px #A1B8D0 , 316px 355px #A1B8D0 , 932px 175px #A1B8D0 , 671px 663px #A1B8D0 , 613px 771px #A1B8D0 , 887px 530px #A1B8D0 , 735px 29px #A1B8D0 , 589px 929px #A1B8D0 , 384px 218px #A1B8D0 , 737px 555px #A1B8D0 , 448px 410px #A1B8D0 , 426px 599px #A1B8D0 , 442px 598px #A1B8D0 , 778px 262px #A1B8D0 , 259px 124px #A1B8D0 , 877px 109px #A1B8D0 , 74px 981px #A1B8D0 , 185px 793px #A1B8D0 , 574px 187px #A1B8D0 , 992px 868px #A1B8D0 , 58px 470px #A1B8D0 , 355px 589px #A1B8D0 , 925px 830px #A1B8D0 , 767px 78px #A1B8D0 , 145px 842px #A1B8D0 , 455px 502px #A1B8D0 , 627px 244px #A1B8D0 , 260px 630px #A1B8D0 , 634px 654px #A1B8D0 , 858px 888px #A1B8D0;
  }
  .glitter_14:after {
    -moz-animation: glitter-14 9s infinite;
    -webkit-animation: glitter-14 9s infinite;
    animation: glitter-14 9s infinite;
    box-shadow: 740px 893px #A1B8D0 , 398px 481px #A1B8D0 , 629px 553px #A1B8D0 , 763px 769px #A1B8D0 , 2px 950px #A1B8D0 , 738px 274px #A1B8D0 , 411px 368px #A1B8D0 , 344px 114px #A1B8D0 , 638px 800px #A1B8D0 , 539px 443px #A1B8D0 , 629px 858px #A1B8D0 , 350px 749px #A1B8D0 , 597px 641px #A1B8D0 , 860px 85px #A1B8D0 , 65px 867px #A1B8D0 , 389px 168px #A1B8D0 , 634px 302px #A1B8D0 , 157px 759px #A1B8D0 , 192px 848px #A1B8D0 , 527px 472px #A1B8D0 , 37px 87px #A1B8D0 , 945px 490px #A1B8D0 , 234px 988px #A1B8D0 , 659px 628px #A1B8D0 , 396px 425px #A1B8D0 , 895px 488px #A1B8D0 , 109px 607px #A1B8D0 , 913px 989px #A1B8D0 , 677px 79px #A1B8D0 , 533px 847px #A1B8D0 , 420px 804px #A1B8D0 , 483px 683px #A1B8D0 , 12px 839px #A1B8D0 , 990px 148px #A1B8D0 , 466px 71px #A1B8D0 , 172px 632px #A1B8D0 , 854px 840px #A1B8D0 , 930px 646px #A1B8D0 , 31px 569px #A1B8D0 , 322px 417px #A1B8D0 , 626px 141px #A1B8D0 , 38px 917px #A1B8D0 , 518px 452px #A1B8D0 , 581px 791px #A1B8D0 , 318px 941px #A1B8D0 , 236px 510px #A1B8D0 , 750px 691px #A1B8D0 , 231px 333px #A1B8D0 , 232px 338px #A1B8D0 , 349px 897px #A1B8D0 , 610px 942px #A1B8D0 , 393px 903px #A1B8D0 , 599px 688px #A1B8D0 , 839px 968px #A1B8D0 , 875px 34px #A1B8D0 , 750px 7px #A1B8D0 , 731px 655px #A1B8D0 , 685px 246px #A1B8D0 , 764px 182px #A1B8D0 , 403px 12px #A1B8D0 , 662px 677px #A1B8D0 , 901px 711px #A1B8D0 , 981px 275px #A1B8D0 , 44px 203px #A1B8D0 , 88px 326px #A1B8D0 , 42px 645px #A1B8D0 , 671px 731px #A1B8D0 , 889px 107px #A1B8D0 , 404px 178px #A1B8D0 , 749px 169px #A1B8D0 , 501px 595px #A1B8D0 , 796px 442px #A1B8D0 , 545px 807px #A1B8D0 , 144px 430px #A1B8D0 , 635px 396px #A1B8D0 , 710px 183px #A1B8D0 , 652px 394px #A1B8D0 , 986px 876px #A1B8D0 , 1000px 578px #A1B8D0 , 956px 664px #A1B8D0 , 503px 852px #A1B8D0 , 184px 507px #A1B8D0 , 121px 946px #A1B8D0 , 613px 558px #A1B8D0 , 715px 760px #A1B8D0 , 461px 104px #A1B8D0 , 154px 133px #A1B8D0 , 353px 289px #A1B8D0 , 13px 639px #A1B8D0 , 101px 157px #A1B8D0 , 722px 492px #A1B8D0 , 604px 102px #A1B8D0 , 392px 638px #A1B8D0 , 512px 841px #A1B8D0 , 737px 910px #A1B8D0 , 387px 276px #A1B8D0 , 253px 673px #A1B8D0 , 181px 330px #A1B8D0 , 598px 809px #A1B8D0 , 795px 178px #A1B8D0 , 913px 125px #A1B8D0 , 167px 787px #A1B8D0 , 952px 56px #A1B8D0 , 583px 489px #A1B8D0 , 363px 574px #A1B8D0 , 349px 43px #A1B8D0 , 826px 691px #A1B8D0 , 13px 825px #A1B8D0 , 318px 933px #A1B8D0 , 759px 42px #A1B8D0 , 149px 500px #A1B8D0 , 411px 601px #A1B8D0 , 488px 164px #A1B8D0 , 261px 740px #A1B8D0 , 912px 974px #A1B8D0 , 301px 455px #A1B8D0 , 961px 974px #A1B8D0 , 268px 330px #A1B8D0 , 961px 832px #A1B8D0 , 630px 649px #A1B8D0 , 868px 332px #A1B8D0 , 711px 74px #A1B8D0 , 262px 409px #A1B8D0 , 425px 772px #A1B8D0 , 878px 203px #A1B8D0 , 468px 385px #A1B8D0 , 653px 52px #A1B8D0 , 940px 146px #A1B8D0 , 928px 581px #A1B8D0 , 505px 989px #A1B8D0 , 675px 852px #A1B8D0 , 189px 938px #A1B8D0 , 998px 797px #A1B8D0 , 988px 54px #A1B8D0 , 922px 405px #A1B8D0 , 976px 563px #A1B8D0 , 418px 678px #A1B8D0 , 213px 695px #A1B8D0 , 460px 213px #A1B8D0 , 351px 761px #A1B8D0 , 680px 619px #A1B8D0 , 461px 717px #A1B8D0 , 452px 336px #A1B8D0 , 483px 496px #A1B8D0 , 547px 652px #A1B8D0 , 92px 152px #A1B8D0 , 854px 818px #A1B8D0 , 532px 452px #A1B8D0 , 541px 870px #A1B8D0 , 725px 572px #A1B8D0 , 301px 672px #A1B8D0 , 31px 699px #A1B8D0 , 403px 314px #A1B8D0 , 83px 387px #A1B8D0 , 291px 678px #A1B8D0 , 704px 956px #A1B8D0 , 181px 832px #A1B8D0 , 472px 831px #A1B8D0 , 926px 765px #A1B8D0 , 181px 806px #A1B8D0 , 418px 407px #A1B8D0 , 762px 416px #A1B8D0 , 507px 415px #A1B8D0 , 907px 744px #A1B8D0 , 627px 816px #A1B8D0 , 83px 21px #A1B8D0 , 845px 158px #A1B8D0 , 119px 282px #A1B8D0 , 51px 285px #A1B8D0 , 635px 627px #A1B8D0 , 212px 366px #A1B8D0 , 316px 355px #A1B8D0 , 932px 175px #A1B8D0 , 671px 663px #A1B8D0 , 613px 771px #A1B8D0 , 887px 530px #A1B8D0 , 735px 29px #A1B8D0 , 589px 929px #A1B8D0 , 384px 218px #A1B8D0 , 737px 555px #A1B8D0 , 448px 410px #A1B8D0 , 426px 599px #A1B8D0 , 442px 598px #A1B8D0 , 778px 262px #A1B8D0 , 259px 124px #A1B8D0 , 877px 109px #A1B8D0 , 74px 981px #A1B8D0 , 185px 793px #A1B8D0 , 574px 187px #A1B8D0 , 992px 868px #A1B8D0 , 58px 470px #A1B8D0 , 355px 589px #A1B8D0 , 925px 830px #A1B8D0 , 767px 78px #A1B8D0 , 145px 842px #A1B8D0 , 455px 502px #A1B8D0 , 627px 244px #A1B8D0 , 260px 630px #A1B8D0 , 634px 654px #A1B8D0 , 858px 888px #A1B8D0;
  }
  
  @-moz-keyframes glitter-15 {
    0%,
      100%,
      40.64516%,
      50.64516% {
      opacity: 0;
    }
    45.64516% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-15 {
    0%,
      100%,
      40.64516%,
      50.64516% {
      opacity: 0;
    }
    45.64516% {
      opacity: 1;
    }
  }
  @keyframes glitter-15 {
    0%,
      100%,
      40.64516%,
      50.64516% {
      opacity: 0;
    }
    45.64516% {
      opacity: 1;
    }
  }
  .glitter_15 {
    -moz-animation: glitter-15 10s infinite;
    -webkit-animation: glitter-15 10s infinite;
    animation: glitter-15 10s infinite;
    box-shadow: 379px 580px #A1B8D0 , 663px 253px #A1B8D0 , 907px 166px #A1B8D0 , 363px 955px #A1B8D0 , 53px 599px #A1B8D0 , 208px 777px #A1B8D0 , 404px 368px #A1B8D0 , 826px 868px #A1B8D0 , 498px 446px #A1B8D0 , 735px 255px #A1B8D0 , 310px 848px #A1B8D0 , 475px 960px #A1B8D0 , 173px 173px #A1B8D0 , 809px 664px #A1B8D0 , 426px 632px #A1B8D0 , 417px 610px #A1B8D0 , 710px 486px #A1B8D0 , 583px 24px #A1B8D0 , 165px 748px #A1B8D0 , 990px 235px #A1B8D0 , 236px 815px #A1B8D0 , 297px 304px #A1B8D0 , 840px 722px #A1B8D0 , 253px 673px #A1B8D0 , 839px 56px #A1B8D0 , 534px 911px #A1B8D0 , 315px 909px #A1B8D0 , 436px 152px #A1B8D0 , 498px 316px #A1B8D0 , 32px 473px #A1B8D0 , 840px 299px #A1B8D0 , 147px 891px #A1B8D0 , 279px 727px #A1B8D0 , 78px 418px #A1B8D0 , 140px 846px #A1B8D0 , 723px 358px #A1B8D0 , 231px 810px #A1B8D0 , 110px 319px #A1B8D0 , 417px 340px #A1B8D0 , 884px 700px #A1B8D0 , 259px 995px #A1B8D0 , 845px 528px #A1B8D0 , 962px 197px #A1B8D0 , 189px 452px #A1B8D0 , 579px 22px #A1B8D0 , 970px 962px #A1B8D0 , 330px 808px #A1B8D0 , 296px 16px #A1B8D0 , 249px 764px #A1B8D0 , 203px 587px #A1B8D0 , 924px 123px #A1B8D0 , 795px 356px #A1B8D0 , 647px 485px #A1B8D0 , 643px 47px #A1B8D0 , 688px 732px #A1B8D0 , 496px 808px #A1B8D0 , 922px 186px #A1B8D0 , 549px 616px #A1B8D0 , 576px 398px #A1B8D0 , 574px 945px #A1B8D0 , 921px 85px #A1B8D0 , 206px 376px #A1B8D0 , 682px 483px #A1B8D0 , 30px 128px #A1B8D0 , 955px 445px #A1B8D0 , 791px 996px #A1B8D0 , 962px 485px #A1B8D0 , 211px 342px #A1B8D0 , 136px 32px #A1B8D0 , 309px 874px #A1B8D0 , 97px 701px #A1B8D0 , 393px 275px #A1B8D0 , 178px 116px #A1B8D0 , 588px 339px #A1B8D0 , 259px 613px #A1B8D0 , 600px 526px #A1B8D0 , 981px 974px #A1B8D0 , 355px 671px #A1B8D0 , 334px 454px #A1B8D0 , 2px 238px #A1B8D0 , 93px 168px #A1B8D0 , 648px 63px #A1B8D0 , 775px 405px #A1B8D0 , 565px 15px #A1B8D0 , 759px 216px #A1B8D0 , 627px 268px #A1B8D0 , 945px 456px #A1B8D0 , 558px 931px #A1B8D0 , 728px 594px #A1B8D0 , 719px 971px #A1B8D0 , 512px 12px #A1B8D0 , 949px 2px #A1B8D0 , 705px 362px #A1B8D0 , 247px 709px #A1B8D0 , 852px 370px #A1B8D0 , 678px 231px #A1B8D0 , 483px 431px #A1B8D0 , 884px 269px #A1B8D0 , 608px 718px #A1B8D0 , 965px 397px #A1B8D0 , 447px 650px #A1B8D0 , 724px 488px #A1B8D0 , 243px 16px #A1B8D0 , 843px 249px #A1B8D0 , 30px 138px #A1B8D0 , 616px 907px #A1B8D0 , 75px 946px #A1B8D0 , 509px 494px #A1B8D0 , 284px 47px #A1B8D0 , 180px 827px #A1B8D0 , 124px 963px #A1B8D0 , 793px 41px #A1B8D0 , 767px 241px #A1B8D0 , 903px 156px #A1B8D0 , 145px 876px #A1B8D0 , 977px 566px #A1B8D0 , 739px 515px #A1B8D0 , 61px 158px #A1B8D0 , 18px 474px #A1B8D0 , 59px 377px #A1B8D0 , 674px 207px #A1B8D0 , 403px 240px #A1B8D0 , 558px 477px #A1B8D0 , 198px 437px #A1B8D0 , 147px 535px #A1B8D0 , 49px 358px #A1B8D0 , 89px 10px #A1B8D0 , 486px 325px #A1B8D0 , 161px 690px #A1B8D0 , 675px 673px #A1B8D0 , 859px 754px #A1B8D0 , 949px 877px #A1B8D0 , 999px 550px #A1B8D0 , 892px 30px #A1B8D0 , 724px 700px #A1B8D0 , 520px 932px #A1B8D0 , 627px 189px #A1B8D0 , 109px 324px #A1B8D0 , 658px 604px #A1B8D0 , 287px 473px #A1B8D0 , 546px 345px #A1B8D0 , 355px 337px #A1B8D0 , 252px 867px #A1B8D0 , 83px 917px #A1B8D0 , 490px 151px #A1B8D0 , 69px 103px #A1B8D0 , 739px 441px #A1B8D0 , 572px 767px #A1B8D0 , 394px 528px #A1B8D0 , 797px 138px #A1B8D0 , 526px 697px #A1B8D0 , 205px 674px #A1B8D0 , 877px 707px #A1B8D0 , 342px 86px #A1B8D0 , 69px 733px #A1B8D0 , 479px 218px #A1B8D0 , 100px 732px #A1B8D0 , 615px 756px #A1B8D0 , 732px 80px #A1B8D0 , 669px 682px #A1B8D0 , 159px 18px #A1B8D0 , 797px 987px #A1B8D0 , 424px 791px #A1B8D0 , 129px 351px #A1B8D0 , 362px 704px #A1B8D0 , 509px 514px #A1B8D0 , 853px 450px #A1B8D0 , 161px 294px #A1B8D0 , 514px 753px #A1B8D0 , 846px 25px #A1B8D0 , 38px 353px #A1B8D0 , 764px 880px #A1B8D0 , 599px 73px #A1B8D0 , 921px 897px #A1B8D0 , 71px 582px #A1B8D0 , 272px 379px #A1B8D0 , 281px 37px #A1B8D0 , 824px 313px #A1B8D0 , 267px 403px #A1B8D0 , 367px 288px #A1B8D0 , 797px 861px #A1B8D0 , 930px 760px #A1B8D0 , 908px 209px #A1B8D0 , 797px 130px #A1B8D0 , 400px 238px #A1B8D0 , 364px 564px #A1B8D0 , 261px 150px #A1B8D0 , 248px 258px #A1B8D0 , 324px 225px #A1B8D0 , 438px 430px #A1B8D0 , 774px 610px #A1B8D0 , 323px 765px #A1B8D0 , 848px 209px #A1B8D0 , 759px 288px #A1B8D0 , 143px 441px #A1B8D0 , 734px 796px #A1B8D0 , 715px 100px #A1B8D0 , 467px 748px #A1B8D0 , 720px 37px #A1B8D0 , 804px 772px #A1B8D0;
  }
  .glitter_15:before {
    -moz-animation: glitter-15 8s infinite;
    -webkit-animation: glitter-15 8s infinite;
    animation: glitter-15 8s infinite;
    box-shadow: 379px 580px #A1B8D0 , 663px 253px #A1B8D0 , 907px 166px #A1B8D0 , 363px 955px #A1B8D0 , 53px 599px #A1B8D0 , 208px 777px #A1B8D0 , 404px 368px #A1B8D0 , 826px 868px #A1B8D0 , 498px 446px #A1B8D0 , 735px 255px #A1B8D0 , 310px 848px #A1B8D0 , 475px 960px #A1B8D0 , 173px 173px #A1B8D0 , 809px 664px #A1B8D0 , 426px 632px #A1B8D0 , 417px 610px #A1B8D0 , 710px 486px #A1B8D0 , 583px 24px #A1B8D0 , 165px 748px #A1B8D0 , 990px 235px #A1B8D0 , 236px 815px #A1B8D0 , 297px 304px #A1B8D0 , 840px 722px #A1B8D0 , 253px 673px #A1B8D0 , 839px 56px #A1B8D0 , 534px 911px #A1B8D0 , 315px 909px #A1B8D0 , 436px 152px #A1B8D0 , 498px 316px #A1B8D0 , 32px 473px #A1B8D0 , 840px 299px #A1B8D0 , 147px 891px #A1B8D0 , 279px 727px #A1B8D0 , 78px 418px #A1B8D0 , 140px 846px #A1B8D0 , 723px 358px #A1B8D0 , 231px 810px #A1B8D0 , 110px 319px #A1B8D0 , 417px 340px #A1B8D0 , 884px 700px #A1B8D0 , 259px 995px #A1B8D0 , 845px 528px #A1B8D0 , 962px 197px #A1B8D0 , 189px 452px #A1B8D0 , 579px 22px #A1B8D0 , 970px 962px #A1B8D0 , 330px 808px #A1B8D0 , 296px 16px #A1B8D0 , 249px 764px #A1B8D0 , 203px 587px #A1B8D0 , 924px 123px #A1B8D0 , 795px 356px #A1B8D0 , 647px 485px #A1B8D0 , 643px 47px #A1B8D0 , 688px 732px #A1B8D0 , 496px 808px #A1B8D0 , 922px 186px #A1B8D0 , 549px 616px #A1B8D0 , 576px 398px #A1B8D0 , 574px 945px #A1B8D0 , 921px 85px #A1B8D0 , 206px 376px #A1B8D0 , 682px 483px #A1B8D0 , 30px 128px #A1B8D0 , 955px 445px #A1B8D0 , 791px 996px #A1B8D0 , 962px 485px #A1B8D0 , 211px 342px #A1B8D0 , 136px 32px #A1B8D0 , 309px 874px #A1B8D0 , 97px 701px #A1B8D0 , 393px 275px #A1B8D0 , 178px 116px #A1B8D0 , 588px 339px #A1B8D0 , 259px 613px #A1B8D0 , 600px 526px #A1B8D0 , 981px 974px #A1B8D0 , 355px 671px #A1B8D0 , 334px 454px #A1B8D0 , 2px 238px #A1B8D0 , 93px 168px #A1B8D0 , 648px 63px #A1B8D0 , 775px 405px #A1B8D0 , 565px 15px #A1B8D0 , 759px 216px #A1B8D0 , 627px 268px #A1B8D0 , 945px 456px #A1B8D0 , 558px 931px #A1B8D0 , 728px 594px #A1B8D0 , 719px 971px #A1B8D0 , 512px 12px #A1B8D0 , 949px 2px #A1B8D0 , 705px 362px #A1B8D0 , 247px 709px #A1B8D0 , 852px 370px #A1B8D0 , 678px 231px #A1B8D0 , 483px 431px #A1B8D0 , 884px 269px #A1B8D0 , 608px 718px #A1B8D0 , 965px 397px #A1B8D0 , 447px 650px #A1B8D0 , 724px 488px #A1B8D0 , 243px 16px #A1B8D0 , 843px 249px #A1B8D0 , 30px 138px #A1B8D0 , 616px 907px #A1B8D0 , 75px 946px #A1B8D0 , 509px 494px #A1B8D0 , 284px 47px #A1B8D0 , 180px 827px #A1B8D0 , 124px 963px #A1B8D0 , 793px 41px #A1B8D0 , 767px 241px #A1B8D0 , 903px 156px #A1B8D0 , 145px 876px #A1B8D0 , 977px 566px #A1B8D0 , 739px 515px #A1B8D0 , 61px 158px #A1B8D0 , 18px 474px #A1B8D0 , 59px 377px #A1B8D0 , 674px 207px #A1B8D0 , 403px 240px #A1B8D0 , 558px 477px #A1B8D0 , 198px 437px #A1B8D0 , 147px 535px #A1B8D0 , 49px 358px #A1B8D0 , 89px 10px #A1B8D0 , 486px 325px #A1B8D0 , 161px 690px #A1B8D0 , 675px 673px #A1B8D0 , 859px 754px #A1B8D0 , 949px 877px #A1B8D0 , 999px 550px #A1B8D0 , 892px 30px #A1B8D0 , 724px 700px #A1B8D0 , 520px 932px #A1B8D0 , 627px 189px #A1B8D0 , 109px 324px #A1B8D0 , 658px 604px #A1B8D0 , 287px 473px #A1B8D0 , 546px 345px #A1B8D0 , 355px 337px #A1B8D0 , 252px 867px #A1B8D0 , 83px 917px #A1B8D0 , 490px 151px #A1B8D0 , 69px 103px #A1B8D0 , 739px 441px #A1B8D0 , 572px 767px #A1B8D0 , 394px 528px #A1B8D0 , 797px 138px #A1B8D0 , 526px 697px #A1B8D0 , 205px 674px #A1B8D0 , 877px 707px #A1B8D0 , 342px 86px #A1B8D0 , 69px 733px #A1B8D0 , 479px 218px #A1B8D0 , 100px 732px #A1B8D0 , 615px 756px #A1B8D0 , 732px 80px #A1B8D0 , 669px 682px #A1B8D0 , 159px 18px #A1B8D0 , 797px 987px #A1B8D0 , 424px 791px #A1B8D0 , 129px 351px #A1B8D0 , 362px 704px #A1B8D0 , 509px 514px #A1B8D0 , 853px 450px #A1B8D0 , 161px 294px #A1B8D0 , 514px 753px #A1B8D0 , 846px 25px #A1B8D0 , 38px 353px #A1B8D0 , 764px 880px #A1B8D0 , 599px 73px #A1B8D0 , 921px 897px #A1B8D0 , 71px 582px #A1B8D0 , 272px 379px #A1B8D0 , 281px 37px #A1B8D0 , 824px 313px #A1B8D0 , 267px 403px #A1B8D0 , 367px 288px #A1B8D0 , 797px 861px #A1B8D0 , 930px 760px #A1B8D0 , 908px 209px #A1B8D0 , 797px 130px #A1B8D0 , 400px 238px #A1B8D0 , 364px 564px #A1B8D0 , 261px 150px #A1B8D0 , 248px 258px #A1B8D0 , 324px 225px #A1B8D0 , 438px 430px #A1B8D0 , 774px 610px #A1B8D0 , 323px 765px #A1B8D0 , 848px 209px #A1B8D0 , 759px 288px #A1B8D0 , 143px 441px #A1B8D0 , 734px 796px #A1B8D0 , 715px 100px #A1B8D0 , 467px 748px #A1B8D0 , 720px 37px #A1B8D0 , 804px 772px #A1B8D0;
  }
  .glitter_15:after {
    -moz-animation: glitter-15 9s infinite;
    -webkit-animation: glitter-15 9s infinite;
    animation: glitter-15 9s infinite;
    box-shadow: 379px 580px #A1B8D0 , 663px 253px #A1B8D0 , 907px 166px #A1B8D0 , 363px 955px #A1B8D0 , 53px 599px #A1B8D0 , 208px 777px #A1B8D0 , 404px 368px #A1B8D0 , 826px 868px #A1B8D0 , 498px 446px #A1B8D0 , 735px 255px #A1B8D0 , 310px 848px #A1B8D0 , 475px 960px #A1B8D0 , 173px 173px #A1B8D0 , 809px 664px #A1B8D0 , 426px 632px #A1B8D0 , 417px 610px #A1B8D0 , 710px 486px #A1B8D0 , 583px 24px #A1B8D0 , 165px 748px #A1B8D0 , 990px 235px #A1B8D0 , 236px 815px #A1B8D0 , 297px 304px #A1B8D0 , 840px 722px #A1B8D0 , 253px 673px #A1B8D0 , 839px 56px #A1B8D0 , 534px 911px #A1B8D0 , 315px 909px #A1B8D0 , 436px 152px #A1B8D0 , 498px 316px #A1B8D0 , 32px 473px #A1B8D0 , 840px 299px #A1B8D0 , 147px 891px #A1B8D0 , 279px 727px #A1B8D0 , 78px 418px #A1B8D0 , 140px 846px #A1B8D0 , 723px 358px #A1B8D0 , 231px 810px #A1B8D0 , 110px 319px #A1B8D0 , 417px 340px #A1B8D0 , 884px 700px #A1B8D0 , 259px 995px #A1B8D0 , 845px 528px #A1B8D0 , 962px 197px #A1B8D0 , 189px 452px #A1B8D0 , 579px 22px #A1B8D0 , 970px 962px #A1B8D0 , 330px 808px #A1B8D0 , 296px 16px #A1B8D0 , 249px 764px #A1B8D0 , 203px 587px #A1B8D0 , 924px 123px #A1B8D0 , 795px 356px #A1B8D0 , 647px 485px #A1B8D0 , 643px 47px #A1B8D0 , 688px 732px #A1B8D0 , 496px 808px #A1B8D0 , 922px 186px #A1B8D0 , 549px 616px #A1B8D0 , 576px 398px #A1B8D0 , 574px 945px #A1B8D0 , 921px 85px #A1B8D0 , 206px 376px #A1B8D0 , 682px 483px #A1B8D0 , 30px 128px #A1B8D0 , 955px 445px #A1B8D0 , 791px 996px #A1B8D0 , 962px 485px #A1B8D0 , 211px 342px #A1B8D0 , 136px 32px #A1B8D0 , 309px 874px #A1B8D0 , 97px 701px #A1B8D0 , 393px 275px #A1B8D0 , 178px 116px #A1B8D0 , 588px 339px #A1B8D0 , 259px 613px #A1B8D0 , 600px 526px #A1B8D0 , 981px 974px #A1B8D0 , 355px 671px #A1B8D0 , 334px 454px #A1B8D0 , 2px 238px #A1B8D0 , 93px 168px #A1B8D0 , 648px 63px #A1B8D0 , 775px 405px #A1B8D0 , 565px 15px #A1B8D0 , 759px 216px #A1B8D0 , 627px 268px #A1B8D0 , 945px 456px #A1B8D0 , 558px 931px #A1B8D0 , 728px 594px #A1B8D0 , 719px 971px #A1B8D0 , 512px 12px #A1B8D0 , 949px 2px #A1B8D0 , 705px 362px #A1B8D0 , 247px 709px #A1B8D0 , 852px 370px #A1B8D0 , 678px 231px #A1B8D0 , 483px 431px #A1B8D0 , 884px 269px #A1B8D0 , 608px 718px #A1B8D0 , 965px 397px #A1B8D0 , 447px 650px #A1B8D0 , 724px 488px #A1B8D0 , 243px 16px #A1B8D0 , 843px 249px #A1B8D0 , 30px 138px #A1B8D0 , 616px 907px #A1B8D0 , 75px 946px #A1B8D0 , 509px 494px #A1B8D0 , 284px 47px #A1B8D0 , 180px 827px #A1B8D0 , 124px 963px #A1B8D0 , 793px 41px #A1B8D0 , 767px 241px #A1B8D0 , 903px 156px #A1B8D0 , 145px 876px #A1B8D0 , 977px 566px #A1B8D0 , 739px 515px #A1B8D0 , 61px 158px #A1B8D0 , 18px 474px #A1B8D0 , 59px 377px #A1B8D0 , 674px 207px #A1B8D0 , 403px 240px #A1B8D0 , 558px 477px #A1B8D0 , 198px 437px #A1B8D0 , 147px 535px #A1B8D0 , 49px 358px #A1B8D0 , 89px 10px #A1B8D0 , 486px 325px #A1B8D0 , 161px 690px #A1B8D0 , 675px 673px #A1B8D0 , 859px 754px #A1B8D0 , 949px 877px #A1B8D0 , 999px 550px #A1B8D0 , 892px 30px #A1B8D0 , 724px 700px #A1B8D0 , 520px 932px #A1B8D0 , 627px 189px #A1B8D0 , 109px 324px #A1B8D0 , 658px 604px #A1B8D0 , 287px 473px #A1B8D0 , 546px 345px #A1B8D0 , 355px 337px #A1B8D0 , 252px 867px #A1B8D0 , 83px 917px #A1B8D0 , 490px 151px #A1B8D0 , 69px 103px #A1B8D0 , 739px 441px #A1B8D0 , 572px 767px #A1B8D0 , 394px 528px #A1B8D0 , 797px 138px #A1B8D0 , 526px 697px #A1B8D0 , 205px 674px #A1B8D0 , 877px 707px #A1B8D0 , 342px 86px #A1B8D0 , 69px 733px #A1B8D0 , 479px 218px #A1B8D0 , 100px 732px #A1B8D0 , 615px 756px #A1B8D0 , 732px 80px #A1B8D0 , 669px 682px #A1B8D0 , 159px 18px #A1B8D0 , 797px 987px #A1B8D0 , 424px 791px #A1B8D0 , 129px 351px #A1B8D0 , 362px 704px #A1B8D0 , 509px 514px #A1B8D0 , 853px 450px #A1B8D0 , 161px 294px #A1B8D0 , 514px 753px #A1B8D0 , 846px 25px #A1B8D0 , 38px 353px #A1B8D0 , 764px 880px #A1B8D0 , 599px 73px #A1B8D0 , 921px 897px #A1B8D0 , 71px 582px #A1B8D0 , 272px 379px #A1B8D0 , 281px 37px #A1B8D0 , 824px 313px #A1B8D0 , 267px 403px #A1B8D0 , 367px 288px #A1B8D0 , 797px 861px #A1B8D0 , 930px 760px #A1B8D0 , 908px 209px #A1B8D0 , 797px 130px #A1B8D0 , 400px 238px #A1B8D0 , 364px 564px #A1B8D0 , 261px 150px #A1B8D0 , 248px 258px #A1B8D0 , 324px 225px #A1B8D0 , 438px 430px #A1B8D0 , 774px 610px #A1B8D0 , 323px 765px #A1B8D0 , 848px 209px #A1B8D0 , 759px 288px #A1B8D0 , 143px 441px #A1B8D0 , 734px 796px #A1B8D0 , 715px 100px #A1B8D0 , 467px 748px #A1B8D0 , 720px 37px #A1B8D0 , 804px 772px #A1B8D0;
  }
  
  @-moz-keyframes glitter-16 {
    0%,
      100%,
      43.54839%,
      53.54839% {
      opacity: 0;
    }
    48.54839% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-16 {
    0%,
      100%,
      43.54839%,
      53.54839% {
      opacity: 0;
    }
    48.54839% {
      opacity: 1;
    }
  }
  @keyframes glitter-16 {
    0%,
      100%,
      43.54839%,
      53.54839% {
      opacity: 0;
    }
    48.54839% {
      opacity: 1;
    }
  }
  .glitter_16 {
    -moz-animation: glitter-16 10s infinite;
    -webkit-animation: glitter-16 10s infinite;
    animation: glitter-16 10s infinite;
    box-shadow: 305px 626px #A1B8D0 , 904px 476px #A1B8D0 , 686px 492px #A1B8D0 , 552px 624px #A1B8D0 , 845px 840px #A1B8D0 , 980px 220px #A1B8D0 , 60px 832px #A1B8D0 , 370px 468px #A1B8D0 , 445px 274px #A1B8D0 , 232px 479px #A1B8D0 , 836px 573px #A1B8D0 , 429px 846px #A1B8D0 , 603px 792px #A1B8D0 , 303px 432px #A1B8D0 , 349px 937px #A1B8D0 , 750px 478px #A1B8D0 , 428px 609px #A1B8D0 , 549px 975px #A1B8D0 , 389px 273px #A1B8D0 , 278px 356px #A1B8D0 , 755px 719px #A1B8D0 , 825px 219px #A1B8D0 , 940px 553px #A1B8D0 , 508px 899px #A1B8D0 , 447px 312px #A1B8D0 , 363px 640px #A1B8D0 , 538px 303px #A1B8D0 , 185px 307px #A1B8D0 , 862px 674px #A1B8D0 , 161px 875px #A1B8D0 , 191px 505px #A1B8D0 , 136px 555px #A1B8D0 , 31px 427px #A1B8D0 , 133px 994px #A1B8D0 , 4px 935px #A1B8D0 , 765px 496px #A1B8D0 , 120px 658px #A1B8D0 , 248px 790px #A1B8D0 , 977px 956px #A1B8D0 , 268px 160px #A1B8D0 , 638px 275px #A1B8D0 , 622px 914px #A1B8D0 , 856px 26px #A1B8D0 , 640px 193px #A1B8D0 , 443px 923px #A1B8D0 , 596px 518px #A1B8D0 , 195px 282px #A1B8D0 , 465px 618px #A1B8D0 , 914px 824px #A1B8D0 , 698px 11px #A1B8D0 , 776px 72px #A1B8D0 , 617px 224px #A1B8D0 , 858px 762px #A1B8D0 , 954px 535px #A1B8D0 , 16px 534px #A1B8D0 , 299px 177px #A1B8D0 , 500px 234px #A1B8D0 , 716px 691px #A1B8D0 , 716px 645px #A1B8D0 , 448px 127px #A1B8D0 , 96px 660px #A1B8D0 , 289px 222px #A1B8D0 , 494px 746px #A1B8D0 , 583px 434px #A1B8D0 , 614px 178px #A1B8D0 , 600px 4px #A1B8D0 , 281px 42px #A1B8D0 , 125px 909px #A1B8D0 , 703px 624px #A1B8D0 , 930px 541px #A1B8D0 , 897px 934px #A1B8D0 , 207px 888px #A1B8D0 , 364px 87px #A1B8D0 , 794px 445px #A1B8D0 , 736px 245px #A1B8D0 , 25px 157px #A1B8D0 , 333px 611px #A1B8D0 , 1px 862px #A1B8D0 , 746px 549px #A1B8D0 , 652px 643px #A1B8D0 , 877px 632px #A1B8D0 , 285px 321px #A1B8D0 , 15px 896px #A1B8D0 , 444px 29px #A1B8D0 , 552px 404px #A1B8D0 , 146px 642px #A1B8D0 , 105px 615px #A1B8D0 , 798px 393px #A1B8D0 , 681px 34px #A1B8D0 , 453px 630px #A1B8D0 , 406px 129px #A1B8D0 , 255px 491px #A1B8D0 , 941px 763px #A1B8D0 , 832px 315px #A1B8D0 , 468px 140px #A1B8D0 , 634px 948px #A1B8D0 , 311px 304px #A1B8D0 , 604px 959px #A1B8D0 , 231px 560px #A1B8D0 , 25px 196px #A1B8D0 , 216px 577px #A1B8D0 , 729px 801px #A1B8D0 , 405px 229px #A1B8D0 , 487px 934px #A1B8D0 , 796px 826px #A1B8D0 , 857px 617px #A1B8D0 , 125px 961px #A1B8D0 , 227px 954px #A1B8D0 , 795px 370px #A1B8D0 , 789px 80px #A1B8D0 , 704px 531px #A1B8D0 , 922px 488px #A1B8D0 , 151px 453px #A1B8D0 , 521px 181px #A1B8D0 , 400px 781px #A1B8D0 , 309px 242px #A1B8D0 , 326px 360px #A1B8D0 , 854px 405px #A1B8D0 , 12px 45px #A1B8D0 , 482px 788px #A1B8D0 , 546px 968px #A1B8D0 , 701px 39px #A1B8D0 , 236px 588px #A1B8D0 , 515px 818px #A1B8D0 , 194px 866px #A1B8D0 , 788px 145px #A1B8D0 , 125px 102px #A1B8D0 , 552px 899px #A1B8D0 , 441px 667px #A1B8D0 , 94px 176px #A1B8D0 , 410px 1000px #A1B8D0 , 841px 543px #A1B8D0 , 870px 238px #A1B8D0 , 689px 41px #A1B8D0 , 925px 979px #A1B8D0 , 991px 903px #A1B8D0 , 581px 905px #A1B8D0 , 267px 951px #A1B8D0 , 223px 594px #A1B8D0 , 509px 954px #A1B8D0 , 861px 213px #A1B8D0 , 27px 159px #A1B8D0 , 898px 127px #A1B8D0 , 226px 191px #A1B8D0 , 693px 876px #A1B8D0 , 795px 806px #A1B8D0 , 846px 757px #A1B8D0 , 544px 669px #A1B8D0 , 935px 666px #A1B8D0 , 717px 369px #A1B8D0 , 404px 718px #A1B8D0 , 167px 37px #A1B8D0 , 775px 732px #A1B8D0 , 244px 405px #A1B8D0 , 237px 367px #A1B8D0 , 745px 647px #A1B8D0 , 803px 863px #A1B8D0 , 288px 214px #A1B8D0 , 526px 321px #A1B8D0 , 284px 668px #A1B8D0 , 304px 549px #A1B8D0 , 474px 771px #A1B8D0 , 516px 968px #A1B8D0 , 400px 910px #A1B8D0 , 427px 206px #A1B8D0 , 493px 572px #A1B8D0 , 761px 360px #A1B8D0 , 156px 386px #A1B8D0 , 767px 246px #A1B8D0 , 32px 635px #A1B8D0 , 161px 460px #A1B8D0 , 444px 127px #A1B8D0 , 33px 728px #A1B8D0 , 230px 769px #A1B8D0 , 992px 501px #A1B8D0 , 320px 638px #A1B8D0 , 157px 671px #A1B8D0 , 94px 37px #A1B8D0 , 501px 694px #A1B8D0 , 338px 628px #A1B8D0 , 29px 456px #A1B8D0 , 261px 147px #A1B8D0 , 5px 970px #A1B8D0 , 956px 79px #A1B8D0 , 860px 794px #A1B8D0 , 44px 638px #A1B8D0 , 840px 939px #A1B8D0 , 199px 599px #A1B8D0 , 938px 220px #A1B8D0 , 506px 444px #A1B8D0 , 159px 490px #A1B8D0 , 16px 213px #A1B8D0 , 90px 223px #A1B8D0 , 393px 310px #A1B8D0 , 515px 353px #A1B8D0 , 523px 214px #A1B8D0 , 180px 461px #A1B8D0 , 258px 736px #A1B8D0 , 544px 783px #A1B8D0 , 861px 691px #A1B8D0;
  }
  .glitter_16:before {
    -moz-animation: glitter-16 8s infinite;
    -webkit-animation: glitter-16 8s infinite;
    animation: glitter-16 8s infinite;
    box-shadow: 305px 626px #A1B8D0 , 904px 476px #A1B8D0 , 686px 492px #A1B8D0 , 552px 624px #A1B8D0 , 845px 840px #A1B8D0 , 980px 220px #A1B8D0 , 60px 832px #A1B8D0 , 370px 468px #A1B8D0 , 445px 274px #A1B8D0 , 232px 479px #A1B8D0 , 836px 573px #A1B8D0 , 429px 846px #A1B8D0 , 603px 792px #A1B8D0 , 303px 432px #A1B8D0 , 349px 937px #A1B8D0 , 750px 478px #A1B8D0 , 428px 609px #A1B8D0 , 549px 975px #A1B8D0 , 389px 273px #A1B8D0 , 278px 356px #A1B8D0 , 755px 719px #A1B8D0 , 825px 219px #A1B8D0 , 940px 553px #A1B8D0 , 508px 899px #A1B8D0 , 447px 312px #A1B8D0 , 363px 640px #A1B8D0 , 538px 303px #A1B8D0 , 185px 307px #A1B8D0 , 862px 674px #A1B8D0 , 161px 875px #A1B8D0 , 191px 505px #A1B8D0 , 136px 555px #A1B8D0 , 31px 427px #A1B8D0 , 133px 994px #A1B8D0 , 4px 935px #A1B8D0 , 765px 496px #A1B8D0 , 120px 658px #A1B8D0 , 248px 790px #A1B8D0 , 977px 956px #A1B8D0 , 268px 160px #A1B8D0 , 638px 275px #A1B8D0 , 622px 914px #A1B8D0 , 856px 26px #A1B8D0 , 640px 193px #A1B8D0 , 443px 923px #A1B8D0 , 596px 518px #A1B8D0 , 195px 282px #A1B8D0 , 465px 618px #A1B8D0 , 914px 824px #A1B8D0 , 698px 11px #A1B8D0 , 776px 72px #A1B8D0 , 617px 224px #A1B8D0 , 858px 762px #A1B8D0 , 954px 535px #A1B8D0 , 16px 534px #A1B8D0 , 299px 177px #A1B8D0 , 500px 234px #A1B8D0 , 716px 691px #A1B8D0 , 716px 645px #A1B8D0 , 448px 127px #A1B8D0 , 96px 660px #A1B8D0 , 289px 222px #A1B8D0 , 494px 746px #A1B8D0 , 583px 434px #A1B8D0 , 614px 178px #A1B8D0 , 600px 4px #A1B8D0 , 281px 42px #A1B8D0 , 125px 909px #A1B8D0 , 703px 624px #A1B8D0 , 930px 541px #A1B8D0 , 897px 934px #A1B8D0 , 207px 888px #A1B8D0 , 364px 87px #A1B8D0 , 794px 445px #A1B8D0 , 736px 245px #A1B8D0 , 25px 157px #A1B8D0 , 333px 611px #A1B8D0 , 1px 862px #A1B8D0 , 746px 549px #A1B8D0 , 652px 643px #A1B8D0 , 877px 632px #A1B8D0 , 285px 321px #A1B8D0 , 15px 896px #A1B8D0 , 444px 29px #A1B8D0 , 552px 404px #A1B8D0 , 146px 642px #A1B8D0 , 105px 615px #A1B8D0 , 798px 393px #A1B8D0 , 681px 34px #A1B8D0 , 453px 630px #A1B8D0 , 406px 129px #A1B8D0 , 255px 491px #A1B8D0 , 941px 763px #A1B8D0 , 832px 315px #A1B8D0 , 468px 140px #A1B8D0 , 634px 948px #A1B8D0 , 311px 304px #A1B8D0 , 604px 959px #A1B8D0 , 231px 560px #A1B8D0 , 25px 196px #A1B8D0 , 216px 577px #A1B8D0 , 729px 801px #A1B8D0 , 405px 229px #A1B8D0 , 487px 934px #A1B8D0 , 796px 826px #A1B8D0 , 857px 617px #A1B8D0 , 125px 961px #A1B8D0 , 227px 954px #A1B8D0 , 795px 370px #A1B8D0 , 789px 80px #A1B8D0 , 704px 531px #A1B8D0 , 922px 488px #A1B8D0 , 151px 453px #A1B8D0 , 521px 181px #A1B8D0 , 400px 781px #A1B8D0 , 309px 242px #A1B8D0 , 326px 360px #A1B8D0 , 854px 405px #A1B8D0 , 12px 45px #A1B8D0 , 482px 788px #A1B8D0 , 546px 968px #A1B8D0 , 701px 39px #A1B8D0 , 236px 588px #A1B8D0 , 515px 818px #A1B8D0 , 194px 866px #A1B8D0 , 788px 145px #A1B8D0 , 125px 102px #A1B8D0 , 552px 899px #A1B8D0 , 441px 667px #A1B8D0 , 94px 176px #A1B8D0 , 410px 1000px #A1B8D0 , 841px 543px #A1B8D0 , 870px 238px #A1B8D0 , 689px 41px #A1B8D0 , 925px 979px #A1B8D0 , 991px 903px #A1B8D0 , 581px 905px #A1B8D0 , 267px 951px #A1B8D0 , 223px 594px #A1B8D0 , 509px 954px #A1B8D0 , 861px 213px #A1B8D0 , 27px 159px #A1B8D0 , 898px 127px #A1B8D0 , 226px 191px #A1B8D0 , 693px 876px #A1B8D0 , 795px 806px #A1B8D0 , 846px 757px #A1B8D0 , 544px 669px #A1B8D0 , 935px 666px #A1B8D0 , 717px 369px #A1B8D0 , 404px 718px #A1B8D0 , 167px 37px #A1B8D0 , 775px 732px #A1B8D0 , 244px 405px #A1B8D0 , 237px 367px #A1B8D0 , 745px 647px #A1B8D0 , 803px 863px #A1B8D0 , 288px 214px #A1B8D0 , 526px 321px #A1B8D0 , 284px 668px #A1B8D0 , 304px 549px #A1B8D0 , 474px 771px #A1B8D0 , 516px 968px #A1B8D0 , 400px 910px #A1B8D0 , 427px 206px #A1B8D0 , 493px 572px #A1B8D0 , 761px 360px #A1B8D0 , 156px 386px #A1B8D0 , 767px 246px #A1B8D0 , 32px 635px #A1B8D0 , 161px 460px #A1B8D0 , 444px 127px #A1B8D0 , 33px 728px #A1B8D0 , 230px 769px #A1B8D0 , 992px 501px #A1B8D0 , 320px 638px #A1B8D0 , 157px 671px #A1B8D0 , 94px 37px #A1B8D0 , 501px 694px #A1B8D0 , 338px 628px #A1B8D0 , 29px 456px #A1B8D0 , 261px 147px #A1B8D0 , 5px 970px #A1B8D0 , 956px 79px #A1B8D0 , 860px 794px #A1B8D0 , 44px 638px #A1B8D0 , 840px 939px #A1B8D0 , 199px 599px #A1B8D0 , 938px 220px #A1B8D0 , 506px 444px #A1B8D0 , 159px 490px #A1B8D0 , 16px 213px #A1B8D0 , 90px 223px #A1B8D0 , 393px 310px #A1B8D0 , 515px 353px #A1B8D0 , 523px 214px #A1B8D0 , 180px 461px #A1B8D0 , 258px 736px #A1B8D0 , 544px 783px #A1B8D0 , 861px 691px #A1B8D0;
  }
  .glitter_16:after {
    -moz-animation: glitter-16 9s infinite;
    -webkit-animation: glitter-16 9s infinite;
    animation: glitter-16 9s infinite;
    box-shadow: 305px 626px #A1B8D0 , 904px 476px #A1B8D0 , 686px 492px #A1B8D0 , 552px 624px #A1B8D0 , 845px 840px #A1B8D0 , 980px 220px #A1B8D0 , 60px 832px #A1B8D0 , 370px 468px #A1B8D0 , 445px 274px #A1B8D0 , 232px 479px #A1B8D0 , 836px 573px #A1B8D0 , 429px 846px #A1B8D0 , 603px 792px #A1B8D0 , 303px 432px #A1B8D0 , 349px 937px #A1B8D0 , 750px 478px #A1B8D0 , 428px 609px #A1B8D0 , 549px 975px #A1B8D0 , 389px 273px #A1B8D0 , 278px 356px #A1B8D0 , 755px 719px #A1B8D0 , 825px 219px #A1B8D0 , 940px 553px #A1B8D0 , 508px 899px #A1B8D0 , 447px 312px #A1B8D0 , 363px 640px #A1B8D0 , 538px 303px #A1B8D0 , 185px 307px #A1B8D0 , 862px 674px #A1B8D0 , 161px 875px #A1B8D0 , 191px 505px #A1B8D0 , 136px 555px #A1B8D0 , 31px 427px #A1B8D0 , 133px 994px #A1B8D0 , 4px 935px #A1B8D0 , 765px 496px #A1B8D0 , 120px 658px #A1B8D0 , 248px 790px #A1B8D0 , 977px 956px #A1B8D0 , 268px 160px #A1B8D0 , 638px 275px #A1B8D0 , 622px 914px #A1B8D0 , 856px 26px #A1B8D0 , 640px 193px #A1B8D0 , 443px 923px #A1B8D0 , 596px 518px #A1B8D0 , 195px 282px #A1B8D0 , 465px 618px #A1B8D0 , 914px 824px #A1B8D0 , 698px 11px #A1B8D0 , 776px 72px #A1B8D0 , 617px 224px #A1B8D0 , 858px 762px #A1B8D0 , 954px 535px #A1B8D0 , 16px 534px #A1B8D0 , 299px 177px #A1B8D0 , 500px 234px #A1B8D0 , 716px 691px #A1B8D0 , 716px 645px #A1B8D0 , 448px 127px #A1B8D0 , 96px 660px #A1B8D0 , 289px 222px #A1B8D0 , 494px 746px #A1B8D0 , 583px 434px #A1B8D0 , 614px 178px #A1B8D0 , 600px 4px #A1B8D0 , 281px 42px #A1B8D0 , 125px 909px #A1B8D0 , 703px 624px #A1B8D0 , 930px 541px #A1B8D0 , 897px 934px #A1B8D0 , 207px 888px #A1B8D0 , 364px 87px #A1B8D0 , 794px 445px #A1B8D0 , 736px 245px #A1B8D0 , 25px 157px #A1B8D0 , 333px 611px #A1B8D0 , 1px 862px #A1B8D0 , 746px 549px #A1B8D0 , 652px 643px #A1B8D0 , 877px 632px #A1B8D0 , 285px 321px #A1B8D0 , 15px 896px #A1B8D0 , 444px 29px #A1B8D0 , 552px 404px #A1B8D0 , 146px 642px #A1B8D0 , 105px 615px #A1B8D0 , 798px 393px #A1B8D0 , 681px 34px #A1B8D0 , 453px 630px #A1B8D0 , 406px 129px #A1B8D0 , 255px 491px #A1B8D0 , 941px 763px #A1B8D0 , 832px 315px #A1B8D0 , 468px 140px #A1B8D0 , 634px 948px #A1B8D0 , 311px 304px #A1B8D0 , 604px 959px #A1B8D0 , 231px 560px #A1B8D0 , 25px 196px #A1B8D0 , 216px 577px #A1B8D0 , 729px 801px #A1B8D0 , 405px 229px #A1B8D0 , 487px 934px #A1B8D0 , 796px 826px #A1B8D0 , 857px 617px #A1B8D0 , 125px 961px #A1B8D0 , 227px 954px #A1B8D0 , 795px 370px #A1B8D0 , 789px 80px #A1B8D0 , 704px 531px #A1B8D0 , 922px 488px #A1B8D0 , 151px 453px #A1B8D0 , 521px 181px #A1B8D0 , 400px 781px #A1B8D0 , 309px 242px #A1B8D0 , 326px 360px #A1B8D0 , 854px 405px #A1B8D0 , 12px 45px #A1B8D0 , 482px 788px #A1B8D0 , 546px 968px #A1B8D0 , 701px 39px #A1B8D0 , 236px 588px #A1B8D0 , 515px 818px #A1B8D0 , 194px 866px #A1B8D0 , 788px 145px #A1B8D0 , 125px 102px #A1B8D0 , 552px 899px #A1B8D0 , 441px 667px #A1B8D0 , 94px 176px #A1B8D0 , 410px 1000px #A1B8D0 , 841px 543px #A1B8D0 , 870px 238px #A1B8D0 , 689px 41px #A1B8D0 , 925px 979px #A1B8D0 , 991px 903px #A1B8D0 , 581px 905px #A1B8D0 , 267px 951px #A1B8D0 , 223px 594px #A1B8D0 , 509px 954px #A1B8D0 , 861px 213px #A1B8D0 , 27px 159px #A1B8D0 , 898px 127px #A1B8D0 , 226px 191px #A1B8D0 , 693px 876px #A1B8D0 , 795px 806px #A1B8D0 , 846px 757px #A1B8D0 , 544px 669px #A1B8D0 , 935px 666px #A1B8D0 , 717px 369px #A1B8D0 , 404px 718px #A1B8D0 , 167px 37px #A1B8D0 , 775px 732px #A1B8D0 , 244px 405px #A1B8D0 , 237px 367px #A1B8D0 , 745px 647px #A1B8D0 , 803px 863px #A1B8D0 , 288px 214px #A1B8D0 , 526px 321px #A1B8D0 , 284px 668px #A1B8D0 , 304px 549px #A1B8D0 , 474px 771px #A1B8D0 , 516px 968px #A1B8D0 , 400px 910px #A1B8D0 , 427px 206px #A1B8D0 , 493px 572px #A1B8D0 , 761px 360px #A1B8D0 , 156px 386px #A1B8D0 , 767px 246px #A1B8D0 , 32px 635px #A1B8D0 , 161px 460px #A1B8D0 , 444px 127px #A1B8D0 , 33px 728px #A1B8D0 , 230px 769px #A1B8D0 , 992px 501px #A1B8D0 , 320px 638px #A1B8D0 , 157px 671px #A1B8D0 , 94px 37px #A1B8D0 , 501px 694px #A1B8D0 , 338px 628px #A1B8D0 , 29px 456px #A1B8D0 , 261px 147px #A1B8D0 , 5px 970px #A1B8D0 , 956px 79px #A1B8D0 , 860px 794px #A1B8D0 , 44px 638px #A1B8D0 , 840px 939px #A1B8D0 , 199px 599px #A1B8D0 , 938px 220px #A1B8D0 , 506px 444px #A1B8D0 , 159px 490px #A1B8D0 , 16px 213px #A1B8D0 , 90px 223px #A1B8D0 , 393px 310px #A1B8D0 , 515px 353px #A1B8D0 , 523px 214px #A1B8D0 , 180px 461px #A1B8D0 , 258px 736px #A1B8D0 , 544px 783px #A1B8D0 , 861px 691px #A1B8D0;
  }
  
  @-moz-keyframes glitter-17 {
    0%,
      100%,
      46.45161%,
      56.45161% {
      opacity: 0;
    }
    51.45161% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-17 {
    0%,
      100%,
      46.45161%,
      56.45161% {
      opacity: 0;
    }
    51.45161% {
      opacity: 1;
    }
  }
  @keyframes glitter-17 {
    0%,
      100%,
      46.45161%,
      56.45161% {
      opacity: 0;
    }
    51.45161% {
      opacity: 1;
    }
  }
  .glitter_17 {
    -moz-animation: glitter-17 10s infinite;
    -webkit-animation: glitter-17 10s infinite;
    animation: glitter-17 10s infinite;
    box-shadow: 834px 560px #A1B8D0 , 30px 226px #A1B8D0 , 296px 170px #A1B8D0 , 517px 179px #A1B8D0 , 851px 921px #A1B8D0 , 409px 43px #A1B8D0 , 799px 514px #A1B8D0 , 339px 28px #A1B8D0 , 597px 660px #A1B8D0 , 910px 501px #A1B8D0 , 76px 252px #A1B8D0 , 793px 574px #A1B8D0 , 226px 519px #A1B8D0 , 172px 810px #A1B8D0 , 346px 674px #A1B8D0 , 55px 495px #A1B8D0 , 844px 107px #A1B8D0 , 43px 22px #A1B8D0 , 678px 40px #A1B8D0 , 569px 34px #A1B8D0 , 191px 187px #A1B8D0 , 914px 267px #A1B8D0 , 443px 561px #A1B8D0 , 636px 320px #A1B8D0 , 235px 918px #A1B8D0 , 647px 845px #A1B8D0 , 806px 858px #A1B8D0 , 762px 839px #A1B8D0 , 33px 924px #A1B8D0 , 203px 445px #A1B8D0 , 98px 946px #A1B8D0 , 379px 563px #A1B8D0 , 412px 69px #A1B8D0 , 712px 758px #A1B8D0 , 323px 463px #A1B8D0 , 193px 551px #A1B8D0 , 270px 722px #A1B8D0 , 604px 774px #A1B8D0 , 60px 496px #A1B8D0 , 732px 71px #A1B8D0 , 671px 87px #A1B8D0 , 80px 670px #A1B8D0 , 388px 447px #A1B8D0 , 809px 194px #A1B8D0 , 361px 67px #A1B8D0 , 565px 147px #A1B8D0 , 582px 600px #A1B8D0 , 411px 630px #A1B8D0 , 621px 430px #A1B8D0 , 280px 37px #A1B8D0 , 828px 862px #A1B8D0 , 837px 719px #A1B8D0 , 31px 252px #A1B8D0 , 658px 225px #A1B8D0 , 506px 889px #A1B8D0 , 507px 509px #A1B8D0 , 360px 178px #A1B8D0 , 650px 167px #A1B8D0 , 368px 327px #A1B8D0 , 480px 270px #A1B8D0 , 623px 900px #A1B8D0 , 722px 905px #A1B8D0 , 148px 702px #A1B8D0 , 966px 554px #A1B8D0 , 134px 155px #A1B8D0 , 219px 626px #A1B8D0 , 94px 171px #A1B8D0 , 991px 767px #A1B8D0 , 141px 35px #A1B8D0 , 77px 368px #A1B8D0 , 507px 397px #A1B8D0 , 23px 516px #A1B8D0 , 468px 254px #A1B8D0 , 869px 28px #A1B8D0 , 320px 9px #A1B8D0 , 177px 50px #A1B8D0 , 842px 786px #A1B8D0 , 356px 590px #A1B8D0 , 787px 878px #A1B8D0 , 26px 709px #A1B8D0 , 376px 994px #A1B8D0 , 439px 71px #A1B8D0 , 40px 368px #A1B8D0 , 554px 221px #A1B8D0 , 866px 576px #A1B8D0 , 454px 768px #A1B8D0 , 41px 172px #A1B8D0 , 74px 334px #A1B8D0 , 813px 593px #A1B8D0 , 346px 396px #A1B8D0 , 551px 129px #A1B8D0 , 32px 647px #A1B8D0 , 414px 562px #A1B8D0 , 20px 63px #A1B8D0 , 928px 200px #A1B8D0 , 942px 786px #A1B8D0 , 200px 921px #A1B8D0 , 279px 269px #A1B8D0 , 567px 701px #A1B8D0 , 884px 35px #A1B8D0 , 888px 996px #A1B8D0 , 931px 35px #A1B8D0 , 823px 356px #A1B8D0 , 310px 943px #A1B8D0 , 723px 501px #A1B8D0 , 273px 558px #A1B8D0 , 898px 661px #A1B8D0 , 771px 993px #A1B8D0 , 587px 81px #A1B8D0 , 956px 80px #A1B8D0 , 938px 871px #A1B8D0 , 724px 617px #A1B8D0 , 478px 60px #A1B8D0 , 955px 210px #A1B8D0 , 725px 494px #A1B8D0 , 239px 537px #A1B8D0 , 837px 684px #A1B8D0 , 211px 518px #A1B8D0 , 897px 361px #A1B8D0 , 872px 134px #A1B8D0 , 125px 713px #A1B8D0 , 543px 110px #A1B8D0 , 554px 476px #A1B8D0 , 364px 990px #A1B8D0 , 833px 966px #A1B8D0 , 689px 715px #A1B8D0 , 938px 250px #A1B8D0 , 583px 40px #A1B8D0 , 246px 544px #A1B8D0 , 194px 160px #A1B8D0 , 870px 538px #A1B8D0 , 735px 268px #A1B8D0 , 716px 274px #A1B8D0 , 157px 618px #A1B8D0 , 142px 611px #A1B8D0 , 448px 858px #A1B8D0 , 939px 42px #A1B8D0 , 393px 589px #A1B8D0 , 515px 428px #A1B8D0 , 57px 348px #A1B8D0 , 758px 725px #A1B8D0 , 469px 257px #A1B8D0 , 543px 419px #A1B8D0 , 532px 608px #A1B8D0 , 579px 44px #A1B8D0 , 722px 666px #A1B8D0 , 969px 837px #A1B8D0 , 503px 476px #A1B8D0 , 442px 666px #A1B8D0 , 126px 600px #A1B8D0 , 830px 688px #A1B8D0 , 459px 416px #A1B8D0 , 359px 104px #A1B8D0 , 155px 159px #A1B8D0 , 860px 125px #A1B8D0 , 701px 510px #A1B8D0 , 265px 106px #A1B8D0 , 628px 48px #A1B8D0 , 159px 768px #A1B8D0 , 715px 681px #A1B8D0 , 589px 253px #A1B8D0 , 272px 636px #A1B8D0 , 763px 687px #A1B8D0 , 874px 159px #A1B8D0 , 400px 229px #A1B8D0 , 416px 258px #A1B8D0 , 872px 68px #A1B8D0 , 497px 577px #A1B8D0 , 929px 727px #A1B8D0 , 202px 649px #A1B8D0 , 749px 368px #A1B8D0 , 800px 815px #A1B8D0 , 352px 610px #A1B8D0 , 368px 240px #A1B8D0 , 693px 244px #A1B8D0 , 558px 902px #A1B8D0 , 308px 891px #A1B8D0 , 274px 654px #A1B8D0 , 538px 148px #A1B8D0 , 725px 543px #A1B8D0 , 586px 844px #A1B8D0 , 395px 55px #A1B8D0 , 624px 228px #A1B8D0 , 837px 276px #A1B8D0 , 503px 706px #A1B8D0 , 115px 95px #A1B8D0 , 206px 945px #A1B8D0 , 653px 502px #A1B8D0 , 808px 122px #A1B8D0 , 528px 937px #A1B8D0 , 244px 609px #A1B8D0 , 284px 573px #A1B8D0 , 119px 372px #A1B8D0 , 884px 371px #A1B8D0 , 203px 891px #A1B8D0 , 211px 465px #A1B8D0 , 533px 728px #A1B8D0 , 325px 456px #A1B8D0 , 608px 606px #A1B8D0 , 48px 741px #A1B8D0;
  }
  .glitter_17:before {
    -moz-animation: glitter-17 8s infinite;
    -webkit-animation: glitter-17 8s infinite;
    animation: glitter-17 8s infinite;
    box-shadow: 834px 560px #A1B8D0 , 30px 226px #A1B8D0 , 296px 170px #A1B8D0 , 517px 179px #A1B8D0 , 851px 921px #A1B8D0 , 409px 43px #A1B8D0 , 799px 514px #A1B8D0 , 339px 28px #A1B8D0 , 597px 660px #A1B8D0 , 910px 501px #A1B8D0 , 76px 252px #A1B8D0 , 793px 574px #A1B8D0 , 226px 519px #A1B8D0 , 172px 810px #A1B8D0 , 346px 674px #A1B8D0 , 55px 495px #A1B8D0 , 844px 107px #A1B8D0 , 43px 22px #A1B8D0 , 678px 40px #A1B8D0 , 569px 34px #A1B8D0 , 191px 187px #A1B8D0 , 914px 267px #A1B8D0 , 443px 561px #A1B8D0 , 636px 320px #A1B8D0 , 235px 918px #A1B8D0 , 647px 845px #A1B8D0 , 806px 858px #A1B8D0 , 762px 839px #A1B8D0 , 33px 924px #A1B8D0 , 203px 445px #A1B8D0 , 98px 946px #A1B8D0 , 379px 563px #A1B8D0 , 412px 69px #A1B8D0 , 712px 758px #A1B8D0 , 323px 463px #A1B8D0 , 193px 551px #A1B8D0 , 270px 722px #A1B8D0 , 604px 774px #A1B8D0 , 60px 496px #A1B8D0 , 732px 71px #A1B8D0 , 671px 87px #A1B8D0 , 80px 670px #A1B8D0 , 388px 447px #A1B8D0 , 809px 194px #A1B8D0 , 361px 67px #A1B8D0 , 565px 147px #A1B8D0 , 582px 600px #A1B8D0 , 411px 630px #A1B8D0 , 621px 430px #A1B8D0 , 280px 37px #A1B8D0 , 828px 862px #A1B8D0 , 837px 719px #A1B8D0 , 31px 252px #A1B8D0 , 658px 225px #A1B8D0 , 506px 889px #A1B8D0 , 507px 509px #A1B8D0 , 360px 178px #A1B8D0 , 650px 167px #A1B8D0 , 368px 327px #A1B8D0 , 480px 270px #A1B8D0 , 623px 900px #A1B8D0 , 722px 905px #A1B8D0 , 148px 702px #A1B8D0 , 966px 554px #A1B8D0 , 134px 155px #A1B8D0 , 219px 626px #A1B8D0 , 94px 171px #A1B8D0 , 991px 767px #A1B8D0 , 141px 35px #A1B8D0 , 77px 368px #A1B8D0 , 507px 397px #A1B8D0 , 23px 516px #A1B8D0 , 468px 254px #A1B8D0 , 869px 28px #A1B8D0 , 320px 9px #A1B8D0 , 177px 50px #A1B8D0 , 842px 786px #A1B8D0 , 356px 590px #A1B8D0 , 787px 878px #A1B8D0 , 26px 709px #A1B8D0 , 376px 994px #A1B8D0 , 439px 71px #A1B8D0 , 40px 368px #A1B8D0 , 554px 221px #A1B8D0 , 866px 576px #A1B8D0 , 454px 768px #A1B8D0 , 41px 172px #A1B8D0 , 74px 334px #A1B8D0 , 813px 593px #A1B8D0 , 346px 396px #A1B8D0 , 551px 129px #A1B8D0 , 32px 647px #A1B8D0 , 414px 562px #A1B8D0 , 20px 63px #A1B8D0 , 928px 200px #A1B8D0 , 942px 786px #A1B8D0 , 200px 921px #A1B8D0 , 279px 269px #A1B8D0 , 567px 701px #A1B8D0 , 884px 35px #A1B8D0 , 888px 996px #A1B8D0 , 931px 35px #A1B8D0 , 823px 356px #A1B8D0 , 310px 943px #A1B8D0 , 723px 501px #A1B8D0 , 273px 558px #A1B8D0 , 898px 661px #A1B8D0 , 771px 993px #A1B8D0 , 587px 81px #A1B8D0 , 956px 80px #A1B8D0 , 938px 871px #A1B8D0 , 724px 617px #A1B8D0 , 478px 60px #A1B8D0 , 955px 210px #A1B8D0 , 725px 494px #A1B8D0 , 239px 537px #A1B8D0 , 837px 684px #A1B8D0 , 211px 518px #A1B8D0 , 897px 361px #A1B8D0 , 872px 134px #A1B8D0 , 125px 713px #A1B8D0 , 543px 110px #A1B8D0 , 554px 476px #A1B8D0 , 364px 990px #A1B8D0 , 833px 966px #A1B8D0 , 689px 715px #A1B8D0 , 938px 250px #A1B8D0 , 583px 40px #A1B8D0 , 246px 544px #A1B8D0 , 194px 160px #A1B8D0 , 870px 538px #A1B8D0 , 735px 268px #A1B8D0 , 716px 274px #A1B8D0 , 157px 618px #A1B8D0 , 142px 611px #A1B8D0 , 448px 858px #A1B8D0 , 939px 42px #A1B8D0 , 393px 589px #A1B8D0 , 515px 428px #A1B8D0 , 57px 348px #A1B8D0 , 758px 725px #A1B8D0 , 469px 257px #A1B8D0 , 543px 419px #A1B8D0 , 532px 608px #A1B8D0 , 579px 44px #A1B8D0 , 722px 666px #A1B8D0 , 969px 837px #A1B8D0 , 503px 476px #A1B8D0 , 442px 666px #A1B8D0 , 126px 600px #A1B8D0 , 830px 688px #A1B8D0 , 459px 416px #A1B8D0 , 359px 104px #A1B8D0 , 155px 159px #A1B8D0 , 860px 125px #A1B8D0 , 701px 510px #A1B8D0 , 265px 106px #A1B8D0 , 628px 48px #A1B8D0 , 159px 768px #A1B8D0 , 715px 681px #A1B8D0 , 589px 253px #A1B8D0 , 272px 636px #A1B8D0 , 763px 687px #A1B8D0 , 874px 159px #A1B8D0 , 400px 229px #A1B8D0 , 416px 258px #A1B8D0 , 872px 68px #A1B8D0 , 497px 577px #A1B8D0 , 929px 727px #A1B8D0 , 202px 649px #A1B8D0 , 749px 368px #A1B8D0 , 800px 815px #A1B8D0 , 352px 610px #A1B8D0 , 368px 240px #A1B8D0 , 693px 244px #A1B8D0 , 558px 902px #A1B8D0 , 308px 891px #A1B8D0 , 274px 654px #A1B8D0 , 538px 148px #A1B8D0 , 725px 543px #A1B8D0 , 586px 844px #A1B8D0 , 395px 55px #A1B8D0 , 624px 228px #A1B8D0 , 837px 276px #A1B8D0 , 503px 706px #A1B8D0 , 115px 95px #A1B8D0 , 206px 945px #A1B8D0 , 653px 502px #A1B8D0 , 808px 122px #A1B8D0 , 528px 937px #A1B8D0 , 244px 609px #A1B8D0 , 284px 573px #A1B8D0 , 119px 372px #A1B8D0 , 884px 371px #A1B8D0 , 203px 891px #A1B8D0 , 211px 465px #A1B8D0 , 533px 728px #A1B8D0 , 325px 456px #A1B8D0 , 608px 606px #A1B8D0 , 48px 741px #A1B8D0;
  }
  .glitter_17:after {
    -moz-animation: glitter-17 9s infinite;
    -webkit-animation: glitter-17 9s infinite;
    animation: glitter-17 9s infinite;
    box-shadow: 834px 560px #A1B8D0 , 30px 226px #A1B8D0 , 296px 170px #A1B8D0 , 517px 179px #A1B8D0 , 851px 921px #A1B8D0 , 409px 43px #A1B8D0 , 799px 514px #A1B8D0 , 339px 28px #A1B8D0 , 597px 660px #A1B8D0 , 910px 501px #A1B8D0 , 76px 252px #A1B8D0 , 793px 574px #A1B8D0 , 226px 519px #A1B8D0 , 172px 810px #A1B8D0 , 346px 674px #A1B8D0 , 55px 495px #A1B8D0 , 844px 107px #A1B8D0 , 43px 22px #A1B8D0 , 678px 40px #A1B8D0 , 569px 34px #A1B8D0 , 191px 187px #A1B8D0 , 914px 267px #A1B8D0 , 443px 561px #A1B8D0 , 636px 320px #A1B8D0 , 235px 918px #A1B8D0 , 647px 845px #A1B8D0 , 806px 858px #A1B8D0 , 762px 839px #A1B8D0 , 33px 924px #A1B8D0 , 203px 445px #A1B8D0 , 98px 946px #A1B8D0 , 379px 563px #A1B8D0 , 412px 69px #A1B8D0 , 712px 758px #A1B8D0 , 323px 463px #A1B8D0 , 193px 551px #A1B8D0 , 270px 722px #A1B8D0 , 604px 774px #A1B8D0 , 60px 496px #A1B8D0 , 732px 71px #A1B8D0 , 671px 87px #A1B8D0 , 80px 670px #A1B8D0 , 388px 447px #A1B8D0 , 809px 194px #A1B8D0 , 361px 67px #A1B8D0 , 565px 147px #A1B8D0 , 582px 600px #A1B8D0 , 411px 630px #A1B8D0 , 621px 430px #A1B8D0 , 280px 37px #A1B8D0 , 828px 862px #A1B8D0 , 837px 719px #A1B8D0 , 31px 252px #A1B8D0 , 658px 225px #A1B8D0 , 506px 889px #A1B8D0 , 507px 509px #A1B8D0 , 360px 178px #A1B8D0 , 650px 167px #A1B8D0 , 368px 327px #A1B8D0 , 480px 270px #A1B8D0 , 623px 900px #A1B8D0 , 722px 905px #A1B8D0 , 148px 702px #A1B8D0 , 966px 554px #A1B8D0 , 134px 155px #A1B8D0 , 219px 626px #A1B8D0 , 94px 171px #A1B8D0 , 991px 767px #A1B8D0 , 141px 35px #A1B8D0 , 77px 368px #A1B8D0 , 507px 397px #A1B8D0 , 23px 516px #A1B8D0 , 468px 254px #A1B8D0 , 869px 28px #A1B8D0 , 320px 9px #A1B8D0 , 177px 50px #A1B8D0 , 842px 786px #A1B8D0 , 356px 590px #A1B8D0 , 787px 878px #A1B8D0 , 26px 709px #A1B8D0 , 376px 994px #A1B8D0 , 439px 71px #A1B8D0 , 40px 368px #A1B8D0 , 554px 221px #A1B8D0 , 866px 576px #A1B8D0 , 454px 768px #A1B8D0 , 41px 172px #A1B8D0 , 74px 334px #A1B8D0 , 813px 593px #A1B8D0 , 346px 396px #A1B8D0 , 551px 129px #A1B8D0 , 32px 647px #A1B8D0 , 414px 562px #A1B8D0 , 20px 63px #A1B8D0 , 928px 200px #A1B8D0 , 942px 786px #A1B8D0 , 200px 921px #A1B8D0 , 279px 269px #A1B8D0 , 567px 701px #A1B8D0 , 884px 35px #A1B8D0 , 888px 996px #A1B8D0 , 931px 35px #A1B8D0 , 823px 356px #A1B8D0 , 310px 943px #A1B8D0 , 723px 501px #A1B8D0 , 273px 558px #A1B8D0 , 898px 661px #A1B8D0 , 771px 993px #A1B8D0 , 587px 81px #A1B8D0 , 956px 80px #A1B8D0 , 938px 871px #A1B8D0 , 724px 617px #A1B8D0 , 478px 60px #A1B8D0 , 955px 210px #A1B8D0 , 725px 494px #A1B8D0 , 239px 537px #A1B8D0 , 837px 684px #A1B8D0 , 211px 518px #A1B8D0 , 897px 361px #A1B8D0 , 872px 134px #A1B8D0 , 125px 713px #A1B8D0 , 543px 110px #A1B8D0 , 554px 476px #A1B8D0 , 364px 990px #A1B8D0 , 833px 966px #A1B8D0 , 689px 715px #A1B8D0 , 938px 250px #A1B8D0 , 583px 40px #A1B8D0 , 246px 544px #A1B8D0 , 194px 160px #A1B8D0 , 870px 538px #A1B8D0 , 735px 268px #A1B8D0 , 716px 274px #A1B8D0 , 157px 618px #A1B8D0 , 142px 611px #A1B8D0 , 448px 858px #A1B8D0 , 939px 42px #A1B8D0 , 393px 589px #A1B8D0 , 515px 428px #A1B8D0 , 57px 348px #A1B8D0 , 758px 725px #A1B8D0 , 469px 257px #A1B8D0 , 543px 419px #A1B8D0 , 532px 608px #A1B8D0 , 579px 44px #A1B8D0 , 722px 666px #A1B8D0 , 969px 837px #A1B8D0 , 503px 476px #A1B8D0 , 442px 666px #A1B8D0 , 126px 600px #A1B8D0 , 830px 688px #A1B8D0 , 459px 416px #A1B8D0 , 359px 104px #A1B8D0 , 155px 159px #A1B8D0 , 860px 125px #A1B8D0 , 701px 510px #A1B8D0 , 265px 106px #A1B8D0 , 628px 48px #A1B8D0 , 159px 768px #A1B8D0 , 715px 681px #A1B8D0 , 589px 253px #A1B8D0 , 272px 636px #A1B8D0 , 763px 687px #A1B8D0 , 874px 159px #A1B8D0 , 400px 229px #A1B8D0 , 416px 258px #A1B8D0 , 872px 68px #A1B8D0 , 497px 577px #A1B8D0 , 929px 727px #A1B8D0 , 202px 649px #A1B8D0 , 749px 368px #A1B8D0 , 800px 815px #A1B8D0 , 352px 610px #A1B8D0 , 368px 240px #A1B8D0 , 693px 244px #A1B8D0 , 558px 902px #A1B8D0 , 308px 891px #A1B8D0 , 274px 654px #A1B8D0 , 538px 148px #A1B8D0 , 725px 543px #A1B8D0 , 586px 844px #A1B8D0 , 395px 55px #A1B8D0 , 624px 228px #A1B8D0 , 837px 276px #A1B8D0 , 503px 706px #A1B8D0 , 115px 95px #A1B8D0 , 206px 945px #A1B8D0 , 653px 502px #A1B8D0 , 808px 122px #A1B8D0 , 528px 937px #A1B8D0 , 244px 609px #A1B8D0 , 284px 573px #A1B8D0 , 119px 372px #A1B8D0 , 884px 371px #A1B8D0 , 203px 891px #A1B8D0 , 211px 465px #A1B8D0 , 533px 728px #A1B8D0 , 325px 456px #A1B8D0 , 608px 606px #A1B8D0 , 48px 741px #A1B8D0;
  }
  
  @-moz-keyframes glitter-18 {
    0%,
      100%,
      49.35484%,
      59.35484% {
      opacity: 0;
    }
    54.35484% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-18 {
    0%,
      100%,
      49.35484%,
      59.35484% {
      opacity: 0;
    }
    54.35484% {
      opacity: 1;
    }
  }
  @keyframes glitter-18 {
    0%,
      100%,
      49.35484%,
      59.35484% {
      opacity: 0;
    }
    54.35484% {
      opacity: 1;
    }
  }
  .glitter_18 {
    -moz-animation: glitter-18 10s infinite;
    -webkit-animation: glitter-18 10s infinite;
    animation: glitter-18 10s infinite;
    box-shadow: 35px 140px #A1B8D0 , 751px 248px #A1B8D0 , 31px 515px #A1B8D0 , 487px 99px #A1B8D0 , 334px 449px #A1B8D0 , 842px 982px #A1B8D0 , 660px 22px #A1B8D0 , 171px 675px #A1B8D0 , 674px 293px #A1B8D0 , 91px 586px #A1B8D0 , 980px 683px #A1B8D0 , 724px 300px #A1B8D0 , 381px 835px #A1B8D0 , 890px 254px #A1B8D0 , 811px 863px #A1B8D0 , 738px 809px #A1B8D0 , 700px 746px #A1B8D0 , 804px 230px #A1B8D0 , 589px 846px #A1B8D0 , 741px 522px #A1B8D0 , 5px 711px #A1B8D0 , 638px 840px #A1B8D0 , 452px 324px #A1B8D0 , 177px 425px #A1B8D0 , 278px 783px #A1B8D0 , 909px 259px #A1B8D0 , 847px 956px #A1B8D0 , 667px 413px #A1B8D0 , 64px 123px #A1B8D0 , 627px 152px #A1B8D0 , 485px 387px #A1B8D0 , 689px 778px #A1B8D0 , 230px 902px #A1B8D0 , 588px 276px #A1B8D0 , 575px 459px #A1B8D0 , 873px 321px #A1B8D0 , 47px 700px #A1B8D0 , 396px 96px #A1B8D0 , 110px 674px #A1B8D0 , 542px 59px #A1B8D0 , 173px 864px #A1B8D0 , 67px 163px #A1B8D0 , 523px 483px #A1B8D0 , 36px 527px #A1B8D0 , 626px 979px #A1B8D0 , 33px 838px #A1B8D0 , 114px 407px #A1B8D0 , 934px 278px #A1B8D0 , 821px 358px #A1B8D0 , 928px 4px #A1B8D0 , 894px 20px #A1B8D0 , 84px 751px #A1B8D0 , 183px 400px #A1B8D0 , 454px 427px #A1B8D0 , 349px 626px #A1B8D0 , 676px 23px #A1B8D0 , 195px 215px #A1B8D0 , 399px 859px #A1B8D0 , 370px 196px #A1B8D0 , 593px 179px #A1B8D0 , 244px 976px #A1B8D0 , 683px 384px #A1B8D0 , 266px 980px #A1B8D0 , 312px 849px #A1B8D0 , 905px 662px #A1B8D0 , 997px 90px #A1B8D0 , 376px 333px #A1B8D0 , 232px 16px #A1B8D0 , 601px 211px #A1B8D0 , 64px 165px #A1B8D0 , 678px 942px #A1B8D0 , 397px 116px #A1B8D0 , 155px 252px #A1B8D0 , 979px 452px #A1B8D0 , 549px 610px #A1B8D0 , 878px 458px #A1B8D0 , 11px 110px #A1B8D0 , 267px 129px #A1B8D0 , 910px 816px #A1B8D0 , 966px 946px #A1B8D0 , 535px 81px #A1B8D0 , 87px 993px #A1B8D0 , 292px 268px #A1B8D0 , 791px 183px #A1B8D0 , 714px 86px #A1B8D0 , 112px 828px #A1B8D0 , 740px 676px #A1B8D0 , 560px 782px #A1B8D0 , 395px 731px #A1B8D0 , 563px 485px #A1B8D0 , 354px 206px #A1B8D0 , 454px 226px #A1B8D0 , 268px 53px #A1B8D0 , 46px 265px #A1B8D0 , 143px 154px #A1B8D0 , 136px 720px #A1B8D0 , 663px 289px #A1B8D0 , 529px 512px #A1B8D0 , 630px 81px #A1B8D0 , 484px 90px #A1B8D0 , 190px 416px #A1B8D0 , 226px 89px #A1B8D0 , 580px 930px #A1B8D0 , 113px 347px #A1B8D0 , 834px 662px #A1B8D0 , 723px 933px #A1B8D0 , 488px 555px #A1B8D0 , 297px 917px #A1B8D0 , 231px 888px #A1B8D0 , 607px 497px #A1B8D0 , 244px 467px #A1B8D0 , 287px 891px #A1B8D0 , 789px 608px #A1B8D0 , 262px 121px #A1B8D0 , 595px 20px #A1B8D0 , 108px 959px #A1B8D0 , 192px 214px #A1B8D0 , 775px 818px #A1B8D0 , 353px 263px #A1B8D0 , 365px 261px #A1B8D0 , 519px 344px #A1B8D0 , 528px 703px #A1B8D0 , 606px 137px #A1B8D0 , 242px 702px #A1B8D0 , 317px 213px #A1B8D0 , 400px 324px #A1B8D0 , 614px 94px #A1B8D0 , 801px 108px #A1B8D0 , 715px 817px #A1B8D0 , 2px 219px #A1B8D0 , 942px 157px #A1B8D0 , 311px 840px #A1B8D0 , 273px 989px #A1B8D0 , 186px 282px #A1B8D0 , 659px 280px #A1B8D0 , 67px 909px #A1B8D0 , 982px 329px #A1B8D0 , 647px 759px #A1B8D0 , 8px 239px #A1B8D0 , 370px 39px #A1B8D0 , 573px 873px #A1B8D0 , 892px 763px #A1B8D0 , 786px 143px #A1B8D0 , 113px 343px #A1B8D0 , 622px 350px #A1B8D0 , 114px 321px #A1B8D0 , 332px 426px #A1B8D0 , 151px 350px #A1B8D0 , 843px 253px #A1B8D0 , 920px 514px #A1B8D0 , 13px 663px #A1B8D0 , 302px 530px #A1B8D0 , 485px 140px #A1B8D0 , 940px 63px #A1B8D0 , 393px 849px #A1B8D0 , 64px 95px #A1B8D0 , 617px 56px #A1B8D0 , 325px 938px #A1B8D0 , 759px 40px #A1B8D0 , 693px 640px #A1B8D0 , 363px 428px #A1B8D0 , 763px 853px #A1B8D0 , 649px 764px #A1B8D0 , 504px 520px #A1B8D0 , 129px 749px #A1B8D0 , 506px 182px #A1B8D0 , 518px 17px #A1B8D0 , 748px 785px #A1B8D0 , 90px 802px #A1B8D0 , 597px 594px #A1B8D0 , 526px 905px #A1B8D0 , 907px 44px #A1B8D0 , 731px 472px #A1B8D0 , 714px 684px #A1B8D0 , 717px 241px #A1B8D0 , 616px 252px #A1B8D0 , 551px 131px #A1B8D0 , 707px 969px #A1B8D0 , 510px 264px #A1B8D0 , 519px 277px #A1B8D0 , 738px 239px #A1B8D0 , 137px 213px #A1B8D0 , 393px 997px #A1B8D0 , 41px 646px #A1B8D0 , 183px 394px #A1B8D0 , 621px 585px #A1B8D0 , 149px 233px #A1B8D0 , 227px 301px #A1B8D0 , 569px 153px #A1B8D0 , 820px 831px #A1B8D0 , 260px 694px #A1B8D0 , 787px 190px #A1B8D0 , 303px 374px #A1B8D0 , 976px 98px #A1B8D0 , 655px 300px #A1B8D0 , 781px 778px #A1B8D0 , 862px 131px #A1B8D0 , 560px 509px #A1B8D0 , 363px 433px #A1B8D0 , 942px 416px #A1B8D0;
  }
  .glitter_18:before {
    -moz-animation: glitter-18 8s infinite;
    -webkit-animation: glitter-18 8s infinite;
    animation: glitter-18 8s infinite;
    box-shadow: 35px 140px #A1B8D0 , 751px 248px #A1B8D0 , 31px 515px #A1B8D0 , 487px 99px #A1B8D0 , 334px 449px #A1B8D0 , 842px 982px #A1B8D0 , 660px 22px #A1B8D0 , 171px 675px #A1B8D0 , 674px 293px #A1B8D0 , 91px 586px #A1B8D0 , 980px 683px #A1B8D0 , 724px 300px #A1B8D0 , 381px 835px #A1B8D0 , 890px 254px #A1B8D0 , 811px 863px #A1B8D0 , 738px 809px #A1B8D0 , 700px 746px #A1B8D0 , 804px 230px #A1B8D0 , 589px 846px #A1B8D0 , 741px 522px #A1B8D0 , 5px 711px #A1B8D0 , 638px 840px #A1B8D0 , 452px 324px #A1B8D0 , 177px 425px #A1B8D0 , 278px 783px #A1B8D0 , 909px 259px #A1B8D0 , 847px 956px #A1B8D0 , 667px 413px #A1B8D0 , 64px 123px #A1B8D0 , 627px 152px #A1B8D0 , 485px 387px #A1B8D0 , 689px 778px #A1B8D0 , 230px 902px #A1B8D0 , 588px 276px #A1B8D0 , 575px 459px #A1B8D0 , 873px 321px #A1B8D0 , 47px 700px #A1B8D0 , 396px 96px #A1B8D0 , 110px 674px #A1B8D0 , 542px 59px #A1B8D0 , 173px 864px #A1B8D0 , 67px 163px #A1B8D0 , 523px 483px #A1B8D0 , 36px 527px #A1B8D0 , 626px 979px #A1B8D0 , 33px 838px #A1B8D0 , 114px 407px #A1B8D0 , 934px 278px #A1B8D0 , 821px 358px #A1B8D0 , 928px 4px #A1B8D0 , 894px 20px #A1B8D0 , 84px 751px #A1B8D0 , 183px 400px #A1B8D0 , 454px 427px #A1B8D0 , 349px 626px #A1B8D0 , 676px 23px #A1B8D0 , 195px 215px #A1B8D0 , 399px 859px #A1B8D0 , 370px 196px #A1B8D0 , 593px 179px #A1B8D0 , 244px 976px #A1B8D0 , 683px 384px #A1B8D0 , 266px 980px #A1B8D0 , 312px 849px #A1B8D0 , 905px 662px #A1B8D0 , 997px 90px #A1B8D0 , 376px 333px #A1B8D0 , 232px 16px #A1B8D0 , 601px 211px #A1B8D0 , 64px 165px #A1B8D0 , 678px 942px #A1B8D0 , 397px 116px #A1B8D0 , 155px 252px #A1B8D0 , 979px 452px #A1B8D0 , 549px 610px #A1B8D0 , 878px 458px #A1B8D0 , 11px 110px #A1B8D0 , 267px 129px #A1B8D0 , 910px 816px #A1B8D0 , 966px 946px #A1B8D0 , 535px 81px #A1B8D0 , 87px 993px #A1B8D0 , 292px 268px #A1B8D0 , 791px 183px #A1B8D0 , 714px 86px #A1B8D0 , 112px 828px #A1B8D0 , 740px 676px #A1B8D0 , 560px 782px #A1B8D0 , 395px 731px #A1B8D0 , 563px 485px #A1B8D0 , 354px 206px #A1B8D0 , 454px 226px #A1B8D0 , 268px 53px #A1B8D0 , 46px 265px #A1B8D0 , 143px 154px #A1B8D0 , 136px 720px #A1B8D0 , 663px 289px #A1B8D0 , 529px 512px #A1B8D0 , 630px 81px #A1B8D0 , 484px 90px #A1B8D0 , 190px 416px #A1B8D0 , 226px 89px #A1B8D0 , 580px 930px #A1B8D0 , 113px 347px #A1B8D0 , 834px 662px #A1B8D0 , 723px 933px #A1B8D0 , 488px 555px #A1B8D0 , 297px 917px #A1B8D0 , 231px 888px #A1B8D0 , 607px 497px #A1B8D0 , 244px 467px #A1B8D0 , 287px 891px #A1B8D0 , 789px 608px #A1B8D0 , 262px 121px #A1B8D0 , 595px 20px #A1B8D0 , 108px 959px #A1B8D0 , 192px 214px #A1B8D0 , 775px 818px #A1B8D0 , 353px 263px #A1B8D0 , 365px 261px #A1B8D0 , 519px 344px #A1B8D0 , 528px 703px #A1B8D0 , 606px 137px #A1B8D0 , 242px 702px #A1B8D0 , 317px 213px #A1B8D0 , 400px 324px #A1B8D0 , 614px 94px #A1B8D0 , 801px 108px #A1B8D0 , 715px 817px #A1B8D0 , 2px 219px #A1B8D0 , 942px 157px #A1B8D0 , 311px 840px #A1B8D0 , 273px 989px #A1B8D0 , 186px 282px #A1B8D0 , 659px 280px #A1B8D0 , 67px 909px #A1B8D0 , 982px 329px #A1B8D0 , 647px 759px #A1B8D0 , 8px 239px #A1B8D0 , 370px 39px #A1B8D0 , 573px 873px #A1B8D0 , 892px 763px #A1B8D0 , 786px 143px #A1B8D0 , 113px 343px #A1B8D0 , 622px 350px #A1B8D0 , 114px 321px #A1B8D0 , 332px 426px #A1B8D0 , 151px 350px #A1B8D0 , 843px 253px #A1B8D0 , 920px 514px #A1B8D0 , 13px 663px #A1B8D0 , 302px 530px #A1B8D0 , 485px 140px #A1B8D0 , 940px 63px #A1B8D0 , 393px 849px #A1B8D0 , 64px 95px #A1B8D0 , 617px 56px #A1B8D0 , 325px 938px #A1B8D0 , 759px 40px #A1B8D0 , 693px 640px #A1B8D0 , 363px 428px #A1B8D0 , 763px 853px #A1B8D0 , 649px 764px #A1B8D0 , 504px 520px #A1B8D0 , 129px 749px #A1B8D0 , 506px 182px #A1B8D0 , 518px 17px #A1B8D0 , 748px 785px #A1B8D0 , 90px 802px #A1B8D0 , 597px 594px #A1B8D0 , 526px 905px #A1B8D0 , 907px 44px #A1B8D0 , 731px 472px #A1B8D0 , 714px 684px #A1B8D0 , 717px 241px #A1B8D0 , 616px 252px #A1B8D0 , 551px 131px #A1B8D0 , 707px 969px #A1B8D0 , 510px 264px #A1B8D0 , 519px 277px #A1B8D0 , 738px 239px #A1B8D0 , 137px 213px #A1B8D0 , 393px 997px #A1B8D0 , 41px 646px #A1B8D0 , 183px 394px #A1B8D0 , 621px 585px #A1B8D0 , 149px 233px #A1B8D0 , 227px 301px #A1B8D0 , 569px 153px #A1B8D0 , 820px 831px #A1B8D0 , 260px 694px #A1B8D0 , 787px 190px #A1B8D0 , 303px 374px #A1B8D0 , 976px 98px #A1B8D0 , 655px 300px #A1B8D0 , 781px 778px #A1B8D0 , 862px 131px #A1B8D0 , 560px 509px #A1B8D0 , 363px 433px #A1B8D0 , 942px 416px #A1B8D0;
  }
  .glitter_18:after {
    -moz-animation: glitter-18 9s infinite;
    -webkit-animation: glitter-18 9s infinite;
    animation: glitter-18 9s infinite;
    box-shadow: 35px 140px #A1B8D0 , 751px 248px #A1B8D0 , 31px 515px #A1B8D0 , 487px 99px #A1B8D0 , 334px 449px #A1B8D0 , 842px 982px #A1B8D0 , 660px 22px #A1B8D0 , 171px 675px #A1B8D0 , 674px 293px #A1B8D0 , 91px 586px #A1B8D0 , 980px 683px #A1B8D0 , 724px 300px #A1B8D0 , 381px 835px #A1B8D0 , 890px 254px #A1B8D0 , 811px 863px #A1B8D0 , 738px 809px #A1B8D0 , 700px 746px #A1B8D0 , 804px 230px #A1B8D0 , 589px 846px #A1B8D0 , 741px 522px #A1B8D0 , 5px 711px #A1B8D0 , 638px 840px #A1B8D0 , 452px 324px #A1B8D0 , 177px 425px #A1B8D0 , 278px 783px #A1B8D0 , 909px 259px #A1B8D0 , 847px 956px #A1B8D0 , 667px 413px #A1B8D0 , 64px 123px #A1B8D0 , 627px 152px #A1B8D0 , 485px 387px #A1B8D0 , 689px 778px #A1B8D0 , 230px 902px #A1B8D0 , 588px 276px #A1B8D0 , 575px 459px #A1B8D0 , 873px 321px #A1B8D0 , 47px 700px #A1B8D0 , 396px 96px #A1B8D0 , 110px 674px #A1B8D0 , 542px 59px #A1B8D0 , 173px 864px #A1B8D0 , 67px 163px #A1B8D0 , 523px 483px #A1B8D0 , 36px 527px #A1B8D0 , 626px 979px #A1B8D0 , 33px 838px #A1B8D0 , 114px 407px #A1B8D0 , 934px 278px #A1B8D0 , 821px 358px #A1B8D0 , 928px 4px #A1B8D0 , 894px 20px #A1B8D0 , 84px 751px #A1B8D0 , 183px 400px #A1B8D0 , 454px 427px #A1B8D0 , 349px 626px #A1B8D0 , 676px 23px #A1B8D0 , 195px 215px #A1B8D0 , 399px 859px #A1B8D0 , 370px 196px #A1B8D0 , 593px 179px #A1B8D0 , 244px 976px #A1B8D0 , 683px 384px #A1B8D0 , 266px 980px #A1B8D0 , 312px 849px #A1B8D0 , 905px 662px #A1B8D0 , 997px 90px #A1B8D0 , 376px 333px #A1B8D0 , 232px 16px #A1B8D0 , 601px 211px #A1B8D0 , 64px 165px #A1B8D0 , 678px 942px #A1B8D0 , 397px 116px #A1B8D0 , 155px 252px #A1B8D0 , 979px 452px #A1B8D0 , 549px 610px #A1B8D0 , 878px 458px #A1B8D0 , 11px 110px #A1B8D0 , 267px 129px #A1B8D0 , 910px 816px #A1B8D0 , 966px 946px #A1B8D0 , 535px 81px #A1B8D0 , 87px 993px #A1B8D0 , 292px 268px #A1B8D0 , 791px 183px #A1B8D0 , 714px 86px #A1B8D0 , 112px 828px #A1B8D0 , 740px 676px #A1B8D0 , 560px 782px #A1B8D0 , 395px 731px #A1B8D0 , 563px 485px #A1B8D0 , 354px 206px #A1B8D0 , 454px 226px #A1B8D0 , 268px 53px #A1B8D0 , 46px 265px #A1B8D0 , 143px 154px #A1B8D0 , 136px 720px #A1B8D0 , 663px 289px #A1B8D0 , 529px 512px #A1B8D0 , 630px 81px #A1B8D0 , 484px 90px #A1B8D0 , 190px 416px #A1B8D0 , 226px 89px #A1B8D0 , 580px 930px #A1B8D0 , 113px 347px #A1B8D0 , 834px 662px #A1B8D0 , 723px 933px #A1B8D0 , 488px 555px #A1B8D0 , 297px 917px #A1B8D0 , 231px 888px #A1B8D0 , 607px 497px #A1B8D0 , 244px 467px #A1B8D0 , 287px 891px #A1B8D0 , 789px 608px #A1B8D0 , 262px 121px #A1B8D0 , 595px 20px #A1B8D0 , 108px 959px #A1B8D0 , 192px 214px #A1B8D0 , 775px 818px #A1B8D0 , 353px 263px #A1B8D0 , 365px 261px #A1B8D0 , 519px 344px #A1B8D0 , 528px 703px #A1B8D0 , 606px 137px #A1B8D0 , 242px 702px #A1B8D0 , 317px 213px #A1B8D0 , 400px 324px #A1B8D0 , 614px 94px #A1B8D0 , 801px 108px #A1B8D0 , 715px 817px #A1B8D0 , 2px 219px #A1B8D0 , 942px 157px #A1B8D0 , 311px 840px #A1B8D0 , 273px 989px #A1B8D0 , 186px 282px #A1B8D0 , 659px 280px #A1B8D0 , 67px 909px #A1B8D0 , 982px 329px #A1B8D0 , 647px 759px #A1B8D0 , 8px 239px #A1B8D0 , 370px 39px #A1B8D0 , 573px 873px #A1B8D0 , 892px 763px #A1B8D0 , 786px 143px #A1B8D0 , 113px 343px #A1B8D0 , 622px 350px #A1B8D0 , 114px 321px #A1B8D0 , 332px 426px #A1B8D0 , 151px 350px #A1B8D0 , 843px 253px #A1B8D0 , 920px 514px #A1B8D0 , 13px 663px #A1B8D0 , 302px 530px #A1B8D0 , 485px 140px #A1B8D0 , 940px 63px #A1B8D0 , 393px 849px #A1B8D0 , 64px 95px #A1B8D0 , 617px 56px #A1B8D0 , 325px 938px #A1B8D0 , 759px 40px #A1B8D0 , 693px 640px #A1B8D0 , 363px 428px #A1B8D0 , 763px 853px #A1B8D0 , 649px 764px #A1B8D0 , 504px 520px #A1B8D0 , 129px 749px #A1B8D0 , 506px 182px #A1B8D0 , 518px 17px #A1B8D0 , 748px 785px #A1B8D0 , 90px 802px #A1B8D0 , 597px 594px #A1B8D0 , 526px 905px #A1B8D0 , 907px 44px #A1B8D0 , 731px 472px #A1B8D0 , 714px 684px #A1B8D0 , 717px 241px #A1B8D0 , 616px 252px #A1B8D0 , 551px 131px #A1B8D0 , 707px 969px #A1B8D0 , 510px 264px #A1B8D0 , 519px 277px #A1B8D0 , 738px 239px #A1B8D0 , 137px 213px #A1B8D0 , 393px 997px #A1B8D0 , 41px 646px #A1B8D0 , 183px 394px #A1B8D0 , 621px 585px #A1B8D0 , 149px 233px #A1B8D0 , 227px 301px #A1B8D0 , 569px 153px #A1B8D0 , 820px 831px #A1B8D0 , 260px 694px #A1B8D0 , 787px 190px #A1B8D0 , 303px 374px #A1B8D0 , 976px 98px #A1B8D0 , 655px 300px #A1B8D0 , 781px 778px #A1B8D0 , 862px 131px #A1B8D0 , 560px 509px #A1B8D0 , 363px 433px #A1B8D0 , 942px 416px #A1B8D0;
  }
  
  @-moz-keyframes glitter-19 {
    0%,
      100%,
      52.25806%,
      62.25806% {
      opacity: 0;
    }
    57.25806% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-19 {
    0%,
      100%,
      52.25806%,
      62.25806% {
      opacity: 0;
    }
    57.25806% {
      opacity: 1;
    }
  }
  @keyframes glitter-19 {
    0%,
      100%,
      52.25806%,
      62.25806% {
      opacity: 0;
    }
    57.25806% {
      opacity: 1;
    }
  }
  .glitter_19 {
    -moz-animation: glitter-19 10s infinite;
    -webkit-animation: glitter-19 10s infinite;
    animation: glitter-19 10s infinite;
    box-shadow: 784px 482px #A1B8D0 , 140px 456px #A1B8D0 , 53px 253px #A1B8D0 , 908px 894px #A1B8D0 , 499px 568px #A1B8D0 , 462px 793px #A1B8D0 , 143px 735px #A1B8D0 , 511px 385px #A1B8D0 , 333px 658px #A1B8D0 , 330px 447px #A1B8D0 , 543px 668px #A1B8D0 , 839px 93px #A1B8D0 , 616px 315px #A1B8D0 , 443px 243px #A1B8D0 , 170px 725px #A1B8D0 , 256px 131px #A1B8D0 , 12px 749px #A1B8D0 , 663px 524px #A1B8D0 , 982px 95px #A1B8D0 , 925px 732px #A1B8D0 , 539px 900px #A1B8D0 , 330px 592px #A1B8D0 , 167px 598px #A1B8D0 , 232px 472px #A1B8D0 , 37px 802px #A1B8D0 , 835px 617px #A1B8D0 , 541px 281px #A1B8D0 , 93px 988px #A1B8D0 , 716px 28px #A1B8D0 , 19px 877px #A1B8D0 , 837px 913px #A1B8D0 , 258px 671px #A1B8D0 , 453px 927px #A1B8D0 , 703px 19px #A1B8D0 , 48px 970px #A1B8D0 , 706px 389px #A1B8D0 , 560px 579px #A1B8D0 , 9px 663px #A1B8D0 , 467px 915px #A1B8D0 , 39px 149px #A1B8D0 , 854px 768px #A1B8D0 , 365px 806px #A1B8D0 , 227px 106px #A1B8D0 , 220px 308px #A1B8D0 , 125px 175px #A1B8D0 , 367px 835px #A1B8D0 , 619px 165px #A1B8D0 , 636px 299px #A1B8D0 , 753px 201px #A1B8D0 , 385px 846px #A1B8D0 , 285px 467px #A1B8D0 , 209px 329px #A1B8D0 , 994px 964px #A1B8D0 , 905px 346px #A1B8D0 , 769px 578px #A1B8D0 , 751px 319px #A1B8D0 , 922px 272px #A1B8D0 , 6px 562px #A1B8D0 , 115px 890px #A1B8D0 , 693px 738px #A1B8D0 , 224px 761px #A1B8D0 , 247px 641px #A1B8D0 , 329px 19px #A1B8D0 , 264px 975px #A1B8D0 , 16px 210px #A1B8D0 , 762px 771px #A1B8D0 , 5px 49px #A1B8D0 , 871px 322px #A1B8D0 , 16px 455px #A1B8D0 , 887px 287px #A1B8D0 , 401px 153px #A1B8D0 , 521px 967px #A1B8D0 , 102px 940px #A1B8D0 , 242px 26px #A1B8D0 , 371px 874px #A1B8D0 , 326px 545px #A1B8D0 , 634px 109px #A1B8D0 , 104px 63px #A1B8D0 , 617px 755px #A1B8D0 , 862px 177px #A1B8D0 , 268px 41px #A1B8D0 , 110px 715px #A1B8D0 , 856px 811px #A1B8D0 , 19px 101px #A1B8D0 , 753px 328px #A1B8D0 , 814px 664px #A1B8D0 , 10px 656px #A1B8D0 , 938px 661px #A1B8D0 , 170px 135px #A1B8D0 , 874px 539px #A1B8D0 , 520px 133px #A1B8D0 , 860px 695px #A1B8D0 , 523px 204px #A1B8D0 , 255px 476px #A1B8D0 , 405px 973px #A1B8D0 , 60px 29px #A1B8D0 , 605px 632px #A1B8D0 , 598px 697px #A1B8D0 , 447px 641px #A1B8D0 , 68px 762px #A1B8D0 , 650px 149px #A1B8D0 , 545px 766px #A1B8D0 , 85px 707px #A1B8D0 , 779px 614px #A1B8D0 , 721px 712px #A1B8D0 , 792px 877px #A1B8D0 , 172px 861px #A1B8D0 , 516px 712px #A1B8D0 , 976px 747px #A1B8D0 , 720px 318px #A1B8D0 , 992px 910px #A1B8D0 , 304px 70px #A1B8D0 , 354px 279px #A1B8D0 , 984px 98px #A1B8D0 , 724px 361px #A1B8D0 , 919px 217px #A1B8D0 , 922px 623px #A1B8D0 , 933px 243px #A1B8D0 , 777px 786px #A1B8D0 , 338px 824px #A1B8D0 , 571px 136px #A1B8D0 , 372px 480px #A1B8D0 , 972px 658px #A1B8D0 , 167px 422px #A1B8D0 , 145px 432px #A1B8D0 , 428px 10px #A1B8D0 , 967px 748px #A1B8D0 , 884px 5px #A1B8D0 , 962px 691px #A1B8D0 , 916px 326px #A1B8D0 , 473px 774px #A1B8D0 , 69px 100px #A1B8D0 , 381px 92px #A1B8D0 , 477px 884px #A1B8D0 , 169px 331px #A1B8D0 , 805px 334px #A1B8D0 , 179px 984px #A1B8D0 , 347px 606px #A1B8D0 , 260px 798px #A1B8D0 , 658px 81px #A1B8D0 , 768px 895px #A1B8D0 , 693px 521px #A1B8D0 , 483px 546px #A1B8D0 , 153px 474px #A1B8D0 , 199px 636px #A1B8D0 , 888px 407px #A1B8D0 , 715px 856px #A1B8D0 , 106px 567px #A1B8D0 , 119px 987px #A1B8D0 , 824px 201px #A1B8D0 , 456px 953px #A1B8D0 , 600px 27px #A1B8D0 , 66px 455px #A1B8D0 , 454px 747px #A1B8D0 , 610px 7px #A1B8D0 , 575px 366px #A1B8D0 , 421px 751px #A1B8D0 , 636px 259px #A1B8D0 , 729px 788px #A1B8D0 , 698px 906px #A1B8D0 , 770px 889px #A1B8D0 , 963px 394px #A1B8D0 , 491px 841px #A1B8D0 , 79px 783px #A1B8D0 , 553px 52px #A1B8D0 , 12px 754px #A1B8D0 , 509px 737px #A1B8D0 , 431px 1000px #A1B8D0 , 261px 132px #A1B8D0 , 874px 733px #A1B8D0 , 820px 417px #A1B8D0 , 380px 881px #A1B8D0 , 814px 740px #A1B8D0 , 982px 300px #A1B8D0 , 931px 755px #A1B8D0 , 214px 566px #A1B8D0 , 453px 311px #A1B8D0 , 149px 600px #A1B8D0 , 748px 817px #A1B8D0 , 640px 87px #A1B8D0 , 527px 299px #A1B8D0 , 45px 17px #A1B8D0 , 31px 746px #A1B8D0 , 418px 870px #A1B8D0 , 623px 330px #A1B8D0 , 141px 753px #A1B8D0 , 682px 447px #A1B8D0 , 737px 395px #A1B8D0 , 885px 577px #A1B8D0 , 722px 42px #A1B8D0 , 512px 149px #A1B8D0 , 290px 642px #A1B8D0 , 361px 320px #A1B8D0 , 891px 247px #A1B8D0 , 574px 903px #A1B8D0 , 362px 720px #A1B8D0 , 373px 341px #A1B8D0 , 727px 425px #A1B8D0 , 331px 103px #A1B8D0 , 432px 798px #A1B8D0;
  }
  .glitter_19:before {
    -moz-animation: glitter-19 8s infinite;
    -webkit-animation: glitter-19 8s infinite;
    animation: glitter-19 8s infinite;
    box-shadow: 784px 482px #A1B8D0 , 140px 456px #A1B8D0 , 53px 253px #A1B8D0 , 908px 894px #A1B8D0 , 499px 568px #A1B8D0 , 462px 793px #A1B8D0 , 143px 735px #A1B8D0 , 511px 385px #A1B8D0 , 333px 658px #A1B8D0 , 330px 447px #A1B8D0 , 543px 668px #A1B8D0 , 839px 93px #A1B8D0 , 616px 315px #A1B8D0 , 443px 243px #A1B8D0 , 170px 725px #A1B8D0 , 256px 131px #A1B8D0 , 12px 749px #A1B8D0 , 663px 524px #A1B8D0 , 982px 95px #A1B8D0 , 925px 732px #A1B8D0 , 539px 900px #A1B8D0 , 330px 592px #A1B8D0 , 167px 598px #A1B8D0 , 232px 472px #A1B8D0 , 37px 802px #A1B8D0 , 835px 617px #A1B8D0 , 541px 281px #A1B8D0 , 93px 988px #A1B8D0 , 716px 28px #A1B8D0 , 19px 877px #A1B8D0 , 837px 913px #A1B8D0 , 258px 671px #A1B8D0 , 453px 927px #A1B8D0 , 703px 19px #A1B8D0 , 48px 970px #A1B8D0 , 706px 389px #A1B8D0 , 560px 579px #A1B8D0 , 9px 663px #A1B8D0 , 467px 915px #A1B8D0 , 39px 149px #A1B8D0 , 854px 768px #A1B8D0 , 365px 806px #A1B8D0 , 227px 106px #A1B8D0 , 220px 308px #A1B8D0 , 125px 175px #A1B8D0 , 367px 835px #A1B8D0 , 619px 165px #A1B8D0 , 636px 299px #A1B8D0 , 753px 201px #A1B8D0 , 385px 846px #A1B8D0 , 285px 467px #A1B8D0 , 209px 329px #A1B8D0 , 994px 964px #A1B8D0 , 905px 346px #A1B8D0 , 769px 578px #A1B8D0 , 751px 319px #A1B8D0 , 922px 272px #A1B8D0 , 6px 562px #A1B8D0 , 115px 890px #A1B8D0 , 693px 738px #A1B8D0 , 224px 761px #A1B8D0 , 247px 641px #A1B8D0 , 329px 19px #A1B8D0 , 264px 975px #A1B8D0 , 16px 210px #A1B8D0 , 762px 771px #A1B8D0 , 5px 49px #A1B8D0 , 871px 322px #A1B8D0 , 16px 455px #A1B8D0 , 887px 287px #A1B8D0 , 401px 153px #A1B8D0 , 521px 967px #A1B8D0 , 102px 940px #A1B8D0 , 242px 26px #A1B8D0 , 371px 874px #A1B8D0 , 326px 545px #A1B8D0 , 634px 109px #A1B8D0 , 104px 63px #A1B8D0 , 617px 755px #A1B8D0 , 862px 177px #A1B8D0 , 268px 41px #A1B8D0 , 110px 715px #A1B8D0 , 856px 811px #A1B8D0 , 19px 101px #A1B8D0 , 753px 328px #A1B8D0 , 814px 664px #A1B8D0 , 10px 656px #A1B8D0 , 938px 661px #A1B8D0 , 170px 135px #A1B8D0 , 874px 539px #A1B8D0 , 520px 133px #A1B8D0 , 860px 695px #A1B8D0 , 523px 204px #A1B8D0 , 255px 476px #A1B8D0 , 405px 973px #A1B8D0 , 60px 29px #A1B8D0 , 605px 632px #A1B8D0 , 598px 697px #A1B8D0 , 447px 641px #A1B8D0 , 68px 762px #A1B8D0 , 650px 149px #A1B8D0 , 545px 766px #A1B8D0 , 85px 707px #A1B8D0 , 779px 614px #A1B8D0 , 721px 712px #A1B8D0 , 792px 877px #A1B8D0 , 172px 861px #A1B8D0 , 516px 712px #A1B8D0 , 976px 747px #A1B8D0 , 720px 318px #A1B8D0 , 992px 910px #A1B8D0 , 304px 70px #A1B8D0 , 354px 279px #A1B8D0 , 984px 98px #A1B8D0 , 724px 361px #A1B8D0 , 919px 217px #A1B8D0 , 922px 623px #A1B8D0 , 933px 243px #A1B8D0 , 777px 786px #A1B8D0 , 338px 824px #A1B8D0 , 571px 136px #A1B8D0 , 372px 480px #A1B8D0 , 972px 658px #A1B8D0 , 167px 422px #A1B8D0 , 145px 432px #A1B8D0 , 428px 10px #A1B8D0 , 967px 748px #A1B8D0 , 884px 5px #A1B8D0 , 962px 691px #A1B8D0 , 916px 326px #A1B8D0 , 473px 774px #A1B8D0 , 69px 100px #A1B8D0 , 381px 92px #A1B8D0 , 477px 884px #A1B8D0 , 169px 331px #A1B8D0 , 805px 334px #A1B8D0 , 179px 984px #A1B8D0 , 347px 606px #A1B8D0 , 260px 798px #A1B8D0 , 658px 81px #A1B8D0 , 768px 895px #A1B8D0 , 693px 521px #A1B8D0 , 483px 546px #A1B8D0 , 153px 474px #A1B8D0 , 199px 636px #A1B8D0 , 888px 407px #A1B8D0 , 715px 856px #A1B8D0 , 106px 567px #A1B8D0 , 119px 987px #A1B8D0 , 824px 201px #A1B8D0 , 456px 953px #A1B8D0 , 600px 27px #A1B8D0 , 66px 455px #A1B8D0 , 454px 747px #A1B8D0 , 610px 7px #A1B8D0 , 575px 366px #A1B8D0 , 421px 751px #A1B8D0 , 636px 259px #A1B8D0 , 729px 788px #A1B8D0 , 698px 906px #A1B8D0 , 770px 889px #A1B8D0 , 963px 394px #A1B8D0 , 491px 841px #A1B8D0 , 79px 783px #A1B8D0 , 553px 52px #A1B8D0 , 12px 754px #A1B8D0 , 509px 737px #A1B8D0 , 431px 1000px #A1B8D0 , 261px 132px #A1B8D0 , 874px 733px #A1B8D0 , 820px 417px #A1B8D0 , 380px 881px #A1B8D0 , 814px 740px #A1B8D0 , 982px 300px #A1B8D0 , 931px 755px #A1B8D0 , 214px 566px #A1B8D0 , 453px 311px #A1B8D0 , 149px 600px #A1B8D0 , 748px 817px #A1B8D0 , 640px 87px #A1B8D0 , 527px 299px #A1B8D0 , 45px 17px #A1B8D0 , 31px 746px #A1B8D0 , 418px 870px #A1B8D0 , 623px 330px #A1B8D0 , 141px 753px #A1B8D0 , 682px 447px #A1B8D0 , 737px 395px #A1B8D0 , 885px 577px #A1B8D0 , 722px 42px #A1B8D0 , 512px 149px #A1B8D0 , 290px 642px #A1B8D0 , 361px 320px #A1B8D0 , 891px 247px #A1B8D0 , 574px 903px #A1B8D0 , 362px 720px #A1B8D0 , 373px 341px #A1B8D0 , 727px 425px #A1B8D0 , 331px 103px #A1B8D0 , 432px 798px #A1B8D0;
  }
  .glitter_19:after {
    -moz-animation: glitter-19 9s infinite;
    -webkit-animation: glitter-19 9s infinite;
    animation: glitter-19 9s infinite;
    box-shadow: 784px 482px #A1B8D0 , 140px 456px #A1B8D0 , 53px 253px #A1B8D0 , 908px 894px #A1B8D0 , 499px 568px #A1B8D0 , 462px 793px #A1B8D0 , 143px 735px #A1B8D0 , 511px 385px #A1B8D0 , 333px 658px #A1B8D0 , 330px 447px #A1B8D0 , 543px 668px #A1B8D0 , 839px 93px #A1B8D0 , 616px 315px #A1B8D0 , 443px 243px #A1B8D0 , 170px 725px #A1B8D0 , 256px 131px #A1B8D0 , 12px 749px #A1B8D0 , 663px 524px #A1B8D0 , 982px 95px #A1B8D0 , 925px 732px #A1B8D0 , 539px 900px #A1B8D0 , 330px 592px #A1B8D0 , 167px 598px #A1B8D0 , 232px 472px #A1B8D0 , 37px 802px #A1B8D0 , 835px 617px #A1B8D0 , 541px 281px #A1B8D0 , 93px 988px #A1B8D0 , 716px 28px #A1B8D0 , 19px 877px #A1B8D0 , 837px 913px #A1B8D0 , 258px 671px #A1B8D0 , 453px 927px #A1B8D0 , 703px 19px #A1B8D0 , 48px 970px #A1B8D0 , 706px 389px #A1B8D0 , 560px 579px #A1B8D0 , 9px 663px #A1B8D0 , 467px 915px #A1B8D0 , 39px 149px #A1B8D0 , 854px 768px #A1B8D0 , 365px 806px #A1B8D0 , 227px 106px #A1B8D0 , 220px 308px #A1B8D0 , 125px 175px #A1B8D0 , 367px 835px #A1B8D0 , 619px 165px #A1B8D0 , 636px 299px #A1B8D0 , 753px 201px #A1B8D0 , 385px 846px #A1B8D0 , 285px 467px #A1B8D0 , 209px 329px #A1B8D0 , 994px 964px #A1B8D0 , 905px 346px #A1B8D0 , 769px 578px #A1B8D0 , 751px 319px #A1B8D0 , 922px 272px #A1B8D0 , 6px 562px #A1B8D0 , 115px 890px #A1B8D0 , 693px 738px #A1B8D0 , 224px 761px #A1B8D0 , 247px 641px #A1B8D0 , 329px 19px #A1B8D0 , 264px 975px #A1B8D0 , 16px 210px #A1B8D0 , 762px 771px #A1B8D0 , 5px 49px #A1B8D0 , 871px 322px #A1B8D0 , 16px 455px #A1B8D0 , 887px 287px #A1B8D0 , 401px 153px #A1B8D0 , 521px 967px #A1B8D0 , 102px 940px #A1B8D0 , 242px 26px #A1B8D0 , 371px 874px #A1B8D0 , 326px 545px #A1B8D0 , 634px 109px #A1B8D0 , 104px 63px #A1B8D0 , 617px 755px #A1B8D0 , 862px 177px #A1B8D0 , 268px 41px #A1B8D0 , 110px 715px #A1B8D0 , 856px 811px #A1B8D0 , 19px 101px #A1B8D0 , 753px 328px #A1B8D0 , 814px 664px #A1B8D0 , 10px 656px #A1B8D0 , 938px 661px #A1B8D0 , 170px 135px #A1B8D0 , 874px 539px #A1B8D0 , 520px 133px #A1B8D0 , 860px 695px #A1B8D0 , 523px 204px #A1B8D0 , 255px 476px #A1B8D0 , 405px 973px #A1B8D0 , 60px 29px #A1B8D0 , 605px 632px #A1B8D0 , 598px 697px #A1B8D0 , 447px 641px #A1B8D0 , 68px 762px #A1B8D0 , 650px 149px #A1B8D0 , 545px 766px #A1B8D0 , 85px 707px #A1B8D0 , 779px 614px #A1B8D0 , 721px 712px #A1B8D0 , 792px 877px #A1B8D0 , 172px 861px #A1B8D0 , 516px 712px #A1B8D0 , 976px 747px #A1B8D0 , 720px 318px #A1B8D0 , 992px 910px #A1B8D0 , 304px 70px #A1B8D0 , 354px 279px #A1B8D0 , 984px 98px #A1B8D0 , 724px 361px #A1B8D0 , 919px 217px #A1B8D0 , 922px 623px #A1B8D0 , 933px 243px #A1B8D0 , 777px 786px #A1B8D0 , 338px 824px #A1B8D0 , 571px 136px #A1B8D0 , 372px 480px #A1B8D0 , 972px 658px #A1B8D0 , 167px 422px #A1B8D0 , 145px 432px #A1B8D0 , 428px 10px #A1B8D0 , 967px 748px #A1B8D0 , 884px 5px #A1B8D0 , 962px 691px #A1B8D0 , 916px 326px #A1B8D0 , 473px 774px #A1B8D0 , 69px 100px #A1B8D0 , 381px 92px #A1B8D0 , 477px 884px #A1B8D0 , 169px 331px #A1B8D0 , 805px 334px #A1B8D0 , 179px 984px #A1B8D0 , 347px 606px #A1B8D0 , 260px 798px #A1B8D0 , 658px 81px #A1B8D0 , 768px 895px #A1B8D0 , 693px 521px #A1B8D0 , 483px 546px #A1B8D0 , 153px 474px #A1B8D0 , 199px 636px #A1B8D0 , 888px 407px #A1B8D0 , 715px 856px #A1B8D0 , 106px 567px #A1B8D0 , 119px 987px #A1B8D0 , 824px 201px #A1B8D0 , 456px 953px #A1B8D0 , 600px 27px #A1B8D0 , 66px 455px #A1B8D0 , 454px 747px #A1B8D0 , 610px 7px #A1B8D0 , 575px 366px #A1B8D0 , 421px 751px #A1B8D0 , 636px 259px #A1B8D0 , 729px 788px #A1B8D0 , 698px 906px #A1B8D0 , 770px 889px #A1B8D0 , 963px 394px #A1B8D0 , 491px 841px #A1B8D0 , 79px 783px #A1B8D0 , 553px 52px #A1B8D0 , 12px 754px #A1B8D0 , 509px 737px #A1B8D0 , 431px 1000px #A1B8D0 , 261px 132px #A1B8D0 , 874px 733px #A1B8D0 , 820px 417px #A1B8D0 , 380px 881px #A1B8D0 , 814px 740px #A1B8D0 , 982px 300px #A1B8D0 , 931px 755px #A1B8D0 , 214px 566px #A1B8D0 , 453px 311px #A1B8D0 , 149px 600px #A1B8D0 , 748px 817px #A1B8D0 , 640px 87px #A1B8D0 , 527px 299px #A1B8D0 , 45px 17px #A1B8D0 , 31px 746px #A1B8D0 , 418px 870px #A1B8D0 , 623px 330px #A1B8D0 , 141px 753px #A1B8D0 , 682px 447px #A1B8D0 , 737px 395px #A1B8D0 , 885px 577px #A1B8D0 , 722px 42px #A1B8D0 , 512px 149px #A1B8D0 , 290px 642px #A1B8D0 , 361px 320px #A1B8D0 , 891px 247px #A1B8D0 , 574px 903px #A1B8D0 , 362px 720px #A1B8D0 , 373px 341px #A1B8D0 , 727px 425px #A1B8D0 , 331px 103px #A1B8D0 , 432px 798px #A1B8D0;
  }
  
  @-moz-keyframes glitter-20 {
    0%,
      100%,
      55.16129%,
      65.16129% {
      opacity: 0;
    }
    60.16129% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-20 {
    0%,
      100%,
      55.16129%,
      65.16129% {
      opacity: 0;
    }
    60.16129% {
      opacity: 1;
    }
  }
  @keyframes glitter-20 {
    0%,
      100%,
      55.16129%,
      65.16129% {
      opacity: 0;
    }
    60.16129% {
      opacity: 1;
    }
  }
  .glitter_20 {
    -moz-animation: glitter-20 10s infinite;
    -webkit-animation: glitter-20 10s infinite;
    animation: glitter-20 10s infinite;
    box-shadow: 932px 496px #A1B8D0 , 351px 88px #A1B8D0 , 240px 890px #A1B8D0 , 748px 590px #A1B8D0 , 850px 285px #A1B8D0 , 836px 721px #A1B8D0 , 751px 112px #A1B8D0 , 408px 891px #A1B8D0 , 68px 746px #A1B8D0 , 486px 58px #A1B8D0 , 34px 216px #A1B8D0 , 489px 340px #A1B8D0 , 215px 624px #A1B8D0 , 681px 744px #A1B8D0 , 611px 633px #A1B8D0 , 360px 437px #A1B8D0 , 591px 667px #A1B8D0 , 152px 453px #A1B8D0 , 405px 368px #A1B8D0 , 634px 513px #A1B8D0 , 986px 146px #A1B8D0 , 207px 964px #A1B8D0 , 705px 894px #A1B8D0 , 792px 723px #A1B8D0 , 62px 309px #A1B8D0 , 792px 61px #A1B8D0 , 945px 684px #A1B8D0 , 252px 807px #A1B8D0 , 197px 744px #A1B8D0 , 634px 808px #A1B8D0 , 378px 109px #A1B8D0 , 623px 100px #A1B8D0 , 439px 752px #A1B8D0 , 590px 712px #A1B8D0 , 607px 895px #A1B8D0 , 293px 735px #A1B8D0 , 588px 292px #A1B8D0 , 388px 72px #A1B8D0 , 546px 728px #A1B8D0 , 827px 420px #A1B8D0 , 503px 708px #A1B8D0 , 674px 332px #A1B8D0 , 834px 433px #A1B8D0 , 282px 45px #A1B8D0 , 975px 232px #A1B8D0 , 307px 35px #A1B8D0 , 597px 646px #A1B8D0 , 150px 318px #A1B8D0 , 226px 533px #A1B8D0 , 494px 861px #A1B8D0 , 73px 327px #A1B8D0 , 313px 342px #A1B8D0 , 223px 156px #A1B8D0 , 68px 722px #A1B8D0 , 516px 278px #A1B8D0 , 40px 959px #A1B8D0 , 112px 46px #A1B8D0 , 479px 871px #A1B8D0 , 258px 667px #A1B8D0 , 269px 444px #A1B8D0 , 458px 694px #A1B8D0 , 565px 198px #A1B8D0 , 460px 817px #A1B8D0 , 965px 233px #A1B8D0 , 143px 960px #A1B8D0 , 149px 976px #A1B8D0 , 36px 968px #A1B8D0 , 992px 363px #A1B8D0 , 795px 952px #A1B8D0 , 242px 818px #A1B8D0 , 1000px 827px #A1B8D0 , 905px 50px #A1B8D0 , 650px 300px #A1B8D0 , 743px 453px #A1B8D0 , 838px 145px #A1B8D0 , 505px 265px #A1B8D0 , 848px 568px #A1B8D0 , 35px 799px #A1B8D0 , 781px 167px #A1B8D0 , 737px 978px #A1B8D0 , 99px 562px #A1B8D0 , 699px 925px #A1B8D0 , 599px 443px #A1B8D0 , 198px 624px #A1B8D0 , 465px 297px #A1B8D0 , 445px 701px #A1B8D0 , 364px 25px #A1B8D0 , 594px 359px #A1B8D0 , 186px 971px #A1B8D0 , 37px 557px #A1B8D0 , 938px 752px #A1B8D0 , 625px 563px #A1B8D0 , 601px 928px #A1B8D0 , 560px 98px #A1B8D0 , 810px 458px #A1B8D0 , 195px 880px #A1B8D0 , 677px 310px #A1B8D0 , 217px 891px #A1B8D0 , 771px 804px #A1B8D0 , 152px 649px #A1B8D0 , 246px 380px #A1B8D0 , 374px 211px #A1B8D0 , 841px 808px #A1B8D0 , 507px 954px #A1B8D0 , 421px 561px #A1B8D0 , 726px 516px #A1B8D0 , 78px 95px #A1B8D0 , 660px 540px #A1B8D0 , 763px 413px #A1B8D0 , 237px 726px #A1B8D0 , 926px 997px #A1B8D0 , 366px 446px #A1B8D0 , 202px 82px #A1B8D0 , 417px 915px #A1B8D0 , 279px 505px #A1B8D0 , 971px 827px #A1B8D0 , 918px 82px #A1B8D0 , 115px 262px #A1B8D0 , 816px 663px #A1B8D0 , 652px 230px #A1B8D0 , 198px 42px #A1B8D0 , 514px 345px #A1B8D0 , 867px 755px #A1B8D0 , 952px 223px #A1B8D0 , 107px 400px #A1B8D0 , 883px 175px #A1B8D0 , 874px 103px #A1B8D0 , 954px 878px #A1B8D0 , 154px 386px #A1B8D0 , 828px 115px #A1B8D0 , 801px 327px #A1B8D0 , 604px 951px #A1B8D0 , 110px 12px #A1B8D0 , 198px 72px #A1B8D0 , 872px 553px #A1B8D0 , 483px 141px #A1B8D0 , 183px 786px #A1B8D0 , 61px 702px #A1B8D0 , 264px 243px #A1B8D0 , 530px 241px #A1B8D0 , 797px 233px #A1B8D0 , 989px 870px #A1B8D0 , 278px 110px #A1B8D0 , 391px 515px #A1B8D0 , 574px 90px #A1B8D0 , 47px 381px #A1B8D0 , 475px 329px #A1B8D0 , 946px 596px #A1B8D0 , 383px 671px #A1B8D0 , 691px 436px #A1B8D0 , 695px 650px #A1B8D0 , 96px 517px #A1B8D0 , 345px 644px #A1B8D0 , 979px 38px #A1B8D0 , 551px 609px #A1B8D0 , 733px 22px #A1B8D0 , 311px 292px #A1B8D0 , 818px 793px #A1B8D0 , 622px 57px #A1B8D0 , 413px 944px #A1B8D0 , 942px 119px #A1B8D0 , 310px 584px #A1B8D0 , 337px 88px #A1B8D0 , 790px 423px #A1B8D0 , 9px 990px #A1B8D0 , 57px 57px #A1B8D0 , 584px 68px #A1B8D0 , 55px 240px #A1B8D0 , 417px 579px #A1B8D0 , 18px 490px #A1B8D0 , 66px 115px #A1B8D0 , 443px 682px #A1B8D0 , 884px 584px #A1B8D0 , 42px 370px #A1B8D0 , 23px 603px #A1B8D0 , 471px 297px #A1B8D0 , 558px 560px #A1B8D0 , 843px 379px #A1B8D0 , 503px 90px #A1B8D0 , 466px 690px #A1B8D0 , 335px 794px #A1B8D0 , 715px 917px #A1B8D0 , 497px 270px #A1B8D0 , 532px 486px #A1B8D0 , 975px 800px #A1B8D0 , 248px 999px #A1B8D0 , 813px 355px #A1B8D0 , 444px 871px #A1B8D0 , 687px 631px #A1B8D0 , 438px 632px #A1B8D0 , 976px 948px #A1B8D0 , 69px 324px #A1B8D0 , 508px 52px #A1B8D0 , 945px 692px #A1B8D0 , 129px 733px #A1B8D0 , 629px 266px #A1B8D0 , 858px 729px #A1B8D0 , 10px 40px #A1B8D0 , 251px 371px #A1B8D0 , 345px 599px #A1B8D0;
  }
  .glitter_20:before {
    -moz-animation: glitter-20 8s infinite;
    -webkit-animation: glitter-20 8s infinite;
    animation: glitter-20 8s infinite;
    box-shadow: 932px 496px #A1B8D0 , 351px 88px #A1B8D0 , 240px 890px #A1B8D0 , 748px 590px #A1B8D0 , 850px 285px #A1B8D0 , 836px 721px #A1B8D0 , 751px 112px #A1B8D0 , 408px 891px #A1B8D0 , 68px 746px #A1B8D0 , 486px 58px #A1B8D0 , 34px 216px #A1B8D0 , 489px 340px #A1B8D0 , 215px 624px #A1B8D0 , 681px 744px #A1B8D0 , 611px 633px #A1B8D0 , 360px 437px #A1B8D0 , 591px 667px #A1B8D0 , 152px 453px #A1B8D0 , 405px 368px #A1B8D0 , 634px 513px #A1B8D0 , 986px 146px #A1B8D0 , 207px 964px #A1B8D0 , 705px 894px #A1B8D0 , 792px 723px #A1B8D0 , 62px 309px #A1B8D0 , 792px 61px #A1B8D0 , 945px 684px #A1B8D0 , 252px 807px #A1B8D0 , 197px 744px #A1B8D0 , 634px 808px #A1B8D0 , 378px 109px #A1B8D0 , 623px 100px #A1B8D0 , 439px 752px #A1B8D0 , 590px 712px #A1B8D0 , 607px 895px #A1B8D0 , 293px 735px #A1B8D0 , 588px 292px #A1B8D0 , 388px 72px #A1B8D0 , 546px 728px #A1B8D0 , 827px 420px #A1B8D0 , 503px 708px #A1B8D0 , 674px 332px #A1B8D0 , 834px 433px #A1B8D0 , 282px 45px #A1B8D0 , 975px 232px #A1B8D0 , 307px 35px #A1B8D0 , 597px 646px #A1B8D0 , 150px 318px #A1B8D0 , 226px 533px #A1B8D0 , 494px 861px #A1B8D0 , 73px 327px #A1B8D0 , 313px 342px #A1B8D0 , 223px 156px #A1B8D0 , 68px 722px #A1B8D0 , 516px 278px #A1B8D0 , 40px 959px #A1B8D0 , 112px 46px #A1B8D0 , 479px 871px #A1B8D0 , 258px 667px #A1B8D0 , 269px 444px #A1B8D0 , 458px 694px #A1B8D0 , 565px 198px #A1B8D0 , 460px 817px #A1B8D0 , 965px 233px #A1B8D0 , 143px 960px #A1B8D0 , 149px 976px #A1B8D0 , 36px 968px #A1B8D0 , 992px 363px #A1B8D0 , 795px 952px #A1B8D0 , 242px 818px #A1B8D0 , 1000px 827px #A1B8D0 , 905px 50px #A1B8D0 , 650px 300px #A1B8D0 , 743px 453px #A1B8D0 , 838px 145px #A1B8D0 , 505px 265px #A1B8D0 , 848px 568px #A1B8D0 , 35px 799px #A1B8D0 , 781px 167px #A1B8D0 , 737px 978px #A1B8D0 , 99px 562px #A1B8D0 , 699px 925px #A1B8D0 , 599px 443px #A1B8D0 , 198px 624px #A1B8D0 , 465px 297px #A1B8D0 , 445px 701px #A1B8D0 , 364px 25px #A1B8D0 , 594px 359px #A1B8D0 , 186px 971px #A1B8D0 , 37px 557px #A1B8D0 , 938px 752px #A1B8D0 , 625px 563px #A1B8D0 , 601px 928px #A1B8D0 , 560px 98px #A1B8D0 , 810px 458px #A1B8D0 , 195px 880px #A1B8D0 , 677px 310px #A1B8D0 , 217px 891px #A1B8D0 , 771px 804px #A1B8D0 , 152px 649px #A1B8D0 , 246px 380px #A1B8D0 , 374px 211px #A1B8D0 , 841px 808px #A1B8D0 , 507px 954px #A1B8D0 , 421px 561px #A1B8D0 , 726px 516px #A1B8D0 , 78px 95px #A1B8D0 , 660px 540px #A1B8D0 , 763px 413px #A1B8D0 , 237px 726px #A1B8D0 , 926px 997px #A1B8D0 , 366px 446px #A1B8D0 , 202px 82px #A1B8D0 , 417px 915px #A1B8D0 , 279px 505px #A1B8D0 , 971px 827px #A1B8D0 , 918px 82px #A1B8D0 , 115px 262px #A1B8D0 , 816px 663px #A1B8D0 , 652px 230px #A1B8D0 , 198px 42px #A1B8D0 , 514px 345px #A1B8D0 , 867px 755px #A1B8D0 , 952px 223px #A1B8D0 , 107px 400px #A1B8D0 , 883px 175px #A1B8D0 , 874px 103px #A1B8D0 , 954px 878px #A1B8D0 , 154px 386px #A1B8D0 , 828px 115px #A1B8D0 , 801px 327px #A1B8D0 , 604px 951px #A1B8D0 , 110px 12px #A1B8D0 , 198px 72px #A1B8D0 , 872px 553px #A1B8D0 , 483px 141px #A1B8D0 , 183px 786px #A1B8D0 , 61px 702px #A1B8D0 , 264px 243px #A1B8D0 , 530px 241px #A1B8D0 , 797px 233px #A1B8D0 , 989px 870px #A1B8D0 , 278px 110px #A1B8D0 , 391px 515px #A1B8D0 , 574px 90px #A1B8D0 , 47px 381px #A1B8D0 , 475px 329px #A1B8D0 , 946px 596px #A1B8D0 , 383px 671px #A1B8D0 , 691px 436px #A1B8D0 , 695px 650px #A1B8D0 , 96px 517px #A1B8D0 , 345px 644px #A1B8D0 , 979px 38px #A1B8D0 , 551px 609px #A1B8D0 , 733px 22px #A1B8D0 , 311px 292px #A1B8D0 , 818px 793px #A1B8D0 , 622px 57px #A1B8D0 , 413px 944px #A1B8D0 , 942px 119px #A1B8D0 , 310px 584px #A1B8D0 , 337px 88px #A1B8D0 , 790px 423px #A1B8D0 , 9px 990px #A1B8D0 , 57px 57px #A1B8D0 , 584px 68px #A1B8D0 , 55px 240px #A1B8D0 , 417px 579px #A1B8D0 , 18px 490px #A1B8D0 , 66px 115px #A1B8D0 , 443px 682px #A1B8D0 , 884px 584px #A1B8D0 , 42px 370px #A1B8D0 , 23px 603px #A1B8D0 , 471px 297px #A1B8D0 , 558px 560px #A1B8D0 , 843px 379px #A1B8D0 , 503px 90px #A1B8D0 , 466px 690px #A1B8D0 , 335px 794px #A1B8D0 , 715px 917px #A1B8D0 , 497px 270px #A1B8D0 , 532px 486px #A1B8D0 , 975px 800px #A1B8D0 , 248px 999px #A1B8D0 , 813px 355px #A1B8D0 , 444px 871px #A1B8D0 , 687px 631px #A1B8D0 , 438px 632px #A1B8D0 , 976px 948px #A1B8D0 , 69px 324px #A1B8D0 , 508px 52px #A1B8D0 , 945px 692px #A1B8D0 , 129px 733px #A1B8D0 , 629px 266px #A1B8D0 , 858px 729px #A1B8D0 , 10px 40px #A1B8D0 , 251px 371px #A1B8D0 , 345px 599px #A1B8D0;
  }
  .glitter_20:after {
    -moz-animation: glitter-20 9s infinite;
    -webkit-animation: glitter-20 9s infinite;
    animation: glitter-20 9s infinite;
    box-shadow: 932px 496px #A1B8D0 , 351px 88px #A1B8D0 , 240px 890px #A1B8D0 , 748px 590px #A1B8D0 , 850px 285px #A1B8D0 , 836px 721px #A1B8D0 , 751px 112px #A1B8D0 , 408px 891px #A1B8D0 , 68px 746px #A1B8D0 , 486px 58px #A1B8D0 , 34px 216px #A1B8D0 , 489px 340px #A1B8D0 , 215px 624px #A1B8D0 , 681px 744px #A1B8D0 , 611px 633px #A1B8D0 , 360px 437px #A1B8D0 , 591px 667px #A1B8D0 , 152px 453px #A1B8D0 , 405px 368px #A1B8D0 , 634px 513px #A1B8D0 , 986px 146px #A1B8D0 , 207px 964px #A1B8D0 , 705px 894px #A1B8D0 , 792px 723px #A1B8D0 , 62px 309px #A1B8D0 , 792px 61px #A1B8D0 , 945px 684px #A1B8D0 , 252px 807px #A1B8D0 , 197px 744px #A1B8D0 , 634px 808px #A1B8D0 , 378px 109px #A1B8D0 , 623px 100px #A1B8D0 , 439px 752px #A1B8D0 , 590px 712px #A1B8D0 , 607px 895px #A1B8D0 , 293px 735px #A1B8D0 , 588px 292px #A1B8D0 , 388px 72px #A1B8D0 , 546px 728px #A1B8D0 , 827px 420px #A1B8D0 , 503px 708px #A1B8D0 , 674px 332px #A1B8D0 , 834px 433px #A1B8D0 , 282px 45px #A1B8D0 , 975px 232px #A1B8D0 , 307px 35px #A1B8D0 , 597px 646px #A1B8D0 , 150px 318px #A1B8D0 , 226px 533px #A1B8D0 , 494px 861px #A1B8D0 , 73px 327px #A1B8D0 , 313px 342px #A1B8D0 , 223px 156px #A1B8D0 , 68px 722px #A1B8D0 , 516px 278px #A1B8D0 , 40px 959px #A1B8D0 , 112px 46px #A1B8D0 , 479px 871px #A1B8D0 , 258px 667px #A1B8D0 , 269px 444px #A1B8D0 , 458px 694px #A1B8D0 , 565px 198px #A1B8D0 , 460px 817px #A1B8D0 , 965px 233px #A1B8D0 , 143px 960px #A1B8D0 , 149px 976px #A1B8D0 , 36px 968px #A1B8D0 , 992px 363px #A1B8D0 , 795px 952px #A1B8D0 , 242px 818px #A1B8D0 , 1000px 827px #A1B8D0 , 905px 50px #A1B8D0 , 650px 300px #A1B8D0 , 743px 453px #A1B8D0 , 838px 145px #A1B8D0 , 505px 265px #A1B8D0 , 848px 568px #A1B8D0 , 35px 799px #A1B8D0 , 781px 167px #A1B8D0 , 737px 978px #A1B8D0 , 99px 562px #A1B8D0 , 699px 925px #A1B8D0 , 599px 443px #A1B8D0 , 198px 624px #A1B8D0 , 465px 297px #A1B8D0 , 445px 701px #A1B8D0 , 364px 25px #A1B8D0 , 594px 359px #A1B8D0 , 186px 971px #A1B8D0 , 37px 557px #A1B8D0 , 938px 752px #A1B8D0 , 625px 563px #A1B8D0 , 601px 928px #A1B8D0 , 560px 98px #A1B8D0 , 810px 458px #A1B8D0 , 195px 880px #A1B8D0 , 677px 310px #A1B8D0 , 217px 891px #A1B8D0 , 771px 804px #A1B8D0 , 152px 649px #A1B8D0 , 246px 380px #A1B8D0 , 374px 211px #A1B8D0 , 841px 808px #A1B8D0 , 507px 954px #A1B8D0 , 421px 561px #A1B8D0 , 726px 516px #A1B8D0 , 78px 95px #A1B8D0 , 660px 540px #A1B8D0 , 763px 413px #A1B8D0 , 237px 726px #A1B8D0 , 926px 997px #A1B8D0 , 366px 446px #A1B8D0 , 202px 82px #A1B8D0 , 417px 915px #A1B8D0 , 279px 505px #A1B8D0 , 971px 827px #A1B8D0 , 918px 82px #A1B8D0 , 115px 262px #A1B8D0 , 816px 663px #A1B8D0 , 652px 230px #A1B8D0 , 198px 42px #A1B8D0 , 514px 345px #A1B8D0 , 867px 755px #A1B8D0 , 952px 223px #A1B8D0 , 107px 400px #A1B8D0 , 883px 175px #A1B8D0 , 874px 103px #A1B8D0 , 954px 878px #A1B8D0 , 154px 386px #A1B8D0 , 828px 115px #A1B8D0 , 801px 327px #A1B8D0 , 604px 951px #A1B8D0 , 110px 12px #A1B8D0 , 198px 72px #A1B8D0 , 872px 553px #A1B8D0 , 483px 141px #A1B8D0 , 183px 786px #A1B8D0 , 61px 702px #A1B8D0 , 264px 243px #A1B8D0 , 530px 241px #A1B8D0 , 797px 233px #A1B8D0 , 989px 870px #A1B8D0 , 278px 110px #A1B8D0 , 391px 515px #A1B8D0 , 574px 90px #A1B8D0 , 47px 381px #A1B8D0 , 475px 329px #A1B8D0 , 946px 596px #A1B8D0 , 383px 671px #A1B8D0 , 691px 436px #A1B8D0 , 695px 650px #A1B8D0 , 96px 517px #A1B8D0 , 345px 644px #A1B8D0 , 979px 38px #A1B8D0 , 551px 609px #A1B8D0 , 733px 22px #A1B8D0 , 311px 292px #A1B8D0 , 818px 793px #A1B8D0 , 622px 57px #A1B8D0 , 413px 944px #A1B8D0 , 942px 119px #A1B8D0 , 310px 584px #A1B8D0 , 337px 88px #A1B8D0 , 790px 423px #A1B8D0 , 9px 990px #A1B8D0 , 57px 57px #A1B8D0 , 584px 68px #A1B8D0 , 55px 240px #A1B8D0 , 417px 579px #A1B8D0 , 18px 490px #A1B8D0 , 66px 115px #A1B8D0 , 443px 682px #A1B8D0 , 884px 584px #A1B8D0 , 42px 370px #A1B8D0 , 23px 603px #A1B8D0 , 471px 297px #A1B8D0 , 558px 560px #A1B8D0 , 843px 379px #A1B8D0 , 503px 90px #A1B8D0 , 466px 690px #A1B8D0 , 335px 794px #A1B8D0 , 715px 917px #A1B8D0 , 497px 270px #A1B8D0 , 532px 486px #A1B8D0 , 975px 800px #A1B8D0 , 248px 999px #A1B8D0 , 813px 355px #A1B8D0 , 444px 871px #A1B8D0 , 687px 631px #A1B8D0 , 438px 632px #A1B8D0 , 976px 948px #A1B8D0 , 69px 324px #A1B8D0 , 508px 52px #A1B8D0 , 945px 692px #A1B8D0 , 129px 733px #A1B8D0 , 629px 266px #A1B8D0 , 858px 729px #A1B8D0 , 10px 40px #A1B8D0 , 251px 371px #A1B8D0 , 345px 599px #A1B8D0;
  }
  
  @-moz-keyframes glitter-21 {
    0%,
      100%,
      58.06452%,
      68.06452% {
      opacity: 0;
    }
    63.06452% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-21 {
    0%,
      100%,
      58.06452%,
      68.06452% {
      opacity: 0;
    }
    63.06452% {
      opacity: 1;
    }
  }
  @keyframes glitter-21 {
    0%,
      100%,
      58.06452%,
      68.06452% {
      opacity: 0;
    }
    63.06452% {
      opacity: 1;
    }
  }
  .glitter_21 {
    -moz-animation: glitter-21 10s infinite;
    -webkit-animation: glitter-21 10s infinite;
    animation: glitter-21 10s infinite;
    box-shadow: 693px 709px #A1B8D0 , 770px 293px #A1B8D0 , 532px 12px #A1B8D0 , 995px 970px #A1B8D0 , 999px 70px #A1B8D0 , 641px 543px #A1B8D0 , 260px 899px #A1B8D0 , 127px 798px #A1B8D0 , 279px 17px #A1B8D0 , 344px 280px #A1B8D0 , 31px 594px #A1B8D0 , 836px 516px #A1B8D0 , 33px 874px #A1B8D0 , 859px 827px #A1B8D0 , 88px 238px #A1B8D0 , 229px 282px #A1B8D0 , 427px 183px #A1B8D0 , 139px 282px #A1B8D0 , 616px 934px #A1B8D0 , 952px 796px #A1B8D0 , 690px 537px #A1B8D0 , 291px 762px #A1B8D0 , 368px 954px #A1B8D0 , 402px 459px #A1B8D0 , 751px 404px #A1B8D0 , 317px 690px #A1B8D0 , 530px 667px #A1B8D0 , 376px 966px #A1B8D0 , 263px 593px #A1B8D0 , 810px 143px #A1B8D0 , 250px 557px #A1B8D0 , 309px 511px #A1B8D0 , 697px 30px #A1B8D0 , 801px 796px #A1B8D0 , 718px 25px #A1B8D0 , 57px 688px #A1B8D0 , 889px 677px #A1B8D0 , 754px 877px #A1B8D0 , 822px 278px #A1B8D0 , 482px 163px #A1B8D0 , 926px 272px #A1B8D0 , 583px 540px #A1B8D0 , 790px 885px #A1B8D0 , 876px 903px #A1B8D0 , 497px 308px #A1B8D0 , 146px 576px #A1B8D0 , 687px 552px #A1B8D0 , 194px 437px #A1B8D0 , 112px 972px #A1B8D0 , 583px 640px #A1B8D0 , 404px 507px #A1B8D0 , 446px 717px #A1B8D0 , 865px 859px #A1B8D0 , 34px 401px #A1B8D0 , 574px 159px #A1B8D0 , 799px 205px #A1B8D0 , 91px 793px #A1B8D0 , 453px 53px #A1B8D0 , 155px 116px #A1B8D0 , 451px 895px #A1B8D0 , 11px 277px #A1B8D0 , 517px 163px #A1B8D0 , 530px 376px #A1B8D0 , 791px 951px #A1B8D0 , 418px 523px #A1B8D0 , 97px 676px #A1B8D0 , 96px 244px #A1B8D0 , 843px 564px #A1B8D0 , 663px 751px #A1B8D0 , 4px 49px #A1B8D0 , 358px 87px #A1B8D0 , 622px 230px #A1B8D0 , 396px 473px #A1B8D0 , 725px 49px #A1B8D0 , 883px 409px #A1B8D0 , 737px 310px #A1B8D0 , 109px 874px #A1B8D0 , 148px 899px #A1B8D0 , 783px 980px #A1B8D0 , 602px 81px #A1B8D0 , 91px 606px #A1B8D0 , 960px 794px #A1B8D0 , 982px 428px #A1B8D0 , 81px 112px #A1B8D0 , 628px 690px #A1B8D0 , 913px 148px #A1B8D0 , 480px 904px #A1B8D0 , 84px 183px #A1B8D0 , 231px 588px #A1B8D0 , 494px 832px #A1B8D0 , 680px 942px #A1B8D0 , 624px 524px #A1B8D0 , 872px 213px #A1B8D0 , 121px 152px #A1B8D0 , 754px 900px #A1B8D0 , 234px 575px #A1B8D0 , 198px 979px #A1B8D0 , 225px 49px #A1B8D0 , 960px 123px #A1B8D0 , 862px 993px #A1B8D0 , 830px 916px #A1B8D0 , 317px 900px #A1B8D0 , 903px 539px #A1B8D0 , 890px 424px #A1B8D0 , 390px 530px #A1B8D0 , 238px 590px #A1B8D0 , 282px 38px #A1B8D0 , 429px 689px #A1B8D0 , 873px 53px #A1B8D0 , 654px 797px #A1B8D0 , 903px 121px #A1B8D0 , 958px 288px #A1B8D0 , 585px 887px #A1B8D0 , 900px 441px #A1B8D0 , 616px 571px #A1B8D0 , 690px 754px #A1B8D0 , 195px 117px #A1B8D0 , 769px 683px #A1B8D0 , 452px 392px #A1B8D0 , 256px 690px #A1B8D0 , 683px 683px #A1B8D0 , 45px 756px #A1B8D0 , 462px 427px #A1B8D0 , 3px 530px #A1B8D0 , 96px 39px #A1B8D0 , 716px 670px #A1B8D0 , 484px 283px #A1B8D0 , 254px 906px #A1B8D0 , 996px 336px #A1B8D0 , 963px 481px #A1B8D0 , 617px 463px #A1B8D0 , 580px 955px #A1B8D0 , 135px 620px #A1B8D0 , 797px 816px #A1B8D0 , 557px 718px #A1B8D0 , 431px 90px #A1B8D0 , 901px 120px #A1B8D0 , 83px 609px #A1B8D0 , 111px 242px #A1B8D0 , 597px 362px #A1B8D0 , 280px 707px #A1B8D0 , 212px 564px #A1B8D0 , 467px 372px #A1B8D0 , 308px 934px #A1B8D0 , 224px 630px #A1B8D0 , 723px 739px #A1B8D0 , 624px 969px #A1B8D0 , 971px 564px #A1B8D0 , 431px 857px #A1B8D0 , 511px 875px #A1B8D0 , 605px 425px #A1B8D0 , 671px 363px #A1B8D0 , 149px 787px #A1B8D0 , 486px 964px #A1B8D0 , 706px 717px #A1B8D0 , 289px 82px #A1B8D0 , 357px 200px #A1B8D0 , 925px 508px #A1B8D0 , 343px 520px #A1B8D0 , 83px 944px #A1B8D0 , 940px 918px #A1B8D0 , 670px 785px #A1B8D0 , 334px 126px #A1B8D0 , 963px 92px #A1B8D0 , 925px 705px #A1B8D0 , 659px 351px #A1B8D0 , 321px 988px #A1B8D0 , 743px 269px #A1B8D0 , 955px 42px #A1B8D0 , 309px 495px #A1B8D0 , 797px 80px #A1B8D0 , 928px 339px #A1B8D0 , 250px 931px #A1B8D0 , 650px 101px #A1B8D0 , 721px 459px #A1B8D0 , 533px 269px #A1B8D0 , 699px 491px #A1B8D0 , 678px 168px #A1B8D0 , 528px 520px #A1B8D0 , 869px 222px #A1B8D0 , 545px 989px #A1B8D0 , 964px 324px #A1B8D0 , 798px 896px #A1B8D0 , 33px 370px #A1B8D0 , 369px 44px #A1B8D0 , 149px 66px #A1B8D0 , 462px 374px #A1B8D0 , 834px 781px #A1B8D0 , 136px 817px #A1B8D0 , 513px 970px #A1B8D0 , 362px 694px #A1B8D0 , 646px 726px #A1B8D0 , 635px 970px #A1B8D0 , 182px 492px #A1B8D0 , 619px 230px #A1B8D0 , 778px 393px #A1B8D0 , 421px 667px #A1B8D0 , 27px 99px #A1B8D0 , 976px 878px #A1B8D0 , 782px 101px #A1B8D0;
  }
  .glitter_21:before {
    -moz-animation: glitter-21 8s infinite;
    -webkit-animation: glitter-21 8s infinite;
    animation: glitter-21 8s infinite;
    box-shadow: 693px 709px #A1B8D0 , 770px 293px #A1B8D0 , 532px 12px #A1B8D0 , 995px 970px #A1B8D0 , 999px 70px #A1B8D0 , 641px 543px #A1B8D0 , 260px 899px #A1B8D0 , 127px 798px #A1B8D0 , 279px 17px #A1B8D0 , 344px 280px #A1B8D0 , 31px 594px #A1B8D0 , 836px 516px #A1B8D0 , 33px 874px #A1B8D0 , 859px 827px #A1B8D0 , 88px 238px #A1B8D0 , 229px 282px #A1B8D0 , 427px 183px #A1B8D0 , 139px 282px #A1B8D0 , 616px 934px #A1B8D0 , 952px 796px #A1B8D0 , 690px 537px #A1B8D0 , 291px 762px #A1B8D0 , 368px 954px #A1B8D0 , 402px 459px #A1B8D0 , 751px 404px #A1B8D0 , 317px 690px #A1B8D0 , 530px 667px #A1B8D0 , 376px 966px #A1B8D0 , 263px 593px #A1B8D0 , 810px 143px #A1B8D0 , 250px 557px #A1B8D0 , 309px 511px #A1B8D0 , 697px 30px #A1B8D0 , 801px 796px #A1B8D0 , 718px 25px #A1B8D0 , 57px 688px #A1B8D0 , 889px 677px #A1B8D0 , 754px 877px #A1B8D0 , 822px 278px #A1B8D0 , 482px 163px #A1B8D0 , 926px 272px #A1B8D0 , 583px 540px #A1B8D0 , 790px 885px #A1B8D0 , 876px 903px #A1B8D0 , 497px 308px #A1B8D0 , 146px 576px #A1B8D0 , 687px 552px #A1B8D0 , 194px 437px #A1B8D0 , 112px 972px #A1B8D0 , 583px 640px #A1B8D0 , 404px 507px #A1B8D0 , 446px 717px #A1B8D0 , 865px 859px #A1B8D0 , 34px 401px #A1B8D0 , 574px 159px #A1B8D0 , 799px 205px #A1B8D0 , 91px 793px #A1B8D0 , 453px 53px #A1B8D0 , 155px 116px #A1B8D0 , 451px 895px #A1B8D0 , 11px 277px #A1B8D0 , 517px 163px #A1B8D0 , 530px 376px #A1B8D0 , 791px 951px #A1B8D0 , 418px 523px #A1B8D0 , 97px 676px #A1B8D0 , 96px 244px #A1B8D0 , 843px 564px #A1B8D0 , 663px 751px #A1B8D0 , 4px 49px #A1B8D0 , 358px 87px #A1B8D0 , 622px 230px #A1B8D0 , 396px 473px #A1B8D0 , 725px 49px #A1B8D0 , 883px 409px #A1B8D0 , 737px 310px #A1B8D0 , 109px 874px #A1B8D0 , 148px 899px #A1B8D0 , 783px 980px #A1B8D0 , 602px 81px #A1B8D0 , 91px 606px #A1B8D0 , 960px 794px #A1B8D0 , 982px 428px #A1B8D0 , 81px 112px #A1B8D0 , 628px 690px #A1B8D0 , 913px 148px #A1B8D0 , 480px 904px #A1B8D0 , 84px 183px #A1B8D0 , 231px 588px #A1B8D0 , 494px 832px #A1B8D0 , 680px 942px #A1B8D0 , 624px 524px #A1B8D0 , 872px 213px #A1B8D0 , 121px 152px #A1B8D0 , 754px 900px #A1B8D0 , 234px 575px #A1B8D0 , 198px 979px #A1B8D0 , 225px 49px #A1B8D0 , 960px 123px #A1B8D0 , 862px 993px #A1B8D0 , 830px 916px #A1B8D0 , 317px 900px #A1B8D0 , 903px 539px #A1B8D0 , 890px 424px #A1B8D0 , 390px 530px #A1B8D0 , 238px 590px #A1B8D0 , 282px 38px #A1B8D0 , 429px 689px #A1B8D0 , 873px 53px #A1B8D0 , 654px 797px #A1B8D0 , 903px 121px #A1B8D0 , 958px 288px #A1B8D0 , 585px 887px #A1B8D0 , 900px 441px #A1B8D0 , 616px 571px #A1B8D0 , 690px 754px #A1B8D0 , 195px 117px #A1B8D0 , 769px 683px #A1B8D0 , 452px 392px #A1B8D0 , 256px 690px #A1B8D0 , 683px 683px #A1B8D0 , 45px 756px #A1B8D0 , 462px 427px #A1B8D0 , 3px 530px #A1B8D0 , 96px 39px #A1B8D0 , 716px 670px #A1B8D0 , 484px 283px #A1B8D0 , 254px 906px #A1B8D0 , 996px 336px #A1B8D0 , 963px 481px #A1B8D0 , 617px 463px #A1B8D0 , 580px 955px #A1B8D0 , 135px 620px #A1B8D0 , 797px 816px #A1B8D0 , 557px 718px #A1B8D0 , 431px 90px #A1B8D0 , 901px 120px #A1B8D0 , 83px 609px #A1B8D0 , 111px 242px #A1B8D0 , 597px 362px #A1B8D0 , 280px 707px #A1B8D0 , 212px 564px #A1B8D0 , 467px 372px #A1B8D0 , 308px 934px #A1B8D0 , 224px 630px #A1B8D0 , 723px 739px #A1B8D0 , 624px 969px #A1B8D0 , 971px 564px #A1B8D0 , 431px 857px #A1B8D0 , 511px 875px #A1B8D0 , 605px 425px #A1B8D0 , 671px 363px #A1B8D0 , 149px 787px #A1B8D0 , 486px 964px #A1B8D0 , 706px 717px #A1B8D0 , 289px 82px #A1B8D0 , 357px 200px #A1B8D0 , 925px 508px #A1B8D0 , 343px 520px #A1B8D0 , 83px 944px #A1B8D0 , 940px 918px #A1B8D0 , 670px 785px #A1B8D0 , 334px 126px #A1B8D0 , 963px 92px #A1B8D0 , 925px 705px #A1B8D0 , 659px 351px #A1B8D0 , 321px 988px #A1B8D0 , 743px 269px #A1B8D0 , 955px 42px #A1B8D0 , 309px 495px #A1B8D0 , 797px 80px #A1B8D0 , 928px 339px #A1B8D0 , 250px 931px #A1B8D0 , 650px 101px #A1B8D0 , 721px 459px #A1B8D0 , 533px 269px #A1B8D0 , 699px 491px #A1B8D0 , 678px 168px #A1B8D0 , 528px 520px #A1B8D0 , 869px 222px #A1B8D0 , 545px 989px #A1B8D0 , 964px 324px #A1B8D0 , 798px 896px #A1B8D0 , 33px 370px #A1B8D0 , 369px 44px #A1B8D0 , 149px 66px #A1B8D0 , 462px 374px #A1B8D0 , 834px 781px #A1B8D0 , 136px 817px #A1B8D0 , 513px 970px #A1B8D0 , 362px 694px #A1B8D0 , 646px 726px #A1B8D0 , 635px 970px #A1B8D0 , 182px 492px #A1B8D0 , 619px 230px #A1B8D0 , 778px 393px #A1B8D0 , 421px 667px #A1B8D0 , 27px 99px #A1B8D0 , 976px 878px #A1B8D0 , 782px 101px #A1B8D0;
  }
  .glitter_21:after {
    -moz-animation: glitter-21 9s infinite;
    -webkit-animation: glitter-21 9s infinite;
    animation: glitter-21 9s infinite;
    box-shadow: 693px 709px #A1B8D0 , 770px 293px #A1B8D0 , 532px 12px #A1B8D0 , 995px 970px #A1B8D0 , 999px 70px #A1B8D0 , 641px 543px #A1B8D0 , 260px 899px #A1B8D0 , 127px 798px #A1B8D0 , 279px 17px #A1B8D0 , 344px 280px #A1B8D0 , 31px 594px #A1B8D0 , 836px 516px #A1B8D0 , 33px 874px #A1B8D0 , 859px 827px #A1B8D0 , 88px 238px #A1B8D0 , 229px 282px #A1B8D0 , 427px 183px #A1B8D0 , 139px 282px #A1B8D0 , 616px 934px #A1B8D0 , 952px 796px #A1B8D0 , 690px 537px #A1B8D0 , 291px 762px #A1B8D0 , 368px 954px #A1B8D0 , 402px 459px #A1B8D0 , 751px 404px #A1B8D0 , 317px 690px #A1B8D0 , 530px 667px #A1B8D0 , 376px 966px #A1B8D0 , 263px 593px #A1B8D0 , 810px 143px #A1B8D0 , 250px 557px #A1B8D0 , 309px 511px #A1B8D0 , 697px 30px #A1B8D0 , 801px 796px #A1B8D0 , 718px 25px #A1B8D0 , 57px 688px #A1B8D0 , 889px 677px #A1B8D0 , 754px 877px #A1B8D0 , 822px 278px #A1B8D0 , 482px 163px #A1B8D0 , 926px 272px #A1B8D0 , 583px 540px #A1B8D0 , 790px 885px #A1B8D0 , 876px 903px #A1B8D0 , 497px 308px #A1B8D0 , 146px 576px #A1B8D0 , 687px 552px #A1B8D0 , 194px 437px #A1B8D0 , 112px 972px #A1B8D0 , 583px 640px #A1B8D0 , 404px 507px #A1B8D0 , 446px 717px #A1B8D0 , 865px 859px #A1B8D0 , 34px 401px #A1B8D0 , 574px 159px #A1B8D0 , 799px 205px #A1B8D0 , 91px 793px #A1B8D0 , 453px 53px #A1B8D0 , 155px 116px #A1B8D0 , 451px 895px #A1B8D0 , 11px 277px #A1B8D0 , 517px 163px #A1B8D0 , 530px 376px #A1B8D0 , 791px 951px #A1B8D0 , 418px 523px #A1B8D0 , 97px 676px #A1B8D0 , 96px 244px #A1B8D0 , 843px 564px #A1B8D0 , 663px 751px #A1B8D0 , 4px 49px #A1B8D0 , 358px 87px #A1B8D0 , 622px 230px #A1B8D0 , 396px 473px #A1B8D0 , 725px 49px #A1B8D0 , 883px 409px #A1B8D0 , 737px 310px #A1B8D0 , 109px 874px #A1B8D0 , 148px 899px #A1B8D0 , 783px 980px #A1B8D0 , 602px 81px #A1B8D0 , 91px 606px #A1B8D0 , 960px 794px #A1B8D0 , 982px 428px #A1B8D0 , 81px 112px #A1B8D0 , 628px 690px #A1B8D0 , 913px 148px #A1B8D0 , 480px 904px #A1B8D0 , 84px 183px #A1B8D0 , 231px 588px #A1B8D0 , 494px 832px #A1B8D0 , 680px 942px #A1B8D0 , 624px 524px #A1B8D0 , 872px 213px #A1B8D0 , 121px 152px #A1B8D0 , 754px 900px #A1B8D0 , 234px 575px #A1B8D0 , 198px 979px #A1B8D0 , 225px 49px #A1B8D0 , 960px 123px #A1B8D0 , 862px 993px #A1B8D0 , 830px 916px #A1B8D0 , 317px 900px #A1B8D0 , 903px 539px #A1B8D0 , 890px 424px #A1B8D0 , 390px 530px #A1B8D0 , 238px 590px #A1B8D0 , 282px 38px #A1B8D0 , 429px 689px #A1B8D0 , 873px 53px #A1B8D0 , 654px 797px #A1B8D0 , 903px 121px #A1B8D0 , 958px 288px #A1B8D0 , 585px 887px #A1B8D0 , 900px 441px #A1B8D0 , 616px 571px #A1B8D0 , 690px 754px #A1B8D0 , 195px 117px #A1B8D0 , 769px 683px #A1B8D0 , 452px 392px #A1B8D0 , 256px 690px #A1B8D0 , 683px 683px #A1B8D0 , 45px 756px #A1B8D0 , 462px 427px #A1B8D0 , 3px 530px #A1B8D0 , 96px 39px #A1B8D0 , 716px 670px #A1B8D0 , 484px 283px #A1B8D0 , 254px 906px #A1B8D0 , 996px 336px #A1B8D0 , 963px 481px #A1B8D0 , 617px 463px #A1B8D0 , 580px 955px #A1B8D0 , 135px 620px #A1B8D0 , 797px 816px #A1B8D0 , 557px 718px #A1B8D0 , 431px 90px #A1B8D0 , 901px 120px #A1B8D0 , 83px 609px #A1B8D0 , 111px 242px #A1B8D0 , 597px 362px #A1B8D0 , 280px 707px #A1B8D0 , 212px 564px #A1B8D0 , 467px 372px #A1B8D0 , 308px 934px #A1B8D0 , 224px 630px #A1B8D0 , 723px 739px #A1B8D0 , 624px 969px #A1B8D0 , 971px 564px #A1B8D0 , 431px 857px #A1B8D0 , 511px 875px #A1B8D0 , 605px 425px #A1B8D0 , 671px 363px #A1B8D0 , 149px 787px #A1B8D0 , 486px 964px #A1B8D0 , 706px 717px #A1B8D0 , 289px 82px #A1B8D0 , 357px 200px #A1B8D0 , 925px 508px #A1B8D0 , 343px 520px #A1B8D0 , 83px 944px #A1B8D0 , 940px 918px #A1B8D0 , 670px 785px #A1B8D0 , 334px 126px #A1B8D0 , 963px 92px #A1B8D0 , 925px 705px #A1B8D0 , 659px 351px #A1B8D0 , 321px 988px #A1B8D0 , 743px 269px #A1B8D0 , 955px 42px #A1B8D0 , 309px 495px #A1B8D0 , 797px 80px #A1B8D0 , 928px 339px #A1B8D0 , 250px 931px #A1B8D0 , 650px 101px #A1B8D0 , 721px 459px #A1B8D0 , 533px 269px #A1B8D0 , 699px 491px #A1B8D0 , 678px 168px #A1B8D0 , 528px 520px #A1B8D0 , 869px 222px #A1B8D0 , 545px 989px #A1B8D0 , 964px 324px #A1B8D0 , 798px 896px #A1B8D0 , 33px 370px #A1B8D0 , 369px 44px #A1B8D0 , 149px 66px #A1B8D0 , 462px 374px #A1B8D0 , 834px 781px #A1B8D0 , 136px 817px #A1B8D0 , 513px 970px #A1B8D0 , 362px 694px #A1B8D0 , 646px 726px #A1B8D0 , 635px 970px #A1B8D0 , 182px 492px #A1B8D0 , 619px 230px #A1B8D0 , 778px 393px #A1B8D0 , 421px 667px #A1B8D0 , 27px 99px #A1B8D0 , 976px 878px #A1B8D0 , 782px 101px #A1B8D0;
  }
  
  @-moz-keyframes glitter-22 {
    0%,
      100%,
      60.96774%,
      70.96774% {
      opacity: 0;
    }
    65.96774% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-22 {
    0%,
      100%,
      60.96774%,
      70.96774% {
      opacity: 0;
    }
    65.96774% {
      opacity: 1;
    }
  }
  @keyframes glitter-22 {
    0%,
      100%,
      60.96774%,
      70.96774% {
      opacity: 0;
    }
    65.96774% {
      opacity: 1;
    }
  }
  .glitter_22 {
    -moz-animation: glitter-22 10s infinite;
    -webkit-animation: glitter-22 10s infinite;
    animation: glitter-22 10s infinite;
    box-shadow: 899px 334px #A1B8D0 , 425px 671px #A1B8D0 , 529px 303px #A1B8D0 , 311px 198px #A1B8D0 , 878px 669px #A1B8D0 , 313px 412px #A1B8D0 , 56px 193px #A1B8D0 , 197px 952px #A1B8D0 , 693px 412px #A1B8D0 , 392px 257px #A1B8D0 , 660px 819px #A1B8D0 , 88px 79px #A1B8D0 , 672px 868px #A1B8D0 , 190px 527px #A1B8D0 , 437px 511px #A1B8D0 , 381px 439px #A1B8D0 , 525px 578px #A1B8D0 , 171px 720px #A1B8D0 , 396px 775px #A1B8D0 , 27px 476px #A1B8D0 , 539px 109px #A1B8D0 , 1px 242px #A1B8D0 , 477px 874px #A1B8D0 , 741px 210px #A1B8D0 , 271px 82px #A1B8D0 , 405px 721px #A1B8D0 , 817px 575px #A1B8D0 , 990px 842px #A1B8D0 , 446px 903px #A1B8D0 , 89px 418px #A1B8D0 , 901px 382px #A1B8D0 , 907px 935px #A1B8D0 , 746px 748px #A1B8D0 , 767px 754px #A1B8D0 , 924px 873px #A1B8D0 , 555px 278px #A1B8D0 , 138px 201px #A1B8D0 , 424px 179px #A1B8D0 , 859px 855px #A1B8D0 , 442px 527px #A1B8D0 , 666px 662px #A1B8D0 , 801px 937px #A1B8D0 , 254px 122px #A1B8D0 , 59px 205px #A1B8D0 , 399px 381px #A1B8D0 , 843px 474px #A1B8D0 , 10px 37px #A1B8D0 , 329px 775px #A1B8D0 , 529px 231px #A1B8D0 , 590px 215px #A1B8D0 , 578px 282px #A1B8D0 , 74px 349px #A1B8D0 , 851px 372px #A1B8D0 , 354px 44px #A1B8D0 , 853px 515px #A1B8D0 , 316px 648px #A1B8D0 , 989px 443px #A1B8D0 , 487px 272px #A1B8D0 , 985px 733px #A1B8D0 , 274px 809px #A1B8D0 , 868px 319px #A1B8D0 , 886px 615px #A1B8D0 , 632px 836px #A1B8D0 , 963px 356px #A1B8D0 , 238px 886px #A1B8D0 , 487px 476px #A1B8D0 , 456px 590px #A1B8D0 , 846px 528px #A1B8D0 , 258px 699px #A1B8D0 , 284px 386px #A1B8D0 , 77px 690px #A1B8D0 , 860px 101px #A1B8D0 , 848px 23px #A1B8D0 , 768px 389px #A1B8D0 , 193px 58px #A1B8D0 , 293px 299px #A1B8D0 , 925px 690px #A1B8D0 , 546px 327px #A1B8D0 , 492px 998px #A1B8D0 , 996px 156px #A1B8D0 , 960px 58px #A1B8D0 , 814px 654px #A1B8D0 , 721px 190px #A1B8D0 , 67px 834px #A1B8D0 , 635px 775px #A1B8D0 , 200px 636px #A1B8D0 , 868px 148px #A1B8D0 , 792px 698px #A1B8D0 , 369px 757px #A1B8D0 , 322px 824px #A1B8D0 , 263px 909px #A1B8D0 , 823px 435px #A1B8D0 , 589px 456px #A1B8D0 , 69px 411px #A1B8D0 , 219px 216px #A1B8D0 , 918px 874px #A1B8D0 , 294px 509px #A1B8D0 , 669px 957px #A1B8D0 , 225px 244px #A1B8D0 , 642px 1px #A1B8D0 , 936px 418px #A1B8D0 , 638px 690px #A1B8D0 , 73px 657px #A1B8D0 , 11px 671px #A1B8D0 , 521px 798px #A1B8D0 , 360px 326px #A1B8D0 , 271px 369px #A1B8D0 , 325px 367px #A1B8D0 , 424px 479px #A1B8D0 , 675px 509px #A1B8D0 , 493px 949px #A1B8D0 , 120px 46px #A1B8D0 , 804px 386px #A1B8D0 , 197px 763px #A1B8D0 , 367px 637px #A1B8D0 , 301px 939px #A1B8D0 , 984px 334px #A1B8D0 , 504px 693px #A1B8D0 , 722px 776px #A1B8D0 , 760px 714px #A1B8D0 , 124px 976px #A1B8D0 , 257px 791px #A1B8D0 , 871px 214px #A1B8D0 , 679px 402px #A1B8D0 , 436px 595px #A1B8D0 , 301px 869px #A1B8D0 , 649px 210px #A1B8D0 , 68px 418px #A1B8D0 , 587px 900px #A1B8D0 , 82px 309px #A1B8D0 , 72px 944px #A1B8D0 , 36px 870px #A1B8D0 , 430px 427px #A1B8D0 , 861px 885px #A1B8D0 , 980px 284px #A1B8D0 , 417px 673px #A1B8D0 , 149px 559px #A1B8D0 , 341px 202px #A1B8D0 , 479px 620px #A1B8D0 , 374px 870px #A1B8D0 , 878px 986px #A1B8D0 , 774px 354px #A1B8D0 , 589px 328px #A1B8D0 , 578px 883px #A1B8D0 , 196px 222px #A1B8D0 , 54px 355px #A1B8D0 , 566px 820px #A1B8D0 , 889px 673px #A1B8D0 , 638px 912px #A1B8D0 , 224px 70px #A1B8D0 , 347px 951px #A1B8D0 , 630px 516px #A1B8D0 , 382px 132px #A1B8D0 , 195px 4px #A1B8D0 , 750px 121px #A1B8D0 , 734px 55px #A1B8D0 , 108px 959px #A1B8D0 , 798px 370px #A1B8D0 , 797px 85px #A1B8D0 , 632px 94px #A1B8D0 , 901px 605px #A1B8D0 , 560px 663px #A1B8D0 , 768px 911px #A1B8D0 , 423px 635px #A1B8D0 , 270px 726px #A1B8D0 , 568px 719px #A1B8D0 , 143px 329px #A1B8D0 , 983px 560px #A1B8D0 , 171px 712px #A1B8D0 , 450px 247px #A1B8D0 , 71px 734px #A1B8D0 , 481px 34px #A1B8D0 , 161px 3px #A1B8D0 , 72px 870px #A1B8D0 , 658px 101px #A1B8D0 , 653px 140px #A1B8D0 , 110px 593px #A1B8D0 , 536px 25px #A1B8D0 , 289px 519px #A1B8D0 , 237px 593px #A1B8D0 , 189px 760px #A1B8D0 , 166px 844px #A1B8D0 , 742px 282px #A1B8D0 , 828px 305px #A1B8D0 , 959px 361px #A1B8D0 , 818px 975px #A1B8D0 , 886px 619px #A1B8D0 , 147px 186px #A1B8D0 , 282px 775px #A1B8D0 , 821px 143px #A1B8D0 , 577px 426px #A1B8D0 , 850px 170px #A1B8D0 , 666px 742px #A1B8D0 , 114px 886px #A1B8D0 , 329px 507px #A1B8D0 , 594px 111px #A1B8D0 , 148px 213px #A1B8D0 , 673px 344px #A1B8D0 , 93px 608px #A1B8D0 , 358px 961px #A1B8D0;
  }
  .glitter_22:before {
    -moz-animation: glitter-22 8s infinite;
    -webkit-animation: glitter-22 8s infinite;
    animation: glitter-22 8s infinite;
    box-shadow: 899px 334px #A1B8D0 , 425px 671px #A1B8D0 , 529px 303px #A1B8D0 , 311px 198px #A1B8D0 , 878px 669px #A1B8D0 , 313px 412px #A1B8D0 , 56px 193px #A1B8D0 , 197px 952px #A1B8D0 , 693px 412px #A1B8D0 , 392px 257px #A1B8D0 , 660px 819px #A1B8D0 , 88px 79px #A1B8D0 , 672px 868px #A1B8D0 , 190px 527px #A1B8D0 , 437px 511px #A1B8D0 , 381px 439px #A1B8D0 , 525px 578px #A1B8D0 , 171px 720px #A1B8D0 , 396px 775px #A1B8D0 , 27px 476px #A1B8D0 , 539px 109px #A1B8D0 , 1px 242px #A1B8D0 , 477px 874px #A1B8D0 , 741px 210px #A1B8D0 , 271px 82px #A1B8D0 , 405px 721px #A1B8D0 , 817px 575px #A1B8D0 , 990px 842px #A1B8D0 , 446px 903px #A1B8D0 , 89px 418px #A1B8D0 , 901px 382px #A1B8D0 , 907px 935px #A1B8D0 , 746px 748px #A1B8D0 , 767px 754px #A1B8D0 , 924px 873px #A1B8D0 , 555px 278px #A1B8D0 , 138px 201px #A1B8D0 , 424px 179px #A1B8D0 , 859px 855px #A1B8D0 , 442px 527px #A1B8D0 , 666px 662px #A1B8D0 , 801px 937px #A1B8D0 , 254px 122px #A1B8D0 , 59px 205px #A1B8D0 , 399px 381px #A1B8D0 , 843px 474px #A1B8D0 , 10px 37px #A1B8D0 , 329px 775px #A1B8D0 , 529px 231px #A1B8D0 , 590px 215px #A1B8D0 , 578px 282px #A1B8D0 , 74px 349px #A1B8D0 , 851px 372px #A1B8D0 , 354px 44px #A1B8D0 , 853px 515px #A1B8D0 , 316px 648px #A1B8D0 , 989px 443px #A1B8D0 , 487px 272px #A1B8D0 , 985px 733px #A1B8D0 , 274px 809px #A1B8D0 , 868px 319px #A1B8D0 , 886px 615px #A1B8D0 , 632px 836px #A1B8D0 , 963px 356px #A1B8D0 , 238px 886px #A1B8D0 , 487px 476px #A1B8D0 , 456px 590px #A1B8D0 , 846px 528px #A1B8D0 , 258px 699px #A1B8D0 , 284px 386px #A1B8D0 , 77px 690px #A1B8D0 , 860px 101px #A1B8D0 , 848px 23px #A1B8D0 , 768px 389px #A1B8D0 , 193px 58px #A1B8D0 , 293px 299px #A1B8D0 , 925px 690px #A1B8D0 , 546px 327px #A1B8D0 , 492px 998px #A1B8D0 , 996px 156px #A1B8D0 , 960px 58px #A1B8D0 , 814px 654px #A1B8D0 , 721px 190px #A1B8D0 , 67px 834px #A1B8D0 , 635px 775px #A1B8D0 , 200px 636px #A1B8D0 , 868px 148px #A1B8D0 , 792px 698px #A1B8D0 , 369px 757px #A1B8D0 , 322px 824px #A1B8D0 , 263px 909px #A1B8D0 , 823px 435px #A1B8D0 , 589px 456px #A1B8D0 , 69px 411px #A1B8D0 , 219px 216px #A1B8D0 , 918px 874px #A1B8D0 , 294px 509px #A1B8D0 , 669px 957px #A1B8D0 , 225px 244px #A1B8D0 , 642px 1px #A1B8D0 , 936px 418px #A1B8D0 , 638px 690px #A1B8D0 , 73px 657px #A1B8D0 , 11px 671px #A1B8D0 , 521px 798px #A1B8D0 , 360px 326px #A1B8D0 , 271px 369px #A1B8D0 , 325px 367px #A1B8D0 , 424px 479px #A1B8D0 , 675px 509px #A1B8D0 , 493px 949px #A1B8D0 , 120px 46px #A1B8D0 , 804px 386px #A1B8D0 , 197px 763px #A1B8D0 , 367px 637px #A1B8D0 , 301px 939px #A1B8D0 , 984px 334px #A1B8D0 , 504px 693px #A1B8D0 , 722px 776px #A1B8D0 , 760px 714px #A1B8D0 , 124px 976px #A1B8D0 , 257px 791px #A1B8D0 , 871px 214px #A1B8D0 , 679px 402px #A1B8D0 , 436px 595px #A1B8D0 , 301px 869px #A1B8D0 , 649px 210px #A1B8D0 , 68px 418px #A1B8D0 , 587px 900px #A1B8D0 , 82px 309px #A1B8D0 , 72px 944px #A1B8D0 , 36px 870px #A1B8D0 , 430px 427px #A1B8D0 , 861px 885px #A1B8D0 , 980px 284px #A1B8D0 , 417px 673px #A1B8D0 , 149px 559px #A1B8D0 , 341px 202px #A1B8D0 , 479px 620px #A1B8D0 , 374px 870px #A1B8D0 , 878px 986px #A1B8D0 , 774px 354px #A1B8D0 , 589px 328px #A1B8D0 , 578px 883px #A1B8D0 , 196px 222px #A1B8D0 , 54px 355px #A1B8D0 , 566px 820px #A1B8D0 , 889px 673px #A1B8D0 , 638px 912px #A1B8D0 , 224px 70px #A1B8D0 , 347px 951px #A1B8D0 , 630px 516px #A1B8D0 , 382px 132px #A1B8D0 , 195px 4px #A1B8D0 , 750px 121px #A1B8D0 , 734px 55px #A1B8D0 , 108px 959px #A1B8D0 , 798px 370px #A1B8D0 , 797px 85px #A1B8D0 , 632px 94px #A1B8D0 , 901px 605px #A1B8D0 , 560px 663px #A1B8D0 , 768px 911px #A1B8D0 , 423px 635px #A1B8D0 , 270px 726px #A1B8D0 , 568px 719px #A1B8D0 , 143px 329px #A1B8D0 , 983px 560px #A1B8D0 , 171px 712px #A1B8D0 , 450px 247px #A1B8D0 , 71px 734px #A1B8D0 , 481px 34px #A1B8D0 , 161px 3px #A1B8D0 , 72px 870px #A1B8D0 , 658px 101px #A1B8D0 , 653px 140px #A1B8D0 , 110px 593px #A1B8D0 , 536px 25px #A1B8D0 , 289px 519px #A1B8D0 , 237px 593px #A1B8D0 , 189px 760px #A1B8D0 , 166px 844px #A1B8D0 , 742px 282px #A1B8D0 , 828px 305px #A1B8D0 , 959px 361px #A1B8D0 , 818px 975px #A1B8D0 , 886px 619px #A1B8D0 , 147px 186px #A1B8D0 , 282px 775px #A1B8D0 , 821px 143px #A1B8D0 , 577px 426px #A1B8D0 , 850px 170px #A1B8D0 , 666px 742px #A1B8D0 , 114px 886px #A1B8D0 , 329px 507px #A1B8D0 , 594px 111px #A1B8D0 , 148px 213px #A1B8D0 , 673px 344px #A1B8D0 , 93px 608px #A1B8D0 , 358px 961px #A1B8D0;
  }
  .glitter_22:after {
    -moz-animation: glitter-22 9s infinite;
    -webkit-animation: glitter-22 9s infinite;
    animation: glitter-22 9s infinite;
    box-shadow: 899px 334px #A1B8D0 , 425px 671px #A1B8D0 , 529px 303px #A1B8D0 , 311px 198px #A1B8D0 , 878px 669px #A1B8D0 , 313px 412px #A1B8D0 , 56px 193px #A1B8D0 , 197px 952px #A1B8D0 , 693px 412px #A1B8D0 , 392px 257px #A1B8D0 , 660px 819px #A1B8D0 , 88px 79px #A1B8D0 , 672px 868px #A1B8D0 , 190px 527px #A1B8D0 , 437px 511px #A1B8D0 , 381px 439px #A1B8D0 , 525px 578px #A1B8D0 , 171px 720px #A1B8D0 , 396px 775px #A1B8D0 , 27px 476px #A1B8D0 , 539px 109px #A1B8D0 , 1px 242px #A1B8D0 , 477px 874px #A1B8D0 , 741px 210px #A1B8D0 , 271px 82px #A1B8D0 , 405px 721px #A1B8D0 , 817px 575px #A1B8D0 , 990px 842px #A1B8D0 , 446px 903px #A1B8D0 , 89px 418px #A1B8D0 , 901px 382px #A1B8D0 , 907px 935px #A1B8D0 , 746px 748px #A1B8D0 , 767px 754px #A1B8D0 , 924px 873px #A1B8D0 , 555px 278px #A1B8D0 , 138px 201px #A1B8D0 , 424px 179px #A1B8D0 , 859px 855px #A1B8D0 , 442px 527px #A1B8D0 , 666px 662px #A1B8D0 , 801px 937px #A1B8D0 , 254px 122px #A1B8D0 , 59px 205px #A1B8D0 , 399px 381px #A1B8D0 , 843px 474px #A1B8D0 , 10px 37px #A1B8D0 , 329px 775px #A1B8D0 , 529px 231px #A1B8D0 , 590px 215px #A1B8D0 , 578px 282px #A1B8D0 , 74px 349px #A1B8D0 , 851px 372px #A1B8D0 , 354px 44px #A1B8D0 , 853px 515px #A1B8D0 , 316px 648px #A1B8D0 , 989px 443px #A1B8D0 , 487px 272px #A1B8D0 , 985px 733px #A1B8D0 , 274px 809px #A1B8D0 , 868px 319px #A1B8D0 , 886px 615px #A1B8D0 , 632px 836px #A1B8D0 , 963px 356px #A1B8D0 , 238px 886px #A1B8D0 , 487px 476px #A1B8D0 , 456px 590px #A1B8D0 , 846px 528px #A1B8D0 , 258px 699px #A1B8D0 , 284px 386px #A1B8D0 , 77px 690px #A1B8D0 , 860px 101px #A1B8D0 , 848px 23px #A1B8D0 , 768px 389px #A1B8D0 , 193px 58px #A1B8D0 , 293px 299px #A1B8D0 , 925px 690px #A1B8D0 , 546px 327px #A1B8D0 , 492px 998px #A1B8D0 , 996px 156px #A1B8D0 , 960px 58px #A1B8D0 , 814px 654px #A1B8D0 , 721px 190px #A1B8D0 , 67px 834px #A1B8D0 , 635px 775px #A1B8D0 , 200px 636px #A1B8D0 , 868px 148px #A1B8D0 , 792px 698px #A1B8D0 , 369px 757px #A1B8D0 , 322px 824px #A1B8D0 , 263px 909px #A1B8D0 , 823px 435px #A1B8D0 , 589px 456px #A1B8D0 , 69px 411px #A1B8D0 , 219px 216px #A1B8D0 , 918px 874px #A1B8D0 , 294px 509px #A1B8D0 , 669px 957px #A1B8D0 , 225px 244px #A1B8D0 , 642px 1px #A1B8D0 , 936px 418px #A1B8D0 , 638px 690px #A1B8D0 , 73px 657px #A1B8D0 , 11px 671px #A1B8D0 , 521px 798px #A1B8D0 , 360px 326px #A1B8D0 , 271px 369px #A1B8D0 , 325px 367px #A1B8D0 , 424px 479px #A1B8D0 , 675px 509px #A1B8D0 , 493px 949px #A1B8D0 , 120px 46px #A1B8D0 , 804px 386px #A1B8D0 , 197px 763px #A1B8D0 , 367px 637px #A1B8D0 , 301px 939px #A1B8D0 , 984px 334px #A1B8D0 , 504px 693px #A1B8D0 , 722px 776px #A1B8D0 , 760px 714px #A1B8D0 , 124px 976px #A1B8D0 , 257px 791px #A1B8D0 , 871px 214px #A1B8D0 , 679px 402px #A1B8D0 , 436px 595px #A1B8D0 , 301px 869px #A1B8D0 , 649px 210px #A1B8D0 , 68px 418px #A1B8D0 , 587px 900px #A1B8D0 , 82px 309px #A1B8D0 , 72px 944px #A1B8D0 , 36px 870px #A1B8D0 , 430px 427px #A1B8D0 , 861px 885px #A1B8D0 , 980px 284px #A1B8D0 , 417px 673px #A1B8D0 , 149px 559px #A1B8D0 , 341px 202px #A1B8D0 , 479px 620px #A1B8D0 , 374px 870px #A1B8D0 , 878px 986px #A1B8D0 , 774px 354px #A1B8D0 , 589px 328px #A1B8D0 , 578px 883px #A1B8D0 , 196px 222px #A1B8D0 , 54px 355px #A1B8D0 , 566px 820px #A1B8D0 , 889px 673px #A1B8D0 , 638px 912px #A1B8D0 , 224px 70px #A1B8D0 , 347px 951px #A1B8D0 , 630px 516px #A1B8D0 , 382px 132px #A1B8D0 , 195px 4px #A1B8D0 , 750px 121px #A1B8D0 , 734px 55px #A1B8D0 , 108px 959px #A1B8D0 , 798px 370px #A1B8D0 , 797px 85px #A1B8D0 , 632px 94px #A1B8D0 , 901px 605px #A1B8D0 , 560px 663px #A1B8D0 , 768px 911px #A1B8D0 , 423px 635px #A1B8D0 , 270px 726px #A1B8D0 , 568px 719px #A1B8D0 , 143px 329px #A1B8D0 , 983px 560px #A1B8D0 , 171px 712px #A1B8D0 , 450px 247px #A1B8D0 , 71px 734px #A1B8D0 , 481px 34px #A1B8D0 , 161px 3px #A1B8D0 , 72px 870px #A1B8D0 , 658px 101px #A1B8D0 , 653px 140px #A1B8D0 , 110px 593px #A1B8D0 , 536px 25px #A1B8D0 , 289px 519px #A1B8D0 , 237px 593px #A1B8D0 , 189px 760px #A1B8D0 , 166px 844px #A1B8D0 , 742px 282px #A1B8D0 , 828px 305px #A1B8D0 , 959px 361px #A1B8D0 , 818px 975px #A1B8D0 , 886px 619px #A1B8D0 , 147px 186px #A1B8D0 , 282px 775px #A1B8D0 , 821px 143px #A1B8D0 , 577px 426px #A1B8D0 , 850px 170px #A1B8D0 , 666px 742px #A1B8D0 , 114px 886px #A1B8D0 , 329px 507px #A1B8D0 , 594px 111px #A1B8D0 , 148px 213px #A1B8D0 , 673px 344px #A1B8D0 , 93px 608px #A1B8D0 , 358px 961px #A1B8D0;
  }
  
  @-moz-keyframes glitter-23 {
    0%,
      100%,
      63.87097%,
      73.87097% {
      opacity: 0;
    }
    68.87097% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-23 {
    0%,
      100%,
      63.87097%,
      73.87097% {
      opacity: 0;
    }
    68.87097% {
      opacity: 1;
    }
  }
  @keyframes glitter-23 {
    0%,
      100%,
      63.87097%,
      73.87097% {
      opacity: 0;
    }
    68.87097% {
      opacity: 1;
    }
  }
  .glitter_23 {
    -moz-animation: glitter-23 10s infinite;
    -webkit-animation: glitter-23 10s infinite;
    animation: glitter-23 10s infinite;
    box-shadow: 689px 920px #A1B8D0 , 308px 280px #A1B8D0 , 198px 969px #A1B8D0 , 440px 499px #A1B8D0 , 68px 259px #A1B8D0 , 318px 902px #A1B8D0 , 826px 120px #A1B8D0 , 693px 664px #A1B8D0 , 326px 276px #A1B8D0 , 819px 454px #A1B8D0 , 869px 237px #A1B8D0 , 262px 595px #A1B8D0 , 546px 722px #A1B8D0 , 917px 594px #A1B8D0 , 711px 604px #A1B8D0 , 342px 784px #A1B8D0 , 455px 912px #A1B8D0 , 267px 561px #A1B8D0 , 660px 925px #A1B8D0 , 659px 736px #A1B8D0 , 65px 774px #A1B8D0 , 841px 281px #A1B8D0 , 74px 612px #A1B8D0 , 608px 767px #A1B8D0 , 524px 117px #A1B8D0 , 814px 640px #A1B8D0 , 424px 208px #A1B8D0 , 6px 488px #A1B8D0 , 978px 915px #A1B8D0 , 194px 210px #A1B8D0 , 839px 211px #A1B8D0 , 928px 451px #A1B8D0 , 813px 213px #A1B8D0 , 546px 519px #A1B8D0 , 708px 418px #A1B8D0 , 159px 268px #A1B8D0 , 565px 819px #A1B8D0 , 297px 215px #A1B8D0 , 624px 650px #A1B8D0 , 94px 938px #A1B8D0 , 312px 1px #A1B8D0 , 583px 20px #A1B8D0 , 359px 706px #A1B8D0 , 482px 791px #A1B8D0 , 487px 608px #A1B8D0 , 135px 214px #A1B8D0 , 421px 30px #A1B8D0 , 583px 1000px #A1B8D0 , 38px 856px #A1B8D0 , 651px 416px #A1B8D0 , 780px 382px #A1B8D0 , 5px 639px #A1B8D0 , 999px 25px #A1B8D0 , 489px 992px #A1B8D0 , 663px 38px #A1B8D0 , 340px 266px #A1B8D0 , 507px 730px #A1B8D0 , 122px 518px #A1B8D0 , 58px 392px #A1B8D0 , 271px 619px #A1B8D0 , 966px 274px #A1B8D0 , 92px 609px #A1B8D0 , 723px 888px #A1B8D0 , 361px 161px #A1B8D0 , 83px 449px #A1B8D0 , 999px 431px #A1B8D0 , 39px 948px #A1B8D0 , 326px 729px #A1B8D0 , 194px 45px #A1B8D0 , 958px 741px #A1B8D0 , 870px 405px #A1B8D0 , 867px 275px #A1B8D0 , 975px 812px #A1B8D0 , 985px 373px #A1B8D0 , 398px 403px #A1B8D0 , 361px 131px #A1B8D0 , 409px 60px #A1B8D0 , 383px 805px #A1B8D0 , 80px 471px #A1B8D0 , 122px 359px #A1B8D0 , 211px 932px #A1B8D0 , 121px 524px #A1B8D0 , 703px 401px #A1B8D0 , 929px 154px #A1B8D0 , 441px 29px #A1B8D0 , 335px 430px #A1B8D0 , 125px 380px #A1B8D0 , 801px 542px #A1B8D0 , 265px 620px #A1B8D0 , 936px 21px #A1B8D0 , 476px 252px #A1B8D0 , 909px 82px #A1B8D0 , 626px 929px #A1B8D0 , 363px 510px #A1B8D0 , 469px 949px #A1B8D0 , 515px 737px #A1B8D0 , 112px 449px #A1B8D0 , 481px 202px #A1B8D0 , 937px 370px #A1B8D0 , 513px 840px #A1B8D0 , 146px 657px #A1B8D0 , 634px 244px #A1B8D0 , 836px 481px #A1B8D0 , 290px 36px #A1B8D0 , 681px 736px #A1B8D0 , 296px 828px #A1B8D0 , 105px 618px #A1B8D0 , 590px 729px #A1B8D0 , 667px 298px #A1B8D0 , 806px 646px #A1B8D0 , 606px 392px #A1B8D0 , 952px 256px #A1B8D0 , 196px 121px #A1B8D0 , 664px 8px #A1B8D0 , 483px 854px #A1B8D0 , 592px 819px #A1B8D0 , 366px 609px #A1B8D0 , 997px 268px #A1B8D0 , 308px 458px #A1B8D0 , 64px 68px #A1B8D0 , 708px 657px #A1B8D0 , 12px 776px #A1B8D0 , 213px 934px #A1B8D0 , 275px 313px #A1B8D0 , 357px 668px #A1B8D0 , 748px 389px #A1B8D0 , 387px 252px #A1B8D0 , 48px 553px #A1B8D0 , 709px 38px #A1B8D0 , 948px 341px #A1B8D0 , 104px 485px #A1B8D0 , 233px 988px #A1B8D0 , 417px 485px #A1B8D0 , 109px 103px #A1B8D0 , 679px 689px #A1B8D0 , 520px 249px #A1B8D0 , 123px 638px #A1B8D0 , 120px 892px #A1B8D0 , 974px 203px #A1B8D0 , 162px 293px #A1B8D0 , 399px 774px #A1B8D0 , 984px 210px #A1B8D0 , 446px 868px #A1B8D0 , 16px 915px #A1B8D0 , 13px 499px #A1B8D0 , 917px 104px #A1B8D0 , 816px 409px #A1B8D0 , 816px 677px #A1B8D0 , 153px 147px #A1B8D0 , 682px 849px #A1B8D0 , 960px 715px #A1B8D0 , 352px 903px #A1B8D0 , 400px 868px #A1B8D0 , 684px 64px #A1B8D0 , 366px 711px #A1B8D0 , 471px 113px #A1B8D0 , 390px 601px #A1B8D0 , 184px 888px #A1B8D0 , 199px 963px #A1B8D0 , 844px 526px #A1B8D0 , 528px 669px #A1B8D0 , 167px 675px #A1B8D0 , 726px 264px #A1B8D0 , 367px 614px #A1B8D0 , 768px 833px #A1B8D0 , 957px 708px #A1B8D0 , 593px 541px #A1B8D0 , 93px 897px #A1B8D0 , 883px 641px #A1B8D0 , 425px 682px #A1B8D0 , 126px 232px #A1B8D0 , 933px 742px #A1B8D0 , 2px 431px #A1B8D0 , 564px 790px #A1B8D0 , 425px 63px #A1B8D0 , 1000px 914px #A1B8D0 , 971px 589px #A1B8D0 , 103px 655px #A1B8D0 , 278px 395px #A1B8D0 , 606px 107px #A1B8D0 , 734px 147px #A1B8D0 , 23px 655px #A1B8D0 , 330px 657px #A1B8D0 , 697px 704px #A1B8D0 , 427px 807px #A1B8D0 , 720px 838px #A1B8D0 , 187px 359px #A1B8D0 , 442px 909px #A1B8D0 , 358px 917px #A1B8D0 , 303px 759px #A1B8D0 , 1px 177px #A1B8D0 , 995px 93px #A1B8D0 , 904px 919px #A1B8D0 , 915px 183px #A1B8D0 , 450px 709px #A1B8D0 , 647px 41px #A1B8D0 , 231px 412px #A1B8D0 , 593px 665px #A1B8D0 , 490px 969px #A1B8D0 , 843px 67px #A1B8D0;
  }
  .glitter_23:before {
    -moz-animation: glitter-23 8s infinite;
    -webkit-animation: glitter-23 8s infinite;
    animation: glitter-23 8s infinite;
    box-shadow: 689px 920px #A1B8D0 , 308px 280px #A1B8D0 , 198px 969px #A1B8D0 , 440px 499px #A1B8D0 , 68px 259px #A1B8D0 , 318px 902px #A1B8D0 , 826px 120px #A1B8D0 , 693px 664px #A1B8D0 , 326px 276px #A1B8D0 , 819px 454px #A1B8D0 , 869px 237px #A1B8D0 , 262px 595px #A1B8D0 , 546px 722px #A1B8D0 , 917px 594px #A1B8D0 , 711px 604px #A1B8D0 , 342px 784px #A1B8D0 , 455px 912px #A1B8D0 , 267px 561px #A1B8D0 , 660px 925px #A1B8D0 , 659px 736px #A1B8D0 , 65px 774px #A1B8D0 , 841px 281px #A1B8D0 , 74px 612px #A1B8D0 , 608px 767px #A1B8D0 , 524px 117px #A1B8D0 , 814px 640px #A1B8D0 , 424px 208px #A1B8D0 , 6px 488px #A1B8D0 , 978px 915px #A1B8D0 , 194px 210px #A1B8D0 , 839px 211px #A1B8D0 , 928px 451px #A1B8D0 , 813px 213px #A1B8D0 , 546px 519px #A1B8D0 , 708px 418px #A1B8D0 , 159px 268px #A1B8D0 , 565px 819px #A1B8D0 , 297px 215px #A1B8D0 , 624px 650px #A1B8D0 , 94px 938px #A1B8D0 , 312px 1px #A1B8D0 , 583px 20px #A1B8D0 , 359px 706px #A1B8D0 , 482px 791px #A1B8D0 , 487px 608px #A1B8D0 , 135px 214px #A1B8D0 , 421px 30px #A1B8D0 , 583px 1000px #A1B8D0 , 38px 856px #A1B8D0 , 651px 416px #A1B8D0 , 780px 382px #A1B8D0 , 5px 639px #A1B8D0 , 999px 25px #A1B8D0 , 489px 992px #A1B8D0 , 663px 38px #A1B8D0 , 340px 266px #A1B8D0 , 507px 730px #A1B8D0 , 122px 518px #A1B8D0 , 58px 392px #A1B8D0 , 271px 619px #A1B8D0 , 966px 274px #A1B8D0 , 92px 609px #A1B8D0 , 723px 888px #A1B8D0 , 361px 161px #A1B8D0 , 83px 449px #A1B8D0 , 999px 431px #A1B8D0 , 39px 948px #A1B8D0 , 326px 729px #A1B8D0 , 194px 45px #A1B8D0 , 958px 741px #A1B8D0 , 870px 405px #A1B8D0 , 867px 275px #A1B8D0 , 975px 812px #A1B8D0 , 985px 373px #A1B8D0 , 398px 403px #A1B8D0 , 361px 131px #A1B8D0 , 409px 60px #A1B8D0 , 383px 805px #A1B8D0 , 80px 471px #A1B8D0 , 122px 359px #A1B8D0 , 211px 932px #A1B8D0 , 121px 524px #A1B8D0 , 703px 401px #A1B8D0 , 929px 154px #A1B8D0 , 441px 29px #A1B8D0 , 335px 430px #A1B8D0 , 125px 380px #A1B8D0 , 801px 542px #A1B8D0 , 265px 620px #A1B8D0 , 936px 21px #A1B8D0 , 476px 252px #A1B8D0 , 909px 82px #A1B8D0 , 626px 929px #A1B8D0 , 363px 510px #A1B8D0 , 469px 949px #A1B8D0 , 515px 737px #A1B8D0 , 112px 449px #A1B8D0 , 481px 202px #A1B8D0 , 937px 370px #A1B8D0 , 513px 840px #A1B8D0 , 146px 657px #A1B8D0 , 634px 244px #A1B8D0 , 836px 481px #A1B8D0 , 290px 36px #A1B8D0 , 681px 736px #A1B8D0 , 296px 828px #A1B8D0 , 105px 618px #A1B8D0 , 590px 729px #A1B8D0 , 667px 298px #A1B8D0 , 806px 646px #A1B8D0 , 606px 392px #A1B8D0 , 952px 256px #A1B8D0 , 196px 121px #A1B8D0 , 664px 8px #A1B8D0 , 483px 854px #A1B8D0 , 592px 819px #A1B8D0 , 366px 609px #A1B8D0 , 997px 268px #A1B8D0 , 308px 458px #A1B8D0 , 64px 68px #A1B8D0 , 708px 657px #A1B8D0 , 12px 776px #A1B8D0 , 213px 934px #A1B8D0 , 275px 313px #A1B8D0 , 357px 668px #A1B8D0 , 748px 389px #A1B8D0 , 387px 252px #A1B8D0 , 48px 553px #A1B8D0 , 709px 38px #A1B8D0 , 948px 341px #A1B8D0 , 104px 485px #A1B8D0 , 233px 988px #A1B8D0 , 417px 485px #A1B8D0 , 109px 103px #A1B8D0 , 679px 689px #A1B8D0 , 520px 249px #A1B8D0 , 123px 638px #A1B8D0 , 120px 892px #A1B8D0 , 974px 203px #A1B8D0 , 162px 293px #A1B8D0 , 399px 774px #A1B8D0 , 984px 210px #A1B8D0 , 446px 868px #A1B8D0 , 16px 915px #A1B8D0 , 13px 499px #A1B8D0 , 917px 104px #A1B8D0 , 816px 409px #A1B8D0 , 816px 677px #A1B8D0 , 153px 147px #A1B8D0 , 682px 849px #A1B8D0 , 960px 715px #A1B8D0 , 352px 903px #A1B8D0 , 400px 868px #A1B8D0 , 684px 64px #A1B8D0 , 366px 711px #A1B8D0 , 471px 113px #A1B8D0 , 390px 601px #A1B8D0 , 184px 888px #A1B8D0 , 199px 963px #A1B8D0 , 844px 526px #A1B8D0 , 528px 669px #A1B8D0 , 167px 675px #A1B8D0 , 726px 264px #A1B8D0 , 367px 614px #A1B8D0 , 768px 833px #A1B8D0 , 957px 708px #A1B8D0 , 593px 541px #A1B8D0 , 93px 897px #A1B8D0 , 883px 641px #A1B8D0 , 425px 682px #A1B8D0 , 126px 232px #A1B8D0 , 933px 742px #A1B8D0 , 2px 431px #A1B8D0 , 564px 790px #A1B8D0 , 425px 63px #A1B8D0 , 1000px 914px #A1B8D0 , 971px 589px #A1B8D0 , 103px 655px #A1B8D0 , 278px 395px #A1B8D0 , 606px 107px #A1B8D0 , 734px 147px #A1B8D0 , 23px 655px #A1B8D0 , 330px 657px #A1B8D0 , 697px 704px #A1B8D0 , 427px 807px #A1B8D0 , 720px 838px #A1B8D0 , 187px 359px #A1B8D0 , 442px 909px #A1B8D0 , 358px 917px #A1B8D0 , 303px 759px #A1B8D0 , 1px 177px #A1B8D0 , 995px 93px #A1B8D0 , 904px 919px #A1B8D0 , 915px 183px #A1B8D0 , 450px 709px #A1B8D0 , 647px 41px #A1B8D0 , 231px 412px #A1B8D0 , 593px 665px #A1B8D0 , 490px 969px #A1B8D0 , 843px 67px #A1B8D0;
  }
  .glitter_23:after {
    -moz-animation: glitter-23 9s infinite;
    -webkit-animation: glitter-23 9s infinite;
    animation: glitter-23 9s infinite;
    box-shadow: 689px 920px #A1B8D0 , 308px 280px #A1B8D0 , 198px 969px #A1B8D0 , 440px 499px #A1B8D0 , 68px 259px #A1B8D0 , 318px 902px #A1B8D0 , 826px 120px #A1B8D0 , 693px 664px #A1B8D0 , 326px 276px #A1B8D0 , 819px 454px #A1B8D0 , 869px 237px #A1B8D0 , 262px 595px #A1B8D0 , 546px 722px #A1B8D0 , 917px 594px #A1B8D0 , 711px 604px #A1B8D0 , 342px 784px #A1B8D0 , 455px 912px #A1B8D0 , 267px 561px #A1B8D0 , 660px 925px #A1B8D0 , 659px 736px #A1B8D0 , 65px 774px #A1B8D0 , 841px 281px #A1B8D0 , 74px 612px #A1B8D0 , 608px 767px #A1B8D0 , 524px 117px #A1B8D0 , 814px 640px #A1B8D0 , 424px 208px #A1B8D0 , 6px 488px #A1B8D0 , 978px 915px #A1B8D0 , 194px 210px #A1B8D0 , 839px 211px #A1B8D0 , 928px 451px #A1B8D0 , 813px 213px #A1B8D0 , 546px 519px #A1B8D0 , 708px 418px #A1B8D0 , 159px 268px #A1B8D0 , 565px 819px #A1B8D0 , 297px 215px #A1B8D0 , 624px 650px #A1B8D0 , 94px 938px #A1B8D0 , 312px 1px #A1B8D0 , 583px 20px #A1B8D0 , 359px 706px #A1B8D0 , 482px 791px #A1B8D0 , 487px 608px #A1B8D0 , 135px 214px #A1B8D0 , 421px 30px #A1B8D0 , 583px 1000px #A1B8D0 , 38px 856px #A1B8D0 , 651px 416px #A1B8D0 , 780px 382px #A1B8D0 , 5px 639px #A1B8D0 , 999px 25px #A1B8D0 , 489px 992px #A1B8D0 , 663px 38px #A1B8D0 , 340px 266px #A1B8D0 , 507px 730px #A1B8D0 , 122px 518px #A1B8D0 , 58px 392px #A1B8D0 , 271px 619px #A1B8D0 , 966px 274px #A1B8D0 , 92px 609px #A1B8D0 , 723px 888px #A1B8D0 , 361px 161px #A1B8D0 , 83px 449px #A1B8D0 , 999px 431px #A1B8D0 , 39px 948px #A1B8D0 , 326px 729px #A1B8D0 , 194px 45px #A1B8D0 , 958px 741px #A1B8D0 , 870px 405px #A1B8D0 , 867px 275px #A1B8D0 , 975px 812px #A1B8D0 , 985px 373px #A1B8D0 , 398px 403px #A1B8D0 , 361px 131px #A1B8D0 , 409px 60px #A1B8D0 , 383px 805px #A1B8D0 , 80px 471px #A1B8D0 , 122px 359px #A1B8D0 , 211px 932px #A1B8D0 , 121px 524px #A1B8D0 , 703px 401px #A1B8D0 , 929px 154px #A1B8D0 , 441px 29px #A1B8D0 , 335px 430px #A1B8D0 , 125px 380px #A1B8D0 , 801px 542px #A1B8D0 , 265px 620px #A1B8D0 , 936px 21px #A1B8D0 , 476px 252px #A1B8D0 , 909px 82px #A1B8D0 , 626px 929px #A1B8D0 , 363px 510px #A1B8D0 , 469px 949px #A1B8D0 , 515px 737px #A1B8D0 , 112px 449px #A1B8D0 , 481px 202px #A1B8D0 , 937px 370px #A1B8D0 , 513px 840px #A1B8D0 , 146px 657px #A1B8D0 , 634px 244px #A1B8D0 , 836px 481px #A1B8D0 , 290px 36px #A1B8D0 , 681px 736px #A1B8D0 , 296px 828px #A1B8D0 , 105px 618px #A1B8D0 , 590px 729px #A1B8D0 , 667px 298px #A1B8D0 , 806px 646px #A1B8D0 , 606px 392px #A1B8D0 , 952px 256px #A1B8D0 , 196px 121px #A1B8D0 , 664px 8px #A1B8D0 , 483px 854px #A1B8D0 , 592px 819px #A1B8D0 , 366px 609px #A1B8D0 , 997px 268px #A1B8D0 , 308px 458px #A1B8D0 , 64px 68px #A1B8D0 , 708px 657px #A1B8D0 , 12px 776px #A1B8D0 , 213px 934px #A1B8D0 , 275px 313px #A1B8D0 , 357px 668px #A1B8D0 , 748px 389px #A1B8D0 , 387px 252px #A1B8D0 , 48px 553px #A1B8D0 , 709px 38px #A1B8D0 , 948px 341px #A1B8D0 , 104px 485px #A1B8D0 , 233px 988px #A1B8D0 , 417px 485px #A1B8D0 , 109px 103px #A1B8D0 , 679px 689px #A1B8D0 , 520px 249px #A1B8D0 , 123px 638px #A1B8D0 , 120px 892px #A1B8D0 , 974px 203px #A1B8D0 , 162px 293px #A1B8D0 , 399px 774px #A1B8D0 , 984px 210px #A1B8D0 , 446px 868px #A1B8D0 , 16px 915px #A1B8D0 , 13px 499px #A1B8D0 , 917px 104px #A1B8D0 , 816px 409px #A1B8D0 , 816px 677px #A1B8D0 , 153px 147px #A1B8D0 , 682px 849px #A1B8D0 , 960px 715px #A1B8D0 , 352px 903px #A1B8D0 , 400px 868px #A1B8D0 , 684px 64px #A1B8D0 , 366px 711px #A1B8D0 , 471px 113px #A1B8D0 , 390px 601px #A1B8D0 , 184px 888px #A1B8D0 , 199px 963px #A1B8D0 , 844px 526px #A1B8D0 , 528px 669px #A1B8D0 , 167px 675px #A1B8D0 , 726px 264px #A1B8D0 , 367px 614px #A1B8D0 , 768px 833px #A1B8D0 , 957px 708px #A1B8D0 , 593px 541px #A1B8D0 , 93px 897px #A1B8D0 , 883px 641px #A1B8D0 , 425px 682px #A1B8D0 , 126px 232px #A1B8D0 , 933px 742px #A1B8D0 , 2px 431px #A1B8D0 , 564px 790px #A1B8D0 , 425px 63px #A1B8D0 , 1000px 914px #A1B8D0 , 971px 589px #A1B8D0 , 103px 655px #A1B8D0 , 278px 395px #A1B8D0 , 606px 107px #A1B8D0 , 734px 147px #A1B8D0 , 23px 655px #A1B8D0 , 330px 657px #A1B8D0 , 697px 704px #A1B8D0 , 427px 807px #A1B8D0 , 720px 838px #A1B8D0 , 187px 359px #A1B8D0 , 442px 909px #A1B8D0 , 358px 917px #A1B8D0 , 303px 759px #A1B8D0 , 1px 177px #A1B8D0 , 995px 93px #A1B8D0 , 904px 919px #A1B8D0 , 915px 183px #A1B8D0 , 450px 709px #A1B8D0 , 647px 41px #A1B8D0 , 231px 412px #A1B8D0 , 593px 665px #A1B8D0 , 490px 969px #A1B8D0 , 843px 67px #A1B8D0;
  }
  
  @-moz-keyframes glitter-24 {
    0%,
      100%,
      66.77419%,
      76.77419% {
      opacity: 0;
    }
    71.77419% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-24 {
    0%,
      100%,
      66.77419%,
      76.77419% {
      opacity: 0;
    }
    71.77419% {
      opacity: 1;
    }
  }
  @keyframes glitter-24 {
    0%,
      100%,
      66.77419%,
      76.77419% {
      opacity: 0;
    }
    71.77419% {
      opacity: 1;
    }
  }
  .glitter_24 {
    -moz-animation: glitter-24 10s infinite;
    -webkit-animation: glitter-24 10s infinite;
    animation: glitter-24 10s infinite;
    box-shadow: 547px 402px #A1B8D0 , 267px 656px #A1B8D0 , 976px 327px #A1B8D0 , 639px 190px #A1B8D0 , 263px 33px #A1B8D0 , 376px 71px #A1B8D0 , 286px 971px #A1B8D0 , 157px 44px #A1B8D0 , 896px 705px #A1B8D0 , 402px 846px #A1B8D0 , 38px 427px #A1B8D0 , 835px 427px #A1B8D0 , 805px 724px #A1B8D0 , 913px 788px #A1B8D0 , 215px 510px #A1B8D0 , 429px 255px #A1B8D0 , 767px 186px #A1B8D0 , 930px 246px #A1B8D0 , 588px 597px #A1B8D0 , 611px 926px #A1B8D0 , 479px 817px #A1B8D0 , 956px 518px #A1B8D0 , 538px 33px #A1B8D0 , 463px 531px #A1B8D0 , 76px 89px #A1B8D0 , 447px 833px #A1B8D0 , 689px 506px #A1B8D0 , 999px 455px #A1B8D0 , 489px 18px #A1B8D0 , 212px 868px #A1B8D0 , 271px 905px #A1B8D0 , 535px 404px #A1B8D0 , 140px 132px #A1B8D0 , 760px 728px #A1B8D0 , 124px 417px #A1B8D0 , 639px 664px #A1B8D0 , 805px 924px #A1B8D0 , 806px 360px #A1B8D0 , 401px 20px #A1B8D0 , 725px 801px #A1B8D0 , 644px 934px #A1B8D0 , 872px 126px #A1B8D0 , 803px 578px #A1B8D0 , 993px 884px #A1B8D0 , 9px 555px #A1B8D0 , 74px 89px #A1B8D0 , 511px 714px #A1B8D0 , 560px 89px #A1B8D0 , 137px 72px #A1B8D0 , 516px 603px #A1B8D0 , 665px 2px #A1B8D0 , 868px 156px #A1B8D0 , 8px 798px #A1B8D0 , 992px 35px #A1B8D0 , 183px 154px #A1B8D0 , 876px 831px #A1B8D0 , 604px 73px #A1B8D0 , 506px 656px #A1B8D0 , 719px 211px #A1B8D0 , 547px 671px #A1B8D0 , 785px 686px #A1B8D0 , 278px 998px #A1B8D0 , 972px 531px #A1B8D0 , 255px 103px #A1B8D0 , 952px 927px #A1B8D0 , 22px 201px #A1B8D0 , 290px 80px #A1B8D0 , 166px 434px #A1B8D0 , 137px 996px #A1B8D0 , 723px 360px #A1B8D0 , 693px 832px #A1B8D0 , 439px 19px #A1B8D0 , 888px 240px #A1B8D0 , 402px 645px #A1B8D0 , 953px 837px #A1B8D0 , 703px 993px #A1B8D0 , 83px 685px #A1B8D0 , 239px 619px #A1B8D0 , 645px 242px #A1B8D0 , 821px 520px #A1B8D0 , 668px 547px #A1B8D0 , 603px 909px #A1B8D0 , 364px 842px #A1B8D0 , 658px 795px #A1B8D0 , 953px 913px #A1B8D0 , 298px 877px #A1B8D0 , 738px 77px #A1B8D0 , 820px 268px #A1B8D0 , 867px 954px #A1B8D0 , 14px 571px #A1B8D0 , 541px 367px #A1B8D0 , 604px 886px #A1B8D0 , 40px 353px #A1B8D0 , 1px 190px #A1B8D0 , 545px 298px #A1B8D0 , 213px 440px #A1B8D0 , 691px 319px #A1B8D0 , 61px 716px #A1B8D0 , 25px 658px #A1B8D0 , 207px 908px #A1B8D0 , 902px 509px #A1B8D0 , 473px 226px #A1B8D0 , 789px 876px #A1B8D0 , 365px 797px #A1B8D0 , 626px 95px #A1B8D0 , 183px 647px #A1B8D0 , 479px 619px #A1B8D0 , 64px 575px #A1B8D0 , 659px 323px #A1B8D0 , 371px 215px #A1B8D0 , 62px 703px #A1B8D0 , 397px 68px #A1B8D0 , 714px 515px #A1B8D0 , 291px 192px #A1B8D0 , 539px 53px #A1B8D0 , 170px 274px #A1B8D0 , 944px 816px #A1B8D0 , 373px 38px #A1B8D0 , 138px 614px #A1B8D0 , 329px 112px #A1B8D0 , 845px 248px #A1B8D0 , 566px 178px #A1B8D0 , 130px 890px #A1B8D0 , 673px 999px #A1B8D0 , 975px 136px #A1B8D0 , 643px 531px #A1B8D0 , 514px 329px #A1B8D0 , 705px 495px #A1B8D0 , 656px 967px #A1B8D0 , 461px 500px #A1B8D0 , 992px 750px #A1B8D0 , 776px 240px #A1B8D0 , 149px 994px #A1B8D0 , 905px 821px #A1B8D0 , 195px 730px #A1B8D0 , 217px 289px #A1B8D0 , 574px 476px #A1B8D0 , 83px 555px #A1B8D0 , 244px 929px #A1B8D0 , 8px 566px #A1B8D0 , 558px 99px #A1B8D0 , 960px 302px #A1B8D0 , 408px 991px #A1B8D0 , 289px 855px #A1B8D0 , 953px 888px #A1B8D0 , 554px 267px #A1B8D0 , 851px 796px #A1B8D0 , 870px 866px #A1B8D0 , 570px 895px #A1B8D0 , 570px 453px #A1B8D0 , 853px 965px #A1B8D0 , 110px 457px #A1B8D0 , 200px 700px #A1B8D0 , 159px 830px #A1B8D0 , 32px 502px #A1B8D0 , 849px 950px #A1B8D0 , 941px 62px #A1B8D0 , 507px 377px #A1B8D0 , 481px 493px #A1B8D0 , 901px 915px #A1B8D0 , 70px 351px #A1B8D0 , 107px 519px #A1B8D0 , 184px 823px #A1B8D0 , 331px 246px #A1B8D0 , 612px 215px #A1B8D0 , 164px 996px #A1B8D0 , 171px 730px #A1B8D0 , 362px 356px #A1B8D0 , 125px 516px #A1B8D0 , 975px 896px #A1B8D0 , 720px 30px #A1B8D0 , 512px 623px #A1B8D0 , 227px 193px #A1B8D0 , 441px 717px #A1B8D0 , 323px 1000px #A1B8D0 , 231px 902px #A1B8D0 , 391px 495px #A1B8D0 , 825px 427px #A1B8D0 , 632px 74px #A1B8D0 , 203px 942px #A1B8D0 , 953px 449px #A1B8D0 , 548px 973px #A1B8D0 , 459px 425px #A1B8D0 , 633px 821px #A1B8D0 , 374px 157px #A1B8D0 , 645px 261px #A1B8D0 , 613px 293px #A1B8D0 , 997px 358px #A1B8D0 , 948px 88px #A1B8D0 , 427px 467px #A1B8D0 , 644px 839px #A1B8D0 , 135px 542px #A1B8D0 , 199px 811px #A1B8D0 , 217px 875px #A1B8D0 , 755px 297px #A1B8D0 , 694px 636px #A1B8D0 , 550px 383px #A1B8D0 , 742px 988px #A1B8D0 , 183px 350px #A1B8D0 , 311px 982px #A1B8D0;
  }
  .glitter_24:before {
    -moz-animation: glitter-24 8s infinite;
    -webkit-animation: glitter-24 8s infinite;
    animation: glitter-24 8s infinite;
    box-shadow: 547px 402px #A1B8D0 , 267px 656px #A1B8D0 , 976px 327px #A1B8D0 , 639px 190px #A1B8D0 , 263px 33px #A1B8D0 , 376px 71px #A1B8D0 , 286px 971px #A1B8D0 , 157px 44px #A1B8D0 , 896px 705px #A1B8D0 , 402px 846px #A1B8D0 , 38px 427px #A1B8D0 , 835px 427px #A1B8D0 , 805px 724px #A1B8D0 , 913px 788px #A1B8D0 , 215px 510px #A1B8D0 , 429px 255px #A1B8D0 , 767px 186px #A1B8D0 , 930px 246px #A1B8D0 , 588px 597px #A1B8D0 , 611px 926px #A1B8D0 , 479px 817px #A1B8D0 , 956px 518px #A1B8D0 , 538px 33px #A1B8D0 , 463px 531px #A1B8D0 , 76px 89px #A1B8D0 , 447px 833px #A1B8D0 , 689px 506px #A1B8D0 , 999px 455px #A1B8D0 , 489px 18px #A1B8D0 , 212px 868px #A1B8D0 , 271px 905px #A1B8D0 , 535px 404px #A1B8D0 , 140px 132px #A1B8D0 , 760px 728px #A1B8D0 , 124px 417px #A1B8D0 , 639px 664px #A1B8D0 , 805px 924px #A1B8D0 , 806px 360px #A1B8D0 , 401px 20px #A1B8D0 , 725px 801px #A1B8D0 , 644px 934px #A1B8D0 , 872px 126px #A1B8D0 , 803px 578px #A1B8D0 , 993px 884px #A1B8D0 , 9px 555px #A1B8D0 , 74px 89px #A1B8D0 , 511px 714px #A1B8D0 , 560px 89px #A1B8D0 , 137px 72px #A1B8D0 , 516px 603px #A1B8D0 , 665px 2px #A1B8D0 , 868px 156px #A1B8D0 , 8px 798px #A1B8D0 , 992px 35px #A1B8D0 , 183px 154px #A1B8D0 , 876px 831px #A1B8D0 , 604px 73px #A1B8D0 , 506px 656px #A1B8D0 , 719px 211px #A1B8D0 , 547px 671px #A1B8D0 , 785px 686px #A1B8D0 , 278px 998px #A1B8D0 , 972px 531px #A1B8D0 , 255px 103px #A1B8D0 , 952px 927px #A1B8D0 , 22px 201px #A1B8D0 , 290px 80px #A1B8D0 , 166px 434px #A1B8D0 , 137px 996px #A1B8D0 , 723px 360px #A1B8D0 , 693px 832px #A1B8D0 , 439px 19px #A1B8D0 , 888px 240px #A1B8D0 , 402px 645px #A1B8D0 , 953px 837px #A1B8D0 , 703px 993px #A1B8D0 , 83px 685px #A1B8D0 , 239px 619px #A1B8D0 , 645px 242px #A1B8D0 , 821px 520px #A1B8D0 , 668px 547px #A1B8D0 , 603px 909px #A1B8D0 , 364px 842px #A1B8D0 , 658px 795px #A1B8D0 , 953px 913px #A1B8D0 , 298px 877px #A1B8D0 , 738px 77px #A1B8D0 , 820px 268px #A1B8D0 , 867px 954px #A1B8D0 , 14px 571px #A1B8D0 , 541px 367px #A1B8D0 , 604px 886px #A1B8D0 , 40px 353px #A1B8D0 , 1px 190px #A1B8D0 , 545px 298px #A1B8D0 , 213px 440px #A1B8D0 , 691px 319px #A1B8D0 , 61px 716px #A1B8D0 , 25px 658px #A1B8D0 , 207px 908px #A1B8D0 , 902px 509px #A1B8D0 , 473px 226px #A1B8D0 , 789px 876px #A1B8D0 , 365px 797px #A1B8D0 , 626px 95px #A1B8D0 , 183px 647px #A1B8D0 , 479px 619px #A1B8D0 , 64px 575px #A1B8D0 , 659px 323px #A1B8D0 , 371px 215px #A1B8D0 , 62px 703px #A1B8D0 , 397px 68px #A1B8D0 , 714px 515px #A1B8D0 , 291px 192px #A1B8D0 , 539px 53px #A1B8D0 , 170px 274px #A1B8D0 , 944px 816px #A1B8D0 , 373px 38px #A1B8D0 , 138px 614px #A1B8D0 , 329px 112px #A1B8D0 , 845px 248px #A1B8D0 , 566px 178px #A1B8D0 , 130px 890px #A1B8D0 , 673px 999px #A1B8D0 , 975px 136px #A1B8D0 , 643px 531px #A1B8D0 , 514px 329px #A1B8D0 , 705px 495px #A1B8D0 , 656px 967px #A1B8D0 , 461px 500px #A1B8D0 , 992px 750px #A1B8D0 , 776px 240px #A1B8D0 , 149px 994px #A1B8D0 , 905px 821px #A1B8D0 , 195px 730px #A1B8D0 , 217px 289px #A1B8D0 , 574px 476px #A1B8D0 , 83px 555px #A1B8D0 , 244px 929px #A1B8D0 , 8px 566px #A1B8D0 , 558px 99px #A1B8D0 , 960px 302px #A1B8D0 , 408px 991px #A1B8D0 , 289px 855px #A1B8D0 , 953px 888px #A1B8D0 , 554px 267px #A1B8D0 , 851px 796px #A1B8D0 , 870px 866px #A1B8D0 , 570px 895px #A1B8D0 , 570px 453px #A1B8D0 , 853px 965px #A1B8D0 , 110px 457px #A1B8D0 , 200px 700px #A1B8D0 , 159px 830px #A1B8D0 , 32px 502px #A1B8D0 , 849px 950px #A1B8D0 , 941px 62px #A1B8D0 , 507px 377px #A1B8D0 , 481px 493px #A1B8D0 , 901px 915px #A1B8D0 , 70px 351px #A1B8D0 , 107px 519px #A1B8D0 , 184px 823px #A1B8D0 , 331px 246px #A1B8D0 , 612px 215px #A1B8D0 , 164px 996px #A1B8D0 , 171px 730px #A1B8D0 , 362px 356px #A1B8D0 , 125px 516px #A1B8D0 , 975px 896px #A1B8D0 , 720px 30px #A1B8D0 , 512px 623px #A1B8D0 , 227px 193px #A1B8D0 , 441px 717px #A1B8D0 , 323px 1000px #A1B8D0 , 231px 902px #A1B8D0 , 391px 495px #A1B8D0 , 825px 427px #A1B8D0 , 632px 74px #A1B8D0 , 203px 942px #A1B8D0 , 953px 449px #A1B8D0 , 548px 973px #A1B8D0 , 459px 425px #A1B8D0 , 633px 821px #A1B8D0 , 374px 157px #A1B8D0 , 645px 261px #A1B8D0 , 613px 293px #A1B8D0 , 997px 358px #A1B8D0 , 948px 88px #A1B8D0 , 427px 467px #A1B8D0 , 644px 839px #A1B8D0 , 135px 542px #A1B8D0 , 199px 811px #A1B8D0 , 217px 875px #A1B8D0 , 755px 297px #A1B8D0 , 694px 636px #A1B8D0 , 550px 383px #A1B8D0 , 742px 988px #A1B8D0 , 183px 350px #A1B8D0 , 311px 982px #A1B8D0;
  }
  .glitter_24:after {
    -moz-animation: glitter-24 9s infinite;
    -webkit-animation: glitter-24 9s infinite;
    animation: glitter-24 9s infinite;
    box-shadow: 547px 402px #A1B8D0 , 267px 656px #A1B8D0 , 976px 327px #A1B8D0 , 639px 190px #A1B8D0 , 263px 33px #A1B8D0 , 376px 71px #A1B8D0 , 286px 971px #A1B8D0 , 157px 44px #A1B8D0 , 896px 705px #A1B8D0 , 402px 846px #A1B8D0 , 38px 427px #A1B8D0 , 835px 427px #A1B8D0 , 805px 724px #A1B8D0 , 913px 788px #A1B8D0 , 215px 510px #A1B8D0 , 429px 255px #A1B8D0 , 767px 186px #A1B8D0 , 930px 246px #A1B8D0 , 588px 597px #A1B8D0 , 611px 926px #A1B8D0 , 479px 817px #A1B8D0 , 956px 518px #A1B8D0 , 538px 33px #A1B8D0 , 463px 531px #A1B8D0 , 76px 89px #A1B8D0 , 447px 833px #A1B8D0 , 689px 506px #A1B8D0 , 999px 455px #A1B8D0 , 489px 18px #A1B8D0 , 212px 868px #A1B8D0 , 271px 905px #A1B8D0 , 535px 404px #A1B8D0 , 140px 132px #A1B8D0 , 760px 728px #A1B8D0 , 124px 417px #A1B8D0 , 639px 664px #A1B8D0 , 805px 924px #A1B8D0 , 806px 360px #A1B8D0 , 401px 20px #A1B8D0 , 725px 801px #A1B8D0 , 644px 934px #A1B8D0 , 872px 126px #A1B8D0 , 803px 578px #A1B8D0 , 993px 884px #A1B8D0 , 9px 555px #A1B8D0 , 74px 89px #A1B8D0 , 511px 714px #A1B8D0 , 560px 89px #A1B8D0 , 137px 72px #A1B8D0 , 516px 603px #A1B8D0 , 665px 2px #A1B8D0 , 868px 156px #A1B8D0 , 8px 798px #A1B8D0 , 992px 35px #A1B8D0 , 183px 154px #A1B8D0 , 876px 831px #A1B8D0 , 604px 73px #A1B8D0 , 506px 656px #A1B8D0 , 719px 211px #A1B8D0 , 547px 671px #A1B8D0 , 785px 686px #A1B8D0 , 278px 998px #A1B8D0 , 972px 531px #A1B8D0 , 255px 103px #A1B8D0 , 952px 927px #A1B8D0 , 22px 201px #A1B8D0 , 290px 80px #A1B8D0 , 166px 434px #A1B8D0 , 137px 996px #A1B8D0 , 723px 360px #A1B8D0 , 693px 832px #A1B8D0 , 439px 19px #A1B8D0 , 888px 240px #A1B8D0 , 402px 645px #A1B8D0 , 953px 837px #A1B8D0 , 703px 993px #A1B8D0 , 83px 685px #A1B8D0 , 239px 619px #A1B8D0 , 645px 242px #A1B8D0 , 821px 520px #A1B8D0 , 668px 547px #A1B8D0 , 603px 909px #A1B8D0 , 364px 842px #A1B8D0 , 658px 795px #A1B8D0 , 953px 913px #A1B8D0 , 298px 877px #A1B8D0 , 738px 77px #A1B8D0 , 820px 268px #A1B8D0 , 867px 954px #A1B8D0 , 14px 571px #A1B8D0 , 541px 367px #A1B8D0 , 604px 886px #A1B8D0 , 40px 353px #A1B8D0 , 1px 190px #A1B8D0 , 545px 298px #A1B8D0 , 213px 440px #A1B8D0 , 691px 319px #A1B8D0 , 61px 716px #A1B8D0 , 25px 658px #A1B8D0 , 207px 908px #A1B8D0 , 902px 509px #A1B8D0 , 473px 226px #A1B8D0 , 789px 876px #A1B8D0 , 365px 797px #A1B8D0 , 626px 95px #A1B8D0 , 183px 647px #A1B8D0 , 479px 619px #A1B8D0 , 64px 575px #A1B8D0 , 659px 323px #A1B8D0 , 371px 215px #A1B8D0 , 62px 703px #A1B8D0 , 397px 68px #A1B8D0 , 714px 515px #A1B8D0 , 291px 192px #A1B8D0 , 539px 53px #A1B8D0 , 170px 274px #A1B8D0 , 944px 816px #A1B8D0 , 373px 38px #A1B8D0 , 138px 614px #A1B8D0 , 329px 112px #A1B8D0 , 845px 248px #A1B8D0 , 566px 178px #A1B8D0 , 130px 890px #A1B8D0 , 673px 999px #A1B8D0 , 975px 136px #A1B8D0 , 643px 531px #A1B8D0 , 514px 329px #A1B8D0 , 705px 495px #A1B8D0 , 656px 967px #A1B8D0 , 461px 500px #A1B8D0 , 992px 750px #A1B8D0 , 776px 240px #A1B8D0 , 149px 994px #A1B8D0 , 905px 821px #A1B8D0 , 195px 730px #A1B8D0 , 217px 289px #A1B8D0 , 574px 476px #A1B8D0 , 83px 555px #A1B8D0 , 244px 929px #A1B8D0 , 8px 566px #A1B8D0 , 558px 99px #A1B8D0 , 960px 302px #A1B8D0 , 408px 991px #A1B8D0 , 289px 855px #A1B8D0 , 953px 888px #A1B8D0 , 554px 267px #A1B8D0 , 851px 796px #A1B8D0 , 870px 866px #A1B8D0 , 570px 895px #A1B8D0 , 570px 453px #A1B8D0 , 853px 965px #A1B8D0 , 110px 457px #A1B8D0 , 200px 700px #A1B8D0 , 159px 830px #A1B8D0 , 32px 502px #A1B8D0 , 849px 950px #A1B8D0 , 941px 62px #A1B8D0 , 507px 377px #A1B8D0 , 481px 493px #A1B8D0 , 901px 915px #A1B8D0 , 70px 351px #A1B8D0 , 107px 519px #A1B8D0 , 184px 823px #A1B8D0 , 331px 246px #A1B8D0 , 612px 215px #A1B8D0 , 164px 996px #A1B8D0 , 171px 730px #A1B8D0 , 362px 356px #A1B8D0 , 125px 516px #A1B8D0 , 975px 896px #A1B8D0 , 720px 30px #A1B8D0 , 512px 623px #A1B8D0 , 227px 193px #A1B8D0 , 441px 717px #A1B8D0 , 323px 1000px #A1B8D0 , 231px 902px #A1B8D0 , 391px 495px #A1B8D0 , 825px 427px #A1B8D0 , 632px 74px #A1B8D0 , 203px 942px #A1B8D0 , 953px 449px #A1B8D0 , 548px 973px #A1B8D0 , 459px 425px #A1B8D0 , 633px 821px #A1B8D0 , 374px 157px #A1B8D0 , 645px 261px #A1B8D0 , 613px 293px #A1B8D0 , 997px 358px #A1B8D0 , 948px 88px #A1B8D0 , 427px 467px #A1B8D0 , 644px 839px #A1B8D0 , 135px 542px #A1B8D0 , 199px 811px #A1B8D0 , 217px 875px #A1B8D0 , 755px 297px #A1B8D0 , 694px 636px #A1B8D0 , 550px 383px #A1B8D0 , 742px 988px #A1B8D0 , 183px 350px #A1B8D0 , 311px 982px #A1B8D0;
  }
  
  @-moz-keyframes glitter-25 {
    0%,
      100%,
      69.67742%,
      79.67742% {
      opacity: 0;
    }
    74.67742% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-25 {
    0%,
      100%,
      69.67742%,
      79.67742% {
      opacity: 0;
    }
    74.67742% {
      opacity: 1;
    }
  }
  @keyframes glitter-25 {
    0%,
      100%,
      69.67742%,
      79.67742% {
      opacity: 0;
    }
    74.67742% {
      opacity: 1;
    }
  }
  .glitter_25 {
    -moz-animation: glitter-25 10s infinite;
    -webkit-animation: glitter-25 10s infinite;
    animation: glitter-25 10s infinite;
    box-shadow: 252px 775px #A1B8D0 , 571px 91px #A1B8D0 , 485px 98px #A1B8D0 , 976px 824px #A1B8D0 , 55px 492px #A1B8D0 , 31px 48px #A1B8D0 , 10px 548px #A1B8D0 , 191px 547px #A1B8D0 , 25px 759px #A1B8D0 , 49px 440px #A1B8D0 , 14px 126px #A1B8D0 , 705px 571px #A1B8D0 , 657px 857px #A1B8D0 , 416px 821px #A1B8D0 , 169px 946px #A1B8D0 , 123px 927px #A1B8D0 , 122px 633px #A1B8D0 , 555px 25px #A1B8D0 , 410px 240px #A1B8D0 , 800px 801px #A1B8D0 , 680px 885px #A1B8D0 , 202px 909px #A1B8D0 , 95px 876px #A1B8D0 , 541px 417px #A1B8D0 , 833px 143px #A1B8D0 , 954px 624px #A1B8D0 , 190px 661px #A1B8D0 , 782px 630px #A1B8D0 , 578px 882px #A1B8D0 , 909px 566px #A1B8D0 , 315px 123px #A1B8D0 , 749px 714px #A1B8D0 , 484px 807px #A1B8D0 , 740px 507px #A1B8D0 , 973px 403px #A1B8D0 , 142px 957px #A1B8D0 , 717px 214px #A1B8D0 , 582px 645px #A1B8D0 , 97px 668px #A1B8D0 , 801px 492px #A1B8D0 , 400px 408px #A1B8D0 , 457px 151px #A1B8D0 , 188px 703px #A1B8D0 , 697px 745px #A1B8D0 , 720px 57px #A1B8D0 , 393px 469px #A1B8D0 , 326px 651px #A1B8D0 , 138px 620px #A1B8D0 , 771px 160px #A1B8D0 , 134px 840px #A1B8D0 , 52px 702px #A1B8D0 , 230px 831px #A1B8D0 , 614px 966px #A1B8D0 , 385px 404px #A1B8D0 , 968px 829px #A1B8D0 , 239px 272px #A1B8D0 , 550px 853px #A1B8D0 , 773px 405px #A1B8D0 , 282px 394px #A1B8D0 , 549px 749px #A1B8D0 , 917px 19px #A1B8D0 , 818px 309px #A1B8D0 , 507px 101px #A1B8D0 , 63px 474px #A1B8D0 , 79px 321px #A1B8D0 , 358px 808px #A1B8D0 , 651px 829px #A1B8D0 , 385px 124px #A1B8D0 , 248px 583px #A1B8D0 , 970px 311px #A1B8D0 , 930px 453px #A1B8D0 , 884px 191px #A1B8D0 , 745px 811px #A1B8D0 , 19px 902px #A1B8D0 , 969px 870px #A1B8D0 , 284px 366px #A1B8D0 , 369px 126px #A1B8D0 , 750px 947px #A1B8D0 , 368px 369px #A1B8D0 , 993px 560px #A1B8D0 , 578px 156px #A1B8D0 , 751px 596px #A1B8D0 , 536px 753px #A1B8D0 , 874px 609px #A1B8D0 , 606px 436px #A1B8D0 , 645px 379px #A1B8D0 , 257px 405px #A1B8D0 , 531px 921px #A1B8D0 , 370px 831px #A1B8D0 , 380px 698px #A1B8D0 , 42px 281px #A1B8D0 , 275px 973px #A1B8D0 , 763px 428px #A1B8D0 , 822px 69px #A1B8D0 , 524px 995px #A1B8D0 , 409px 695px #A1B8D0 , 97px 771px #A1B8D0 , 751px 439px #A1B8D0 , 736px 720px #A1B8D0 , 629px 847px #A1B8D0 , 16px 868px #A1B8D0 , 166px 397px #A1B8D0 , 757px 98px #A1B8D0 , 438px 703px #A1B8D0 , 373px 386px #A1B8D0 , 271px 221px #A1B8D0 , 929px 984px #A1B8D0 , 40px 924px #A1B8D0 , 326px 167px #A1B8D0 , 436px 339px #A1B8D0 , 421px 167px #A1B8D0 , 39px 751px #A1B8D0 , 297px 665px #A1B8D0 , 162px 794px #A1B8D0 , 749px 930px #A1B8D0 , 625px 865px #A1B8D0 , 955px 33px #A1B8D0 , 801px 623px #A1B8D0 , 430px 127px #A1B8D0 , 659px 208px #A1B8D0 , 474px 353px #A1B8D0 , 517px 897px #A1B8D0 , 551px 833px #A1B8D0 , 280px 189px #A1B8D0 , 221px 907px #A1B8D0 , 579px 888px #A1B8D0 , 308px 868px #A1B8D0 , 141px 633px #A1B8D0 , 482px 356px #A1B8D0 , 684px 176px #A1B8D0 , 330px 828px #A1B8D0 , 211px 51px #A1B8D0 , 454px 685px #A1B8D0 , 458px 117px #A1B8D0 , 255px 603px #A1B8D0 , 529px 45px #A1B8D0 , 937px 91px #A1B8D0 , 889px 313px #A1B8D0 , 483px 744px #A1B8D0 , 120px 40px #A1B8D0 , 471px 8px #A1B8D0 , 816px 684px #A1B8D0 , 120px 183px #A1B8D0 , 441px 272px #A1B8D0 , 165px 345px #A1B8D0 , 261px 753px #A1B8D0 , 753px 822px #A1B8D0 , 721px 172px #A1B8D0 , 181px 789px #A1B8D0 , 56px 769px #A1B8D0 , 619px 641px #A1B8D0 , 794px 623px #A1B8D0 , 124px 777px #A1B8D0 , 134px 951px #A1B8D0 , 878px 390px #A1B8D0 , 475px 464px #A1B8D0 , 739px 776px #A1B8D0 , 299px 414px #A1B8D0 , 244px 346px #A1B8D0 , 918px 539px #A1B8D0 , 958px 887px #A1B8D0 , 576px 151px #A1B8D0 , 257px 386px #A1B8D0 , 612px 833px #A1B8D0 , 368px 32px #A1B8D0 , 375px 679px #A1B8D0 , 807px 382px #A1B8D0 , 305px 212px #A1B8D0 , 418px 152px #A1B8D0 , 803px 30px #A1B8D0 , 402px 203px #A1B8D0 , 986px 820px #A1B8D0 , 977px 802px #A1B8D0 , 874px 485px #A1B8D0 , 204px 854px #A1B8D0 , 238px 956px #A1B8D0 , 7px 122px #A1B8D0 , 220px 107px #A1B8D0 , 993px 255px #A1B8D0 , 586px 895px #A1B8D0 , 983px 26px #A1B8D0 , 951px 281px #A1B8D0 , 913px 102px #A1B8D0 , 861px 596px #A1B8D0 , 247px 732px #A1B8D0 , 710px 447px #A1B8D0 , 832px 299px #A1B8D0 , 860px 164px #A1B8D0 , 653px 516px #A1B8D0 , 597px 564px #A1B8D0 , 527px 516px #A1B8D0 , 689px 7px #A1B8D0 , 283px 344px #A1B8D0 , 580px 137px #A1B8D0 , 8px 417px #A1B8D0 , 892px 337px #A1B8D0 , 441px 880px #A1B8D0 , 224px 239px #A1B8D0 , 901px 631px #A1B8D0 , 439px 284px #A1B8D0;
  }
  .glitter_25:before {
    -moz-animation: glitter-25 8s infinite;
    -webkit-animation: glitter-25 8s infinite;
    animation: glitter-25 8s infinite;
    box-shadow: 252px 775px #A1B8D0 , 571px 91px #A1B8D0 , 485px 98px #A1B8D0 , 976px 824px #A1B8D0 , 55px 492px #A1B8D0 , 31px 48px #A1B8D0 , 10px 548px #A1B8D0 , 191px 547px #A1B8D0 , 25px 759px #A1B8D0 , 49px 440px #A1B8D0 , 14px 126px #A1B8D0 , 705px 571px #A1B8D0 , 657px 857px #A1B8D0 , 416px 821px #A1B8D0 , 169px 946px #A1B8D0 , 123px 927px #A1B8D0 , 122px 633px #A1B8D0 , 555px 25px #A1B8D0 , 410px 240px #A1B8D0 , 800px 801px #A1B8D0 , 680px 885px #A1B8D0 , 202px 909px #A1B8D0 , 95px 876px #A1B8D0 , 541px 417px #A1B8D0 , 833px 143px #A1B8D0 , 954px 624px #A1B8D0 , 190px 661px #A1B8D0 , 782px 630px #A1B8D0 , 578px 882px #A1B8D0 , 909px 566px #A1B8D0 , 315px 123px #A1B8D0 , 749px 714px #A1B8D0 , 484px 807px #A1B8D0 , 740px 507px #A1B8D0 , 973px 403px #A1B8D0 , 142px 957px #A1B8D0 , 717px 214px #A1B8D0 , 582px 645px #A1B8D0 , 97px 668px #A1B8D0 , 801px 492px #A1B8D0 , 400px 408px #A1B8D0 , 457px 151px #A1B8D0 , 188px 703px #A1B8D0 , 697px 745px #A1B8D0 , 720px 57px #A1B8D0 , 393px 469px #A1B8D0 , 326px 651px #A1B8D0 , 138px 620px #A1B8D0 , 771px 160px #A1B8D0 , 134px 840px #A1B8D0 , 52px 702px #A1B8D0 , 230px 831px #A1B8D0 , 614px 966px #A1B8D0 , 385px 404px #A1B8D0 , 968px 829px #A1B8D0 , 239px 272px #A1B8D0 , 550px 853px #A1B8D0 , 773px 405px #A1B8D0 , 282px 394px #A1B8D0 , 549px 749px #A1B8D0 , 917px 19px #A1B8D0 , 818px 309px #A1B8D0 , 507px 101px #A1B8D0 , 63px 474px #A1B8D0 , 79px 321px #A1B8D0 , 358px 808px #A1B8D0 , 651px 829px #A1B8D0 , 385px 124px #A1B8D0 , 248px 583px #A1B8D0 , 970px 311px #A1B8D0 , 930px 453px #A1B8D0 , 884px 191px #A1B8D0 , 745px 811px #A1B8D0 , 19px 902px #A1B8D0 , 969px 870px #A1B8D0 , 284px 366px #A1B8D0 , 369px 126px #A1B8D0 , 750px 947px #A1B8D0 , 368px 369px #A1B8D0 , 993px 560px #A1B8D0 , 578px 156px #A1B8D0 , 751px 596px #A1B8D0 , 536px 753px #A1B8D0 , 874px 609px #A1B8D0 , 606px 436px #A1B8D0 , 645px 379px #A1B8D0 , 257px 405px #A1B8D0 , 531px 921px #A1B8D0 , 370px 831px #A1B8D0 , 380px 698px #A1B8D0 , 42px 281px #A1B8D0 , 275px 973px #A1B8D0 , 763px 428px #A1B8D0 , 822px 69px #A1B8D0 , 524px 995px #A1B8D0 , 409px 695px #A1B8D0 , 97px 771px #A1B8D0 , 751px 439px #A1B8D0 , 736px 720px #A1B8D0 , 629px 847px #A1B8D0 , 16px 868px #A1B8D0 , 166px 397px #A1B8D0 , 757px 98px #A1B8D0 , 438px 703px #A1B8D0 , 373px 386px #A1B8D0 , 271px 221px #A1B8D0 , 929px 984px #A1B8D0 , 40px 924px #A1B8D0 , 326px 167px #A1B8D0 , 436px 339px #A1B8D0 , 421px 167px #A1B8D0 , 39px 751px #A1B8D0 , 297px 665px #A1B8D0 , 162px 794px #A1B8D0 , 749px 930px #A1B8D0 , 625px 865px #A1B8D0 , 955px 33px #A1B8D0 , 801px 623px #A1B8D0 , 430px 127px #A1B8D0 , 659px 208px #A1B8D0 , 474px 353px #A1B8D0 , 517px 897px #A1B8D0 , 551px 833px #A1B8D0 , 280px 189px #A1B8D0 , 221px 907px #A1B8D0 , 579px 888px #A1B8D0 , 308px 868px #A1B8D0 , 141px 633px #A1B8D0 , 482px 356px #A1B8D0 , 684px 176px #A1B8D0 , 330px 828px #A1B8D0 , 211px 51px #A1B8D0 , 454px 685px #A1B8D0 , 458px 117px #A1B8D0 , 255px 603px #A1B8D0 , 529px 45px #A1B8D0 , 937px 91px #A1B8D0 , 889px 313px #A1B8D0 , 483px 744px #A1B8D0 , 120px 40px #A1B8D0 , 471px 8px #A1B8D0 , 816px 684px #A1B8D0 , 120px 183px #A1B8D0 , 441px 272px #A1B8D0 , 165px 345px #A1B8D0 , 261px 753px #A1B8D0 , 753px 822px #A1B8D0 , 721px 172px #A1B8D0 , 181px 789px #A1B8D0 , 56px 769px #A1B8D0 , 619px 641px #A1B8D0 , 794px 623px #A1B8D0 , 124px 777px #A1B8D0 , 134px 951px #A1B8D0 , 878px 390px #A1B8D0 , 475px 464px #A1B8D0 , 739px 776px #A1B8D0 , 299px 414px #A1B8D0 , 244px 346px #A1B8D0 , 918px 539px #A1B8D0 , 958px 887px #A1B8D0 , 576px 151px #A1B8D0 , 257px 386px #A1B8D0 , 612px 833px #A1B8D0 , 368px 32px #A1B8D0 , 375px 679px #A1B8D0 , 807px 382px #A1B8D0 , 305px 212px #A1B8D0 , 418px 152px #A1B8D0 , 803px 30px #A1B8D0 , 402px 203px #A1B8D0 , 986px 820px #A1B8D0 , 977px 802px #A1B8D0 , 874px 485px #A1B8D0 , 204px 854px #A1B8D0 , 238px 956px #A1B8D0 , 7px 122px #A1B8D0 , 220px 107px #A1B8D0 , 993px 255px #A1B8D0 , 586px 895px #A1B8D0 , 983px 26px #A1B8D0 , 951px 281px #A1B8D0 , 913px 102px #A1B8D0 , 861px 596px #A1B8D0 , 247px 732px #A1B8D0 , 710px 447px #A1B8D0 , 832px 299px #A1B8D0 , 860px 164px #A1B8D0 , 653px 516px #A1B8D0 , 597px 564px #A1B8D0 , 527px 516px #A1B8D0 , 689px 7px #A1B8D0 , 283px 344px #A1B8D0 , 580px 137px #A1B8D0 , 8px 417px #A1B8D0 , 892px 337px #A1B8D0 , 441px 880px #A1B8D0 , 224px 239px #A1B8D0 , 901px 631px #A1B8D0 , 439px 284px #A1B8D0;
  }
  .glitter_25:after {
    -moz-animation: glitter-25 9s infinite;
    -webkit-animation: glitter-25 9s infinite;
    animation: glitter-25 9s infinite;
    box-shadow: 252px 775px #A1B8D0 , 571px 91px #A1B8D0 , 485px 98px #A1B8D0 , 976px 824px #A1B8D0 , 55px 492px #A1B8D0 , 31px 48px #A1B8D0 , 10px 548px #A1B8D0 , 191px 547px #A1B8D0 , 25px 759px #A1B8D0 , 49px 440px #A1B8D0 , 14px 126px #A1B8D0 , 705px 571px #A1B8D0 , 657px 857px #A1B8D0 , 416px 821px #A1B8D0 , 169px 946px #A1B8D0 , 123px 927px #A1B8D0 , 122px 633px #A1B8D0 , 555px 25px #A1B8D0 , 410px 240px #A1B8D0 , 800px 801px #A1B8D0 , 680px 885px #A1B8D0 , 202px 909px #A1B8D0 , 95px 876px #A1B8D0 , 541px 417px #A1B8D0 , 833px 143px #A1B8D0 , 954px 624px #A1B8D0 , 190px 661px #A1B8D0 , 782px 630px #A1B8D0 , 578px 882px #A1B8D0 , 909px 566px #A1B8D0 , 315px 123px #A1B8D0 , 749px 714px #A1B8D0 , 484px 807px #A1B8D0 , 740px 507px #A1B8D0 , 973px 403px #A1B8D0 , 142px 957px #A1B8D0 , 717px 214px #A1B8D0 , 582px 645px #A1B8D0 , 97px 668px #A1B8D0 , 801px 492px #A1B8D0 , 400px 408px #A1B8D0 , 457px 151px #A1B8D0 , 188px 703px #A1B8D0 , 697px 745px #A1B8D0 , 720px 57px #A1B8D0 , 393px 469px #A1B8D0 , 326px 651px #A1B8D0 , 138px 620px #A1B8D0 , 771px 160px #A1B8D0 , 134px 840px #A1B8D0 , 52px 702px #A1B8D0 , 230px 831px #A1B8D0 , 614px 966px #A1B8D0 , 385px 404px #A1B8D0 , 968px 829px #A1B8D0 , 239px 272px #A1B8D0 , 550px 853px #A1B8D0 , 773px 405px #A1B8D0 , 282px 394px #A1B8D0 , 549px 749px #A1B8D0 , 917px 19px #A1B8D0 , 818px 309px #A1B8D0 , 507px 101px #A1B8D0 , 63px 474px #A1B8D0 , 79px 321px #A1B8D0 , 358px 808px #A1B8D0 , 651px 829px #A1B8D0 , 385px 124px #A1B8D0 , 248px 583px #A1B8D0 , 970px 311px #A1B8D0 , 930px 453px #A1B8D0 , 884px 191px #A1B8D0 , 745px 811px #A1B8D0 , 19px 902px #A1B8D0 , 969px 870px #A1B8D0 , 284px 366px #A1B8D0 , 369px 126px #A1B8D0 , 750px 947px #A1B8D0 , 368px 369px #A1B8D0 , 993px 560px #A1B8D0 , 578px 156px #A1B8D0 , 751px 596px #A1B8D0 , 536px 753px #A1B8D0 , 874px 609px #A1B8D0 , 606px 436px #A1B8D0 , 645px 379px #A1B8D0 , 257px 405px #A1B8D0 , 531px 921px #A1B8D0 , 370px 831px #A1B8D0 , 380px 698px #A1B8D0 , 42px 281px #A1B8D0 , 275px 973px #A1B8D0 , 763px 428px #A1B8D0 , 822px 69px #A1B8D0 , 524px 995px #A1B8D0 , 409px 695px #A1B8D0 , 97px 771px #A1B8D0 , 751px 439px #A1B8D0 , 736px 720px #A1B8D0 , 629px 847px #A1B8D0 , 16px 868px #A1B8D0 , 166px 397px #A1B8D0 , 757px 98px #A1B8D0 , 438px 703px #A1B8D0 , 373px 386px #A1B8D0 , 271px 221px #A1B8D0 , 929px 984px #A1B8D0 , 40px 924px #A1B8D0 , 326px 167px #A1B8D0 , 436px 339px #A1B8D0 , 421px 167px #A1B8D0 , 39px 751px #A1B8D0 , 297px 665px #A1B8D0 , 162px 794px #A1B8D0 , 749px 930px #A1B8D0 , 625px 865px #A1B8D0 , 955px 33px #A1B8D0 , 801px 623px #A1B8D0 , 430px 127px #A1B8D0 , 659px 208px #A1B8D0 , 474px 353px #A1B8D0 , 517px 897px #A1B8D0 , 551px 833px #A1B8D0 , 280px 189px #A1B8D0 , 221px 907px #A1B8D0 , 579px 888px #A1B8D0 , 308px 868px #A1B8D0 , 141px 633px #A1B8D0 , 482px 356px #A1B8D0 , 684px 176px #A1B8D0 , 330px 828px #A1B8D0 , 211px 51px #A1B8D0 , 454px 685px #A1B8D0 , 458px 117px #A1B8D0 , 255px 603px #A1B8D0 , 529px 45px #A1B8D0 , 937px 91px #A1B8D0 , 889px 313px #A1B8D0 , 483px 744px #A1B8D0 , 120px 40px #A1B8D0 , 471px 8px #A1B8D0 , 816px 684px #A1B8D0 , 120px 183px #A1B8D0 , 441px 272px #A1B8D0 , 165px 345px #A1B8D0 , 261px 753px #A1B8D0 , 753px 822px #A1B8D0 , 721px 172px #A1B8D0 , 181px 789px #A1B8D0 , 56px 769px #A1B8D0 , 619px 641px #A1B8D0 , 794px 623px #A1B8D0 , 124px 777px #A1B8D0 , 134px 951px #A1B8D0 , 878px 390px #A1B8D0 , 475px 464px #A1B8D0 , 739px 776px #A1B8D0 , 299px 414px #A1B8D0 , 244px 346px #A1B8D0 , 918px 539px #A1B8D0 , 958px 887px #A1B8D0 , 576px 151px #A1B8D0 , 257px 386px #A1B8D0 , 612px 833px #A1B8D0 , 368px 32px #A1B8D0 , 375px 679px #A1B8D0 , 807px 382px #A1B8D0 , 305px 212px #A1B8D0 , 418px 152px #A1B8D0 , 803px 30px #A1B8D0 , 402px 203px #A1B8D0 , 986px 820px #A1B8D0 , 977px 802px #A1B8D0 , 874px 485px #A1B8D0 , 204px 854px #A1B8D0 , 238px 956px #A1B8D0 , 7px 122px #A1B8D0 , 220px 107px #A1B8D0 , 993px 255px #A1B8D0 , 586px 895px #A1B8D0 , 983px 26px #A1B8D0 , 951px 281px #A1B8D0 , 913px 102px #A1B8D0 , 861px 596px #A1B8D0 , 247px 732px #A1B8D0 , 710px 447px #A1B8D0 , 832px 299px #A1B8D0 , 860px 164px #A1B8D0 , 653px 516px #A1B8D0 , 597px 564px #A1B8D0 , 527px 516px #A1B8D0 , 689px 7px #A1B8D0 , 283px 344px #A1B8D0 , 580px 137px #A1B8D0 , 8px 417px #A1B8D0 , 892px 337px #A1B8D0 , 441px 880px #A1B8D0 , 224px 239px #A1B8D0 , 901px 631px #A1B8D0 , 439px 284px #A1B8D0;
  }
  
  @-moz-keyframes glitter-26 {
    0%,
      100%,
      72.58065%,
      82.58065% {
      opacity: 0;
    }
    77.58065% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-26 {
    0%,
      100%,
      72.58065%,
      82.58065% {
      opacity: 0;
    }
    77.58065% {
      opacity: 1;
    }
  }
  @keyframes glitter-26 {
    0%,
      100%,
      72.58065%,
      82.58065% {
      opacity: 0;
    }
    77.58065% {
      opacity: 1;
    }
  }
  .glitter_26 {
    -moz-animation: glitter-26 10s infinite;
    -webkit-animation: glitter-26 10s infinite;
    animation: glitter-26 10s infinite;
    box-shadow: 972px 304px #A1B8D0 , 268px 972px #A1B8D0 , 241px 377px #A1B8D0 , 223px 562px #A1B8D0 , 233px 538px #A1B8D0 , 472px 259px #A1B8D0 , 249px 974px #A1B8D0 , 719px 407px #A1B8D0 , 923px 113px #A1B8D0 , 252px 995px #A1B8D0 , 560px 796px #A1B8D0 , 764px 593px #A1B8D0 , 525px 223px #A1B8D0 , 824px 568px #A1B8D0 , 828px 881px #A1B8D0 , 504px 755px #A1B8D0 , 893px 629px #A1B8D0 , 703px 709px #A1B8D0 , 3px 107px #A1B8D0 , 557px 155px #A1B8D0 , 832px 585px #A1B8D0 , 619px 658px #A1B8D0 , 69px 279px #A1B8D0 , 449px 291px #A1B8D0 , 957px 474px #A1B8D0 , 230px 19px #A1B8D0 , 850px 540px #A1B8D0 , 183px 223px #A1B8D0 , 405px 177px #A1B8D0 , 126px 201px #A1B8D0 , 830px 851px #A1B8D0 , 544px 635px #A1B8D0 , 925px 759px #A1B8D0 , 241px 637px #A1B8D0 , 404px 592px #A1B8D0 , 570px 955px #A1B8D0 , 860px 625px #A1B8D0 , 928px 609px #A1B8D0 , 374px 780px #A1B8D0 , 365px 308px #A1B8D0 , 681px 234px #A1B8D0 , 762px 670px #A1B8D0 , 70px 950px #A1B8D0 , 812px 673px #A1B8D0 , 156px 636px #A1B8D0 , 937px 202px #A1B8D0 , 484px 145px #A1B8D0 , 817px 891px #A1B8D0 , 55px 676px #A1B8D0 , 394px 941px #A1B8D0 , 269px 116px #A1B8D0 , 385px 183px #A1B8D0 , 598px 757px #A1B8D0 , 184px 100px #A1B8D0 , 923px 941px #A1B8D0 , 107px 881px #A1B8D0 , 657px 572px #A1B8D0 , 657px 632px #A1B8D0 , 390px 955px #A1B8D0 , 372px 923px #A1B8D0 , 550px 279px #A1B8D0 , 470px 989px #A1B8D0 , 126px 970px #A1B8D0 , 847px 254px #A1B8D0 , 122px 535px #A1B8D0 , 937px 677px #A1B8D0 , 652px 177px #A1B8D0 , 824px 892px #A1B8D0 , 510px 773px #A1B8D0 , 253px 977px #A1B8D0 , 64px 774px #A1B8D0 , 350px 145px #A1B8D0 , 999px 948px #A1B8D0 , 734px 468px #A1B8D0 , 618px 115px #A1B8D0 , 60px 173px #A1B8D0 , 689px 395px #A1B8D0 , 699px 954px #A1B8D0 , 298px 449px #A1B8D0 , 471px 761px #A1B8D0 , 180px 333px #A1B8D0 , 919px 265px #A1B8D0 , 917px 634px #A1B8D0 , 49px 180px #A1B8D0 , 627px 695px #A1B8D0 , 254px 929px #A1B8D0 , 526px 604px #A1B8D0 , 575px 472px #A1B8D0 , 208px 930px #A1B8D0 , 466px 12px #A1B8D0 , 656px 430px #A1B8D0 , 307px 453px #A1B8D0 , 896px 289px #A1B8D0 , 936px 828px #A1B8D0 , 310px 607px #A1B8D0 , 670px 682px #A1B8D0 , 517px 297px #A1B8D0 , 802px 89px #A1B8D0 , 404px 629px #A1B8D0 , 229px 780px #A1B8D0 , 70px 447px #A1B8D0 , 774px 240px #A1B8D0 , 943px 175px #A1B8D0 , 861px 533px #A1B8D0 , 330px 988px #A1B8D0 , 418px 985px #A1B8D0 , 643px 75px #A1B8D0 , 446px 235px #A1B8D0 , 955px 59px #A1B8D0 , 437px 614px #A1B8D0 , 408px 905px #A1B8D0 , 898px 157px #A1B8D0 , 241px 489px #A1B8D0 , 449px 754px #A1B8D0 , 971px 925px #A1B8D0 , 722px 192px #A1B8D0 , 932px 524px #A1B8D0 , 580px 508px #A1B8D0 , 689px 121px #A1B8D0 , 944px 69px #A1B8D0 , 870px 746px #A1B8D0 , 877px 323px #A1B8D0 , 530px 233px #A1B8D0 , 335px 731px #A1B8D0 , 756px 234px #A1B8D0 , 168px 414px #A1B8D0 , 23px 114px #A1B8D0 , 200px 153px #A1B8D0 , 679px 505px #A1B8D0 , 854px 335px #A1B8D0 , 266px 997px #A1B8D0 , 158px 780px #A1B8D0 , 871px 307px #A1B8D0 , 36px 256px #A1B8D0 , 215px 624px #A1B8D0 , 824px 850px #A1B8D0 , 964px 917px #A1B8D0 , 294px 540px #A1B8D0 , 646px 395px #A1B8D0 , 586px 566px #A1B8D0 , 985px 542px #A1B8D0 , 236px 540px #A1B8D0 , 169px 707px #A1B8D0 , 950px 295px #A1B8D0 , 864px 917px #A1B8D0 , 108px 105px #A1B8D0 , 284px 861px #A1B8D0 , 820px 610px #A1B8D0 , 154px 971px #A1B8D0 , 944px 105px #A1B8D0 , 556px 587px #A1B8D0 , 794px 114px #A1B8D0 , 334px 951px #A1B8D0 , 269px 143px #A1B8D0 , 339px 742px #A1B8D0 , 584px 445px #A1B8D0 , 211px 367px #A1B8D0 , 259px 994px #A1B8D0 , 441px 622px #A1B8D0 , 771px 83px #A1B8D0 , 63px 820px #A1B8D0 , 619px 422px #A1B8D0 , 984px 639px #A1B8D0 , 527px 22px #A1B8D0 , 159px 770px #A1B8D0 , 572px 660px #A1B8D0 , 994px 228px #A1B8D0 , 693px 998px #A1B8D0 , 956px 425px #A1B8D0 , 539px 438px #A1B8D0 , 895px 905px #A1B8D0 , 241px 5px #A1B8D0 , 348px 628px #A1B8D0 , 388px 375px #A1B8D0 , 178px 774px #A1B8D0 , 451px 440px #A1B8D0 , 131px 106px #A1B8D0 , 232px 707px #A1B8D0 , 414px 377px #A1B8D0 , 720px 968px #A1B8D0 , 185px 337px #A1B8D0 , 611px 513px #A1B8D0 , 455px 933px #A1B8D0 , 807px 756px #A1B8D0 , 100px 852px #A1B8D0 , 617px 102px #A1B8D0 , 699px 261px #A1B8D0 , 172px 270px #A1B8D0 , 253px 813px #A1B8D0 , 472px 384px #A1B8D0 , 918px 231px #A1B8D0 , 656px 319px #A1B8D0 , 930px 167px #A1B8D0 , 322px 490px #A1B8D0 , 413px 582px #A1B8D0 , 152px 320px #A1B8D0 , 721px 590px #A1B8D0 , 864px 529px #A1B8D0 , 111px 829px #A1B8D0 , 814px 130px #A1B8D0;
  }
  .glitter_26:before {
    -moz-animation: glitter-26 8s infinite;
    -webkit-animation: glitter-26 8s infinite;
    animation: glitter-26 8s infinite;
    box-shadow: 972px 304px #A1B8D0 , 268px 972px #A1B8D0 , 241px 377px #A1B8D0 , 223px 562px #A1B8D0 , 233px 538px #A1B8D0 , 472px 259px #A1B8D0 , 249px 974px #A1B8D0 , 719px 407px #A1B8D0 , 923px 113px #A1B8D0 , 252px 995px #A1B8D0 , 560px 796px #A1B8D0 , 764px 593px #A1B8D0 , 525px 223px #A1B8D0 , 824px 568px #A1B8D0 , 828px 881px #A1B8D0 , 504px 755px #A1B8D0 , 893px 629px #A1B8D0 , 703px 709px #A1B8D0 , 3px 107px #A1B8D0 , 557px 155px #A1B8D0 , 832px 585px #A1B8D0 , 619px 658px #A1B8D0 , 69px 279px #A1B8D0 , 449px 291px #A1B8D0 , 957px 474px #A1B8D0 , 230px 19px #A1B8D0 , 850px 540px #A1B8D0 , 183px 223px #A1B8D0 , 405px 177px #A1B8D0 , 126px 201px #A1B8D0 , 830px 851px #A1B8D0 , 544px 635px #A1B8D0 , 925px 759px #A1B8D0 , 241px 637px #A1B8D0 , 404px 592px #A1B8D0 , 570px 955px #A1B8D0 , 860px 625px #A1B8D0 , 928px 609px #A1B8D0 , 374px 780px #A1B8D0 , 365px 308px #A1B8D0 , 681px 234px #A1B8D0 , 762px 670px #A1B8D0 , 70px 950px #A1B8D0 , 812px 673px #A1B8D0 , 156px 636px #A1B8D0 , 937px 202px #A1B8D0 , 484px 145px #A1B8D0 , 817px 891px #A1B8D0 , 55px 676px #A1B8D0 , 394px 941px #A1B8D0 , 269px 116px #A1B8D0 , 385px 183px #A1B8D0 , 598px 757px #A1B8D0 , 184px 100px #A1B8D0 , 923px 941px #A1B8D0 , 107px 881px #A1B8D0 , 657px 572px #A1B8D0 , 657px 632px #A1B8D0 , 390px 955px #A1B8D0 , 372px 923px #A1B8D0 , 550px 279px #A1B8D0 , 470px 989px #A1B8D0 , 126px 970px #A1B8D0 , 847px 254px #A1B8D0 , 122px 535px #A1B8D0 , 937px 677px #A1B8D0 , 652px 177px #A1B8D0 , 824px 892px #A1B8D0 , 510px 773px #A1B8D0 , 253px 977px #A1B8D0 , 64px 774px #A1B8D0 , 350px 145px #A1B8D0 , 999px 948px #A1B8D0 , 734px 468px #A1B8D0 , 618px 115px #A1B8D0 , 60px 173px #A1B8D0 , 689px 395px #A1B8D0 , 699px 954px #A1B8D0 , 298px 449px #A1B8D0 , 471px 761px #A1B8D0 , 180px 333px #A1B8D0 , 919px 265px #A1B8D0 , 917px 634px #A1B8D0 , 49px 180px #A1B8D0 , 627px 695px #A1B8D0 , 254px 929px #A1B8D0 , 526px 604px #A1B8D0 , 575px 472px #A1B8D0 , 208px 930px #A1B8D0 , 466px 12px #A1B8D0 , 656px 430px #A1B8D0 , 307px 453px #A1B8D0 , 896px 289px #A1B8D0 , 936px 828px #A1B8D0 , 310px 607px #A1B8D0 , 670px 682px #A1B8D0 , 517px 297px #A1B8D0 , 802px 89px #A1B8D0 , 404px 629px #A1B8D0 , 229px 780px #A1B8D0 , 70px 447px #A1B8D0 , 774px 240px #A1B8D0 , 943px 175px #A1B8D0 , 861px 533px #A1B8D0 , 330px 988px #A1B8D0 , 418px 985px #A1B8D0 , 643px 75px #A1B8D0 , 446px 235px #A1B8D0 , 955px 59px #A1B8D0 , 437px 614px #A1B8D0 , 408px 905px #A1B8D0 , 898px 157px #A1B8D0 , 241px 489px #A1B8D0 , 449px 754px #A1B8D0 , 971px 925px #A1B8D0 , 722px 192px #A1B8D0 , 932px 524px #A1B8D0 , 580px 508px #A1B8D0 , 689px 121px #A1B8D0 , 944px 69px #A1B8D0 , 870px 746px #A1B8D0 , 877px 323px #A1B8D0 , 530px 233px #A1B8D0 , 335px 731px #A1B8D0 , 756px 234px #A1B8D0 , 168px 414px #A1B8D0 , 23px 114px #A1B8D0 , 200px 153px #A1B8D0 , 679px 505px #A1B8D0 , 854px 335px #A1B8D0 , 266px 997px #A1B8D0 , 158px 780px #A1B8D0 , 871px 307px #A1B8D0 , 36px 256px #A1B8D0 , 215px 624px #A1B8D0 , 824px 850px #A1B8D0 , 964px 917px #A1B8D0 , 294px 540px #A1B8D0 , 646px 395px #A1B8D0 , 586px 566px #A1B8D0 , 985px 542px #A1B8D0 , 236px 540px #A1B8D0 , 169px 707px #A1B8D0 , 950px 295px #A1B8D0 , 864px 917px #A1B8D0 , 108px 105px #A1B8D0 , 284px 861px #A1B8D0 , 820px 610px #A1B8D0 , 154px 971px #A1B8D0 , 944px 105px #A1B8D0 , 556px 587px #A1B8D0 , 794px 114px #A1B8D0 , 334px 951px #A1B8D0 , 269px 143px #A1B8D0 , 339px 742px #A1B8D0 , 584px 445px #A1B8D0 , 211px 367px #A1B8D0 , 259px 994px #A1B8D0 , 441px 622px #A1B8D0 , 771px 83px #A1B8D0 , 63px 820px #A1B8D0 , 619px 422px #A1B8D0 , 984px 639px #A1B8D0 , 527px 22px #A1B8D0 , 159px 770px #A1B8D0 , 572px 660px #A1B8D0 , 994px 228px #A1B8D0 , 693px 998px #A1B8D0 , 956px 425px #A1B8D0 , 539px 438px #A1B8D0 , 895px 905px #A1B8D0 , 241px 5px #A1B8D0 , 348px 628px #A1B8D0 , 388px 375px #A1B8D0 , 178px 774px #A1B8D0 , 451px 440px #A1B8D0 , 131px 106px #A1B8D0 , 232px 707px #A1B8D0 , 414px 377px #A1B8D0 , 720px 968px #A1B8D0 , 185px 337px #A1B8D0 , 611px 513px #A1B8D0 , 455px 933px #A1B8D0 , 807px 756px #A1B8D0 , 100px 852px #A1B8D0 , 617px 102px #A1B8D0 , 699px 261px #A1B8D0 , 172px 270px #A1B8D0 , 253px 813px #A1B8D0 , 472px 384px #A1B8D0 , 918px 231px #A1B8D0 , 656px 319px #A1B8D0 , 930px 167px #A1B8D0 , 322px 490px #A1B8D0 , 413px 582px #A1B8D0 , 152px 320px #A1B8D0 , 721px 590px #A1B8D0 , 864px 529px #A1B8D0 , 111px 829px #A1B8D0 , 814px 130px #A1B8D0;
  }
  .glitter_26:after {
    -moz-animation: glitter-26 9s infinite;
    -webkit-animation: glitter-26 9s infinite;
    animation: glitter-26 9s infinite;
    box-shadow: 972px 304px #A1B8D0 , 268px 972px #A1B8D0 , 241px 377px #A1B8D0 , 223px 562px #A1B8D0 , 233px 538px #A1B8D0 , 472px 259px #A1B8D0 , 249px 974px #A1B8D0 , 719px 407px #A1B8D0 , 923px 113px #A1B8D0 , 252px 995px #A1B8D0 , 560px 796px #A1B8D0 , 764px 593px #A1B8D0 , 525px 223px #A1B8D0 , 824px 568px #A1B8D0 , 828px 881px #A1B8D0 , 504px 755px #A1B8D0 , 893px 629px #A1B8D0 , 703px 709px #A1B8D0 , 3px 107px #A1B8D0 , 557px 155px #A1B8D0 , 832px 585px #A1B8D0 , 619px 658px #A1B8D0 , 69px 279px #A1B8D0 , 449px 291px #A1B8D0 , 957px 474px #A1B8D0 , 230px 19px #A1B8D0 , 850px 540px #A1B8D0 , 183px 223px #A1B8D0 , 405px 177px #A1B8D0 , 126px 201px #A1B8D0 , 830px 851px #A1B8D0 , 544px 635px #A1B8D0 , 925px 759px #A1B8D0 , 241px 637px #A1B8D0 , 404px 592px #A1B8D0 , 570px 955px #A1B8D0 , 860px 625px #A1B8D0 , 928px 609px #A1B8D0 , 374px 780px #A1B8D0 , 365px 308px #A1B8D0 , 681px 234px #A1B8D0 , 762px 670px #A1B8D0 , 70px 950px #A1B8D0 , 812px 673px #A1B8D0 , 156px 636px #A1B8D0 , 937px 202px #A1B8D0 , 484px 145px #A1B8D0 , 817px 891px #A1B8D0 , 55px 676px #A1B8D0 , 394px 941px #A1B8D0 , 269px 116px #A1B8D0 , 385px 183px #A1B8D0 , 598px 757px #A1B8D0 , 184px 100px #A1B8D0 , 923px 941px #A1B8D0 , 107px 881px #A1B8D0 , 657px 572px #A1B8D0 , 657px 632px #A1B8D0 , 390px 955px #A1B8D0 , 372px 923px #A1B8D0 , 550px 279px #A1B8D0 , 470px 989px #A1B8D0 , 126px 970px #A1B8D0 , 847px 254px #A1B8D0 , 122px 535px #A1B8D0 , 937px 677px #A1B8D0 , 652px 177px #A1B8D0 , 824px 892px #A1B8D0 , 510px 773px #A1B8D0 , 253px 977px #A1B8D0 , 64px 774px #A1B8D0 , 350px 145px #A1B8D0 , 999px 948px #A1B8D0 , 734px 468px #A1B8D0 , 618px 115px #A1B8D0 , 60px 173px #A1B8D0 , 689px 395px #A1B8D0 , 699px 954px #A1B8D0 , 298px 449px #A1B8D0 , 471px 761px #A1B8D0 , 180px 333px #A1B8D0 , 919px 265px #A1B8D0 , 917px 634px #A1B8D0 , 49px 180px #A1B8D0 , 627px 695px #A1B8D0 , 254px 929px #A1B8D0 , 526px 604px #A1B8D0 , 575px 472px #A1B8D0 , 208px 930px #A1B8D0 , 466px 12px #A1B8D0 , 656px 430px #A1B8D0 , 307px 453px #A1B8D0 , 896px 289px #A1B8D0 , 936px 828px #A1B8D0 , 310px 607px #A1B8D0 , 670px 682px #A1B8D0 , 517px 297px #A1B8D0 , 802px 89px #A1B8D0 , 404px 629px #A1B8D0 , 229px 780px #A1B8D0 , 70px 447px #A1B8D0 , 774px 240px #A1B8D0 , 943px 175px #A1B8D0 , 861px 533px #A1B8D0 , 330px 988px #A1B8D0 , 418px 985px #A1B8D0 , 643px 75px #A1B8D0 , 446px 235px #A1B8D0 , 955px 59px #A1B8D0 , 437px 614px #A1B8D0 , 408px 905px #A1B8D0 , 898px 157px #A1B8D0 , 241px 489px #A1B8D0 , 449px 754px #A1B8D0 , 971px 925px #A1B8D0 , 722px 192px #A1B8D0 , 932px 524px #A1B8D0 , 580px 508px #A1B8D0 , 689px 121px #A1B8D0 , 944px 69px #A1B8D0 , 870px 746px #A1B8D0 , 877px 323px #A1B8D0 , 530px 233px #A1B8D0 , 335px 731px #A1B8D0 , 756px 234px #A1B8D0 , 168px 414px #A1B8D0 , 23px 114px #A1B8D0 , 200px 153px #A1B8D0 , 679px 505px #A1B8D0 , 854px 335px #A1B8D0 , 266px 997px #A1B8D0 , 158px 780px #A1B8D0 , 871px 307px #A1B8D0 , 36px 256px #A1B8D0 , 215px 624px #A1B8D0 , 824px 850px #A1B8D0 , 964px 917px #A1B8D0 , 294px 540px #A1B8D0 , 646px 395px #A1B8D0 , 586px 566px #A1B8D0 , 985px 542px #A1B8D0 , 236px 540px #A1B8D0 , 169px 707px #A1B8D0 , 950px 295px #A1B8D0 , 864px 917px #A1B8D0 , 108px 105px #A1B8D0 , 284px 861px #A1B8D0 , 820px 610px #A1B8D0 , 154px 971px #A1B8D0 , 944px 105px #A1B8D0 , 556px 587px #A1B8D0 , 794px 114px #A1B8D0 , 334px 951px #A1B8D0 , 269px 143px #A1B8D0 , 339px 742px #A1B8D0 , 584px 445px #A1B8D0 , 211px 367px #A1B8D0 , 259px 994px #A1B8D0 , 441px 622px #A1B8D0 , 771px 83px #A1B8D0 , 63px 820px #A1B8D0 , 619px 422px #A1B8D0 , 984px 639px #A1B8D0 , 527px 22px #A1B8D0 , 159px 770px #A1B8D0 , 572px 660px #A1B8D0 , 994px 228px #A1B8D0 , 693px 998px #A1B8D0 , 956px 425px #A1B8D0 , 539px 438px #A1B8D0 , 895px 905px #A1B8D0 , 241px 5px #A1B8D0 , 348px 628px #A1B8D0 , 388px 375px #A1B8D0 , 178px 774px #A1B8D0 , 451px 440px #A1B8D0 , 131px 106px #A1B8D0 , 232px 707px #A1B8D0 , 414px 377px #A1B8D0 , 720px 968px #A1B8D0 , 185px 337px #A1B8D0 , 611px 513px #A1B8D0 , 455px 933px #A1B8D0 , 807px 756px #A1B8D0 , 100px 852px #A1B8D0 , 617px 102px #A1B8D0 , 699px 261px #A1B8D0 , 172px 270px #A1B8D0 , 253px 813px #A1B8D0 , 472px 384px #A1B8D0 , 918px 231px #A1B8D0 , 656px 319px #A1B8D0 , 930px 167px #A1B8D0 , 322px 490px #A1B8D0 , 413px 582px #A1B8D0 , 152px 320px #A1B8D0 , 721px 590px #A1B8D0 , 864px 529px #A1B8D0 , 111px 829px #A1B8D0 , 814px 130px #A1B8D0;
  }
  
  @-moz-keyframes glitter-27 {
    0%,
      100%,
      75.48387%,
      85.48387% {
      opacity: 0;
    }
    80.48387% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-27 {
    0%,
      100%,
      75.48387%,
      85.48387% {
      opacity: 0;
    }
    80.48387% {
      opacity: 1;
    }
  }
  @keyframes glitter-27 {
    0%,
      100%,
      75.48387%,
      85.48387% {
      opacity: 0;
    }
    80.48387% {
      opacity: 1;
    }
  }
  .glitter_27 {
    -moz-animation: glitter-27 10s infinite;
    -webkit-animation: glitter-27 10s infinite;
    animation: glitter-27 10s infinite;
    box-shadow: 202px 38px #A1B8D0 , 707px 196px #A1B8D0 , 469px 425px #A1B8D0 , 215px 268px #A1B8D0 , 728px 531px #A1B8D0 , 534px 103px #A1B8D0 , 874px 874px #A1B8D0 , 589px 743px #A1B8D0 , 882px 329px #A1B8D0 , 672px 477px #A1B8D0 , 68px 75px #A1B8D0 , 396px 758px #A1B8D0 , 82px 741px #A1B8D0 , 453px 397px #A1B8D0 , 971px 704px #A1B8D0 , 871px 937px #A1B8D0 , 888px 728px #A1B8D0 , 710px 692px #A1B8D0 , 594px 729px #A1B8D0 , 906px 507px #A1B8D0 , 513px 124px #A1B8D0 , 882px 416px #A1B8D0 , 756px 336px #A1B8D0 , 866px 344px #A1B8D0 , 956px 243px #A1B8D0 , 14px 687px #A1B8D0 , 509px 748px #A1B8D0 , 914px 80px #A1B8D0 , 920px 673px #A1B8D0 , 550px 547px #A1B8D0 , 681px 473px #A1B8D0 , 294px 447px #A1B8D0 , 884px 447px #A1B8D0 , 690px 542px #A1B8D0 , 111px 257px #A1B8D0 , 365px 529px #A1B8D0 , 862px 500px #A1B8D0 , 308px 774px #A1B8D0 , 370px 248px #A1B8D0 , 290px 50px #A1B8D0 , 760px 727px #A1B8D0 , 561px 754px #A1B8D0 , 146px 632px #A1B8D0 , 411px 720px #A1B8D0 , 156px 668px #A1B8D0 , 887px 337px #A1B8D0 , 528px 364px #A1B8D0 , 79px 158px #A1B8D0 , 644px 213px #A1B8D0 , 119px 504px #A1B8D0 , 121px 847px #A1B8D0 , 447px 938px #A1B8D0 , 950px 818px #A1B8D0 , 327px 466px #A1B8D0 , 389px 483px #A1B8D0 , 269px 761px #A1B8D0 , 253px 919px #A1B8D0 , 103px 442px #A1B8D0 , 602px 813px #A1B8D0 , 700px 397px #A1B8D0 , 464px 419px #A1B8D0 , 884px 461px #A1B8D0 , 625px 90px #A1B8D0 , 301px 595px #A1B8D0 , 601px 505px #A1B8D0 , 800px 371px #A1B8D0 , 155px 257px #A1B8D0 , 242px 349px #A1B8D0 , 767px 898px #A1B8D0 , 229px 107px #A1B8D0 , 911px 648px #A1B8D0 , 890px 305px #A1B8D0 , 791px 156px #A1B8D0 , 524px 850px #A1B8D0 , 766px 197px #A1B8D0 , 742px 268px #A1B8D0 , 869px 745px #A1B8D0 , 586px 56px #A1B8D0 , 870px 822px #A1B8D0 , 745px 645px #A1B8D0 , 215px 182px #A1B8D0 , 524px 450px #A1B8D0 , 815px 837px #A1B8D0 , 614px 997px #A1B8D0 , 395px 98px #A1B8D0 , 444px 940px #A1B8D0 , 431px 806px #A1B8D0 , 543px 783px #A1B8D0 , 690px 641px #A1B8D0 , 312px 718px #A1B8D0 , 236px 886px #A1B8D0 , 799px 574px #A1B8D0 , 104px 493px #A1B8D0 , 577px 715px #A1B8D0 , 170px 552px #A1B8D0 , 805px 346px #A1B8D0 , 14px 445px #A1B8D0 , 1px 893px #A1B8D0 , 34px 47px #A1B8D0 , 400px 700px #A1B8D0 , 812px 413px #A1B8D0 , 277px 516px #A1B8D0 , 859px 242px #A1B8D0 , 50px 410px #A1B8D0 , 281px 981px #A1B8D0 , 734px 179px #A1B8D0 , 616px 881px #A1B8D0 , 371px 111px #A1B8D0 , 53px 621px #A1B8D0 , 152px 182px #A1B8D0 , 288px 217px #A1B8D0 , 557px 512px #A1B8D0 , 987px 813px #A1B8D0 , 827px 390px #A1B8D0 , 435px 72px #A1B8D0 , 717px 37px #A1B8D0 , 632px 417px #A1B8D0 , 664px 426px #A1B8D0 , 89px 885px #A1B8D0 , 515px 741px #A1B8D0 , 873px 206px #A1B8D0 , 199px 395px #A1B8D0 , 666px 598px #A1B8D0 , 470px 6px #A1B8D0 , 70px 724px #A1B8D0 , 749px 669px #A1B8D0 , 143px 887px #A1B8D0 , 712px 898px #A1B8D0 , 608px 623px #A1B8D0 , 692px 878px #A1B8D0 , 214px 730px #A1B8D0 , 521px 582px #A1B8D0 , 311px 822px #A1B8D0 , 368px 494px #A1B8D0 , 69px 913px #A1B8D0 , 680px 604px #A1B8D0 , 909px 450px #A1B8D0 , 719px 304px #A1B8D0 , 36px 676px #A1B8D0 , 216px 921px #A1B8D0 , 462px 32px #A1B8D0 , 872px 232px #A1B8D0 , 909px 543px #A1B8D0 , 923px 741px #A1B8D0 , 785px 405px #A1B8D0 , 917px 9px #A1B8D0 , 32px 311px #A1B8D0 , 541px 242px #A1B8D0 , 490px 749px #A1B8D0 , 896px 718px #A1B8D0 , 375px 117px #A1B8D0 , 92px 30px #A1B8D0 , 930px 662px #A1B8D0 , 672px 683px #A1B8D0 , 251px 740px #A1B8D0 , 84px 929px #A1B8D0 , 337px 376px #A1B8D0 , 194px 153px #A1B8D0 , 210px 812px #A1B8D0 , 658px 723px #A1B8D0 , 30px 874px #A1B8D0 , 366px 978px #A1B8D0 , 954px 879px #A1B8D0 , 19px 768px #A1B8D0 , 415px 818px #A1B8D0 , 754px 62px #A1B8D0 , 828px 966px #A1B8D0 , 109px 199px #A1B8D0 , 838px 850px #A1B8D0 , 445px 980px #A1B8D0 , 947px 965px #A1B8D0 , 821px 998px #A1B8D0 , 528px 957px #A1B8D0 , 894px 460px #A1B8D0 , 366px 622px #A1B8D0 , 409px 253px #A1B8D0 , 969px 49px #A1B8D0 , 373px 546px #A1B8D0 , 824px 425px #A1B8D0 , 330px 803px #A1B8D0 , 452px 367px #A1B8D0 , 561px 399px #A1B8D0 , 174px 326px #A1B8D0 , 478px 109px #A1B8D0 , 602px 857px #A1B8D0 , 794px 820px #A1B8D0 , 537px 758px #A1B8D0 , 932px 272px #A1B8D0 , 541px 789px #A1B8D0 , 703px 847px #A1B8D0 , 41px 416px #A1B8D0 , 528px 749px #A1B8D0 , 492px 794px #A1B8D0 , 740px 382px #A1B8D0 , 357px 224px #A1B8D0 , 285px 993px #A1B8D0 , 420px 414px #A1B8D0 , 650px 866px #A1B8D0 , 568px 674px #A1B8D0 , 415px 883px #A1B8D0;
  }
  .glitter_27:before {
    -moz-animation: glitter-27 8s infinite;
    -webkit-animation: glitter-27 8s infinite;
    animation: glitter-27 8s infinite;
    box-shadow: 202px 38px #A1B8D0 , 707px 196px #A1B8D0 , 469px 425px #A1B8D0 , 215px 268px #A1B8D0 , 728px 531px #A1B8D0 , 534px 103px #A1B8D0 , 874px 874px #A1B8D0 , 589px 743px #A1B8D0 , 882px 329px #A1B8D0 , 672px 477px #A1B8D0 , 68px 75px #A1B8D0 , 396px 758px #A1B8D0 , 82px 741px #A1B8D0 , 453px 397px #A1B8D0 , 971px 704px #A1B8D0 , 871px 937px #A1B8D0 , 888px 728px #A1B8D0 , 710px 692px #A1B8D0 , 594px 729px #A1B8D0 , 906px 507px #A1B8D0 , 513px 124px #A1B8D0 , 882px 416px #A1B8D0 , 756px 336px #A1B8D0 , 866px 344px #A1B8D0 , 956px 243px #A1B8D0 , 14px 687px #A1B8D0 , 509px 748px #A1B8D0 , 914px 80px #A1B8D0 , 920px 673px #A1B8D0 , 550px 547px #A1B8D0 , 681px 473px #A1B8D0 , 294px 447px #A1B8D0 , 884px 447px #A1B8D0 , 690px 542px #A1B8D0 , 111px 257px #A1B8D0 , 365px 529px #A1B8D0 , 862px 500px #A1B8D0 , 308px 774px #A1B8D0 , 370px 248px #A1B8D0 , 290px 50px #A1B8D0 , 760px 727px #A1B8D0 , 561px 754px #A1B8D0 , 146px 632px #A1B8D0 , 411px 720px #A1B8D0 , 156px 668px #A1B8D0 , 887px 337px #A1B8D0 , 528px 364px #A1B8D0 , 79px 158px #A1B8D0 , 644px 213px #A1B8D0 , 119px 504px #A1B8D0 , 121px 847px #A1B8D0 , 447px 938px #A1B8D0 , 950px 818px #A1B8D0 , 327px 466px #A1B8D0 , 389px 483px #A1B8D0 , 269px 761px #A1B8D0 , 253px 919px #A1B8D0 , 103px 442px #A1B8D0 , 602px 813px #A1B8D0 , 700px 397px #A1B8D0 , 464px 419px #A1B8D0 , 884px 461px #A1B8D0 , 625px 90px #A1B8D0 , 301px 595px #A1B8D0 , 601px 505px #A1B8D0 , 800px 371px #A1B8D0 , 155px 257px #A1B8D0 , 242px 349px #A1B8D0 , 767px 898px #A1B8D0 , 229px 107px #A1B8D0 , 911px 648px #A1B8D0 , 890px 305px #A1B8D0 , 791px 156px #A1B8D0 , 524px 850px #A1B8D0 , 766px 197px #A1B8D0 , 742px 268px #A1B8D0 , 869px 745px #A1B8D0 , 586px 56px #A1B8D0 , 870px 822px #A1B8D0 , 745px 645px #A1B8D0 , 215px 182px #A1B8D0 , 524px 450px #A1B8D0 , 815px 837px #A1B8D0 , 614px 997px #A1B8D0 , 395px 98px #A1B8D0 , 444px 940px #A1B8D0 , 431px 806px #A1B8D0 , 543px 783px #A1B8D0 , 690px 641px #A1B8D0 , 312px 718px #A1B8D0 , 236px 886px #A1B8D0 , 799px 574px #A1B8D0 , 104px 493px #A1B8D0 , 577px 715px #A1B8D0 , 170px 552px #A1B8D0 , 805px 346px #A1B8D0 , 14px 445px #A1B8D0 , 1px 893px #A1B8D0 , 34px 47px #A1B8D0 , 400px 700px #A1B8D0 , 812px 413px #A1B8D0 , 277px 516px #A1B8D0 , 859px 242px #A1B8D0 , 50px 410px #A1B8D0 , 281px 981px #A1B8D0 , 734px 179px #A1B8D0 , 616px 881px #A1B8D0 , 371px 111px #A1B8D0 , 53px 621px #A1B8D0 , 152px 182px #A1B8D0 , 288px 217px #A1B8D0 , 557px 512px #A1B8D0 , 987px 813px #A1B8D0 , 827px 390px #A1B8D0 , 435px 72px #A1B8D0 , 717px 37px #A1B8D0 , 632px 417px #A1B8D0 , 664px 426px #A1B8D0 , 89px 885px #A1B8D0 , 515px 741px #A1B8D0 , 873px 206px #A1B8D0 , 199px 395px #A1B8D0 , 666px 598px #A1B8D0 , 470px 6px #A1B8D0 , 70px 724px #A1B8D0 , 749px 669px #A1B8D0 , 143px 887px #A1B8D0 , 712px 898px #A1B8D0 , 608px 623px #A1B8D0 , 692px 878px #A1B8D0 , 214px 730px #A1B8D0 , 521px 582px #A1B8D0 , 311px 822px #A1B8D0 , 368px 494px #A1B8D0 , 69px 913px #A1B8D0 , 680px 604px #A1B8D0 , 909px 450px #A1B8D0 , 719px 304px #A1B8D0 , 36px 676px #A1B8D0 , 216px 921px #A1B8D0 , 462px 32px #A1B8D0 , 872px 232px #A1B8D0 , 909px 543px #A1B8D0 , 923px 741px #A1B8D0 , 785px 405px #A1B8D0 , 917px 9px #A1B8D0 , 32px 311px #A1B8D0 , 541px 242px #A1B8D0 , 490px 749px #A1B8D0 , 896px 718px #A1B8D0 , 375px 117px #A1B8D0 , 92px 30px #A1B8D0 , 930px 662px #A1B8D0 , 672px 683px #A1B8D0 , 251px 740px #A1B8D0 , 84px 929px #A1B8D0 , 337px 376px #A1B8D0 , 194px 153px #A1B8D0 , 210px 812px #A1B8D0 , 658px 723px #A1B8D0 , 30px 874px #A1B8D0 , 366px 978px #A1B8D0 , 954px 879px #A1B8D0 , 19px 768px #A1B8D0 , 415px 818px #A1B8D0 , 754px 62px #A1B8D0 , 828px 966px #A1B8D0 , 109px 199px #A1B8D0 , 838px 850px #A1B8D0 , 445px 980px #A1B8D0 , 947px 965px #A1B8D0 , 821px 998px #A1B8D0 , 528px 957px #A1B8D0 , 894px 460px #A1B8D0 , 366px 622px #A1B8D0 , 409px 253px #A1B8D0 , 969px 49px #A1B8D0 , 373px 546px #A1B8D0 , 824px 425px #A1B8D0 , 330px 803px #A1B8D0 , 452px 367px #A1B8D0 , 561px 399px #A1B8D0 , 174px 326px #A1B8D0 , 478px 109px #A1B8D0 , 602px 857px #A1B8D0 , 794px 820px #A1B8D0 , 537px 758px #A1B8D0 , 932px 272px #A1B8D0 , 541px 789px #A1B8D0 , 703px 847px #A1B8D0 , 41px 416px #A1B8D0 , 528px 749px #A1B8D0 , 492px 794px #A1B8D0 , 740px 382px #A1B8D0 , 357px 224px #A1B8D0 , 285px 993px #A1B8D0 , 420px 414px #A1B8D0 , 650px 866px #A1B8D0 , 568px 674px #A1B8D0 , 415px 883px #A1B8D0;
  }
  .glitter_27:after {
    -moz-animation: glitter-27 9s infinite;
    -webkit-animation: glitter-27 9s infinite;
    animation: glitter-27 9s infinite;
    box-shadow: 202px 38px #A1B8D0 , 707px 196px #A1B8D0 , 469px 425px #A1B8D0 , 215px 268px #A1B8D0 , 728px 531px #A1B8D0 , 534px 103px #A1B8D0 , 874px 874px #A1B8D0 , 589px 743px #A1B8D0 , 882px 329px #A1B8D0 , 672px 477px #A1B8D0 , 68px 75px #A1B8D0 , 396px 758px #A1B8D0 , 82px 741px #A1B8D0 , 453px 397px #A1B8D0 , 971px 704px #A1B8D0 , 871px 937px #A1B8D0 , 888px 728px #A1B8D0 , 710px 692px #A1B8D0 , 594px 729px #A1B8D0 , 906px 507px #A1B8D0 , 513px 124px #A1B8D0 , 882px 416px #A1B8D0 , 756px 336px #A1B8D0 , 866px 344px #A1B8D0 , 956px 243px #A1B8D0 , 14px 687px #A1B8D0 , 509px 748px #A1B8D0 , 914px 80px #A1B8D0 , 920px 673px #A1B8D0 , 550px 547px #A1B8D0 , 681px 473px #A1B8D0 , 294px 447px #A1B8D0 , 884px 447px #A1B8D0 , 690px 542px #A1B8D0 , 111px 257px #A1B8D0 , 365px 529px #A1B8D0 , 862px 500px #A1B8D0 , 308px 774px #A1B8D0 , 370px 248px #A1B8D0 , 290px 50px #A1B8D0 , 760px 727px #A1B8D0 , 561px 754px #A1B8D0 , 146px 632px #A1B8D0 , 411px 720px #A1B8D0 , 156px 668px #A1B8D0 , 887px 337px #A1B8D0 , 528px 364px #A1B8D0 , 79px 158px #A1B8D0 , 644px 213px #A1B8D0 , 119px 504px #A1B8D0 , 121px 847px #A1B8D0 , 447px 938px #A1B8D0 , 950px 818px #A1B8D0 , 327px 466px #A1B8D0 , 389px 483px #A1B8D0 , 269px 761px #A1B8D0 , 253px 919px #A1B8D0 , 103px 442px #A1B8D0 , 602px 813px #A1B8D0 , 700px 397px #A1B8D0 , 464px 419px #A1B8D0 , 884px 461px #A1B8D0 , 625px 90px #A1B8D0 , 301px 595px #A1B8D0 , 601px 505px #A1B8D0 , 800px 371px #A1B8D0 , 155px 257px #A1B8D0 , 242px 349px #A1B8D0 , 767px 898px #A1B8D0 , 229px 107px #A1B8D0 , 911px 648px #A1B8D0 , 890px 305px #A1B8D0 , 791px 156px #A1B8D0 , 524px 850px #A1B8D0 , 766px 197px #A1B8D0 , 742px 268px #A1B8D0 , 869px 745px #A1B8D0 , 586px 56px #A1B8D0 , 870px 822px #A1B8D0 , 745px 645px #A1B8D0 , 215px 182px #A1B8D0 , 524px 450px #A1B8D0 , 815px 837px #A1B8D0 , 614px 997px #A1B8D0 , 395px 98px #A1B8D0 , 444px 940px #A1B8D0 , 431px 806px #A1B8D0 , 543px 783px #A1B8D0 , 690px 641px #A1B8D0 , 312px 718px #A1B8D0 , 236px 886px #A1B8D0 , 799px 574px #A1B8D0 , 104px 493px #A1B8D0 , 577px 715px #A1B8D0 , 170px 552px #A1B8D0 , 805px 346px #A1B8D0 , 14px 445px #A1B8D0 , 1px 893px #A1B8D0 , 34px 47px #A1B8D0 , 400px 700px #A1B8D0 , 812px 413px #A1B8D0 , 277px 516px #A1B8D0 , 859px 242px #A1B8D0 , 50px 410px #A1B8D0 , 281px 981px #A1B8D0 , 734px 179px #A1B8D0 , 616px 881px #A1B8D0 , 371px 111px #A1B8D0 , 53px 621px #A1B8D0 , 152px 182px #A1B8D0 , 288px 217px #A1B8D0 , 557px 512px #A1B8D0 , 987px 813px #A1B8D0 , 827px 390px #A1B8D0 , 435px 72px #A1B8D0 , 717px 37px #A1B8D0 , 632px 417px #A1B8D0 , 664px 426px #A1B8D0 , 89px 885px #A1B8D0 , 515px 741px #A1B8D0 , 873px 206px #A1B8D0 , 199px 395px #A1B8D0 , 666px 598px #A1B8D0 , 470px 6px #A1B8D0 , 70px 724px #A1B8D0 , 749px 669px #A1B8D0 , 143px 887px #A1B8D0 , 712px 898px #A1B8D0 , 608px 623px #A1B8D0 , 692px 878px #A1B8D0 , 214px 730px #A1B8D0 , 521px 582px #A1B8D0 , 311px 822px #A1B8D0 , 368px 494px #A1B8D0 , 69px 913px #A1B8D0 , 680px 604px #A1B8D0 , 909px 450px #A1B8D0 , 719px 304px #A1B8D0 , 36px 676px #A1B8D0 , 216px 921px #A1B8D0 , 462px 32px #A1B8D0 , 872px 232px #A1B8D0 , 909px 543px #A1B8D0 , 923px 741px #A1B8D0 , 785px 405px #A1B8D0 , 917px 9px #A1B8D0 , 32px 311px #A1B8D0 , 541px 242px #A1B8D0 , 490px 749px #A1B8D0 , 896px 718px #A1B8D0 , 375px 117px #A1B8D0 , 92px 30px #A1B8D0 , 930px 662px #A1B8D0 , 672px 683px #A1B8D0 , 251px 740px #A1B8D0 , 84px 929px #A1B8D0 , 337px 376px #A1B8D0 , 194px 153px #A1B8D0 , 210px 812px #A1B8D0 , 658px 723px #A1B8D0 , 30px 874px #A1B8D0 , 366px 978px #A1B8D0 , 954px 879px #A1B8D0 , 19px 768px #A1B8D0 , 415px 818px #A1B8D0 , 754px 62px #A1B8D0 , 828px 966px #A1B8D0 , 109px 199px #A1B8D0 , 838px 850px #A1B8D0 , 445px 980px #A1B8D0 , 947px 965px #A1B8D0 , 821px 998px #A1B8D0 , 528px 957px #A1B8D0 , 894px 460px #A1B8D0 , 366px 622px #A1B8D0 , 409px 253px #A1B8D0 , 969px 49px #A1B8D0 , 373px 546px #A1B8D0 , 824px 425px #A1B8D0 , 330px 803px #A1B8D0 , 452px 367px #A1B8D0 , 561px 399px #A1B8D0 , 174px 326px #A1B8D0 , 478px 109px #A1B8D0 , 602px 857px #A1B8D0 , 794px 820px #A1B8D0 , 537px 758px #A1B8D0 , 932px 272px #A1B8D0 , 541px 789px #A1B8D0 , 703px 847px #A1B8D0 , 41px 416px #A1B8D0 , 528px 749px #A1B8D0 , 492px 794px #A1B8D0 , 740px 382px #A1B8D0 , 357px 224px #A1B8D0 , 285px 993px #A1B8D0 , 420px 414px #A1B8D0 , 650px 866px #A1B8D0 , 568px 674px #A1B8D0 , 415px 883px #A1B8D0;
  }
  
  @-moz-keyframes glitter-28 {
    0%,
      100%,
      78.3871%,
      88.3871% {
      opacity: 0;
    }
    83.3871% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-28 {
    0%,
      100%,
      78.3871%,
      88.3871% {
      opacity: 0;
    }
    83.3871% {
      opacity: 1;
    }
  }
  @keyframes glitter-28 {
    0%,
      100%,
      78.3871%,
      88.3871% {
      opacity: 0;
    }
    83.3871% {
      opacity: 1;
    }
  }
  .glitter_28 {
    -moz-animation: glitter-28 10s infinite;
    -webkit-animation: glitter-28 10s infinite;
    animation: glitter-28 10s infinite;
    box-shadow: 216px 207px #A1B8D0 , 957px 220px #A1B8D0 , 344px 203px #A1B8D0 , 594px 981px #A1B8D0 , 154px 782px #A1B8D0 , 431px 82px #A1B8D0 , 204px 129px #A1B8D0 , 314px 154px #A1B8D0 , 295px 278px #A1B8D0 , 976px 463px #A1B8D0 , 696px 155px #A1B8D0 , 603px 795px #A1B8D0 , 140px 883px #A1B8D0 , 78px 647px #A1B8D0 , 758px 848px #A1B8D0 , 505px 970px #A1B8D0 , 386px 780px #A1B8D0 , 757px 243px #A1B8D0 , 152px 775px #A1B8D0 , 157px 947px #A1B8D0 , 860px 853px #A1B8D0 , 739px 949px #A1B8D0 , 466px 592px #A1B8D0 , 509px 216px #A1B8D0 , 290px 22px #A1B8D0 , 455px 361px #A1B8D0 , 715px 128px #A1B8D0 , 688px 125px #A1B8D0 , 472px 352px #A1B8D0 , 151px 298px #A1B8D0 , 40px 796px #A1B8D0 , 891px 236px #A1B8D0 , 239px 522px #A1B8D0 , 720px 655px #A1B8D0 , 901px 556px #A1B8D0 , 44px 110px #A1B8D0 , 612px 256px #A1B8D0 , 667px 643px #A1B8D0 , 404px 909px #A1B8D0 , 409px 654px #A1B8D0 , 91px 528px #A1B8D0 , 436px 689px #A1B8D0 , 824px 327px #A1B8D0 , 850px 751px #A1B8D0 , 933px 979px #A1B8D0 , 293px 282px #A1B8D0 , 276px 61px #A1B8D0 , 265px 677px #A1B8D0 , 21px 129px #A1B8D0 , 856px 247px #A1B8D0 , 945px 10px #A1B8D0 , 551px 828px #A1B8D0 , 131px 956px #A1B8D0 , 508px 34px #A1B8D0 , 746px 558px #A1B8D0 , 721px 318px #A1B8D0 , 119px 355px #A1B8D0 , 602px 312px #A1B8D0 , 956px 1px #A1B8D0 , 475px 147px #A1B8D0 , 354px 593px #A1B8D0 , 428px 342px #A1B8D0 , 982px 221px #A1B8D0 , 982px 131px #A1B8D0 , 521px 660px #A1B8D0 , 11px 516px #A1B8D0 , 384px 447px #A1B8D0 , 517px 620px #A1B8D0 , 594px 773px #A1B8D0 , 851px 919px #A1B8D0 , 679px 236px #A1B8D0 , 818px 330px #A1B8D0 , 108px 865px #A1B8D0 , 5px 752px #A1B8D0 , 171px 718px #A1B8D0 , 740px 31px #A1B8D0 , 515px 787px #A1B8D0 , 602px 269px #A1B8D0 , 617px 362px #A1B8D0 , 630px 874px #A1B8D0 , 64px 729px #A1B8D0 , 338px 903px #A1B8D0 , 249px 306px #A1B8D0 , 626px 830px #A1B8D0 , 139px 39px #A1B8D0 , 367px 164px #A1B8D0 , 390px 150px #A1B8D0 , 631px 807px #A1B8D0 , 869px 279px #A1B8D0 , 78px 605px #A1B8D0 , 34px 851px #A1B8D0 , 429px 307px #A1B8D0 , 790px 115px #A1B8D0 , 183px 991px #A1B8D0 , 862px 911px #A1B8D0 , 559px 170px #A1B8D0 , 341px 148px #A1B8D0 , 382px 518px #A1B8D0 , 991px 884px #A1B8D0 , 492px 267px #A1B8D0 , 780px 952px #A1B8D0 , 482px 592px #A1B8D0 , 358px 211px #A1B8D0 , 241px 973px #A1B8D0 , 265px 701px #A1B8D0 , 189px 111px #A1B8D0 , 510px 965px #A1B8D0 , 671px 248px #A1B8D0 , 583px 179px #A1B8D0 , 913px 420px #A1B8D0 , 253px 251px #A1B8D0 , 749px 157px #A1B8D0 , 324px 687px #A1B8D0 , 995px 697px #A1B8D0 , 774px 986px #A1B8D0 , 459px 351px #A1B8D0 , 160px 57px #A1B8D0 , 476px 152px #A1B8D0 , 895px 443px #A1B8D0 , 168px 124px #A1B8D0 , 434px 511px #A1B8D0 , 679px 458px #A1B8D0 , 662px 280px #A1B8D0 , 594px 359px #A1B8D0 , 653px 300px #A1B8D0 , 894px 118px #A1B8D0 , 454px 883px #A1B8D0 , 82px 496px #A1B8D0 , 153px 417px #A1B8D0 , 173px 535px #A1B8D0 , 678px 716px #A1B8D0 , 942px 514px #A1B8D0 , 164px 150px #A1B8D0 , 323px 641px #A1B8D0 , 612px 435px #A1B8D0 , 302px 985px #A1B8D0 , 485px 460px #A1B8D0 , 710px 905px #A1B8D0 , 589px 310px #A1B8D0 , 66px 622px #A1B8D0 , 749px 576px #A1B8D0 , 768px 873px #A1B8D0 , 170px 291px #A1B8D0 , 875px 272px #A1B8D0 , 919px 237px #A1B8D0 , 379px 9px #A1B8D0 , 567px 880px #A1B8D0 , 668px 227px #A1B8D0 , 74px 241px #A1B8D0 , 517px 648px #A1B8D0 , 754px 750px #A1B8D0 , 612px 621px #A1B8D0 , 415px 479px #A1B8D0 , 613px 578px #A1B8D0 , 578px 704px #A1B8D0 , 981px 291px #A1B8D0 , 692px 83px #A1B8D0 , 716px 417px #A1B8D0 , 143px 461px #A1B8D0 , 151px 166px #A1B8D0 , 458px 68px #A1B8D0 , 713px 975px #A1B8D0 , 689px 362px #A1B8D0 , 267px 591px #A1B8D0 , 749px 555px #A1B8D0 , 302px 649px #A1B8D0 , 388px 255px #A1B8D0 , 216px 821px #A1B8D0 , 177px 77px #A1B8D0 , 489px 239px #A1B8D0 , 25px 130px #A1B8D0 , 326px 961px #A1B8D0 , 802px 631px #A1B8D0 , 327px 213px #A1B8D0 , 296px 452px #A1B8D0 , 309px 855px #A1B8D0 , 350px 886px #A1B8D0 , 365px 131px #A1B8D0 , 905px 250px #A1B8D0 , 913px 184px #A1B8D0 , 448px 399px #A1B8D0 , 925px 807px #A1B8D0 , 37px 548px #A1B8D0 , 495px 676px #A1B8D0 , 598px 2px #A1B8D0 , 918px 701px #A1B8D0 , 268px 973px #A1B8D0 , 250px 719px #A1B8D0 , 839px 159px #A1B8D0 , 446px 764px #A1B8D0 , 421px 692px #A1B8D0 , 18px 75px #A1B8D0 , 160px 483px #A1B8D0 , 766px 46px #A1B8D0 , 271px 943px #A1B8D0 , 418px 473px #A1B8D0 , 308px 735px #A1B8D0 , 99px 310px #A1B8D0 , 698px 270px #A1B8D0 , 989px 937px #A1B8D0;
  }
  .glitter_28:before {
    -moz-animation: glitter-28 8s infinite;
    -webkit-animation: glitter-28 8s infinite;
    animation: glitter-28 8s infinite;
    box-shadow: 216px 207px #A1B8D0 , 957px 220px #A1B8D0 , 344px 203px #A1B8D0 , 594px 981px #A1B8D0 , 154px 782px #A1B8D0 , 431px 82px #A1B8D0 , 204px 129px #A1B8D0 , 314px 154px #A1B8D0 , 295px 278px #A1B8D0 , 976px 463px #A1B8D0 , 696px 155px #A1B8D0 , 603px 795px #A1B8D0 , 140px 883px #A1B8D0 , 78px 647px #A1B8D0 , 758px 848px #A1B8D0 , 505px 970px #A1B8D0 , 386px 780px #A1B8D0 , 757px 243px #A1B8D0 , 152px 775px #A1B8D0 , 157px 947px #A1B8D0 , 860px 853px #A1B8D0 , 739px 949px #A1B8D0 , 466px 592px #A1B8D0 , 509px 216px #A1B8D0 , 290px 22px #A1B8D0 , 455px 361px #A1B8D0 , 715px 128px #A1B8D0 , 688px 125px #A1B8D0 , 472px 352px #A1B8D0 , 151px 298px #A1B8D0 , 40px 796px #A1B8D0 , 891px 236px #A1B8D0 , 239px 522px #A1B8D0 , 720px 655px #A1B8D0 , 901px 556px #A1B8D0 , 44px 110px #A1B8D0 , 612px 256px #A1B8D0 , 667px 643px #A1B8D0 , 404px 909px #A1B8D0 , 409px 654px #A1B8D0 , 91px 528px #A1B8D0 , 436px 689px #A1B8D0 , 824px 327px #A1B8D0 , 850px 751px #A1B8D0 , 933px 979px #A1B8D0 , 293px 282px #A1B8D0 , 276px 61px #A1B8D0 , 265px 677px #A1B8D0 , 21px 129px #A1B8D0 , 856px 247px #A1B8D0 , 945px 10px #A1B8D0 , 551px 828px #A1B8D0 , 131px 956px #A1B8D0 , 508px 34px #A1B8D0 , 746px 558px #A1B8D0 , 721px 318px #A1B8D0 , 119px 355px #A1B8D0 , 602px 312px #A1B8D0 , 956px 1px #A1B8D0 , 475px 147px #A1B8D0 , 354px 593px #A1B8D0 , 428px 342px #A1B8D0 , 982px 221px #A1B8D0 , 982px 131px #A1B8D0 , 521px 660px #A1B8D0 , 11px 516px #A1B8D0 , 384px 447px #A1B8D0 , 517px 620px #A1B8D0 , 594px 773px #A1B8D0 , 851px 919px #A1B8D0 , 679px 236px #A1B8D0 , 818px 330px #A1B8D0 , 108px 865px #A1B8D0 , 5px 752px #A1B8D0 , 171px 718px #A1B8D0 , 740px 31px #A1B8D0 , 515px 787px #A1B8D0 , 602px 269px #A1B8D0 , 617px 362px #A1B8D0 , 630px 874px #A1B8D0 , 64px 729px #A1B8D0 , 338px 903px #A1B8D0 , 249px 306px #A1B8D0 , 626px 830px #A1B8D0 , 139px 39px #A1B8D0 , 367px 164px #A1B8D0 , 390px 150px #A1B8D0 , 631px 807px #A1B8D0 , 869px 279px #A1B8D0 , 78px 605px #A1B8D0 , 34px 851px #A1B8D0 , 429px 307px #A1B8D0 , 790px 115px #A1B8D0 , 183px 991px #A1B8D0 , 862px 911px #A1B8D0 , 559px 170px #A1B8D0 , 341px 148px #A1B8D0 , 382px 518px #A1B8D0 , 991px 884px #A1B8D0 , 492px 267px #A1B8D0 , 780px 952px #A1B8D0 , 482px 592px #A1B8D0 , 358px 211px #A1B8D0 , 241px 973px #A1B8D0 , 265px 701px #A1B8D0 , 189px 111px #A1B8D0 , 510px 965px #A1B8D0 , 671px 248px #A1B8D0 , 583px 179px #A1B8D0 , 913px 420px #A1B8D0 , 253px 251px #A1B8D0 , 749px 157px #A1B8D0 , 324px 687px #A1B8D0 , 995px 697px #A1B8D0 , 774px 986px #A1B8D0 , 459px 351px #A1B8D0 , 160px 57px #A1B8D0 , 476px 152px #A1B8D0 , 895px 443px #A1B8D0 , 168px 124px #A1B8D0 , 434px 511px #A1B8D0 , 679px 458px #A1B8D0 , 662px 280px #A1B8D0 , 594px 359px #A1B8D0 , 653px 300px #A1B8D0 , 894px 118px #A1B8D0 , 454px 883px #A1B8D0 , 82px 496px #A1B8D0 , 153px 417px #A1B8D0 , 173px 535px #A1B8D0 , 678px 716px #A1B8D0 , 942px 514px #A1B8D0 , 164px 150px #A1B8D0 , 323px 641px #A1B8D0 , 612px 435px #A1B8D0 , 302px 985px #A1B8D0 , 485px 460px #A1B8D0 , 710px 905px #A1B8D0 , 589px 310px #A1B8D0 , 66px 622px #A1B8D0 , 749px 576px #A1B8D0 , 768px 873px #A1B8D0 , 170px 291px #A1B8D0 , 875px 272px #A1B8D0 , 919px 237px #A1B8D0 , 379px 9px #A1B8D0 , 567px 880px #A1B8D0 , 668px 227px #A1B8D0 , 74px 241px #A1B8D0 , 517px 648px #A1B8D0 , 754px 750px #A1B8D0 , 612px 621px #A1B8D0 , 415px 479px #A1B8D0 , 613px 578px #A1B8D0 , 578px 704px #A1B8D0 , 981px 291px #A1B8D0 , 692px 83px #A1B8D0 , 716px 417px #A1B8D0 , 143px 461px #A1B8D0 , 151px 166px #A1B8D0 , 458px 68px #A1B8D0 , 713px 975px #A1B8D0 , 689px 362px #A1B8D0 , 267px 591px #A1B8D0 , 749px 555px #A1B8D0 , 302px 649px #A1B8D0 , 388px 255px #A1B8D0 , 216px 821px #A1B8D0 , 177px 77px #A1B8D0 , 489px 239px #A1B8D0 , 25px 130px #A1B8D0 , 326px 961px #A1B8D0 , 802px 631px #A1B8D0 , 327px 213px #A1B8D0 , 296px 452px #A1B8D0 , 309px 855px #A1B8D0 , 350px 886px #A1B8D0 , 365px 131px #A1B8D0 , 905px 250px #A1B8D0 , 913px 184px #A1B8D0 , 448px 399px #A1B8D0 , 925px 807px #A1B8D0 , 37px 548px #A1B8D0 , 495px 676px #A1B8D0 , 598px 2px #A1B8D0 , 918px 701px #A1B8D0 , 268px 973px #A1B8D0 , 250px 719px #A1B8D0 , 839px 159px #A1B8D0 , 446px 764px #A1B8D0 , 421px 692px #A1B8D0 , 18px 75px #A1B8D0 , 160px 483px #A1B8D0 , 766px 46px #A1B8D0 , 271px 943px #A1B8D0 , 418px 473px #A1B8D0 , 308px 735px #A1B8D0 , 99px 310px #A1B8D0 , 698px 270px #A1B8D0 , 989px 937px #A1B8D0;
  }
  .glitter_28:after {
    -moz-animation: glitter-28 9s infinite;
    -webkit-animation: glitter-28 9s infinite;
    animation: glitter-28 9s infinite;
    box-shadow: 216px 207px #A1B8D0 , 957px 220px #A1B8D0 , 344px 203px #A1B8D0 , 594px 981px #A1B8D0 , 154px 782px #A1B8D0 , 431px 82px #A1B8D0 , 204px 129px #A1B8D0 , 314px 154px #A1B8D0 , 295px 278px #A1B8D0 , 976px 463px #A1B8D0 , 696px 155px #A1B8D0 , 603px 795px #A1B8D0 , 140px 883px #A1B8D0 , 78px 647px #A1B8D0 , 758px 848px #A1B8D0 , 505px 970px #A1B8D0 , 386px 780px #A1B8D0 , 757px 243px #A1B8D0 , 152px 775px #A1B8D0 , 157px 947px #A1B8D0 , 860px 853px #A1B8D0 , 739px 949px #A1B8D0 , 466px 592px #A1B8D0 , 509px 216px #A1B8D0 , 290px 22px #A1B8D0 , 455px 361px #A1B8D0 , 715px 128px #A1B8D0 , 688px 125px #A1B8D0 , 472px 352px #A1B8D0 , 151px 298px #A1B8D0 , 40px 796px #A1B8D0 , 891px 236px #A1B8D0 , 239px 522px #A1B8D0 , 720px 655px #A1B8D0 , 901px 556px #A1B8D0 , 44px 110px #A1B8D0 , 612px 256px #A1B8D0 , 667px 643px #A1B8D0 , 404px 909px #A1B8D0 , 409px 654px #A1B8D0 , 91px 528px #A1B8D0 , 436px 689px #A1B8D0 , 824px 327px #A1B8D0 , 850px 751px #A1B8D0 , 933px 979px #A1B8D0 , 293px 282px #A1B8D0 , 276px 61px #A1B8D0 , 265px 677px #A1B8D0 , 21px 129px #A1B8D0 , 856px 247px #A1B8D0 , 945px 10px #A1B8D0 , 551px 828px #A1B8D0 , 131px 956px #A1B8D0 , 508px 34px #A1B8D0 , 746px 558px #A1B8D0 , 721px 318px #A1B8D0 , 119px 355px #A1B8D0 , 602px 312px #A1B8D0 , 956px 1px #A1B8D0 , 475px 147px #A1B8D0 , 354px 593px #A1B8D0 , 428px 342px #A1B8D0 , 982px 221px #A1B8D0 , 982px 131px #A1B8D0 , 521px 660px #A1B8D0 , 11px 516px #A1B8D0 , 384px 447px #A1B8D0 , 517px 620px #A1B8D0 , 594px 773px #A1B8D0 , 851px 919px #A1B8D0 , 679px 236px #A1B8D0 , 818px 330px #A1B8D0 , 108px 865px #A1B8D0 , 5px 752px #A1B8D0 , 171px 718px #A1B8D0 , 740px 31px #A1B8D0 , 515px 787px #A1B8D0 , 602px 269px #A1B8D0 , 617px 362px #A1B8D0 , 630px 874px #A1B8D0 , 64px 729px #A1B8D0 , 338px 903px #A1B8D0 , 249px 306px #A1B8D0 , 626px 830px #A1B8D0 , 139px 39px #A1B8D0 , 367px 164px #A1B8D0 , 390px 150px #A1B8D0 , 631px 807px #A1B8D0 , 869px 279px #A1B8D0 , 78px 605px #A1B8D0 , 34px 851px #A1B8D0 , 429px 307px #A1B8D0 , 790px 115px #A1B8D0 , 183px 991px #A1B8D0 , 862px 911px #A1B8D0 , 559px 170px #A1B8D0 , 341px 148px #A1B8D0 , 382px 518px #A1B8D0 , 991px 884px #A1B8D0 , 492px 267px #A1B8D0 , 780px 952px #A1B8D0 , 482px 592px #A1B8D0 , 358px 211px #A1B8D0 , 241px 973px #A1B8D0 , 265px 701px #A1B8D0 , 189px 111px #A1B8D0 , 510px 965px #A1B8D0 , 671px 248px #A1B8D0 , 583px 179px #A1B8D0 , 913px 420px #A1B8D0 , 253px 251px #A1B8D0 , 749px 157px #A1B8D0 , 324px 687px #A1B8D0 , 995px 697px #A1B8D0 , 774px 986px #A1B8D0 , 459px 351px #A1B8D0 , 160px 57px #A1B8D0 , 476px 152px #A1B8D0 , 895px 443px #A1B8D0 , 168px 124px #A1B8D0 , 434px 511px #A1B8D0 , 679px 458px #A1B8D0 , 662px 280px #A1B8D0 , 594px 359px #A1B8D0 , 653px 300px #A1B8D0 , 894px 118px #A1B8D0 , 454px 883px #A1B8D0 , 82px 496px #A1B8D0 , 153px 417px #A1B8D0 , 173px 535px #A1B8D0 , 678px 716px #A1B8D0 , 942px 514px #A1B8D0 , 164px 150px #A1B8D0 , 323px 641px #A1B8D0 , 612px 435px #A1B8D0 , 302px 985px #A1B8D0 , 485px 460px #A1B8D0 , 710px 905px #A1B8D0 , 589px 310px #A1B8D0 , 66px 622px #A1B8D0 , 749px 576px #A1B8D0 , 768px 873px #A1B8D0 , 170px 291px #A1B8D0 , 875px 272px #A1B8D0 , 919px 237px #A1B8D0 , 379px 9px #A1B8D0 , 567px 880px #A1B8D0 , 668px 227px #A1B8D0 , 74px 241px #A1B8D0 , 517px 648px #A1B8D0 , 754px 750px #A1B8D0 , 612px 621px #A1B8D0 , 415px 479px #A1B8D0 , 613px 578px #A1B8D0 , 578px 704px #A1B8D0 , 981px 291px #A1B8D0 , 692px 83px #A1B8D0 , 716px 417px #A1B8D0 , 143px 461px #A1B8D0 , 151px 166px #A1B8D0 , 458px 68px #A1B8D0 , 713px 975px #A1B8D0 , 689px 362px #A1B8D0 , 267px 591px #A1B8D0 , 749px 555px #A1B8D0 , 302px 649px #A1B8D0 , 388px 255px #A1B8D0 , 216px 821px #A1B8D0 , 177px 77px #A1B8D0 , 489px 239px #A1B8D0 , 25px 130px #A1B8D0 , 326px 961px #A1B8D0 , 802px 631px #A1B8D0 , 327px 213px #A1B8D0 , 296px 452px #A1B8D0 , 309px 855px #A1B8D0 , 350px 886px #A1B8D0 , 365px 131px #A1B8D0 , 905px 250px #A1B8D0 , 913px 184px #A1B8D0 , 448px 399px #A1B8D0 , 925px 807px #A1B8D0 , 37px 548px #A1B8D0 , 495px 676px #A1B8D0 , 598px 2px #A1B8D0 , 918px 701px #A1B8D0 , 268px 973px #A1B8D0 , 250px 719px #A1B8D0 , 839px 159px #A1B8D0 , 446px 764px #A1B8D0 , 421px 692px #A1B8D0 , 18px 75px #A1B8D0 , 160px 483px #A1B8D0 , 766px 46px #A1B8D0 , 271px 943px #A1B8D0 , 418px 473px #A1B8D0 , 308px 735px #A1B8D0 , 99px 310px #A1B8D0 , 698px 270px #A1B8D0 , 989px 937px #A1B8D0;
  }
  
  @-moz-keyframes glitter-29 {
    0%,
      100%,
      81.29032%,
      91.29032% {
      opacity: 0;
    }
    86.29032% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-29 {
    0%,
      100%,
      81.29032%,
      91.29032% {
      opacity: 0;
    }
    86.29032% {
      opacity: 1;
    }
  }
  @keyframes glitter-29 {
    0%,
      100%,
      81.29032%,
      91.29032% {
      opacity: 0;
    }
    86.29032% {
      opacity: 1;
    }
  }
  .glitter_29 {
    -moz-animation: glitter-29 10s infinite;
    -webkit-animation: glitter-29 10s infinite;
    animation: glitter-29 10s infinite;
    box-shadow: 355px 912px #A1B8D0 , 298px 140px #A1B8D0 , 624px 140px #A1B8D0 , 324px 509px #A1B8D0 , 309px 527px #A1B8D0 , 820px 475px #A1B8D0 , 690px 457px #A1B8D0 , 722px 164px #A1B8D0 , 259px 505px #A1B8D0 , 938px 805px #A1B8D0 , 861px 289px #A1B8D0 , 686px 234px #A1B8D0 , 778px 908px #A1B8D0 , 27px 50px #A1B8D0 , 565px 444px #A1B8D0 , 644px 402px #A1B8D0 , 922px 540px #A1B8D0 , 611px 395px #A1B8D0 , 416px 873px #A1B8D0 , 847px 697px #A1B8D0 , 473px 957px #A1B8D0 , 138px 315px #A1B8D0 , 241px 170px #A1B8D0 , 582px 685px #A1B8D0 , 366px 528px #A1B8D0 , 44px 319px #A1B8D0 , 920px 3px #A1B8D0 , 682px 292px #A1B8D0 , 18px 102px #A1B8D0 , 281px 983px #A1B8D0 , 542px 726px #A1B8D0 , 996px 294px #A1B8D0 , 427px 445px #A1B8D0 , 208px 63px #A1B8D0 , 961px 121px #A1B8D0 , 535px 659px #A1B8D0 , 787px 691px #A1B8D0 , 853px 935px #A1B8D0 , 514px 489px #A1B8D0 , 685px 416px #A1B8D0 , 168px 124px #A1B8D0 , 886px 373px #A1B8D0 , 575px 589px #A1B8D0 , 436px 923px #A1B8D0 , 170px 950px #A1B8D0 , 254px 891px #A1B8D0 , 465px 290px #A1B8D0 , 575px 755px #A1B8D0 , 257px 748px #A1B8D0 , 789px 832px #A1B8D0 , 581px 330px #A1B8D0 , 849px 775px #A1B8D0 , 262px 912px #A1B8D0 , 997px 222px #A1B8D0 , 72px 616px #A1B8D0 , 796px 99px #A1B8D0 , 116px 410px #A1B8D0 , 210px 614px #A1B8D0 , 405px 658px #A1B8D0 , 855px 820px #A1B8D0 , 528px 363px #A1B8D0 , 35px 171px #A1B8D0 , 587px 698px #A1B8D0 , 542px 205px #A1B8D0 , 228px 772px #A1B8D0 , 818px 776px #A1B8D0 , 388px 263px #A1B8D0 , 618px 431px #A1B8D0 , 408px 463px #A1B8D0 , 756px 502px #A1B8D0 , 920px 541px #A1B8D0 , 685px 689px #A1B8D0 , 483px 267px #A1B8D0 , 941px 756px #A1B8D0 , 397px 460px #A1B8D0 , 128px 940px #A1B8D0 , 192px 567px #A1B8D0 , 389px 364px #A1B8D0 , 178px 291px #A1B8D0 , 344px 363px #A1B8D0 , 335px 445px #A1B8D0 , 459px 536px #A1B8D0 , 663px 778px #A1B8D0 , 844px 198px #A1B8D0 , 837px 67px #A1B8D0 , 426px 392px #A1B8D0 , 582px 999px #A1B8D0 , 314px 886px #A1B8D0 , 639px 349px #A1B8D0 , 435px 649px #A1B8D0 , 443px 728px #A1B8D0 , 132px 441px #A1B8D0 , 491px 661px #A1B8D0 , 622px 547px #A1B8D0 , 395px 44px #A1B8D0 , 852px 863px #A1B8D0 , 920px 658px #A1B8D0 , 688px 739px #A1B8D0 , 870px 95px #A1B8D0 , 844px 129px #A1B8D0 , 565px 490px #A1B8D0 , 521px 176px #A1B8D0 , 811px 15px #A1B8D0 , 102px 954px #A1B8D0 , 678px 471px #A1B8D0 , 664px 161px #A1B8D0 , 254px 297px #A1B8D0 , 139px 813px #A1B8D0 , 688px 143px #A1B8D0 , 134px 828px #A1B8D0 , 304px 706px #A1B8D0 , 730px 811px #A1B8D0 , 882px 269px #A1B8D0 , 170px 160px #A1B8D0 , 65px 929px #A1B8D0 , 576px 248px #A1B8D0 , 497px 243px #A1B8D0 , 257px 908px #A1B8D0 , 702px 961px #A1B8D0 , 805px 687px #A1B8D0 , 59px 612px #A1B8D0 , 174px 131px #A1B8D0 , 493px 777px #A1B8D0 , 229px 921px #A1B8D0 , 105px 365px #A1B8D0 , 167px 410px #A1B8D0 , 980px 941px #A1B8D0 , 82px 15px #A1B8D0 , 638px 975px #A1B8D0 , 832px 941px #A1B8D0 , 905px 241px #A1B8D0 , 635px 43px #A1B8D0 , 68px 305px #A1B8D0 , 100px 509px #A1B8D0 , 91px 896px #A1B8D0 , 35px 682px #A1B8D0 , 615px 168px #A1B8D0 , 502px 504px #A1B8D0 , 21px 352px #A1B8D0 , 28px 911px #A1B8D0 , 896px 903px #A1B8D0 , 81px 807px #A1B8D0 , 892px 45px #A1B8D0 , 84px 217px #A1B8D0 , 797px 680px #A1B8D0 , 165px 337px #A1B8D0 , 916px 329px #A1B8D0 , 960px 953px #A1B8D0 , 780px 294px #A1B8D0 , 796px 940px #A1B8D0 , 894px 265px #A1B8D0 , 620px 192px #A1B8D0 , 624px 146px #A1B8D0 , 93px 485px #A1B8D0 , 563px 492px #A1B8D0 , 989px 948px #A1B8D0 , 824px 365px #A1B8D0 , 556px 737px #A1B8D0 , 582px 322px #A1B8D0 , 302px 814px #A1B8D0 , 677px 13px #A1B8D0 , 101px 738px #A1B8D0 , 243px 68px #A1B8D0 , 60px 580px #A1B8D0 , 328px 347px #A1B8D0 , 437px 208px #A1B8D0 , 524px 136px #A1B8D0 , 91px 200px #A1B8D0 , 340px 621px #A1B8D0 , 227px 427px #A1B8D0 , 737px 480px #A1B8D0 , 564px 251px #A1B8D0 , 44px 966px #A1B8D0 , 168px 806px #A1B8D0 , 519px 962px #A1B8D0 , 213px 359px #A1B8D0 , 467px 861px #A1B8D0 , 377px 282px #A1B8D0 , 598px 921px #A1B8D0 , 878px 186px #A1B8D0 , 755px 318px #A1B8D0 , 356px 547px #A1B8D0 , 904px 330px #A1B8D0 , 481px 85px #A1B8D0 , 803px 662px #A1B8D0 , 276px 208px #A1B8D0 , 86px 95px #A1B8D0 , 994px 628px #A1B8D0 , 706px 610px #A1B8D0 , 639px 15px #A1B8D0 , 885px 134px #A1B8D0 , 109px 700px #A1B8D0 , 342px 357px #A1B8D0 , 627px 618px #A1B8D0 , 736px 616px #A1B8D0 , 273px 316px #A1B8D0 , 154px 877px #A1B8D0 , 88px 748px #A1B8D0 , 682px 100px #A1B8D0 , 16px 359px #A1B8D0;
  }
  .glitter_29:before {
    -moz-animation: glitter-29 8s infinite;
    -webkit-animation: glitter-29 8s infinite;
    animation: glitter-29 8s infinite;
    box-shadow: 355px 912px #A1B8D0 , 298px 140px #A1B8D0 , 624px 140px #A1B8D0 , 324px 509px #A1B8D0 , 309px 527px #A1B8D0 , 820px 475px #A1B8D0 , 690px 457px #A1B8D0 , 722px 164px #A1B8D0 , 259px 505px #A1B8D0 , 938px 805px #A1B8D0 , 861px 289px #A1B8D0 , 686px 234px #A1B8D0 , 778px 908px #A1B8D0 , 27px 50px #A1B8D0 , 565px 444px #A1B8D0 , 644px 402px #A1B8D0 , 922px 540px #A1B8D0 , 611px 395px #A1B8D0 , 416px 873px #A1B8D0 , 847px 697px #A1B8D0 , 473px 957px #A1B8D0 , 138px 315px #A1B8D0 , 241px 170px #A1B8D0 , 582px 685px #A1B8D0 , 366px 528px #A1B8D0 , 44px 319px #A1B8D0 , 920px 3px #A1B8D0 , 682px 292px #A1B8D0 , 18px 102px #A1B8D0 , 281px 983px #A1B8D0 , 542px 726px #A1B8D0 , 996px 294px #A1B8D0 , 427px 445px #A1B8D0 , 208px 63px #A1B8D0 , 961px 121px #A1B8D0 , 535px 659px #A1B8D0 , 787px 691px #A1B8D0 , 853px 935px #A1B8D0 , 514px 489px #A1B8D0 , 685px 416px #A1B8D0 , 168px 124px #A1B8D0 , 886px 373px #A1B8D0 , 575px 589px #A1B8D0 , 436px 923px #A1B8D0 , 170px 950px #A1B8D0 , 254px 891px #A1B8D0 , 465px 290px #A1B8D0 , 575px 755px #A1B8D0 , 257px 748px #A1B8D0 , 789px 832px #A1B8D0 , 581px 330px #A1B8D0 , 849px 775px #A1B8D0 , 262px 912px #A1B8D0 , 997px 222px #A1B8D0 , 72px 616px #A1B8D0 , 796px 99px #A1B8D0 , 116px 410px #A1B8D0 , 210px 614px #A1B8D0 , 405px 658px #A1B8D0 , 855px 820px #A1B8D0 , 528px 363px #A1B8D0 , 35px 171px #A1B8D0 , 587px 698px #A1B8D0 , 542px 205px #A1B8D0 , 228px 772px #A1B8D0 , 818px 776px #A1B8D0 , 388px 263px #A1B8D0 , 618px 431px #A1B8D0 , 408px 463px #A1B8D0 , 756px 502px #A1B8D0 , 920px 541px #A1B8D0 , 685px 689px #A1B8D0 , 483px 267px #A1B8D0 , 941px 756px #A1B8D0 , 397px 460px #A1B8D0 , 128px 940px #A1B8D0 , 192px 567px #A1B8D0 , 389px 364px #A1B8D0 , 178px 291px #A1B8D0 , 344px 363px #A1B8D0 , 335px 445px #A1B8D0 , 459px 536px #A1B8D0 , 663px 778px #A1B8D0 , 844px 198px #A1B8D0 , 837px 67px #A1B8D0 , 426px 392px #A1B8D0 , 582px 999px #A1B8D0 , 314px 886px #A1B8D0 , 639px 349px #A1B8D0 , 435px 649px #A1B8D0 , 443px 728px #A1B8D0 , 132px 441px #A1B8D0 , 491px 661px #A1B8D0 , 622px 547px #A1B8D0 , 395px 44px #A1B8D0 , 852px 863px #A1B8D0 , 920px 658px #A1B8D0 , 688px 739px #A1B8D0 , 870px 95px #A1B8D0 , 844px 129px #A1B8D0 , 565px 490px #A1B8D0 , 521px 176px #A1B8D0 , 811px 15px #A1B8D0 , 102px 954px #A1B8D0 , 678px 471px #A1B8D0 , 664px 161px #A1B8D0 , 254px 297px #A1B8D0 , 139px 813px #A1B8D0 , 688px 143px #A1B8D0 , 134px 828px #A1B8D0 , 304px 706px #A1B8D0 , 730px 811px #A1B8D0 , 882px 269px #A1B8D0 , 170px 160px #A1B8D0 , 65px 929px #A1B8D0 , 576px 248px #A1B8D0 , 497px 243px #A1B8D0 , 257px 908px #A1B8D0 , 702px 961px #A1B8D0 , 805px 687px #A1B8D0 , 59px 612px #A1B8D0 , 174px 131px #A1B8D0 , 493px 777px #A1B8D0 , 229px 921px #A1B8D0 , 105px 365px #A1B8D0 , 167px 410px #A1B8D0 , 980px 941px #A1B8D0 , 82px 15px #A1B8D0 , 638px 975px #A1B8D0 , 832px 941px #A1B8D0 , 905px 241px #A1B8D0 , 635px 43px #A1B8D0 , 68px 305px #A1B8D0 , 100px 509px #A1B8D0 , 91px 896px #A1B8D0 , 35px 682px #A1B8D0 , 615px 168px #A1B8D0 , 502px 504px #A1B8D0 , 21px 352px #A1B8D0 , 28px 911px #A1B8D0 , 896px 903px #A1B8D0 , 81px 807px #A1B8D0 , 892px 45px #A1B8D0 , 84px 217px #A1B8D0 , 797px 680px #A1B8D0 , 165px 337px #A1B8D0 , 916px 329px #A1B8D0 , 960px 953px #A1B8D0 , 780px 294px #A1B8D0 , 796px 940px #A1B8D0 , 894px 265px #A1B8D0 , 620px 192px #A1B8D0 , 624px 146px #A1B8D0 , 93px 485px #A1B8D0 , 563px 492px #A1B8D0 , 989px 948px #A1B8D0 , 824px 365px #A1B8D0 , 556px 737px #A1B8D0 , 582px 322px #A1B8D0 , 302px 814px #A1B8D0 , 677px 13px #A1B8D0 , 101px 738px #A1B8D0 , 243px 68px #A1B8D0 , 60px 580px #A1B8D0 , 328px 347px #A1B8D0 , 437px 208px #A1B8D0 , 524px 136px #A1B8D0 , 91px 200px #A1B8D0 , 340px 621px #A1B8D0 , 227px 427px #A1B8D0 , 737px 480px #A1B8D0 , 564px 251px #A1B8D0 , 44px 966px #A1B8D0 , 168px 806px #A1B8D0 , 519px 962px #A1B8D0 , 213px 359px #A1B8D0 , 467px 861px #A1B8D0 , 377px 282px #A1B8D0 , 598px 921px #A1B8D0 , 878px 186px #A1B8D0 , 755px 318px #A1B8D0 , 356px 547px #A1B8D0 , 904px 330px #A1B8D0 , 481px 85px #A1B8D0 , 803px 662px #A1B8D0 , 276px 208px #A1B8D0 , 86px 95px #A1B8D0 , 994px 628px #A1B8D0 , 706px 610px #A1B8D0 , 639px 15px #A1B8D0 , 885px 134px #A1B8D0 , 109px 700px #A1B8D0 , 342px 357px #A1B8D0 , 627px 618px #A1B8D0 , 736px 616px #A1B8D0 , 273px 316px #A1B8D0 , 154px 877px #A1B8D0 , 88px 748px #A1B8D0 , 682px 100px #A1B8D0 , 16px 359px #A1B8D0;
  }
  .glitter_29:after {
    -moz-animation: glitter-29 9s infinite;
    -webkit-animation: glitter-29 9s infinite;
    animation: glitter-29 9s infinite;
    box-shadow: 355px 912px #A1B8D0 , 298px 140px #A1B8D0 , 624px 140px #A1B8D0 , 324px 509px #A1B8D0 , 309px 527px #A1B8D0 , 820px 475px #A1B8D0 , 690px 457px #A1B8D0 , 722px 164px #A1B8D0 , 259px 505px #A1B8D0 , 938px 805px #A1B8D0 , 861px 289px #A1B8D0 , 686px 234px #A1B8D0 , 778px 908px #A1B8D0 , 27px 50px #A1B8D0 , 565px 444px #A1B8D0 , 644px 402px #A1B8D0 , 922px 540px #A1B8D0 , 611px 395px #A1B8D0 , 416px 873px #A1B8D0 , 847px 697px #A1B8D0 , 473px 957px #A1B8D0 , 138px 315px #A1B8D0 , 241px 170px #A1B8D0 , 582px 685px #A1B8D0 , 366px 528px #A1B8D0 , 44px 319px #A1B8D0 , 920px 3px #A1B8D0 , 682px 292px #A1B8D0 , 18px 102px #A1B8D0 , 281px 983px #A1B8D0 , 542px 726px #A1B8D0 , 996px 294px #A1B8D0 , 427px 445px #A1B8D0 , 208px 63px #A1B8D0 , 961px 121px #A1B8D0 , 535px 659px #A1B8D0 , 787px 691px #A1B8D0 , 853px 935px #A1B8D0 , 514px 489px #A1B8D0 , 685px 416px #A1B8D0 , 168px 124px #A1B8D0 , 886px 373px #A1B8D0 , 575px 589px #A1B8D0 , 436px 923px #A1B8D0 , 170px 950px #A1B8D0 , 254px 891px #A1B8D0 , 465px 290px #A1B8D0 , 575px 755px #A1B8D0 , 257px 748px #A1B8D0 , 789px 832px #A1B8D0 , 581px 330px #A1B8D0 , 849px 775px #A1B8D0 , 262px 912px #A1B8D0 , 997px 222px #A1B8D0 , 72px 616px #A1B8D0 , 796px 99px #A1B8D0 , 116px 410px #A1B8D0 , 210px 614px #A1B8D0 , 405px 658px #A1B8D0 , 855px 820px #A1B8D0 , 528px 363px #A1B8D0 , 35px 171px #A1B8D0 , 587px 698px #A1B8D0 , 542px 205px #A1B8D0 , 228px 772px #A1B8D0 , 818px 776px #A1B8D0 , 388px 263px #A1B8D0 , 618px 431px #A1B8D0 , 408px 463px #A1B8D0 , 756px 502px #A1B8D0 , 920px 541px #A1B8D0 , 685px 689px #A1B8D0 , 483px 267px #A1B8D0 , 941px 756px #A1B8D0 , 397px 460px #A1B8D0 , 128px 940px #A1B8D0 , 192px 567px #A1B8D0 , 389px 364px #A1B8D0 , 178px 291px #A1B8D0 , 344px 363px #A1B8D0 , 335px 445px #A1B8D0 , 459px 536px #A1B8D0 , 663px 778px #A1B8D0 , 844px 198px #A1B8D0 , 837px 67px #A1B8D0 , 426px 392px #A1B8D0 , 582px 999px #A1B8D0 , 314px 886px #A1B8D0 , 639px 349px #A1B8D0 , 435px 649px #A1B8D0 , 443px 728px #A1B8D0 , 132px 441px #A1B8D0 , 491px 661px #A1B8D0 , 622px 547px #A1B8D0 , 395px 44px #A1B8D0 , 852px 863px #A1B8D0 , 920px 658px #A1B8D0 , 688px 739px #A1B8D0 , 870px 95px #A1B8D0 , 844px 129px #A1B8D0 , 565px 490px #A1B8D0 , 521px 176px #A1B8D0 , 811px 15px #A1B8D0 , 102px 954px #A1B8D0 , 678px 471px #A1B8D0 , 664px 161px #A1B8D0 , 254px 297px #A1B8D0 , 139px 813px #A1B8D0 , 688px 143px #A1B8D0 , 134px 828px #A1B8D0 , 304px 706px #A1B8D0 , 730px 811px #A1B8D0 , 882px 269px #A1B8D0 , 170px 160px #A1B8D0 , 65px 929px #A1B8D0 , 576px 248px #A1B8D0 , 497px 243px #A1B8D0 , 257px 908px #A1B8D0 , 702px 961px #A1B8D0 , 805px 687px #A1B8D0 , 59px 612px #A1B8D0 , 174px 131px #A1B8D0 , 493px 777px #A1B8D0 , 229px 921px #A1B8D0 , 105px 365px #A1B8D0 , 167px 410px #A1B8D0 , 980px 941px #A1B8D0 , 82px 15px #A1B8D0 , 638px 975px #A1B8D0 , 832px 941px #A1B8D0 , 905px 241px #A1B8D0 , 635px 43px #A1B8D0 , 68px 305px #A1B8D0 , 100px 509px #A1B8D0 , 91px 896px #A1B8D0 , 35px 682px #A1B8D0 , 615px 168px #A1B8D0 , 502px 504px #A1B8D0 , 21px 352px #A1B8D0 , 28px 911px #A1B8D0 , 896px 903px #A1B8D0 , 81px 807px #A1B8D0 , 892px 45px #A1B8D0 , 84px 217px #A1B8D0 , 797px 680px #A1B8D0 , 165px 337px #A1B8D0 , 916px 329px #A1B8D0 , 960px 953px #A1B8D0 , 780px 294px #A1B8D0 , 796px 940px #A1B8D0 , 894px 265px #A1B8D0 , 620px 192px #A1B8D0 , 624px 146px #A1B8D0 , 93px 485px #A1B8D0 , 563px 492px #A1B8D0 , 989px 948px #A1B8D0 , 824px 365px #A1B8D0 , 556px 737px #A1B8D0 , 582px 322px #A1B8D0 , 302px 814px #A1B8D0 , 677px 13px #A1B8D0 , 101px 738px #A1B8D0 , 243px 68px #A1B8D0 , 60px 580px #A1B8D0 , 328px 347px #A1B8D0 , 437px 208px #A1B8D0 , 524px 136px #A1B8D0 , 91px 200px #A1B8D0 , 340px 621px #A1B8D0 , 227px 427px #A1B8D0 , 737px 480px #A1B8D0 , 564px 251px #A1B8D0 , 44px 966px #A1B8D0 , 168px 806px #A1B8D0 , 519px 962px #A1B8D0 , 213px 359px #A1B8D0 , 467px 861px #A1B8D0 , 377px 282px #A1B8D0 , 598px 921px #A1B8D0 , 878px 186px #A1B8D0 , 755px 318px #A1B8D0 , 356px 547px #A1B8D0 , 904px 330px #A1B8D0 , 481px 85px #A1B8D0 , 803px 662px #A1B8D0 , 276px 208px #A1B8D0 , 86px 95px #A1B8D0 , 994px 628px #A1B8D0 , 706px 610px #A1B8D0 , 639px 15px #A1B8D0 , 885px 134px #A1B8D0 , 109px 700px #A1B8D0 , 342px 357px #A1B8D0 , 627px 618px #A1B8D0 , 736px 616px #A1B8D0 , 273px 316px #A1B8D0 , 154px 877px #A1B8D0 , 88px 748px #A1B8D0 , 682px 100px #A1B8D0 , 16px 359px #A1B8D0;
  }
  
  @-moz-keyframes glitter-30 {
    0%,
      100%,
      84.19355%,
      94.19355% {
      opacity: 0;
    }
    89.19355% {
      opacity: 1;
    }
  }
  @-webkit-keyframes glitter-30 {
    0%,
      100%,
      84.19355%,
      94.19355% {
      opacity: 0;
    }
    89.19355% {
      opacity: 1;
    }
  }
  @keyframes glitter-30 {
    0%,
      100%,
      84.19355%,
      94.19355% {
      opacity: 0;
    }
    89.19355% {
      opacity: 1;
    }
  }
  .glitter_30 {
    -moz-animation: glitter-30 10s infinite;
    -webkit-animation: glitter-30 10s infinite;
    animation: glitter-30 10s infinite;
    box-shadow: 83px 190px #A1B8D0 , 263px 700px #A1B8D0 , 169px 490px #A1B8D0 , 872px 882px #A1B8D0 , 671px 953px #A1B8D0 , 272px 812px #A1B8D0 , 197px 771px #A1B8D0 , 237px 704px #A1B8D0 , 502px 36px #A1B8D0 , 291px 389px #A1B8D0 , 930px 548px #A1B8D0 , 662px 272px #A1B8D0 , 624px 316px #A1B8D0 , 933px 115px #A1B8D0 , 194px 998px #A1B8D0 , 728px 34px #A1B8D0 , 473px 560px #A1B8D0 , 169px 445px #A1B8D0 , 423px 712px #A1B8D0 , 415px 610px #A1B8D0 , 107px 544px #A1B8D0 , 710px 133px #A1B8D0 , 379px 388px #A1B8D0 , 52px 965px #A1B8D0 , 767px 744px #A1B8D0 , 428px 216px #A1B8D0 , 804px 697px #A1B8D0 , 957px 5px #A1B8D0 , 939px 991px #A1B8D0 , 470px 988px #A1B8D0 , 277px 288px #A1B8D0 , 176px 42px #A1B8D0 , 47px 226px #A1B8D0 , 145px 988px #A1B8D0 , 990px 503px #A1B8D0 , 858px 281px #A1B8D0 , 15px 990px #A1B8D0 , 870px 413px #A1B8D0 , 444px 689px #A1B8D0 , 325px 567px #A1B8D0 , 671px 657px #A1B8D0 , 745px 805px #A1B8D0 , 327px 152px #A1B8D0 , 186px 9px #A1B8D0 , 825px 993px #A1B8D0 , 914px 334px #A1B8D0 , 980px 475px #A1B8D0 , 822px 659px #A1B8D0 , 390px 395px #A1B8D0 , 756px 123px #A1B8D0 , 679px 199px #A1B8D0 , 689px 782px #A1B8D0 , 441px 792px #A1B8D0 , 892px 633px #A1B8D0 , 851px 287px #A1B8D0 , 945px 302px #A1B8D0 , 89px 651px #A1B8D0 , 768px 566px #A1B8D0 , 194px 308px #A1B8D0 , 427px 988px #A1B8D0 , 654px 231px #A1B8D0 , 947px 527px #A1B8D0 , 459px 785px #A1B8D0 , 728px 439px #A1B8D0 , 690px 788px #A1B8D0 , 836px 264px #A1B8D0 , 644px 270px #A1B8D0 , 189px 604px #A1B8D0 , 920px 820px #A1B8D0 , 112px 554px #A1B8D0 , 918px 826px #A1B8D0 , 878px 799px #A1B8D0 , 270px 728px #A1B8D0 , 549px 768px #A1B8D0 , 607px 582px #A1B8D0 , 59px 6px #A1B8D0 , 644px 443px #A1B8D0 , 56px 140px #A1B8D0 , 758px 823px #A1B8D0 , 760px 703px #A1B8D0 , 83px 814px #A1B8D0 , 292px 527px #A1B8D0 , 741px 893px #A1B8D0 , 249px 45px #A1B8D0 , 978px 989px #A1B8D0 , 749px 305px #A1B8D0 , 244px 693px #A1B8D0 , 480px 930px #A1B8D0 , 343px 552px #A1B8D0 , 354px 205px #A1B8D0 , 113px 579px #A1B8D0 , 675px 720px #A1B8D0 , 226px 738px #A1B8D0 , 174px 939px #A1B8D0 , 277px 774px #A1B8D0 , 668px 1000px #A1B8D0 , 224px 247px #A1B8D0 , 388px 947px #A1B8D0 , 8px 497px #A1B8D0 , 895px 500px #A1B8D0 , 917px 67px #A1B8D0 , 404px 959px #A1B8D0 , 673px 898px #A1B8D0 , 527px 38px #A1B8D0 , 216px 960px #A1B8D0 , 640px 432px #A1B8D0 , 924px 94px #A1B8D0 , 558px 274px #A1B8D0 , 225px 542px #A1B8D0 , 380px 351px #A1B8D0 , 872px 977px #A1B8D0 , 593px 872px #A1B8D0 , 768px 889px #A1B8D0 , 898px 134px #A1B8D0 , 490px 310px #A1B8D0 , 780px 345px #A1B8D0 , 427px 287px #A1B8D0 , 499px 383px #A1B8D0 , 745px 66px #A1B8D0 , 786px 825px #A1B8D0 , 282px 603px #A1B8D0 , 506px 706px #A1B8D0 , 16px 670px #A1B8D0 , 711px 246px #A1B8D0 , 881px 278px #A1B8D0 , 166px 466px #A1B8D0 , 680px 342px #A1B8D0 , 348px 400px #A1B8D0 , 35px 667px #A1B8D0 , 746px 761px #A1B8D0 , 830px 485px #A1B8D0 , 164px 294px #A1B8D0 , 726px 753px #A1B8D0 , 774px 735px #A1B8D0 , 638px 458px #A1B8D0 , 655px 812px #A1B8D0 , 781px 340px #A1B8D0 , 431px 208px #A1B8D0 , 935px 937px #A1B8D0 , 662px 79px #A1B8D0 , 812px 398px #A1B8D0 , 459px 967px #A1B8D0 , 556px 405px #A1B8D0 , 894px 234px #A1B8D0 , 461px 908px #A1B8D0 , 881px 287px #A1B8D0 , 436px 589px #A1B8D0 , 320px 383px #A1B8D0 , 884px 264px #A1B8D0 , 268px 883px #A1B8D0 , 669px 309px #A1B8D0 , 172px 306px #A1B8D0 , 105px 61px #A1B8D0 , 95px 387px #A1B8D0 , 372px 579px #A1B8D0 , 698px 640px #A1B8D0 , 787px 546px #A1B8D0 , 180px 295px #A1B8D0 , 638px 809px #A1B8D0 , 622px 274px #A1B8D0 , 634px 2px #A1B8D0 , 187px 152px #A1B8D0 , 419px 454px #A1B8D0 , 432px 692px #A1B8D0 , 478px 666px #A1B8D0 , 630px 864px #A1B8D0 , 809px 301px #A1B8D0 , 631px 330px #A1B8D0 , 621px 573px #A1B8D0 , 964px 597px #A1B8D0 , 118px 751px #A1B8D0 , 442px 879px #A1B8D0 , 314px 742px #A1B8D0 , 280px 190px #A1B8D0 , 394px 481px #A1B8D0 , 447px 752px #A1B8D0 , 552px 944px #A1B8D0 , 590px 740px #A1B8D0 , 678px 423px #A1B8D0 , 81px 167px #A1B8D0 , 681px 984px #A1B8D0 , 324px 204px #A1B8D0 , 761px 393px #A1B8D0 , 455px 225px #A1B8D0 , 351px 404px #A1B8D0 , 157px 593px #A1B8D0 , 367px 53px #A1B8D0 , 52px 85px #A1B8D0 , 971px 26px #A1B8D0 , 892px 658px #A1B8D0 , 925px 857px #A1B8D0 , 196px 671px #A1B8D0 , 262px 61px #A1B8D0 , 486px 808px #A1B8D0 , 869px 81px #A1B8D0 , 278px 235px #A1B8D0 , 163px 826px #A1B8D0 , 390px 858px #A1B8D0 , 576px 155px #A1B8D0 , 386px 299px #A1B8D0;
  }
  .glitter_30:before {
    -moz-animation: glitter-30 8s infinite;
    -webkit-animation: glitter-30 8s infinite;
    animation: glitter-30 8s infinite;
    box-shadow: 83px 190px #A1B8D0 , 263px 700px #A1B8D0 , 169px 490px #A1B8D0 , 872px 882px #A1B8D0 , 671px 953px #A1B8D0 , 272px 812px #A1B8D0 , 197px 771px #A1B8D0 , 237px 704px #A1B8D0 , 502px 36px #A1B8D0 , 291px 389px #A1B8D0 , 930px 548px #A1B8D0 , 662px 272px #A1B8D0 , 624px 316px #A1B8D0 , 933px 115px #A1B8D0 , 194px 998px #A1B8D0 , 728px 34px #A1B8D0 , 473px 560px #A1B8D0 , 169px 445px #A1B8D0 , 423px 712px #A1B8D0 , 415px 610px #A1B8D0 , 107px 544px #A1B8D0 , 710px 133px #A1B8D0 , 379px 388px #A1B8D0 , 52px 965px #A1B8D0 , 767px 744px #A1B8D0 , 428px 216px #A1B8D0 , 804px 697px #A1B8D0 , 957px 5px #A1B8D0 , 939px 991px #A1B8D0 , 470px 988px #A1B8D0 , 277px 288px #A1B8D0 , 176px 42px #A1B8D0 , 47px 226px #A1B8D0 , 145px 988px #A1B8D0 , 990px 503px #A1B8D0 , 858px 281px #A1B8D0 , 15px 990px #A1B8D0 , 870px 413px #A1B8D0 , 444px 689px #A1B8D0 , 325px 567px #A1B8D0 , 671px 657px #A1B8D0 , 745px 805px #A1B8D0 , 327px 152px #A1B8D0 , 186px 9px #A1B8D0 , 825px 993px #A1B8D0 , 914px 334px #A1B8D0 , 980px 475px #A1B8D0 , 822px 659px #A1B8D0 , 390px 395px #A1B8D0 , 756px 123px #A1B8D0 , 679px 199px #A1B8D0 , 689px 782px #A1B8D0 , 441px 792px #A1B8D0 , 892px 633px #A1B8D0 , 851px 287px #A1B8D0 , 945px 302px #A1B8D0 , 89px 651px #A1B8D0 , 768px 566px #A1B8D0 , 194px 308px #A1B8D0 , 427px 988px #A1B8D0 , 654px 231px #A1B8D0 , 947px 527px #A1B8D0 , 459px 785px #A1B8D0 , 728px 439px #A1B8D0 , 690px 788px #A1B8D0 , 836px 264px #A1B8D0 , 644px 270px #A1B8D0 , 189px 604px #A1B8D0 , 920px 820px #A1B8D0 , 112px 554px #A1B8D0 , 918px 826px #A1B8D0 , 878px 799px #A1B8D0 , 270px 728px #A1B8D0 , 549px 768px #A1B8D0 , 607px 582px #A1B8D0 , 59px 6px #A1B8D0 , 644px 443px #A1B8D0 , 56px 140px #A1B8D0 , 758px 823px #A1B8D0 , 760px 703px #A1B8D0 , 83px 814px #A1B8D0 , 292px 527px #A1B8D0 , 741px 893px #A1B8D0 , 249px 45px #A1B8D0 , 978px 989px #A1B8D0 , 749px 305px #A1B8D0 , 244px 693px #A1B8D0 , 480px 930px #A1B8D0 , 343px 552px #A1B8D0 , 354px 205px #A1B8D0 , 113px 579px #A1B8D0 , 675px 720px #A1B8D0 , 226px 738px #A1B8D0 , 174px 939px #A1B8D0 , 277px 774px #A1B8D0 , 668px 1000px #A1B8D0 , 224px 247px #A1B8D0 , 388px 947px #A1B8D0 , 8px 497px #A1B8D0 , 895px 500px #A1B8D0 , 917px 67px #A1B8D0 , 404px 959px #A1B8D0 , 673px 898px #A1B8D0 , 527px 38px #A1B8D0 , 216px 960px #A1B8D0 , 640px 432px #A1B8D0 , 924px 94px #A1B8D0 , 558px 274px #A1B8D0 , 225px 542px #A1B8D0 , 380px 351px #A1B8D0 , 872px 977px #A1B8D0 , 593px 872px #A1B8D0 , 768px 889px #A1B8D0 , 898px 134px #A1B8D0 , 490px 310px #A1B8D0 , 780px 345px #A1B8D0 , 427px 287px #A1B8D0 , 499px 383px #A1B8D0 , 745px 66px #A1B8D0 , 786px 825px #A1B8D0 , 282px 603px #A1B8D0 , 506px 706px #A1B8D0 , 16px 670px #A1B8D0 , 711px 246px #A1B8D0 , 881px 278px #A1B8D0 , 166px 466px #A1B8D0 , 680px 342px #A1B8D0 , 348px 400px #A1B8D0 , 35px 667px #A1B8D0 , 746px 761px #A1B8D0 , 830px 485px #A1B8D0 , 164px 294px #A1B8D0 , 726px 753px #A1B8D0 , 774px 735px #A1B8D0 , 638px 458px #A1B8D0 , 655px 812px #A1B8D0 , 781px 340px #A1B8D0 , 431px 208px #A1B8D0 , 935px 937px #A1B8D0 , 662px 79px #A1B8D0 , 812px 398px #A1B8D0 , 459px 967px #A1B8D0 , 556px 405px #A1B8D0 , 894px 234px #A1B8D0 , 461px 908px #A1B8D0 , 881px 287px #A1B8D0 , 436px 589px #A1B8D0 , 320px 383px #A1B8D0 , 884px 264px #A1B8D0 , 268px 883px #A1B8D0 , 669px 309px #A1B8D0 , 172px 306px #A1B8D0 , 105px 61px #A1B8D0 , 95px 387px #A1B8D0 , 372px 579px #A1B8D0 , 698px 640px #A1B8D0 , 787px 546px #A1B8D0 , 180px 295px #A1B8D0 , 638px 809px #A1B8D0 , 622px 274px #A1B8D0 , 634px 2px #A1B8D0 , 187px 152px #A1B8D0 , 419px 454px #A1B8D0 , 432px 692px #A1B8D0 , 478px 666px #A1B8D0 , 630px 864px #A1B8D0 , 809px 301px #A1B8D0 , 631px 330px #A1B8D0 , 621px 573px #A1B8D0 , 964px 597px #A1B8D0 , 118px 751px #A1B8D0 , 442px 879px #A1B8D0 , 314px 742px #A1B8D0 , 280px 190px #A1B8D0 , 394px 481px #A1B8D0 , 447px 752px #A1B8D0 , 552px 944px #A1B8D0 , 590px 740px #A1B8D0 , 678px 423px #A1B8D0 , 81px 167px #A1B8D0 , 681px 984px #A1B8D0 , 324px 204px #A1B8D0 , 761px 393px #A1B8D0 , 455px 225px #A1B8D0 , 351px 404px #A1B8D0 , 157px 593px #A1B8D0 , 367px 53px #A1B8D0 , 52px 85px #A1B8D0 , 971px 26px #A1B8D0 , 892px 658px #A1B8D0 , 925px 857px #A1B8D0 , 196px 671px #A1B8D0 , 262px 61px #A1B8D0 , 486px 808px #A1B8D0 , 869px 81px #A1B8D0 , 278px 235px #A1B8D0 , 163px 826px #A1B8D0 , 390px 858px #A1B8D0 , 576px 155px #A1B8D0 , 386px 299px #A1B8D0;
  }
  .glitter_30:after {
    -moz-animation: glitter-30 9s infinite;
    -webkit-animation: glitter-30 9s infinite;
    animation: glitter-30 9s infinite;
    box-shadow: 83px 190px #A1B8D0 , 263px 700px #A1B8D0 , 169px 490px #A1B8D0 , 872px 882px #A1B8D0 , 671px 953px #A1B8D0 , 272px 812px #A1B8D0 , 197px 771px #A1B8D0 , 237px 704px #A1B8D0 , 502px 36px #A1B8D0 , 291px 389px #A1B8D0 , 930px 548px #A1B8D0 , 662px 272px #A1B8D0 , 624px 316px #A1B8D0 , 933px 115px #A1B8D0 , 194px 998px #A1B8D0 , 728px 34px #A1B8D0 , 473px 560px #A1B8D0 , 169px 445px #A1B8D0 , 423px 712px #A1B8D0 , 415px 610px #A1B8D0 , 107px 544px #A1B8D0 , 710px 133px #A1B8D0 , 379px 388px #A1B8D0 , 52px 965px #A1B8D0 , 767px 744px #A1B8D0 , 428px 216px #A1B8D0 , 804px 697px #A1B8D0 , 957px 5px #A1B8D0 , 939px 991px #A1B8D0 , 470px 988px #A1B8D0 , 277px 288px #A1B8D0 , 176px 42px #A1B8D0 , 47px 226px #A1B8D0 , 145px 988px #A1B8D0 , 990px 503px #A1B8D0 , 858px 281px #A1B8D0 , 15px 990px #A1B8D0 , 870px 413px #A1B8D0 , 444px 689px #A1B8D0 , 325px 567px #A1B8D0 , 671px 657px #A1B8D0 , 745px 805px #A1B8D0 , 327px 152px #A1B8D0 , 186px 9px #A1B8D0 , 825px 993px #A1B8D0 , 914px 334px #A1B8D0 , 980px 475px #A1B8D0 , 822px 659px #A1B8D0 , 390px 395px #A1B8D0 , 756px 123px #A1B8D0 , 679px 199px #A1B8D0 , 689px 782px #A1B8D0 , 441px 792px #A1B8D0 , 892px 633px #A1B8D0 , 851px 287px #A1B8D0 , 945px 302px #A1B8D0 , 89px 651px #A1B8D0 , 768px 566px #A1B8D0 , 194px 308px #A1B8D0 , 427px 988px #A1B8D0 , 654px 231px #A1B8D0 , 947px 527px #A1B8D0 , 459px 785px #A1B8D0 , 728px 439px #A1B8D0 , 690px 788px #A1B8D0 , 836px 264px #A1B8D0 , 644px 270px #A1B8D0 , 189px 604px #A1B8D0 , 920px 820px #A1B8D0 , 112px 554px #A1B8D0 , 918px 826px #A1B8D0 , 878px 799px #A1B8D0 , 270px 728px #A1B8D0 , 549px 768px #A1B8D0 , 607px 582px #A1B8D0 , 59px 6px #A1B8D0 , 644px 443px #A1B8D0 , 56px 140px #A1B8D0 , 758px 823px #A1B8D0 , 760px 703px #A1B8D0 , 83px 814px #A1B8D0 , 292px 527px #A1B8D0 , 741px 893px #A1B8D0 , 249px 45px #A1B8D0 , 978px 989px #A1B8D0 , 749px 305px #A1B8D0 , 244px 693px #A1B8D0 , 480px 930px #A1B8D0 , 343px 552px #A1B8D0 , 354px 205px #A1B8D0 , 113px 579px #A1B8D0 , 675px 720px #A1B8D0 , 226px 738px #A1B8D0 , 174px 939px #A1B8D0 , 277px 774px #A1B8D0 , 668px 1000px #A1B8D0 , 224px 247px #A1B8D0 , 388px 947px #A1B8D0 , 8px 497px #A1B8D0 , 895px 500px #A1B8D0 , 917px 67px #A1B8D0 , 404px 959px #A1B8D0 , 673px 898px #A1B8D0 , 527px 38px #A1B8D0 , 216px 960px #A1B8D0 , 640px 432px #A1B8D0 , 924px 94px #A1B8D0 , 558px 274px #A1B8D0 , 225px 542px #A1B8D0 , 380px 351px #A1B8D0 , 872px 977px #A1B8D0 , 593px 872px #A1B8D0 , 768px 889px #A1B8D0 , 898px 134px #A1B8D0 , 490px 310px #A1B8D0 , 780px 345px #A1B8D0 , 427px 287px #A1B8D0 , 499px 383px #A1B8D0 , 745px 66px #A1B8D0 , 786px 825px #A1B8D0 , 282px 603px #A1B8D0 , 506px 706px #A1B8D0 , 16px 670px #A1B8D0 , 711px 246px #A1B8D0 , 881px 278px #A1B8D0 , 166px 466px #A1B8D0 , 680px 342px #A1B8D0 , 348px 400px #A1B8D0 , 35px 667px #A1B8D0 , 746px 761px #A1B8D0 , 830px 485px #A1B8D0 , 164px 294px #A1B8D0 , 726px 753px #A1B8D0 , 774px 735px #A1B8D0 , 638px 458px #A1B8D0 , 655px 812px #A1B8D0 , 781px 340px #A1B8D0 , 431px 208px #A1B8D0 , 935px 937px #A1B8D0 , 662px 79px #A1B8D0 , 812px 398px #A1B8D0 , 459px 967px #A1B8D0 , 556px 405px #A1B8D0 , 894px 234px #A1B8D0 , 461px 908px #A1B8D0 , 881px 287px #A1B8D0 , 436px 589px #A1B8D0 , 320px 383px #A1B8D0 , 884px 264px #A1B8D0 , 268px 883px #A1B8D0 , 669px 309px #A1B8D0 , 172px 306px #A1B8D0 , 105px 61px #A1B8D0 , 95px 387px #A1B8D0 , 372px 579px #A1B8D0 , 698px 640px #A1B8D0 , 787px 546px #A1B8D0 , 180px 295px #A1B8D0 , 638px 809px #A1B8D0 , 622px 274px #A1B8D0 , 634px 2px #A1B8D0 , 187px 152px #A1B8D0 , 419px 454px #A1B8D0 , 432px 692px #A1B8D0 , 478px 666px #A1B8D0 , 630px 864px #A1B8D0 , 809px 301px #A1B8D0 , 631px 330px #A1B8D0 , 621px 573px #A1B8D0 , 964px 597px #A1B8D0 , 118px 751px #A1B8D0 , 442px 879px #A1B8D0 , 314px 742px #A1B8D0 , 280px 190px #A1B8D0 , 394px 481px #A1B8D0 , 447px 752px #A1B8D0 , 552px 944px #A1B8D0 , 590px 740px #A1B8D0 , 678px 423px #A1B8D0 , 81px 167px #A1B8D0 , 681px 984px #A1B8D0 , 324px 204px #A1B8D0 , 761px 393px #A1B8D0 , 455px 225px #A1B8D0 , 351px 404px #A1B8D0 , 157px 593px #A1B8D0 , 367px 53px #A1B8D0 , 52px 85px #A1B8D0 , 971px 26px #A1B8D0 , 892px 658px #A1B8D0 , 925px 857px #A1B8D0 , 196px 671px #A1B8D0 , 262px 61px #A1B8D0 , 486px 808px #A1B8D0 , 869px 81px #A1B8D0 , 278px 235px #A1B8D0 , 163px 826px #A1B8D0 , 390px 858px #A1B8D0 , 576px 155px #A1B8D0 , 386px 299px #A1B8D0;
  }
  .snow-container {
    position: absolute;
    height: 100vh;
    width: 100%;
    max-width: 100%;
    top: 0;
    overflow: hidden;
    z-index: 2;
    pointer-events: none;
  }
  
  .snow {
    display: block;
    position: absolute;
    z-index: 2;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    pointer-events: none;
    transform: translate3d(0, -100%, 0);
    -webkit-animation: snow linear infinite;
            animation: snow linear infinite;
  }
  .snow.foreground {
    background-image: url("https://dl6rt3mwcjzxg.cloudfront.net/assets/snow/snow-large-075d267ecbc42e3564c8ed43516dd557.png");
    -webkit-animation-duration: 15s;
            animation-duration: 15s;
  }
  .snow.foreground.layered {
    -webkit-animation-delay: 7.5s;
            animation-delay: 7.5s;
  }
  .snow.middleground {
    background-image: image-url("https://dl6rt3mwcjzxg.cloudfront.net/assets/snow/snow-medium-0b8a5e0732315b68e1f54185be7a1ad9.png");
    -webkit-animation-duration: 20s;
            animation-duration: 20s;
  }
  .snow.middleground.layered {
    -webkit-animation-delay: 10s;
            animation-delay: 10s;
  }
  .snow.background {
    background-image: image-url("https://dl6rt3mwcjzxg.cloudfront.net/assets/snow/snow-small-1ecd03b1fce08c24e064ff8c0a72c519.png");
    -webkit-animation-duration: 30s;
            animation-duration: 30s;
  }
  .snow.background.layered {
    -webkit-animation-delay: 15s;
            animation-delay: 15s;
  }
  
  @-webkit-keyframes snow {
    0% {
      transform: translate3d(0, -100%, 0);
    }
    100% {
      transform: translate3d(15%, 100%, 0);
    }
  }
  
  @keyframes snow {
    0% {
      transform: translate3d(0, -100%, 0);
    }
    100% {
      transform: translate3d(15%, 100%, 0);
    }
  }
  
/* .container {
  background-color: white;
  border-radius: 4px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
  height: 300px;
  margin: 40px auto 50px auto;
  position: relative;
  width: 450px;
} */

.artboard {
  height: 50%;
  overflow: hidden;
  position: relative;
  width: 10%;
  margin: 24%  0 0 30%;
}

.deer {
  width: 50px;
  margin: 0 auto;
  position: relative;
}

.rocking {
  animation: rocking 0.4s ease-in-out infinite alternate-reverse;
  transform-origin: bottom left;
  position: relative;
  z-index: 1;
}

.head {
  position: relative;
  width: 50px;
}

.horns {
  animation: rocking 0.4s cubic-bezier(0.4, 0, 0.2, 1) infinite alternate-reverse;
  height: 55px;
  position: relative;
  top: 21px;
  width: 50px;
}

.horn {
  position: relative;
}
.horn:before {
  background-color: #91655d;
  border-radius: 7px 7px 0 0;
  content: "";
  display: block;
  height: 55px;
  position: absolute;
  width: 7px;
  z-index: 1;
}
.horn .line {
  background-color: #91655d;
  border-radius: 7px 0 0 7px;
  height: 7px;
  width: 20px;
  margin-bottom: 15px;
  position: relative;
  top: 10px;
}
.horn .line-one {
  width: 15px;
}
.horn .line-three {
  top: -22px;
  width: 17px;
}
.horn-left {
  top: -7px;
  transform: rotate(-25deg);
}
.horn-left:before {
  /* box-shadow: inset 2px 0 0 0 #9c7169; */
}
.horn-left .line {
  /* box-shadow: inset 0 2px 0 0 #9c7169; */
  right: 15px;
  transform: rotate(30deg);
}
.horn-left .line-one {
  right: 10px;
}
.horn-left .line-three {
  /* box-shadow: inset 0 -2px 0 0 #9c7169; */
  right: -3px;
  transform: rotate(160deg);
}
.horn-right {
  bottom: 55px;
  left: 40px;
  transform: rotate(25deg);
}
.horn-right:before {
  /* box-shadow: inset -2px 0 0 0 #835f5a; */
}
.horn-right .line {
  /* box-shadow: inset 0 2px 0 0 #835f5a; */
  right: -2px;
  transform: rotate(150deg);
}
.horn-right .line-three {
  right: 13px;
  transform: rotate(20deg);
}

.ears {
  position: absolute;
  top: 70px;
}

.ear {
  background-color: #91655d;
  border-radius: 100% 50% 50% 50%;
  height: 18px;
  position: relative;
  right: 20px;
  top: 10px;
  transform: rotate(30deg);
  transform-origin: 100%;
  width: 30px;
}
.ear:before {
  background-color: #e7beb2;
  border-radius: 100% 50% 50% 50%;
  height: 9px;
  content: "";
  display: block;
  left: 5px;
  position: relative;
  top: 5px;
  width: 15px;
}
.ear-left {
  animation: ear-left 2s cubic-bezier(0.6, -0.28, 0.74, 0.05) infinite alternate-reverse;
  transform: rotate(30deg);
}
.ear-right {
  animation: ear-right 2s cubic-bezier(0.6, -0.28, 0.74, 0.05) 2s infinite alternate-reverse;
  left: 10px;
  right: 0;
  top: -8px;
  transform: rotate(160deg);
}

.eyes {
  position: absolute;
  top: 90px;
  right: -5px;
  width: 32px;
  z-index: 2;
}
.eyes .eye {
  background: linear-gradient(0deg, white 50%, #aa8275 50%);
  border-radius: 15px;
  height: 15px;
  width: 15px;
}
.eyes .eye:before {
  animation: eaves 3s infinite alternate-reverse;
  background-color: #aa8275;
  border-radius: 9px 9px 0 0;
  height: 9px;
  content: "";
  display: block;
  position: relative;
  width: 15px;
  top: -1px;
  z-index: 1;
}
.eyes .eye:after {
  animation: eyes 3s infinite alternate-reverse;
  background-color: #495169;
  border-radius: 5px;
  height: 5px;
  content: "";
  display: block;
  left: 5px;
  position: relative;
  top: -3px;
  transform: translate(3px, 2px);
  width: 5px;
}
.eyes .eye-left {
  float: left;
}
.eyes .eye-right {
  float: right;
}

.nose {
  background-color: #91655d;
  border-radius: 0 7px 15px;
  top: 47px;
  height: 18px;
  left: 40px;
  position: relative;
  width: 20px;
  z-index: 2;
}
.nose:before {
  background-color: #fb5d5d;
  border-radius: 15px;
  content: "";
  display: block;
  height: 14px;
  position: absolute;
  right: -0.5px;
  top: -0.5px;
  width: 16px;
}
.nose:after {
  background-color: white;
  border-radius: 5px;
  content: "";
  display: block;
  height: 2px;
  position: absolute;
  right: 4px;
  top: 2px;
  width: 5px;
}

.body {
  background-color: #91655d;
  border-radius: 50px 50px 0;
  box-shadow: inset 7px 0 0 0 #9c7169;
  height: 140px;
  position: relative;
  width: 50px;
  z-index: 1;
}
.body:before {
  background-color: #e7beb2;
  border-radius: 20px 0 0 20px;
  bottom: 20px;
  box-shadow: inset -7px 0 0 0 #c39e9a;
  content: "";
  display: block;
  height: 65px;
  position: absolute;
  right: 0;
  width: 20px;
}

.hooves {
  position: relative;
  bottom: 40px;
  right: 34px;
}

.hoof-one {
  animation: jump 0.3s ease-in-out infinite alternate-reverse;
  left: 10px;
  position: relative;
  top: 70px;
  transform: rotate(25deg);
  transform-origin: 100% 50%;
}
.hoof-one .line {
  height: 30px;
  border: 20px solid;
  border-radius: 40px;
  border-color: transparent transparent #91655d transparent;
  left: 25px;
  width: 30px;
  position: relative;
  top: 5px;
  transform: rotate(-30deg);
}
.hoof-one .anim-part {
  position: relative;
  bottom: 23px;
  left: 81px;
  transform: rotate(-75deg);
  transform-origin: left;
}
.hoof-one .circle {
  animation: hoof-one 0.3s ease-in-out infinite alternate-reverse;
  background-color: #91655d;
  height: 20px;
  width: 20px;
  border-radius: 30px;
  transform: translateX(3px) rotate(0deg);
}
.hoof-one .circle-last {
  border-radius: 20px 0 0 20px;
  transform: translateX(2px) rotate(0deg);
}
.hoof-one .circle-last:before {
  content: "";
  display: block;
  border-top: 20px solid #674a4a;
  border-left: 7px solid transparent;
  height: 0;
  left: 10px;
  width: 7px;
  position: relative;
  z-index: 1;
}
.hoof-one .circle-last:after {
  background-color: #ffb63c;
  border-radius: 10px;
  bottom: 30px;
  content: "";
  display: block;
  height: 40px;
  left: 19px;
  position: relative;
  width: 9px;
}
.hoof-two {
  animation: jump-two 0.3s ease-in-out infinite alternate-reverse;
  left: 55px;
  position: relative;
  top: 10px;
  z-index: -1;
}
.hoof-two .line-one, .hoof-two .line-two {
  height: 10px;
  border: 20px solid;
  border-radius: 40px;
  border-color: transparent transparent #91655d transparent;
  width: 10px;
  position: absolute;
}
.hoof-two .line-one {
  transform: rotate(-45deg);
}
.hoof-two .line-two {
  left: 30px;
  transform: rotate(135deg);
}

.tail {
  background-color: #9c7169;
  bottom: 0;
  left: 4px;
  position: absolute;
  width: 20px;
  z-index: 0;
}
.tail .circle {
  -webkit-animation: tail 2s cubic-bezier(0, 0.02, 0.9, 2) infinite;
          animation: tail 2s cubic-bezier(0, 0.02, 0.9, 2) infinite;
  background-color: #9c7169;
  border-radius: 11px;
  height: 12px;
  position: relative;
  right: 2px;
  transform: rotate(-5deg);
  width: 12px;
}

.legs {
  position: relative;
}
.legs:before {
  background: linear-gradient(to left, #91655d 50%, #9c7169 50%);
  bottom: 0;
  content: "";
  display: block;
  height: 10px;
  left: 7px;
  position: absolute;
  width: 30px;
  z-index: 0;
}

.leg-left:before, .leg-left:after, .leg-right:before, .leg-right:after {
  content: "";
  display: block;
  position: absolute;
  z-index: 1;
}
.leg-left .anim-part {
  animation: leg-left 0.4s ease-out infinite alternate-reverse;
  position: relative;
  top: 1px;
  transform: rotate(5deg) translateX(3px);
  transform-origin: right;
  z-index: 2;
}
.leg-left .anim-part:before, .leg-left .anim-part:after {
  content: "";
  display: block;
  position: absolute;
  z-index: 1;
}
.leg-left .anim-part:before {
  height: 16px;
  width: 16px;
  border: 20px solid;
  border-radius: 30px;
  border-color: transparent #835f5b transparent transparent;
  transform: rotate(-45deg);
  top: -17px;
  left: 17px;
}
.leg-left .anim-part .line {
  background-color: #835f5b;
  height: 25px;
  position: absolute;
  width: 20px;
  left: 51px;
  top: 7px;
  z-index: 2;
  transform: skew(-9deg);
}
.leg-left .anim-part:after {
  background-color: #835f5b;
  height: 20px;
  left: 33px;
  top: -20px;
  width: 24px;
}
.leg-left:after {
  background-color: #674a4a;
  height: 13px;
  left: 48px;
  top: 32px;
  transform: skew(-8deg);
  width: 20px;
  z-index: 2;
}
.leg-right {
  position: relative;
  right: 10px;
}
.leg-right:before {
  height: 30px;
  width: 38px;
  border: 20px solid;
  border-radius: 40px;
  border-color: #91655d transparent transparent transparent;
  transform: rotate(-15deg);
  z-index: 3;
  top: -29px;
  left: 21px;
}
.leg-right .anim-part {
  position: absolute;
  left: 64px;
  bottom: 9px;
  transform: rotate(43deg);
  z-index: 2;
}
.leg-right .anim-part .circle {
  animation: leg-right 0.4s ease-out infinite alternate-reverse;
  width: 20px;
  height: 20px;
  background-color: #91655d;
  border-radius: 20px;
  transform: translateX(4px) rotate(4deg);
}
.leg-right .anim-part .circle-last {
  border-radius: 20px 0 0 20px;
}
.leg-right .anim-part .circle-last:before {
  content: "";
  display: block;
  border-bottom: 20px solid #674a4a;
  border-right: 2px solid transparent;
  height: 0;
  left: 15px;
  width: 11px;
  position: relative;
  z-index: 1;
}

.presents {
  top: 3px;
  height: 45px;
  margin: 0 auto;
  position: relative;
  width: 110px;
}
.presents:after {
  animation: shadow 0.4s ease-out infinite alternate-reverse;
  background-color: #e7eff7;
  bottom: 0;
  border-radius: 7px;
  content: "";
  display: block;
  height: 7px;
  left: -22px;
  position: absolute;
  width: 170px;
}

.present {
  border-radius: 4px;
  bottom: 3px;
  position: absolute;
  z-index: 1;
}
.present:before, .present:after {
  content: "";
  display: block;
  position: relative;
}
.present:before {
  border-radius: 4px 4px 2px 2px;
  box-shadow: 0 2px 0 0 rgba(0, 0, 0, 0.04);
  right: 1px;
}
.present-one {
  background-color: #fb5d5d;
  height: 45px;
  right: 32px;
  width: 45px;
  z-index: 2;
}
.present-one:before {
  background-color: #fc7676;
  height: 12px;
  width: 47px;
}
.present-two {
  background-color: #82dfe3;
  height: 30px;
  width: 30px;
}
.present-two:before {
  background-color: #97e4e8;
  height: 10px;
  width: 32px;
}
.present-two:after {
  background-color: #69b2cb;
  bottom: 10px;
  height: 100%;
  left: 7px;
  width: 5px;
}
.present-two-right {
  right: 5px;
}
.present-three {
  background-color: #ffb63c;
  height: 25px;
  left: 25px;
  margin: auto;
  width: 25px;
  z-index: 2;
}
.present-three:before {
  background-color: #ffc056;
  height: 8px;
  width: 27px;
}
.present-three:after {
  background-color: #fb5353;
  bottom: 8px;
  height: 100%;
  left: 13px;
  width: 5px;
}

.snowflake {
  background-color: #e4e4e4;
  border-radius: 3px;
  height: 3px;
  position: absolute;
  top: 0;
  width: 3px;
  z-index: 3;
}

.snowflake:nth-child(0) {
  -webkit-animation: snow-0 8s infinite;
          animation: snow-0 8s infinite;
}

@-webkit-keyframes snow-0 {
  from {
    transform: translate(434px, -210px);
  }
  to {
    transform: translate(434px, 473px);
  }
}

@keyframes snow-0 {
  from {
    transform: translate(434px, -210px);
  }
  to {
    transform: translate(434px, 473px);
  }
}
.snowflake:nth-child(1) {
  -webkit-animation: snow-1 8s infinite;
          animation: snow-1 8s infinite;
}

@-webkit-keyframes snow-1 {
  from {
    transform: translate(228px, -114px);
  }
  to {
    transform: translate(228px, 614px);
  }
}

@keyframes snow-1 {
  from {
    transform: translate(228px, -114px);
  }
  to {
    transform: translate(228px, 614px);
  }
}
.snowflake:nth-child(2) {
  -webkit-animation: snow-2 6s infinite;
          animation: snow-2 6s infinite;
}

@-webkit-keyframes snow-2 {
  from {
    transform: translate(125px, -128px);
  }
  to {
    transform: translate(125px, 456px);
  }
}

@keyframes snow-2 {
  from {
    transform: translate(125px, -128px);
  }
  to {
    transform: translate(125px, 456px);
  }
}
.snowflake:nth-child(3) {
  -webkit-animation: snow-3 14s infinite;
          animation: snow-3 14s infinite;
}

@-webkit-keyframes snow-3 {
  from {
    transform: translate(394px, -162px);
  }
  to {
    transform: translate(394px, 586px);
  }
}

@keyframes snow-3 {
  from {
    transform: translate(394px, -162px);
  }
  to {
    transform: translate(394px, 586px);
  }
}
.snowflake:nth-child(4) {
  -webkit-animation: snow-4 14s infinite;
          animation: snow-4 14s infinite;
}

@-webkit-keyframes snow-4 {
  from {
    transform: translate(260px, -236px);
  }
  to {
    transform: translate(260px, 601px);
  }
}

@keyframes snow-4 {
  from {
    transform: translate(260px, -236px);
  }
  to {
    transform: translate(260px, 601px);
  }
}
.snowflake:nth-child(5) {
  -webkit-animation: snow-5 10s infinite;
          animation: snow-5 10s infinite;
}

@-webkit-keyframes snow-5 {
  from {
    transform: translate(398px, -203px);
  }
  to {
    transform: translate(398px, 621px);
  }
}

@keyframes snow-5 {
  from {
    transform: translate(398px, -203px);
  }
  to {
    transform: translate(398px, 621px);
  }
}
.snowflake:nth-child(6) {
  -webkit-animation: snow-6 12s infinite;
          animation: snow-6 12s infinite;
}

@-webkit-keyframes snow-6 {
  from {
    transform: translate(425px, -100px);
  }
  to {
    transform: translate(425px, 505px);
  }
}

@keyframes snow-6 {
  from {
    transform: translate(425px, -100px);
  }
  to {
    transform: translate(425px, 505px);
  }
}
.snowflake:nth-child(7) {
  -webkit-animation: snow-7 8s infinite;
          animation: snow-7 8s infinite;
}

@-webkit-keyframes snow-7 {
  from {
    transform: translate(326px, -44px);
  }
  to {
    transform: translate(326px, 593px);
  }
}

@keyframes snow-7 {
  from {
    transform: translate(326px, -44px);
  }
  to {
    transform: translate(326px, 593px);
  }
}
.snowflake:nth-child(8) {
  -webkit-animation: snow-8 6s infinite;
          animation: snow-8 6s infinite;
}

@-webkit-keyframes snow-8 {
  from {
    transform: translate(35px, -249px);
  }
  to {
    transform: translate(35px, 547px);
  }
}

@keyframes snow-8 {
  from {
    transform: translate(35px, -249px);
  }
  to {
    transform: translate(35px, 547px);
  }
}
.snowflake:nth-child(9) {
  -webkit-animation: snow-9 12s infinite;
          animation: snow-9 12s infinite;
}

@-webkit-keyframes snow-9 {
  from {
    transform: translate(316px, -284px);
  }
  to {
    transform: translate(316px, 534px);
  }
}

@keyframes snow-9 {
  from {
    transform: translate(316px, -284px);
  }
  to {
    transform: translate(316px, 534px);
  }
}
.snowflake:nth-child(10) {
  -webkit-animation: snow-10 15s infinite;
          animation: snow-10 15s infinite;
}

@-webkit-keyframes snow-10 {
  from {
    transform: translate(305px, -205px);
  }
  to {
    transform: translate(305px, 471px);
  }
}

@keyframes snow-10 {
  from {
    transform: translate(305px, -205px);
  }
  to {
    transform: translate(305px, 471px);
  }
}
.snowflake:nth-child(11) {
  -webkit-animation: snow-11 7s infinite;
          animation: snow-11 7s infinite;
}

@-webkit-keyframes snow-11 {
  from {
    transform: translate(17px, -259px);
  }
  to {
    transform: translate(17px, 616px);
  }
}

@keyframes snow-11 {
  from {
    transform: translate(17px, -259px);
  }
  to {
    transform: translate(17px, 616px);
  }
}
.snowflake:nth-child(12) {
  -webkit-animation: snow-12 8s infinite;
          animation: snow-12 8s infinite;
}

@-webkit-keyframes snow-12 {
  from {
    transform: translate(339px, -190px);
  }
  to {
    transform: translate(339px, 536px);
  }
}

@keyframes snow-12 {
  from {
    transform: translate(339px, -190px);
  }
  to {
    transform: translate(339px, 536px);
  }
}
.snowflake:nth-child(13) {
  -webkit-animation: snow-13 12s infinite;
          animation: snow-13 12s infinite;
}

@-webkit-keyframes snow-13 {
  from {
    transform: translate(352px, -57px);
  }
  to {
    transform: translate(352px, 655px);
  }
}

@keyframes snow-13 {
  from {
    transform: translate(352px, -57px);
  }
  to {
    transform: translate(352px, 655px);
  }
}
.snowflake:nth-child(14) {
  -webkit-animation: snow-14 11s infinite;
          animation: snow-14 11s infinite;
}

@-webkit-keyframes snow-14 {
  from {
    transform: translate(437px, -111px);
  }
  to {
    transform: translate(437px, 618px);
  }
}

@keyframes snow-14 {
  from {
    transform: translate(437px, -111px);
  }
  to {
    transform: translate(437px, 618px);
  }
}
.snowflake:nth-child(15) {
  -webkit-animation: snow-15 13s infinite;
          animation: snow-15 13s infinite;
}

@-webkit-keyframes snow-15 {
  from {
    transform: translate(240px, -255px);
  }
  to {
    transform: translate(240px, 620px);
  }
}

@keyframes snow-15 {
  from {
    transform: translate(240px, -255px);
  }
  to {
    transform: translate(240px, 620px);
  }
}
.snowflake:nth-child(16) {
  -webkit-animation: snow-16 7s infinite;
          animation: snow-16 7s infinite;
}

@-webkit-keyframes snow-16 {
  from {
    transform: translate(297px, -151px);
  }
  to {
    transform: translate(297px, 636px);
  }
}

@keyframes snow-16 {
  from {
    transform: translate(297px, -151px);
  }
  to {
    transform: translate(297px, 636px);
  }
}
.snowflake:nth-child(17) {
  -webkit-animation: snow-17 11s infinite;
          animation: snow-17 11s infinite;
}

@-webkit-keyframes snow-17 {
  from {
    transform: translate(69px, 0px);
  }
  to {
    transform: translate(69px, 409px);
  }
}

@keyframes snow-17 {
  from {
    transform: translate(69px, 0px);
  }
  to {
    transform: translate(69px, 409px);
  }
}
.snowflake:nth-child(18) {
  -webkit-animation: snow-18 13s infinite;
          animation: snow-18 13s infinite;
}

@-webkit-keyframes snow-18 {
  from {
    transform: translate(238px, -3px);
  }
  to {
    transform: translate(238px, 443px);
  }
}

@keyframes snow-18 {
  from {
    transform: translate(238px, -3px);
  }
  to {
    transform: translate(238px, 443px);
  }
}
.snowflake:nth-child(19) {
  -webkit-animation: snow-19 10s infinite;
          animation: snow-19 10s infinite;
}

@-webkit-keyframes snow-19 {
  from {
    transform: translate(424px, -151px);
  }
  to {
    transform: translate(424px, 435px);
  }
}

@keyframes snow-19 {
  from {
    transform: translate(424px, -151px);
  }
  to {
    transform: translate(424px, 435px);
  }
}
.snowflake:nth-child(20) {
  -webkit-animation: snow-20 15s infinite;
          animation: snow-20 15s infinite;
}

@-webkit-keyframes snow-20 {
  from {
    transform: translate(181px, -188px);
  }
  to {
    transform: translate(181px, 578px);
  }
}

@keyframes snow-20 {
  from {
    transform: translate(181px, -188px);
  }
  to {
    transform: translate(181px, 578px);
  }
}
.snowflake:nth-child(21) {
  -webkit-animation: snow-21 11s infinite;
          animation: snow-21 11s infinite;
}

@-webkit-keyframes snow-21 {
  from {
    transform: translate(294px, -213px);
  }
  to {
    transform: translate(294px, 692px);
  }
}

@keyframes snow-21 {
  from {
    transform: translate(294px, -213px);
  }
  to {
    transform: translate(294px, 692px);
  }
}
.snowflake:nth-child(22) {
  -webkit-animation: snow-22 10s infinite;
          animation: snow-22 10s infinite;
}

@-webkit-keyframes snow-22 {
  from {
    transform: translate(296px, -280px);
  }
  to {
    transform: translate(296px, 429px);
  }
}

@keyframes snow-22 {
  from {
    transform: translate(296px, -280px);
  }
  to {
    transform: translate(296px, 429px);
  }
}
.snowflake:nth-child(23) {
  -webkit-animation: snow-23 6s infinite;
          animation: snow-23 6s infinite;
}

@-webkit-keyframes snow-23 {
  from {
    transform: translate(246px, -160px);
  }
  to {
    transform: translate(246px, 617px);
  }
}

@keyframes snow-23 {
  from {
    transform: translate(246px, -160px);
  }
  to {
    transform: translate(246px, 617px);
  }
}
.snowflake:nth-child(24) {
  -webkit-animation: snow-24 11s infinite;
          animation: snow-24 11s infinite;
}

@-webkit-keyframes snow-24 {
  from {
    transform: translate(230px, -4px);
  }
  to {
    transform: translate(230px, 612px);
  }
}

@keyframes snow-24 {
  from {
    transform: translate(230px, -4px);
  }
  to {
    transform: translate(230px, 612px);
  }
}
.snowflake:nth-child(25) {
  -webkit-animation: snow-25 9s infinite;
          animation: snow-25 9s infinite;
}

@-webkit-keyframes snow-25 {
  from {
    transform: translate(237px, -212px);
  }
  to {
    transform: translate(237px, 613px);
  }
}

@keyframes snow-25 {
  from {
    transform: translate(237px, -212px);
  }
  to {
    transform: translate(237px, 613px);
  }
}
.snowflake:nth-child(26) {
  -webkit-animation: snow-26 11s infinite;
          animation: snow-26 11s infinite;
}

@-webkit-keyframes snow-26 {
  from {
    transform: translate(269px, -64px);
  }
  to {
    transform: translate(269px, 418px);
  }
}

@keyframes snow-26 {
  from {
    transform: translate(269px, -64px);
  }
  to {
    transform: translate(269px, 418px);
  }
}
.snowflake:nth-child(27) {
  -webkit-animation: snow-27 9s infinite;
          animation: snow-27 9s infinite;
}

@-webkit-keyframes snow-27 {
  from {
    transform: translate(320px, -107px);
  }
  to {
    transform: translate(320px, 603px);
  }
}

@keyframes snow-27 {
  from {
    transform: translate(320px, -107px);
  }
  to {
    transform: translate(320px, 603px);
  }
}
.snowflake:nth-child(28) {
  -webkit-animation: snow-28 14s infinite;
          animation: snow-28 14s infinite;
}

@-webkit-keyframes snow-28 {
  from {
    transform: translate(421px, -151px);
  }
  to {
    transform: translate(421px, 507px);
  }
}

@keyframes snow-28 {
  from {
    transform: translate(421px, -151px);
  }
  to {
    transform: translate(421px, 507px);
  }
}
.snowflake:nth-child(29) {
  -webkit-animation: snow-29 11s infinite;
          animation: snow-29 11s infinite;
}

@-webkit-keyframes snow-29 {
  from {
    transform: translate(377px, -70px);
  }
  to {
    transform: translate(377px, 592px);
  }
}

@keyframes snow-29 {
  from {
    transform: translate(377px, -70px);
  }
  to {
    transform: translate(377px, 592px);
  }
}
.snowflake:nth-child(30) {
  -webkit-animation: snow-30 8s infinite;
          animation: snow-30 8s infinite;
}

@-webkit-keyframes snow-30 {
  from {
    transform: translate(69px, -99px);
  }
  to {
    transform: translate(69px, 416px);
  }
}

@keyframes snow-30 {
  from {
    transform: translate(69px, -99px);
  }
  to {
    transform: translate(69px, 416px);
  }
}
.snowflake:nth-child(31) {
  -webkit-animation: snow-31 9s infinite;
          animation: snow-31 9s infinite;
}

@-webkit-keyframes snow-31 {
  from {
    transform: translate(428px, -111px);
  }
  to {
    transform: translate(428px, 614px);
  }
}

@keyframes snow-31 {
  from {
    transform: translate(428px, -111px);
  }
  to {
    transform: translate(428px, 614px);
  }
}
.snowflake:nth-child(32) {
  -webkit-animation: snow-32 6s infinite;
          animation: snow-32 6s infinite;
}

@-webkit-keyframes snow-32 {
  from {
    transform: translate(173px, -19px);
  }
  to {
    transform: translate(173px, 423px);
  }
}

@keyframes snow-32 {
  from {
    transform: translate(173px, -19px);
  }
  to {
    transform: translate(173px, 423px);
  }
}
.snowflake:nth-child(33) {
  -webkit-animation: snow-33 12s infinite;
          animation: snow-33 12s infinite;
}

@-webkit-keyframes snow-33 {
  from {
    transform: translate(258px, -159px);
  }
  to {
    transform: translate(258px, 401px);
  }
}

@keyframes snow-33 {
  from {
    transform: translate(258px, -159px);
  }
  to {
    transform: translate(258px, 401px);
  }
}
.snowflake:nth-child(34) {
  -webkit-animation: snow-34 9s infinite;
          animation: snow-34 9s infinite;
}

@-webkit-keyframes snow-34 {
  from {
    transform: translate(435px, -155px);
  }
  to {
    transform: translate(435px, 451px);
  }
}

@keyframes snow-34 {
  from {
    transform: translate(435px, -155px);
  }
  to {
    transform: translate(435px, 451px);
  }
}
.snowflake:nth-child(35) {
  -webkit-animation: snow-35 13s infinite;
          animation: snow-35 13s infinite;
}

@-webkit-keyframes snow-35 {
  from {
    transform: translate(351px, -63px);
  }
  to {
    transform: translate(351px, 670px);
  }
}

@keyframes snow-35 {
  from {
    transform: translate(351px, -63px);
  }
  to {
    transform: translate(351px, 670px);
  }
}
.snowflake:nth-child(36) {
  -webkit-animation: snow-36 8s infinite;
          animation: snow-36 8s infinite;
}

@-webkit-keyframes snow-36 {
  from {
    transform: translate(80px, -5px);
  }
  to {
    transform: translate(80px, 440px);
  }
}

@keyframes snow-36 {
  from {
    transform: translate(80px, -5px);
  }
  to {
    transform: translate(80px, 440px);
  }
}
.snowflake:nth-child(37) {
  -webkit-animation: snow-37 8s infinite;
          animation: snow-37 8s infinite;
}

@-webkit-keyframes snow-37 {
  from {
    transform: translate(211px, -64px);
  }
  to {
    transform: translate(211px, 426px);
  }
}

@keyframes snow-37 {
  from {
    transform: translate(211px, -64px);
  }
  to {
    transform: translate(211px, 426px);
  }
}
.snowflake:nth-child(38) {
  -webkit-animation: snow-38 15s infinite;
          animation: snow-38 15s infinite;
}

@-webkit-keyframes snow-38 {
  from {
    transform: translate(313px, -160px);
  }
  to {
    transform: translate(313px, 452px);
  }
}

@keyframes snow-38 {
  from {
    transform: translate(313px, -160px);
  }
  to {
    transform: translate(313px, 452px);
  }
}
.snowflake:nth-child(39) {
  -webkit-animation: snow-39 10s infinite;
          animation: snow-39 10s infinite;
}

@-webkit-keyframes snow-39 {
  from {
    transform: translate(310px, -10px);
  }
  to {
    transform: translate(310px, 522px);
  }
}

@keyframes snow-39 {
  from {
    transform: translate(310px, -10px);
  }
  to {
    transform: translate(310px, 522px);
  }
}
.snowflake:nth-child(40) {
  -webkit-animation: snow-40 9s infinite;
          animation: snow-40 9s infinite;
}

@-webkit-keyframes snow-40 {
  from {
    transform: translate(388px, -142px);
  }
  to {
    transform: translate(388px, 421px);
  }
}

@keyframes snow-40 {
  from {
    transform: translate(388px, -142px);
  }
  to {
    transform: translate(388px, 421px);
  }
}
.snowflake:nth-child(41) {
  -webkit-animation: snow-41 12s infinite;
          animation: snow-41 12s infinite;
}

@-webkit-keyframes snow-41 {
  from {
    transform: translate(132px, 0px);
  }
  to {
    transform: translate(132px, 453px);
  }
}

@keyframes snow-41 {
  from {
    transform: translate(132px, 0px);
  }
  to {
    transform: translate(132px, 453px);
  }
}
.snowflake:nth-child(42) {
  -webkit-animation: snow-42 6s infinite;
          animation: snow-42 6s infinite;
}

@-webkit-keyframes snow-42 {
  from {
    transform: translate(80px, -119px);
  }
  to {
    transform: translate(80px, 638px);
  }
}

@keyframes snow-42 {
  from {
    transform: translate(80px, -119px);
  }
  to {
    transform: translate(80px, 638px);
  }
}
.snowflake:nth-child(43) {
  -webkit-animation: snow-43 15s infinite;
          animation: snow-43 15s infinite;
}

@-webkit-keyframes snow-43 {
  from {
    transform: translate(301px, -248px);
  }
  to {
    transform: translate(301px, 487px);
  }
}

@keyframes snow-43 {
  from {
    transform: translate(301px, -248px);
  }
  to {
    transform: translate(301px, 487px);
  }
}
.snowflake:nth-child(44) {
  -webkit-animation: snow-44 15s infinite;
          animation: snow-44 15s infinite;
}

@-webkit-keyframes snow-44 {
  from {
    transform: translate(220px, -175px);
  }
  to {
    transform: translate(220px, 665px);
  }
}

@keyframes snow-44 {
  from {
    transform: translate(220px, -175px);
  }
  to {
    transform: translate(220px, 665px);
  }
}
.snowflake:nth-child(45) {
  -webkit-animation: snow-45 9s infinite;
          animation: snow-45 9s infinite;
}

@-webkit-keyframes snow-45 {
  from {
    transform: translate(425px, -67px);
  }
  to {
    transform: translate(425px, 684px);
  }
}

@keyframes snow-45 {
  from {
    transform: translate(425px, -67px);
  }
  to {
    transform: translate(425px, 684px);
  }
}
.snowflake:nth-child(46) {
  -webkit-animation: snow-46 7s infinite;
          animation: snow-46 7s infinite;
}

@-webkit-keyframes snow-46 {
  from {
    transform: translate(288px, -234px);
  }
  to {
    transform: translate(288px, 583px);
  }
}

@keyframes snow-46 {
  from {
    transform: translate(288px, -234px);
  }
  to {
    transform: translate(288px, 583px);
  }
}
.snowflake:nth-child(47) {
  -webkit-animation: snow-47 12s infinite;
          animation: snow-47 12s infinite;
}

@-webkit-keyframes snow-47 {
  from {
    transform: translate(184px, -153px);
  }
  to {
    transform: translate(184px, 597px);
  }
}

@keyframes snow-47 {
  from {
    transform: translate(184px, -153px);
  }
  to {
    transform: translate(184px, 597px);
  }
}
.snowflake:nth-child(48) {
  -webkit-animation: snow-48 14s infinite;
          animation: snow-48 14s infinite;
}

@-webkit-keyframes snow-48 {
  from {
    transform: translate(88px, -70px);
  }
  to {
    transform: translate(88px, 665px);
  }
}

@keyframes snow-48 {
  from {
    transform: translate(88px, -70px);
  }
  to {
    transform: translate(88px, 665px);
  }
}
.snowflake:nth-child(49) {
  -webkit-animation: snow-49 15s infinite;
          animation: snow-49 15s infinite;
}

@-webkit-keyframes snow-49 {
  from {
    transform: translate(292px, -168px);
  }
  to {
    transform: translate(292px, 676px);
  }
}

@keyframes snow-49 {
  from {
    transform: translate(292px, -168px);
  }
  to {
    transform: translate(292px, 676px);
  }
}
.snowflake:nth-child(50) {
  -webkit-animation: snow-50 11s infinite;
          animation: snow-50 11s infinite;
}

@-webkit-keyframes snow-50 {
  from {
    transform: translate(355px, -206px);
  }
  to {
    transform: translate(355px, 466px);
  }
}

@keyframes snow-50 {
  from {
    transform: translate(355px, -206px);
  }
  to {
    transform: translate(355px, 466px);
  }
}
.snowflake:nth-child(51) {
  -webkit-animation: snow-51 13s infinite;
          animation: snow-51 13s infinite;
}

@-webkit-keyframes snow-51 {
  from {
    transform: translate(292px, -284px);
  }
  to {
    transform: translate(292px, 680px);
  }
}

@keyframes snow-51 {
  from {
    transform: translate(292px, -284px);
  }
  to {
    transform: translate(292px, 680px);
  }
}
.snowflake:nth-child(52) {
  -webkit-animation: snow-52 6s infinite;
          animation: snow-52 6s infinite;
}

@-webkit-keyframes snow-52 {
  from {
    transform: translate(134px, -150px);
  }
  to {
    transform: translate(134px, 486px);
  }
}

@keyframes snow-52 {
  from {
    transform: translate(134px, -150px);
  }
  to {
    transform: translate(134px, 486px);
  }
}
.snowflake:nth-child(53) {
  -webkit-animation: snow-53 13s infinite;
          animation: snow-53 13s infinite;
}

@-webkit-keyframes snow-53 {
  from {
    transform: translate(172px, -163px);
  }
  to {
    transform: translate(172px, 483px);
  }
}

@keyframes snow-53 {
  from {
    transform: translate(172px, -163px);
  }
  to {
    transform: translate(172px, 483px);
  }
}
.snowflake:nth-child(54) {
  -webkit-animation: snow-54 11s infinite;
          animation: snow-54 11s infinite;
}

@-webkit-keyframes snow-54 {
  from {
    transform: translate(31px, -77px);
  }
  to {
    transform: translate(31px, 565px);
  }
}

@keyframes snow-54 {
  from {
    transform: translate(31px, -77px);
  }
  to {
    transform: translate(31px, 565px);
  }
}
.snowflake:nth-child(55) {
  -webkit-animation: snow-55 8s infinite;
          animation: snow-55 8s infinite;
}

@-webkit-keyframes snow-55 {
  from {
    transform: translate(138px, -29px);
  }
  to {
    transform: translate(138px, 431px);
  }
}

@keyframes snow-55 {
  from {
    transform: translate(138px, -29px);
  }
  to {
    transform: translate(138px, 431px);
  }
}
.snowflake:nth-child(56) {
  -webkit-animation: snow-56 12s infinite;
          animation: snow-56 12s infinite;
}

@-webkit-keyframes snow-56 {
  from {
    transform: translate(414px, -224px);
  }
  to {
    transform: translate(414px, 412px);
  }
}

@keyframes snow-56 {
  from {
    transform: translate(414px, -224px);
  }
  to {
    transform: translate(414px, 412px);
  }
}
.snowflake:nth-child(57) {
  -webkit-animation: snow-57 14s infinite;
          animation: snow-57 14s infinite;
}

@-webkit-keyframes snow-57 {
  from {
    transform: translate(427px, -297px);
  }
  to {
    transform: translate(427px, 695px);
  }
}

@keyframes snow-57 {
  from {
    transform: translate(427px, -297px);
  }
  to {
    transform: translate(427px, 695px);
  }
}
.snowflake:nth-child(58) {
  -webkit-animation: snow-58 7s infinite;
          animation: snow-58 7s infinite;
}

@-webkit-keyframes snow-58 {
  from {
    transform: translate(89px, -152px);
  }
  to {
    transform: translate(89px, 547px);
  }
}

@keyframes snow-58 {
  from {
    transform: translate(89px, -152px);
  }
  to {
    transform: translate(89px, 547px);
  }
}
.snowflake:nth-child(59) {
  -webkit-animation: snow-59 6s infinite;
          animation: snow-59 6s infinite;
}

@-webkit-keyframes snow-59 {
  from {
    transform: translate(129px, -66px);
  }
  to {
    transform: translate(129px, 572px);
  }
}

@keyframes snow-59 {
  from {
    transform: translate(129px, -66px);
  }
  to {
    transform: translate(129px, 572px);
  }
}
.snowflake:nth-child(60) {
  -webkit-animation: snow-60 12s infinite;
          animation: snow-60 12s infinite;
}

@-webkit-keyframes snow-60 {
  from {
    transform: translate(215px, -18px);
  }
  to {
    transform: translate(215px, 639px);
  }
}

@keyframes snow-60 {
  from {
    transform: translate(215px, -18px);
  }
  to {
    transform: translate(215px, 639px);
  }
}
.snowflake:nth-child(61) {
  -webkit-animation: snow-61 9s infinite;
          animation: snow-61 9s infinite;
}

@-webkit-keyframes snow-61 {
  from {
    transform: translate(447px, -261px);
  }
  to {
    transform: translate(447px, 481px);
  }
}

@keyframes snow-61 {
  from {
    transform: translate(447px, -261px);
  }
  to {
    transform: translate(447px, 481px);
  }
}
.snowflake:nth-child(62) {
  -webkit-animation: snow-62 8s infinite;
          animation: snow-62 8s infinite;
}

@-webkit-keyframes snow-62 {
  from {
    transform: translate(355px, -247px);
  }
  to {
    transform: translate(355px, 666px);
  }
}

@keyframes snow-62 {
  from {
    transform: translate(355px, -247px);
  }
  to {
    transform: translate(355px, 666px);
  }
}
.snowflake:nth-child(63) {
  -webkit-animation: snow-63 14s infinite;
          animation: snow-63 14s infinite;
}

@-webkit-keyframes snow-63 {
  from {
    transform: translate(270px, -37px);
  }
  to {
    transform: translate(270px, 660px);
  }
}

@keyframes snow-63 {
  from {
    transform: translate(270px, -37px);
  }
  to {
    transform: translate(270px, 660px);
  }
}
.snowflake:nth-child(64) {
  -webkit-animation: snow-64 6s infinite;
          animation: snow-64 6s infinite;
}

@-webkit-keyframes snow-64 {
  from {
    transform: translate(130px, -272px);
  }
  to {
    transform: translate(130px, 514px);
  }
}

@keyframes snow-64 {
  from {
    transform: translate(130px, -272px);
  }
  to {
    transform: translate(130px, 514px);
  }
}
.snowflake:nth-child(65) {
  -webkit-animation: snow-65 9s infinite;
          animation: snow-65 9s infinite;
}

@-webkit-keyframes snow-65 {
  from {
    transform: translate(78px, -133px);
  }
  to {
    transform: translate(78px, 539px);
  }
}

@keyframes snow-65 {
  from {
    transform: translate(78px, -133px);
  }
  to {
    transform: translate(78px, 539px);
  }
}
.snowflake:nth-child(66) {
  -webkit-animation: snow-66 10s infinite;
          animation: snow-66 10s infinite;
}

@-webkit-keyframes snow-66 {
  from {
    transform: translate(302px, -234px);
  }
  to {
    transform: translate(302px, 440px);
  }
}

@keyframes snow-66 {
  from {
    transform: translate(302px, -234px);
  }
  to {
    transform: translate(302px, 440px);
  }
}
.snowflake:nth-child(67) {
  -webkit-animation: snow-67 11s infinite;
          animation: snow-67 11s infinite;
}

@-webkit-keyframes snow-67 {
  from {
    transform: translate(139px, -239px);
  }
  to {
    transform: translate(139px, 572px);
  }
}

@keyframes snow-67 {
  from {
    transform: translate(139px, -239px);
  }
  to {
    transform: translate(139px, 572px);
  }
}
.snowflake:nth-child(68) {
  -webkit-animation: snow-68 15s infinite;
          animation: snow-68 15s infinite;
}

@-webkit-keyframes snow-68 {
  from {
    transform: translate(11px, -174px);
  }
  to {
    transform: translate(11px, 595px);
  }
}

@keyframes snow-68 {
  from {
    transform: translate(11px, -174px);
  }
  to {
    transform: translate(11px, 595px);
  }
}
.snowflake:nth-child(69) {
  -webkit-animation: snow-69 14s infinite;
          animation: snow-69 14s infinite;
}

@-webkit-keyframes snow-69 {
  from {
    transform: translate(245px, -157px);
  }
  to {
    transform: translate(245px, 439px);
  }
}

@keyframes snow-69 {
  from {
    transform: translate(245px, -157px);
  }
  to {
    transform: translate(245px, 439px);
  }
}
.snowflake:nth-child(70) {
  -webkit-animation: snow-70 9s infinite;
          animation: snow-70 9s infinite;
}

@-webkit-keyframes snow-70 {
  from {
    transform: translate(230px, -262px);
  }
  to {
    transform: translate(230px, 442px);
  }
}

@keyframes snow-70 {
  from {
    transform: translate(230px, -262px);
  }
  to {
    transform: translate(230px, 442px);
  }
}
.snowflake:nth-child(71) {
  -webkit-animation: snow-71 11s infinite;
          animation: snow-71 11s infinite;
}

@-webkit-keyframes snow-71 {
  from {
    transform: translate(54px, -263px);
  }
  to {
    transform: translate(54px, 417px);
  }
}

@keyframes snow-71 {
  from {
    transform: translate(54px, -263px);
  }
  to {
    transform: translate(54px, 417px);
  }
}
.snowflake:nth-child(72) {
  -webkit-animation: snow-72 13s infinite;
          animation: snow-72 13s infinite;
}

@-webkit-keyframes snow-72 {
  from {
    transform: translate(143px, -269px);
  }
  to {
    transform: translate(143px, 507px);
  }
}

@keyframes snow-72 {
  from {
    transform: translate(143px, -269px);
  }
  to {
    transform: translate(143px, 507px);
  }
}
.snowflake:nth-child(73) {
  -webkit-animation: snow-73 13s infinite;
          animation: snow-73 13s infinite;
}

@-webkit-keyframes snow-73 {
  from {
    transform: translate(157px, -150px);
  }
  to {
    transform: translate(157px, 671px);
  }
}

@keyframes snow-73 {
  from {
    transform: translate(157px, -150px);
  }
  to {
    transform: translate(157px, 671px);
  }
}
.snowflake:nth-child(74) {
  -webkit-animation: snow-74 8s infinite;
          animation: snow-74 8s infinite;
}

@-webkit-keyframes snow-74 {
  from {
    transform: translate(389px, -79px);
  }
  to {
    transform: translate(389px, 493px);
  }
}

@keyframes snow-74 {
  from {
    transform: translate(389px, -79px);
  }
  to {
    transform: translate(389px, 493px);
  }
}
.snowflake:nth-child(75) {
  -webkit-animation: snow-75 9s infinite;
          animation: snow-75 9s infinite;
}

@-webkit-keyframes snow-75 {
  from {
    transform: translate(34px, -277px);
  }
  to {
    transform: translate(34px, 477px);
  }
}

@keyframes snow-75 {
  from {
    transform: translate(34px, -277px);
  }
  to {
    transform: translate(34px, 477px);
  }
}
.snowflake:nth-child(76) {
  -webkit-animation: snow-76 10s infinite;
          animation: snow-76 10s infinite;
}

@-webkit-keyframes snow-76 {
  from {
    transform: translate(335px, -185px);
  }
  to {
    transform: translate(335px, 489px);
  }
}

@keyframes snow-76 {
  from {
    transform: translate(335px, -185px);
  }
  to {
    transform: translate(335px, 489px);
  }
}
.snowflake:nth-child(77) {
  -webkit-animation: snow-77 14s infinite;
          animation: snow-77 14s infinite;
}

@-webkit-keyframes snow-77 {
  from {
    transform: translate(163px, -57px);
  }
  to {
    transform: translate(163px, 437px);
  }
}

@keyframes snow-77 {
  from {
    transform: translate(163px, -57px);
  }
  to {
    transform: translate(163px, 437px);
  }
}
.snowflake:nth-child(78) {
  -webkit-animation: snow-78 8s infinite;
          animation: snow-78 8s infinite;
}

@-webkit-keyframes snow-78 {
  from {
    transform: translate(450px, -25px);
  }
  to {
    transform: translate(450px, 694px);
  }
}

@keyframes snow-78 {
  from {
    transform: translate(450px, -25px);
  }
  to {
    transform: translate(450px, 694px);
  }
}
.snowflake:nth-child(79) {
  -webkit-animation: snow-79 6s infinite;
          animation: snow-79 6s infinite;
}

@-webkit-keyframes snow-79 {
  from {
    transform: translate(308px, -119px);
  }
  to {
    transform: translate(308px, 541px);
  }
}

@keyframes snow-79 {
  from {
    transform: translate(308px, -119px);
  }
  to {
    transform: translate(308px, 541px);
  }
}
.snowflake:nth-child(80) {
  -webkit-animation: snow-80 8s infinite;
          animation: snow-80 8s infinite;
}

@-webkit-keyframes snow-80 {
  from {
    transform: translate(155px, -127px);
  }
  to {
    transform: translate(155px, 453px);
  }
}

@keyframes snow-80 {
  from {
    transform: translate(155px, -127px);
  }
  to {
    transform: translate(155px, 453px);
  }
}
.snowflake:nth-child(81) {
  -webkit-animation: snow-81 14s infinite;
          animation: snow-81 14s infinite;
}

@-webkit-keyframes snow-81 {
  from {
    transform: translate(448px, -212px);
  }
  to {
    transform: translate(448px, 531px);
  }
}

@keyframes snow-81 {
  from {
    transform: translate(448px, -212px);
  }
  to {
    transform: translate(448px, 531px);
  }
}
.snowflake:nth-child(82) {
  -webkit-animation: snow-82 12s infinite;
          animation: snow-82 12s infinite;
}

@-webkit-keyframes snow-82 {
  from {
    transform: translate(386px, -86px);
  }
  to {
    transform: translate(386px, 611px);
  }
}

@keyframes snow-82 {
  from {
    transform: translate(386px, -86px);
  }
  to {
    transform: translate(386px, 611px);
  }
}
.snowflake:nth-child(83) {
  -webkit-animation: snow-83 8s infinite;
          animation: snow-83 8s infinite;
}

@-webkit-keyframes snow-83 {
  from {
    transform: translate(318px, -58px);
  }
  to {
    transform: translate(318px, 593px);
  }
}

@keyframes snow-83 {
  from {
    transform: translate(318px, -58px);
  }
  to {
    transform: translate(318px, 593px);
  }
}
.snowflake:nth-child(84) {
  -webkit-animation: snow-84 13s infinite;
          animation: snow-84 13s infinite;
}

@-webkit-keyframes snow-84 {
  from {
    transform: translate(179px, -238px);
  }
  to {
    transform: translate(179px, 461px);
  }
}

@keyframes snow-84 {
  from {
    transform: translate(179px, -238px);
  }
  to {
    transform: translate(179px, 461px);
  }
}
.snowflake:nth-child(85) {
  -webkit-animation: snow-85 13s infinite;
          animation: snow-85 13s infinite;
}

@-webkit-keyframes snow-85 {
  from {
    transform: translate(274px, -130px);
  }
  to {
    transform: translate(274px, 580px);
  }
}

@keyframes snow-85 {
  from {
    transform: translate(274px, -130px);
  }
  to {
    transform: translate(274px, 580px);
  }
}
.snowflake:nth-child(86) {
  -webkit-animation: snow-86 7s infinite;
          animation: snow-86 7s infinite;
}

@-webkit-keyframes snow-86 {
  from {
    transform: translate(283px, -26px);
  }
  to {
    transform: translate(283px, 569px);
  }
}

@keyframes snow-86 {
  from {
    transform: translate(283px, -26px);
  }
  to {
    transform: translate(283px, 569px);
  }
}
.snowflake:nth-child(87) {
  -webkit-animation: snow-87 10s infinite;
          animation: snow-87 10s infinite;
}

@-webkit-keyframes snow-87 {
  from {
    transform: translate(237px, -48px);
  }
  to {
    transform: translate(237px, 529px);
  }
}

@keyframes snow-87 {
  from {
    transform: translate(237px, -48px);
  }
  to {
    transform: translate(237px, 529px);
  }
}
.snowflake:nth-child(88) {
  -webkit-animation: snow-88 9s infinite;
          animation: snow-88 9s infinite;
}

@-webkit-keyframes snow-88 {
  from {
    transform: translate(338px, -253px);
  }
  to {
    transform: translate(338px, 556px);
  }
}

@keyframes snow-88 {
  from {
    transform: translate(338px, -253px);
  }
  to {
    transform: translate(338px, 556px);
  }
}
.snowflake:nth-child(89) {
  -webkit-animation: snow-89 10s infinite;
          animation: snow-89 10s infinite;
}

@-webkit-keyframes snow-89 {
  from {
    transform: translate(420px, -51px);
  }
  to {
    transform: translate(420px, 617px);
  }
}

@keyframes snow-89 {
  from {
    transform: translate(420px, -51px);
  }
  to {
    transform: translate(420px, 617px);
  }
}
.snowflake:nth-child(90) {
  -webkit-animation: snow-90 8s infinite;
          animation: snow-90 8s infinite;
}

@-webkit-keyframes snow-90 {
  from {
    transform: translate(450px, -132px);
  }
  to {
    transform: translate(450px, 574px);
  }
}

@keyframes snow-90 {
  from {
    transform: translate(450px, -132px);
  }
  to {
    transform: translate(450px, 574px);
  }
}
.snowflake:nth-child(91) {
  -webkit-animation: snow-91 8s infinite;
          animation: snow-91 8s infinite;
}

@-webkit-keyframes snow-91 {
  from {
    transform: translate(213px, -88px);
  }
  to {
    transform: translate(213px, 444px);
  }
}

@keyframes snow-91 {
  from {
    transform: translate(213px, -88px);
  }
  to {
    transform: translate(213px, 444px);
  }
}
.snowflake:nth-child(92) {
  -webkit-animation: snow-92 13s infinite;
          animation: snow-92 13s infinite;
}

@-webkit-keyframes snow-92 {
  from {
    transform: translate(444px, -263px);
  }
  to {
    transform: translate(444px, 543px);
  }
}

@keyframes snow-92 {
  from {
    transform: translate(444px, -263px);
  }
  to {
    transform: translate(444px, 543px);
  }
}
.snowflake:nth-child(93) {
  -webkit-animation: snow-93 7s infinite;
          animation: snow-93 7s infinite;
}

@-webkit-keyframes snow-93 {
  from {
    transform: translate(425px, -197px);
  }
  to {
    transform: translate(425px, 689px);
  }
}

@keyframes snow-93 {
  from {
    transform: translate(425px, -197px);
  }
  to {
    transform: translate(425px, 689px);
  }
}
.snowflake:nth-child(94) {
  -webkit-animation: snow-94 7s infinite;
          animation: snow-94 7s infinite;
}

@-webkit-keyframes snow-94 {
  from {
    transform: translate(217px, -232px);
  }
  to {
    transform: translate(217px, 456px);
  }
}

@keyframes snow-94 {
  from {
    transform: translate(217px, -232px);
  }
  to {
    transform: translate(217px, 456px);
  }
}
.snowflake:nth-child(95) {
  -webkit-animation: snow-95 9s infinite;
          animation: snow-95 9s infinite;
}

@-webkit-keyframes snow-95 {
  from {
    transform: translate(16px, -73px);
  }
  to {
    transform: translate(16px, 599px);
  }
}

@keyframes snow-95 {
  from {
    transform: translate(16px, -73px);
  }
  to {
    transform: translate(16px, 599px);
  }
}
.snowflake:nth-child(96) {
  -webkit-animation: snow-96 11s infinite;
          animation: snow-96 11s infinite;
}

@-webkit-keyframes snow-96 {
  from {
    transform: translate(40px, -137px);
  }
  to {
    transform: translate(40px, 700px);
  }
}

@keyframes snow-96 {
  from {
    transform: translate(40px, -137px);
  }
  to {
    transform: translate(40px, 700px);
  }
}
.snowflake:nth-child(97) {
  -webkit-animation: snow-97 12s infinite;
          animation: snow-97 12s infinite;
}

@-webkit-keyframes snow-97 {
  from {
    transform: translate(411px, -203px);
  }
  to {
    transform: translate(411px, 569px);
  }
}

@keyframes snow-97 {
  from {
    transform: translate(411px, -203px);
  }
  to {
    transform: translate(411px, 569px);
  }
}
.snowflake:nth-child(98) {
  -webkit-animation: snow-98 12s infinite;
          animation: snow-98 12s infinite;
}

@-webkit-keyframes snow-98 {
  from {
    transform: translate(6px, -89px);
  }
  to {
    transform: translate(6px, 474px);
  }
}

@keyframes snow-98 {
  from {
    transform: translate(6px, -89px);
  }
  to {
    transform: translate(6px, 474px);
  }
}
.snowflake:nth-child(99) {
  -webkit-animation: snow-99 7s infinite;
          animation: snow-99 7s infinite;
}

@-webkit-keyframes snow-99 {
  from {
    transform: translate(149px, -50px);
  }
  to {
    transform: translate(149px, 451px);
  }
}

@keyframes snow-99 {
  from {
    transform: translate(149px, -50px);
  }
  to {
    transform: translate(149px, 451px);
  }
}
.snowflake:nth-child(100) {
  -webkit-animation: snow-100 9s infinite;
          animation: snow-100 9s infinite;
}

@-webkit-keyframes snow-100 {
  from {
    transform: translate(237px, -263px);
  }
  to {
    transform: translate(237px, 547px);
  }
}

@keyframes snow-100 {
  from {
    transform: translate(237px, -263px);
  }
  to {
    transform: translate(237px, 547px);
  }
}
@-webkit-keyframes tail {
  10% {
    transform: rotate(2deg);
  }
  20% {
    transform: rotate(-5deg);
  }
}
@keyframes tail {
  10% {
    transform: rotate(2deg);
  }
  20% {
    transform: rotate(-5deg);
  }
}
@-webkit-keyframes shadow {
  to {
    width: 185px;
  }
}
@keyframes shadow {
  to {
    width: 185px;
  }
}
@-webkit-keyframes eyes {
  50% {
    transform: translate(3px, 2px);
  }
  60% {
    transform: translate(0, 0);
  }
  100% {
    transform: translate(0, 0);
  }
}
@keyframes eyes {
  50% {
    transform: translate(3px, 2px);
  }
  60% {
    transform: translate(0, 0);
  }
  100% {
    transform: translate(0, 0);
  }
}
@-webkit-keyframes eaves {
  50% {
    transform: translateY(0);
  }
  60% {
    transform: translateY(-1px);
  }
  100% {
    transform: translateY(-1px);
  }
}
@keyframes eaves {
  50% {
    transform: translateY(0);
  }
  60% {
    transform: translateY(-1px);
  }
  100% {
    transform: translateY(-1px);
  }
}
@-webkit-keyframes hoof-one {
  to {
    transform: translateX(2px) rotate(5deg);
  }
}
@keyframes hoof-one {
  to {
    transform: translateX(2px) rotate(5deg);
  }
}
@-webkit-keyframes jump {
  to {
    transform: translateY(-2px) rotate(25deg);
  }
}
@keyframes jump {
  to {
    transform: translateY(-2px) rotate(25deg);
  }
}
@-webkit-keyframes jump-two {
  to {
    transform: translateY(2px);
  }
}
@keyframes jump-two {
  to {
    transform: translateY(2px);
  }
}
@-webkit-keyframes rocking {
  to {
    transform: rotate(-1deg);
  }
}
@keyframes rocking {
  to {
    transform: rotate(-1deg);
  }
}
@-webkit-keyframes ear-left {
  85% {
    transform: rotate(30deg);
  }
  100% {
    transform: rotate(-10deg);
  }
}
@keyframes ear-left {
  85% {
    transform: rotate(30deg);
  }
  100% {
    transform: rotate(-10deg);
  }
}
@-webkit-keyframes ear-right {
  85% {
    transform: rotate(160deg);
  }
  100% {
    transform: rotate(170deg);
  }
}
@keyframes ear-right {
  85% {
    transform: rotate(160deg);
  }
  100% {
    transform: rotate(170deg);
  }
}
@-webkit-keyframes leg-right {
  to {
    transform: translateX(4px) rotate(2deg);
  }
}
@keyframes leg-right {
  to {
    transform: translateX(4px) rotate(2deg);
  }
}
@-webkit-keyframes leg-left {
  0% {
    transform: rotate(0deg) translateX(0px);
  }
  50% {
    transform: rotate(5deg) translateX(3px);
  }
}
@keyframes leg-left {
  0% {
    transform: rotate(0deg) translateX(0px);
  }
  50% {
    transform: rotate(5deg) translateX(3px);
  }
}
a {
  font-weight: 600;
  color: #91a7ff;
  text-decoration: none;
}
a:hover {
  color: #5c7cfa;
  text-decoration: underline;
}

html,
body {
  font-family: "Open Sans";
}

body {
  background-color: #f8f9fa;
  color: #adb5bd;
}

.title {
  text-align: center;
}
.title h1 {
  font-size: 1.5em;
  margin: 100px 0 10px 0;
}

.socials {
  display: block;
  font-size: 14px;
  margin: 0;
  padding: 0;
}
.socials li {
  display: inline;
}
.socials li:not(:last-child) {
  margin-right: 0.75em;
}
.socials li a {
  vertical-align: middle;
}
.socials li a:hover img {
  -webkit-animation: link 0.5s;
          animation: link 0.5s;
}
.socials li a img {
  width: 1.3em;
}

.credits {
  font-size: 0.8em;
  text-align: center;
}

.love {
  background: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/42764/heart-smil.svg);
  display: inline-block;
  height: 16px;
  vertical-align: middle;
  width: 16px;
}
body{
    width: 100%;
    height: 100vh;
    overflow: hidden;
    /* background: #f2adab; */
}

.box{
    position: fixed;
    left: calc(50vw - 40vmin);
    top: calc(50vh - 27.5vmin);
    width: 90vmin;
    height: 75vmin;
}

svg{
    overflow: visible;
}

#snow {
    pointer-events: none;
}
.snow-clone{
    opacity: 0;
}
