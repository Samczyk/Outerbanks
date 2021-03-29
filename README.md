<head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>COMMING SOON...</title>
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Bowlby+One+SC&display=swap" rel="stylesheet">
    <style>
        body{
            background-color: #010101;
            font-family: 'Bowlby One SC', cursive;
            color: #eee4af;

        }
        p {
            text-align: center;
            font-size: 60px;
            margin-top: 0px;
        }
    </style>
</head>
<body>
<div id="container" style="margin-left auto; margin-right:auto; padding-top:40px;"></div>
<h1 style="text-align:center; font-size:50px; padding:20px;">COMMING SOON...</h1>
<p id="demo"></p>
<h1 style="text-align:center; font-size:40px; padding:20px;">01.04.2021 18:00</h1>

<script>
    var countDownDate = new Date("2021-04-01 18:00:00").getTime();

    var x = setInterval(function() {

        var now = new Date().getTime();

        var distance = countDownDate - now;

        var days = Math.floor(distance / (1000 * 60 * 60 * 24));
        var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
        var seconds = Math.floor((distance % (1000 * 60)) / 1000);

        document.getElementById("demo").innerHTML = days + "d " + hours + "h "
            + minutes + "m " + seconds + "s ";
        if (distance < 0) {
            clearInterval(x);
            document.getElementById("demo").innerHTML = "EXPIRED";
        }
    }, 1000);
</script>

</body>
