📄 index.html

<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <title>جيلان</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>مرحباً بك في موقع جيلان</h1>

    <div class="buttons">
        <a class="btn" onclick="showImage('tree')">جيلان</a>
        <a class="btn" onclick="showImage('house')">عبدالسلام</a>
        <a class="btn" onclick="showText('عدنان')">عدنان</a>
    </div>

    <div id="content" class="content"></div>

    <script>
        function showImage(type) {
            const content = document.getElementById('content');
            const imgSrc = type === 'tree' 
                ? 'https://cdn-icons-png.flaticon.com/512/427/427735.png' 
                : 'https://cdn-icons-png.flaticon.com/512/616/616408.png';
            content.innerHTML = '<img src="' + imgSrc + '" class="image">';
        }

        function showText(name) {
            document.getElementById('content').innerHTML = '<h2>مرحباً بك يا ' + name + '!</h2>';
        }
    </script>
</body>
</html>
