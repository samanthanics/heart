<html>
    <head>
        <style>
          body {
    margin: 0;
    padding: 0;
    min-height: 100;
    display: flex;
    align-items: center;
    justify-content: center;
    background: black;
}
.hart {
    height: 70px;
    width: 70px;
    background: #f20044;
    position: relative;
    transform: rotate(-45deg);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    animation: heart 0.6s linear infinite;
}
@keyframes heart {
    0% {
        transform: rotate(-45deg) scale(1.07);
    }
    80% {
        transform: rotate(-45deg) scale(1.0);
    }
    100% {
        transform: rotate(-45deg) scale(0.8);
    }
}
.hart::before, 
.hart::after {
    content: '';
    position: absolute;
    height: 70px;
    width: 70px;
    background: #f20044;
    border-radius: 50%;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}
.hart::before {
    top: -35px;
    left: 0;
}
.hart::after {
    left: 35px;
    top: 0;
}
h1 {
    color: aliceblue;
    text-align: center;
    font-family: 'Times New Roman', Times, serif;
    position: relative;
    font-style: oblique;
    bottom: -100px;
    right: 100px;
}
.name{
        position: absolute;
        top: 10px;
        left: 20px;
        font-family: 'Arial', sans-serif;
        font-size: 18px;
        font-weight: bold;
        color: #ffffff;
        z-index: 10;
}
</style>
    </head>
    <body>
        <h4 class="name"> Sam</h4>
        <div class="hart"></div>
        <h1>I Really Love You Babe</h1>
    </body>
</html>
