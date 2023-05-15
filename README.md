<html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Project</title>
    <link rel="stylesheet" type="text/css" href="style.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css">
</head>
<style>
    body{
    background-image: linear-gradient(rgba(0,0,0,0.5),rgba(0,0,0,0.5)),url(bg.jpg);
    background-size: cover;
    background-position:center;
}

.booking-form-box{
    max-width: 350px;
    border: 1px solid #ced4da;
    margin: 10% auto 0;
}

.radio-btn{
    color: #fff;
    margin: 0 20px;
}

.radio-btn .btn{
    margin: 20px 10px 20px 0;
    box-shadow: none;
}

.radio-btn .btn::after{
    content: '';
    height: 15px;
    width: 15px;
    top: -2px;
    left: -1px;
    background-color: #fff;
    position: relative;
    display: inline-block;
    visibility: visible;
    border-radius: 50%;
}

.radio-btn .btn:checked:after{
    content: '';
    background-color: #000;
    transition: 0.5s;
}

.radio-btn span{
    color: #fff;
    margin-right: 5px;
    font-size: 16px;
}

.booking-form{
    padding: 0 20px 20px;
}

.booking-form label{
    margin-bottom: 5px;
    margin-top: 10px;
    font-size: 18px;
    color: #fff;
}

input::placeholder{
    color: #fff !important;
}

.input-grp{
    width: 151px;
    display: inline-block;
}

.form-control{
    font-size: 18px !important;
    border-radius: 0 !important;
    color: #fff !important;
    background: transparent !important;
    box-shadow: none !important;
} 

.select-date::-webkit-inner-spin-button,
.select-date::-webkit-inner-spin-button
{
    -webkit-appearance: none;
    margin: 0;
}

.select-date::-webkit-calender-picker-indicator{
    background: transparent !important;
}

.custom-select{
    color:#fff !important;
    font-size: 18px !important;
    border: 1px solid #ced4da !important;
    box-shadow: none !important;
    border-radius: 0 !important;
    background: transparent !important;
}

.custom-select option{
    color: #333;
}

.flight{
    width:  100%;
    padding: 9px 0;
    font-size: 18px;
    border: 1px solid #ced4da !important;
    background: transparent!important;
    box-shadow: none !important;
    border-radius: 0 !important;
}

.flight:hover{
    background: #fff !important; ;
    color: #000 !important;
    transition: 0.5s;
}
.sidebar ul li{
      padding: 8px;
      list-style-type: none;
      float: left;
      font-size: 15px;
      font-weight: bold;
      text-decoration: none;
      margin: 7px;
     color: yellowgreen;
    }
     .sidebar ul {
      display: inline-block;
    }      
    img {
  opacity: 0.5;
}

img:hover {
  opacity: 1.0;
}
body{
    background-image: url(img.jpeg);
    background-size: cover;
}  
</style>
<body>
    <div class="sidebar">
        <center>
    <nav>
        <header>
            <ul>
<a href="book" target="_blank"><li>BOOK</li></a>
<a href="trip" target="_blank"><li>MY TRIPS</li></a>
<a href="check" target="_blank"><li>CHECK IN</li></a>
<a href="status" target="_blank"><li>FLIGHT STATUS</li></a>
<a href="home.html" target="_self"><li><b><font size="25px">Airline</font></b></li></a>
<a href="cancel" target="_blank"><li>CANCELLATION</li></a>
<a href="contact" target="_blank"><li>CONTACT US</li></a>
<a href="sign.html" target="_blank"><input type="button" value="Sign-in"></a>
    </ul></header>
</nav></center>
</div>
    <div class="booking-form-box">
        <div class="radio-btn">
            <span>Roundtrip : </span>
            <input type="radio" class="btn" name="check"><span>One Way</span>
            <input type="radio" class="btn" name="check"><span>Multi-City</span>
        </div>
        <div class="booking-form">
            <label>Form : <select id="from">
                <option value="0"></option>
                <option value="1">Nepal</option>
                <option value="2">Japan</option>
                <option value="3">China</option>
                <option value="4">Korea</option>
                <option value="5">Australia</option>
                <option value="6">Canada</option>
                <option value="7">Thailand</option>    
            </select></label>
            <label>To : <select id="to">
                <option value="0"></option>
                <option value="1">Nepal</option>
                <option value="2">Japan</option>
                <option value="3">China</option>
                <option value="4">Korea</option>
                <option value="5">Australia</option>
                <option value="6">Canada</option>
                <option value="7">Thailand</option>    
            </select>
            
            </label>
            
            
            <div class="input-grp">
                <label>Departing</label>
                <input type="date" name="" class="form-control select-date">
            </div>

            <div class="input-grp">
                <label>Returning</label>
                <input type="date" name="" class="form-control select-date">
            </div>

            <div class="input-grp">
                <label>Adults</label>
                <input type="number" name="" class="form-control" value="1">
            </div>

            <div class="input-grp">
                <label>Childerns</label>
                <input type="number" name="" class="form-control" value="0">
            </div>

            <div class="input-grp">
            <label>Travel Class</label>
            <select class="custom-select">
                 <option value="1">Economy class</option>
                <option value="2">Business class</option>
                </select>
            </div>
            
            <div class="input-grp">
                <button type="button" class="btn btn-primary flight">Show Flights</button>
            </div>

        </div>
    </div>
</body>

</html>
