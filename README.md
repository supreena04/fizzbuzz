# fizzbuzz <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FizzBuzz</title>
</head>
<body>
    <h1>FizzBuzz</h1>
    <ul id="output"></ul>

    <script>
        // Function to solve the FizzBuzz problem for a given range
        function fizzBuzz(start, end) {
            let output = '';

            for (let num = start; num <= end; num++) {
                if (num % 3 === 0 && num % 5 === 0) {
                    output += '<li>FizzBuzz</li>';
                } else if (num % 3 === 0) {
                    output += '<li>Fizz</li>';
                } else if (num % 5 === 0) {
                    output += '<li>Buzz</li>';
                } else {
                    output += `<li>${num}</li>`;
                }
            }

            document.getElementById('output').innerHTML = output;
        }

        // Call the fizzBuzz function with the specified range
        fizzBuzz(1, 150);
    </script>
</body>
</html>
