# Johnny_Walker_NinjaManChallenge
<!DOCTYPE html>
<html>
<head>
    <title>NinjaMan</title>
    <style type="text/css">
        div {
            background-color: yellow;
            margin: 10px;
            padding: 10px;
        }
    </style>
</head>
<body>
    <div id='world'>
        <div class = 'row'>
            <div class = 'wall'></div>
            <div class = 'wall'></div>
            <div class = 'wall'></div>
            <div class = 'wall'></div>
            <div class = 'wall'></div>
        </div>
   <div class = 'row'>
            <div class = 'wall'></div>
            <div class = 'blank'></div>
            <div class = 'sushi'></div>
            <div class = 'sushi'></div>
            <div class = 'wall'></div>
        </div>
    <div class = 'row'>
            <div class = 'wall'></div>
            <div class = 'sushi'></div>
            <div class = 'wall'></div>
            <div class = 'sushi'></div>
            <div class = 'wall'></div>
        </div>
   <div class = 'row'>
            <div class = 'wall'></div>
            <div class = 'sushi'></div>
            <div class = 'sushi'></div>
            <div class = 'sushi'></div>
            <div class = 'wall'></div>
        </div>
   <div class = 'row'>
            <div class = 'wall'></div>
            <div class = 'wall'></div>
            <div class = 'wall'></div>
            <div class = 'wall'></div>
        }      
    </style>
</head>
<body>
    <div id='world'></div>
    <div id='ninjaman'></div>
</body>
<script type="text/javascript">
    var world = [
        [1,1,1,1,1]
        [1,0,2,2,1]
        [1,2,1,2,1]
        [1,2,2,2,1]
        [1,1,1,1,1]
    ];
    var worldDict = {
        0: 'blank',
        1: 'wall',
        2: 'sushi'
    }

    function drawWorld(){
        output = "";

        for(var row = 0; row <world. length;  row++){
            output += "div class = 'row'>"
            for (var x = 0; x <world [row]. length; x++){
                output +=  "div class= ' " +  worldDict[
                    world[row] [x]] +"'></div>'"
                   
            }
            output += "</div>"
        }
        document.getElementById('world').innerHTML =
            output;
    }
    drawWorld()
</script>
</html>
