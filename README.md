<!DOCTYPE html>
<html>
<head>
    <title>Quiz</title>
    <script>
    function result() {
        var ques = [
            { name: 'capital', correctAnswer: 'Hyderabad' },
            { name: 'language', correctAnswer: 'Telugu' },
            { name: 'river', correctAnswer: 'Godavari' },
            { name: 'bird', correctAnswer: 'Indian Roller' },
            { name: 'flower', correctAnswer: 'Tangidi Puvvu' },
            { name: 'chiefminister', correctAnswer: 'K. Chandrashekar Rao' },
            { name: 'stateanimal', correctAnswer: 'Deer' },
            { name: 'stateflower', correctAnswer: 'Tangidi Puvvu' },
            { name: 'statetree', correctAnswer: 'Jammi Chettu' },
            { name: 'nickname', correctAnswer: 'The Pearl City' }
        ];
        for (var i = 0; i < ques.length; i++) {
            var ele = document.getElementsByName(ques[i].name);
            var resultDiv = document.getElementById(ques[i].name + "_res");
            var answered = false;
            for (var j = 0; j < ele.length; j++) {
                if (ele[j].checked) {
                    answered = true;
                    if (ele[j].value === ques[i].correctAnswer) {
                        resultDiv.innerHTML = "<span style='color: green;'>Correct</span>";
                    } else {
                        resultDiv.innerHTML = "<span style='color: red;'>Incorrect</span>";
                    }
                    break;
                }
            }
            if (!answered) {
                resultDiv.innerHTML = "<span style='color: red;'>Not Attempted</span>";
            }
        }
    }
    </script>
</head>
<body>
    <center>Welcome to the Telangana Quiz</center>
    <center>All questions carry equal marks</center>
    <p>1. What is the capital of Telangana?</p>
    <input type="radio" name="capital" value="Hyderabad">Hyderabad<br>
    <input type="radio" name="capital" value="Mumbai">Mumbai<br>
    <input type="radio" name="capital" value="Bangalore">Bangalore<br>
    <input type="radio" name="capital" value="Delhi">Delhi<br>
    <div id="capital_res"></div>
    
    <p>2. What is the official language of Telangana?</p>
    <input type="radio" name="language" value="Telugu">Telugu<br>
    <input type="radio" name="language" value="Hindi">Hindi<br>
    <input type="radio" name="language" value="English">English<br>
    <input type="radio" name="language" value="Kannada">Kannada<br>
    <div id="language_res"></div>
    
    <p>3. Which river flows through Telangana?</p>
    <input type="radio" name="river" value="Godavari">Godavari<br>
    <input type="radio" name="river" value="Krishna">Krishna<br>
    <input type="radio" name="river" value="Yamuna">Yamuna<br>
    <input type="radio" name="river" value="Ganges">Ganges<br>
    <div id="river_res"></div>
    
    <p>4. What is the state bird of Telangana?</p>
    <input type="radio" name="bird" value="Indian Roller">Indian Roller<br>
    <input type="radio" name="bird" value="Peacock">Peacock<br>
    <input type="radio" name="bird" value="Sparrow">Sparrow<br>
    <input type="radio" name="bird" value="Pigeon">Pigeon<br>
    <div id="bird_res"></div>
    
    <p>5. What is the state flower of Telangana?</p>
    <input type="radio" name="flower" value="Tangidi Puvvu">Tangidi Puvvu<br>
    <input type="radio" name="flower" value="Jasmine">Jasmine<br>
    <input type="radio" name="flower" value="Rose">Rose<br>
    <input type="radio" name="flower" value="Sunflower">Sunflower<br>
    <div id="flower_res"></div>
    
    <p>6. Who is the Chief Minister of Telangana?</p>
    <input type="radio" name="chiefminister" value="K. Chandrashekar Rao">K. Chandrashekar Rao<br>
    <input type="radio" name="chiefminister" value="N. Chandrababu Naidu">N. Chandrababu Naidu<br>
    <input type="radio" name="chiefminister" value="P. V. Narasimha Rao">P. V. Narasimha Rao<br>
    <input type="radio" name="chiefminister" value="Y. S. Jagan Mohan Reddy">Y. S. Jagan Mohan Reddy<br>
    <div id="chiefminister_res"></div>
    
    <p>7. What is the state animal of Telangana?</p>
    <input type="radio" name="stateanimal" value="Deer">Deer<br>
    <input type="radio" name="stateanimal" value="Tiger">Tiger<br>
    <input type="radio" name="stateanimal" value="Elephant">Elephant<br>
    <input type="radio" name="stateanimal" value="Lion">Lion<br>
    <div id="stateanimal_res"></div>
    
    <p>8. What is the state flower of Telangana?</p>
    <input type="radio" name="stateflower" value="Tangidi Puvvu">Tangidi Puvvu<br>
    <input type="radio" name="stateflower" value="Jasmine">Jasmine<br>
    <input type="radio" name="stateflower" value="Rose">Rose<br>
    <input type="radio" name="stateflower" value="Sunflower">Sunflower<br>
    <div id="stateflower_res"></div>
    
    <p>9. What is the state tree of Telangana?</p>
    <input type="radio" name="statetree" value="Jammi Chettu">Jammi Chettu<br>
    <input type="radio" name="statetree" value="Banyan Tree">Banyan Tree<br>
    <input type="radio" name="statetree" value="Neem Tree">Neem Tree<br>
    <input type="radio" name="statetree" value="Peepal Tree">Peepal Tree<br>
    <div id="statetree_res"></div>
    
    <p>10. What is the nickname of Hyderabad?</p>
    <input type="radio" name="nickname" value="The Pearl City">The Pearl City<br>
    <input type="radio" name="nickname" value="The Garden City">The Garden City<br>
    <input type="radio" name="nickname" value="The Pink City">The Pink City<br>
    <input type="radio" name="nickname" value="The City of Joy">The City of Joy<br>
    <div id="nickname_res"></div>

    <input type="submit" value="Submit" onclick="result()">
</body>
</html>
# Js_programs.github.io
