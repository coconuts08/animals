<?php

use Fieg\Bayes\Classifier;
use Fieg\Bayes\Tokenizer\WhitespaceAndPunctuationTokenizer;

class animalClassifier {
    private $tokenizer;
    private $classifier;

    public function __construct() {
        include './vendor/autoload.php';

        $this->tokenizer = new WhitespaceAndPunctuationTokenizer();
        $this->classifier = new Classifier($this->tokenizer);

        // Training data...
        $this->trainData();
    }

    private function trainData() {
        $this->classifier->train('Land animals', 'dog');
        $this->classifier->train('Land animals', 'cat');
        $this->classifier->train('Land animals', 'rat');
        $this->classifier->train('Land animals', 'lion');
        $this->classifier->train('Land animals', 'koala');
        $this->classifier->train('Land animals', 'monkey');
        $this->classifier->train('Land animals', 'brown bear');
        $this->classifier->train('Land animals', 'tiger');
        $this->classifier->train('Land animals', 'horse');
        $this->classifier->train('marine', 'whale');
        $this->classifier->train('marine', 'seahorse');
        $this->classifier->train('marine', 'tiger shark');
        $this->classifier->train('marine', 'octopus');
        $this->classifier->train('marine', 'squid');
        $this->classifier->train('marine', 'dolphin');
        $this->classifier->train('marine', 'tuna');
        $this->classifier->train('marine', 'salmon');
        $this->classifier->train('marine', 'sea urchin');
        $this->classifier->train('marine', 'orca');
        $this->classifier->train('marine', 'sperm whale');
        $this->classifier->train('marine', 'sea lion');
        $this->classifier->train('marine', 'jellyfish');
        $this->classifier->train('marine', 'stingray');
        $this->classifier->train('marine', 'megalodon');
        $this->classifier->train('marine', 'shrimp');
        $this->classifier->train('flying', 'falcon');
        $this->classifier->train('flying', 'eagle');
        $this->classifier->train('flying', 'bats');
        $this->classifier->train('flying', 'owl');
        $this->classifier->train('flying', 'dove');
        $this->classifier->train('flying', 'sparrow');
        $this->classifier->train('flying', 'tucan');
        $this->classifier->train('flying', 'pigeon');
        $this->classifier->train('flying', 'swallow');
        $this->classifier->train('flying', 'wasp');
        $this->classifier->train('flying', 'butterfly');
        
    }

    public function classifyAnimal($animalQuery) {
        $result = $this->classifier->classify($animalQuery);

        // Find the category with the optimal score
        $optimalCategory = '';
        $optimalScore = -INF; // Initialize with negative infinity

        foreach ($result as $category => $score) {
            if ($score > $optimalScore) {
                $optimalScore = $score;
                $optimalCategory = $category;
            }
        }

        // Return the optimal category with its score
        return [
            'animal_query' => $animalQuery,
            'optimal_category' => $optimalCategory,
            'optimal_score' => $optimalScore
        ];
    }
}

// Initialize animal classifier
$animalClassifier = new animalClassifier();

// Process the form submission
if ($_SERVER["REQUEST_METHOD"] == "POST" && isset($_POST["animal_query"])) {
    $result = $animalClassifier->classifyAnimal($_POST["animal_query"]);

    // Output the classification result
    echo "<hr>animal query: " . $result['animal_query'] . "<br>";
    echo "optimal Category: " . $result['optimal_category'] . " with Score: " . $result['optimal_score'];
} elseif ($_SERVER["REQUEST_METHOD"] == "POST") {
    // If no animal query is provided, display an error message
    echo "<hr>Please provide a animal query.";
}
?>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>animal Classifier</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-image: url(cheetah.jpg);
            margin: 0;
            padding: 0;
        }
        
        .container {
            max-width: 600px;
            margin: 50px auto;
            padding: 20px;
            background-color: green;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        
        h2 {
            text-align: center;
            color: #333;
        }
        
        form {
            text-align: center;
        }
        
        label {
            font-weight: bold;
        }
        
        input[type="text"] {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid black;
            border-radius: 4px;
            box-sizing: border-box;
            background-color: #5c5346;
        }
        
        input[type="submit"] {
            background-color: #5c5346;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        
        input[type="submit"]:hover {
            background-color: #cba328;
        }

        .result {
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>animal categorizer</h2>
        <form action="<?php echo htmlspecialchars($_SERVER["PHP_SELF"]); ?>" method="post">
            <label for="animal_query">Enter your animal:</label><br>
            <input type="text" id="animal_query" name="animal_query"><br><br>
            <input type="submit" value="Categorize">
        </form>

        <?php
        if ($_SERVER["REQUEST_METHOD"] == "POST" && isset($_POST["animal_query"])) {
            // Output the classification result
            echo "<div class='result'>";
            $result = $animalClassifier->classifyAnimal($_POST["animal_query"]);
            echo "<hr>animal query: " . $result['animal_query'] . "<br>";
            echo "optimal Category: " . $result['optimal_category'] . " with Score: " . $result['optimal_score'];
            echo "</div>";
        }
        ?>
    </div>
</body>
</html>
