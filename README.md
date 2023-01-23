# test

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Добрый день</title>
</head>
<body>

    <h1> Тестовая задача </h1>


    <h2>Первоначальный массив: </h2>
    <p class="array-first" id="array-first"></p>

    <hr>
    <h2>Измененный массив: </h2>
    <p class="array-changed" id="array-changed"></p>

    <script>
		
        const firstOutput = document.getElementById('array-first');
        const firstChanged = document.getElementById('array-changed');
        
        const arr = ['школа' , 'dad' , 'чай' , 'coffee' , 'ma'];
        firstOutput.innerHTML = arr;

        console.log(arr);

        const arrChanged = [];

        const arrChanged = arr.forEach(function (item) {
            if(item.length <= 3) {
                arrChanged.push(item)
            }
        })

        console.log(arrChanged);

        firstChanged.innerHTML = arrChanged;

    </script>
    
</body>
</html>
