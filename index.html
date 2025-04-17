<?php
// Get 'question' from the URL parameter
$question = isset($_GET['question']) ? $_GET['question'] : null;

if ($question) {
    // Set up the data to send in the POST request
    $data = [
        "contents" => [
            [
                "role" => "user",
                "parts" => [
                    ["text" => $question]
                ]
            ]
        ]
    ];

    // Initialize a cURL session
    $ch = curl_init();

    // Set the API URL with your actual API key
    $api_key = "AIzaSyAVQzttzQt1JkVSDQQ_zWMqhhMNq9kaECU"; // Replace with your actual API key
    $url = "https://generativelanguage.googleapis.com/v1/models/gemini-pro:generateContent?key=" . $api_key;

    // Set cURL options for the POST request
    curl_setopt($ch, CURLOPT_URL, $url);
    curl_setopt($ch, CURLOPT_POST, true);
    curl_setopt($ch, CURLOPT_HTTPHEADER, ["Content-Type: application/json"]);
    curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
    curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode($data));

    // Execute the cURL request and get the response
    $response = curl_exec($ch);

    // Close the cURL session
    curl_close($ch);

    // Decode the response
    $response_data = json_decode($response, true);

    // Prepare the JSON output
    if (isset($response_data['candidates'][0]['content']['parts'][0]['text'])) {
        $text = $response_data['candidates'][0]['content']['parts'][0]['text'];
        $output = [
            "status" => "true",
            "answer" => $text,
            "credit" => "t.me/BjsWorks"
        ];
    } else {
        $output = [
            "status" => "false",
            "answer" => "Unable to generate response.",
            "credit" => "t.me/BjsWorks"
        ];
    }
} else {
    $output = [
        "status" => "false",
        "answer" => "No 'question' provided.",
        "credit" => "t.me/BjsWorks"
    ];
}

// Output the result in JSON format
header('Content-Type: application/json');
echo json_encode($output);
