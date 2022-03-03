<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>AJAX-API Assignment</title>

    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-validate/1.19.3/jquery.validate.min.js" integrity="sha512-37T7leoNS06R80c8Ulq7cdCDU5MNQBwlYoy1TX/WUsLFC2eYNqtKlV0QjH7r8JpG/S0GUMZwebnVFLPd6SU5yg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

    

    <script>
        function dataSent(){
      $.ajax({
          url: "http://dummy.restapiexample.com/api/v1/employees",
          type : "GET",
            success : function(data){

                console.log(data);
                var tab = "<tr><th>id</th><th>Employee Name</th><th>Employee Salary</th><th>Employee Age</th><th>Profile Image</th></tr>";
                for( x=0;x<data.data.length;x++){
                    // console.log(data.data[x].id);
                    // console.log(data.data[x].employee_name);
                    // console.log(data.data[x].employee_salary);
                    // console.log(data.data[x].employee_age);
                    // console.log(data.data[x].profile_image);

                    tab += '<tr>';
                        tab += '<td>'+ data.data[x].id + '</td>';
                        tab += '<td>' + data.data[x].employee_name + '</td>';
                        tab += '<td>' + data.data[x].employee_salary + '</td>';
                        tab += '<td>' + data.data[x].employee_age + '</td>';
                        tab += '<td>' + data.data[x].profile_image + '</td>';
                        tab += '</tr>';
                }
                $("#table1").append(tab);
                if(success){
                  document.getElementById('success1').innerHTML = data.message;
                }
          }
      });
        }
    </script>
    <script>
      function postData() {
        $.ajax({
          url: "http://dummy.restapiexample.com/api/v1/create",
          type: "POST",
          
          dataType: "JSON",
          data: {"first_name":"Aditya", "last_name": "Pandey", "salary": "230000"},
          success: function(data){
          if(success){
          document.getElementById('success').innerHTML = data.message;
          console.log(data);
        }
          }
          
        });   
        
      }
    </script>


<script>
  function putData(){
    $.ajax({
      url : "http://dummy.restapiexample.com/public/api/v1/update/21",
      type : "PUT",
      data: {"Employee_Name": "Aditya Pandey", "Employee_Salary": "360000", "Employee_Age":"23"},
      success: function(data){
        if(success){
          document.getElementById('put').innerHTML = data.message;
          console.log(data);
        }
      }
    });
  }
</script>

<script>
  function deleteData(){
    $.ajax({
      url : "http://dummy.restapiexample.com/public/api/v1/delete/2",
      type : "DELETE",
      success: function(data){
        if(success){
          document.getElementById('delete').innerHTML = data.message;
          console.log(data);
        }
      }
    });
  }
</script>


    <style>
      #table1 {
        background-color: thistle;
        border-radius: 10px;
        border: 1px solid black;
        text-align: center;
        margin: 5%;
        padding: 20px;
      }
      td {
        border-right: 1px solid black;
      }
    </style>
  </head>
  <body>
    <h1 style="text-align: center">
      AJAX API Assignment
    </h1>
    <table id="table1" class="table"></table>
    <button style="margin-top: 2%;background-color: greenyellow;" type="button" onclick="dataSent()" >Get Data</button>
    <h1 id="success1"></h1>
    

    <button style="margin-top: 2%;background-color: greenyellow;" type="button" onclick="postData()">Post Data</button>
    <h1 id="success"></h1>

    <button style="margin-top: 2%;background-color: greenyellow;" type="button" onclick="putData()">Put Data</button>
    <h1 id="put"></h1>

    <button style="margin-top: 2%;background-color: greenyellow;" type="button" onclick="deleteData()">Delete Data</button>
    <h1 id="delete"></h1>
  </body>
</html>
