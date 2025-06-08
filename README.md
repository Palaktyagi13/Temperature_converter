# Temperature_converter
function convertFromCelsius() {
    let celsius = parseFloat(document.getElementById("celsius").value);
    if (!isNaN(celsius)) {
        document.getElementById("fahrenheit").value = (celsius * 9/5 + 32).toFixed(2);
        document.getElementById("kelvin").value = (celsius + 273.15).toFixed(2);
    }
}

function convertFromFahrenheit() {
    let fahrenheit = parseFloat(document.getElementById("fahrenheit").value);
    if (!isNaN(fahrenheit)) {
        document.getElementById("celsius").value = ((fahrenheit - 32) * 5/9).toFixed(2);
        document.getElementById("kelvin").value = (((fahrenheit - 32) * 5/9) + 273.15).toFixed(2);
    }
}

function convertFromKelvin() {
    let kelvin = parseFloat(document.getElementById("kelvin").value);
    if (!isNaN(kelvin)) {
        document.getElementById("celsius").value = (kelvin - 273.15).toFixed(2);
        document.getElementById("fahrenheit").value = ((kelvin - 273.15) * 9/5 + 32).toFixed(2);
    }
}

body {
    font-family: Arial, sans-serif;
    background: #f4f4f4;
    text-align: center;
    padding: 20px;
}

.container {
    background: white;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
    max-width: 400px;
    margin: auto;
}

h2 {
    color: #333;
}

.input-group {
    margin: 15px 0;
}

label {
    display: block;
    font-weight: bold;
    margin-bottom: 5px;
}

input {
    width: 100%;
    padding: 10px;
    font-size: 16px;
    border: 1px solid #ccc;
    border-radius: 5px;
}
