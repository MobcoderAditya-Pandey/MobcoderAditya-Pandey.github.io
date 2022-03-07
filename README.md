<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Table</title>
    <!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">

<!-- jQuery library -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>

<!-- Latest compiled JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
<style>
    .heading{
        background-color: green;
        color: white;
    }
    .dark{
            background-color: #222;
            color: #e6e6e6;
        }
        .btn{
            margin: 5%;
        }
        #animated_div{
            margin-top: 5%;
            width: 200px;
            height: 47px;
            background-color: aqua;
            position: relative;
            animation-name: animated_div;
            animation-duration: 5s;
            animation-iteration-count: infinite;
            padding: 10px;
            border-radius: 5px;
            font-size: 20px;
            font-weight: bold;
        }
        @keyframes animated_div{
            0%{
                transform: rotate(0deg);
                left: 0px;
            }
            25%{
                transform: rotate(20deg);
                left: 0px;
            }
            50%{
                transform : rotate(0deg);
                left : 500px;
            }
            55%{
                transform: rotate(0deg);
                left: 500px;
            }
            70%{
                transform: rotate(0deg);
                left: 500px;
                background-color: #1ec71e;
            }
            100%{
                transform: rotate(-360deg);
                left: 0px;
            }

        }
</style>
<script src="https://code.jquery.com/jquery-3.5.1.js">
    </script>   
    <script>
        function darkMode(){
         var ele = document.body;
         ele.classList.toggle("dark");
         document.getElementById('dMode').innerHTML = "Light Mode";
        }
    </script>

    <script>
    function myFunction(){
       
                var price = {"_id":"5f0d9edf8c53f01714b87c69","harvestStatus":1,"chargeId":"ch_1H4XhFHitCcHm9i6qrcOixPU","transferGroup":"4365f9a4-c0cd-2ea5-a318-ab424c913add","userId":"5ef1e000f3dd1e32bc340b2b","amount":191.5,"deliveryFees":0,"totalPrice":191.5,"billingInfo":{"firstName":"ritesh","lastName":"ritesh","addressLine1":"ritesh","addressLine2":"ritesh","city":"ritesh","state":"ritesh","country":"India","postalCode":"712232","phoneNumber":"5099962370"},"buyList":[{"totalPrice":188,"deliveryType":"","totalPayPrice":188,"courierType":"Pickup","deliveryFees":10,"addressLine1":"","addressLine2":"","city":"","state":"","postalCode":"","address":" Thursday ,04:30 PM-04:30 PM","farmName":"raj1's farm","_id":"5f0c42b85a4a35242b739ef9","farmId":"5ef4503152c6905b98e6dad2","productList":[{"productQuantity":1,"productPrice":20,"totalPayPrice":20,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594636861375_IMG_8415.JPG","productName":"Pizzad","unit":"kt","variety":"Qdddert","itemStatus":1,"_id":"5f0c42b85a4a35242b739efa","productId":"5f0c3a3e5a4a35242b739d5e"},{"productQuantity":2,"productPrice":79,"totalPayPrice":158,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594298231380_veg4.jfif","productName":"Ddddddddd","unit":"pint","variety":"1","itemStatus":1,"_id":"5f0cbaf45a4a35242b739f75","productId":"5f070f7758b2dd2650b7ef33"},{"productQuantity":1,"productPrice":10,"totalPayPrice":10,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594636664122_Carrots.jpeg","productName":"Bananas","unit":"pint","variety":"12","itemStatus":1,"_id":"5f0cbb135a4a35242b739f7b","productId":"5f0c39865a4a35242b739d56"}],"farmUserId":"5eedd8ca09e7b15ae52c3e3a"},{"totalPrice":3.5,"deliveryType":"","totalPayPrice":3.5,"courierType":"Pickup","deliveryFees":9,"addressLine1":"","addressLine2":"","city":"","state":"","postalCode":"","address":"vijay nagar sector-71 noida 201301 Thursday ,11:30 AM-01:30 PM","farmName":"bani's ","_id":"5f0c43c95a4a35242b739f01","farmId":"5ef1dabef3dd1e32bc340b26","productList":[{"productQuantity":1,"productPrice":3.5,"totalPayPrice":3.5,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594112569818_veg2.jfif","productName":"Fddddddddddd","unit":"1","variety":"Latest","itemStatus":1,"_id":"5f0c43c95a4a35242b739f02","productId":"5f043a39f2c29e6ae856f796"}],"farmUserId":"5ef1d9d9f3dd1e32bc340b24"},{"totalPrice":260,"deliveryType":"","totalPayPrice":240,"courierType":"Pickup","deliveryFees":20,"addressLine1":"","addressLine2":"","city":"","state":"","postalCode":"","address":" Thursday ,04:30 PM-04:30 PM","farmName":"marvel's farm","_id":"5f0c42b85a4a35242b739ef9","farmId":"5ef4503152c6905b98e6dad2","productList":[{"productQuantity":1,"productPrice":100,"totalPayPrice":100,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594636861375_IMG_8415.JPG","productName":"iron","unit":"kt","variety":"Qdddert","itemStatus":1,"_id":"5f0c42b85a4a35242b71qw2","productId":"5f0c3a3e5a4a35242b739d5e"},{"productQuantity":2,"productPrice":40,"totalPayPrice":80,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594298231380_veg4.jfif","productName":"nickle","unit":"pint","variety":"1","itemStatus":1,"_id":"5f0cbaf45a4a35242b739f75","productId":"5f070f7758b2dd2650b7ef33"},{"productQuantity":4,"productPrice":15,"totalPayPrice":60,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594636664122_Carrots.jpeg","productName":"copper","unit":"pint","variety":"12","itemStatus":1,"_id":"5f0cbb135a4a123442b739f7b","productId":"5f0c39865a4a35242b739d56"}],"farmUserId":"5eedd8ca09e7b15ae52c3e3a"},{"totalPrice":500,"deliveryType":"","totalPayPrice":500,"courierType":"Pickup","deliveryFees":0,"addressLine1":"","addressLine2":"","city":"","state":"","postalCode":"","address":" Thursday ,04:30 PM-04:30 PM","farmName":"old's farm","_id":"5f0c42b85a4a35242b739ef9","farmId":"5ef4503152c6905b98e6dad2","productList":[{"productQuantity":1,"productPrice":240,"totalPayPrice":240,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594636861375_IMG_8415.JPG","productName":"gold","unit":"kt","variety":"Qdddert","itemStatus":1,"_id":"5f0c42b85a4a35242b739efa","productId":"5f0c3a3e5a4a35242b739d5e"},{"productQuantity":2,"productPrice":5,"totalPayPrice":10,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594298231380_veg4.jfif","productName":"silver","unit":"pint","variety":"1","itemStatus":1,"_id":"5f0cbaf45a4a35242b739f75","productId":"5f070f7758b2dd2650b7ef33"},{"productQuantity":10,"productPrice":25,"totalPayPrice":250,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594636664122_Carrots.jpeg","productName":"plates","unit":"pint","variety":"12","itemStatus":1,"_id":"5f0cbb11qsdwa35242b739f7b","productId":"5f0c39865a4a35242b739d56"}],"farmUserId":"5eedd8ca09e7b15ae52c3e3a"},{"totalPrice":1800,"deliveryType":"","totalPayPrice":1800,"courierType":"Pickup","deliveryFees":100,"addressLine1":"","addressLine2":"","city":"","state":"","postalCode":"","address":" Thursday ,04:30 PM-04:30 PM","farmName":"new mart","_id":"5f0c42b85a4a31qw32qwe39ef9","farmId":"5ef4503152c6905b98e6dad2","productList":[{"productQuantity":1,"productPrice":200,"totalPayPrice":200,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594636861375_IMG_8415.JPG","productName":"Pizza","unit":"kt","variety":"Qdddert","itemStatus":1,"_id":"5f0c42b85a4a35242b739efa","productId":"5f0c3a3e5a4a35242b739d5e"},{"productQuantity":4,"productPrice":25,"totalPayPrice":100,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594298231380_veg4.jfif","productName":"Ddddddddd","unit":"pint","variety":"1","itemStatus":1,"_id":"5f0cbaf45a4a35242b739f75","productId":"5f070f7758b2dd2650b7ef33"},{"productQuantity":150,"productPrice":10,"totalPayPrice":1500,"image":"https://healtyplanet-dev.nyc3.digitaloceanspaces.com/fileData_1594636664122_Carrots.jpeg","productName":"Bananas","unit":"pint","variety":"12","itemStatus":1,"_id":"5f0cbb135a4a35242b739f7b","productId":"5f0c39865a4a35242b739d56"}],"farmUserId":"5eedd8ca09e7b15ae52c3e3a"}],"status":"1","created":"2020-07-13T19:52:17.588Z","updated":"2020-07-13T19:52:17.588Z","__v":0};
                console.log(price);
                var s ="<tr class='heading'><th>Total Price</th> <th>Order Price</th> <th>Fees</th> <th>Form Name</th></tr>";
                for(let x in price.buyList){
                    s = s +  "<tr><td>" + price.buyList[x].totalPrice + "</td><td>" + price.buyList[x].totalPayPrice + "</td><td>" + price.buyList[x].deliveryFees + "</td><td>" + price.buyList[x].farmName + "</td></tr>";
                }
                //console.log(s);
                $('#table1').append(s);
                $('#table1').html(s);

                var s1 = "<tr class='heading'><th>Total Quantity</th><th>Total Price</th><th>Per Item Price</th><th>Product Name</th></tr>";
                for (let y in price.buyList) {

            for (let z in price.buyList[y].productList) {

                        s1 = s1 + "<tr><td>" + price.buyList[y].productList[z].productQuantity + "</td><td>" + (Number(price.buyList[y].productList[z].productQuantity) * Number(price.buyList[y].productList[z].productPrice)) + "</td><td>" + price.buyList[y].productList[z].productPrice + "</td><td>" + price.buyList[y].productList[z].productName + "</td></tr>";
                    }
                }
                

                $('#table2').append(s1);
                $('#table2').html(s1);
   }


    </script>

</head>
<body>
    <h1> <b> BuyList</b></h1>
     <table class="table table-striped" id="table1">
   
</table>
<hr>
<table class="table" id="table2">
    <h1> <b> ItemList</b></h1>

</table>
<input type="button"  class="btn btn-success" value="Click me" onclick="myFunction()">
<hr>
    <div id="animated_div">Aditya Pandey</div>
    <button type="button" id="dMode" onclick="darkMode()" class="btn btn-warning"><i class="fa-solid fa-eye"></i>&nbsp;Switch Mode</button>
</body>
</html>
