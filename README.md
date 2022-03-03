<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>AJAX-API Assignment</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <style>
        #table1{
            background-color: thistle;
            border-radius: 10px;
            border: 1px solid black;
            text-align: center;
            margin: 5%;
            padding: 20px;
        }
        td{
            border-right: 1px solid black;
        }
    </style>
  </head>
  <body>
    <h1 style="text-align: center">
      Getting data from an API using AJAX and displaying it in the form of Table
    </h1>
    <table id="table1" class="table table-success"></table>
    <button style="margin-top: 2%;background-color: greenyellow;" type="button" onclick="myFunction()" >Click Me</button>

    <script>
        function myFunction(){
      $.ajax({
          url: "http://dummy.restapiexample.com/api/v1/employees",
          type : "GET",
       dataType:json,
      cors: true,
      contentType:application/json,
      secure: true,
                  headers: { 'Access-Control-Allow-Origin': '*',
      },
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
          }
      });
        }
    </script>
  </body>
</html>
