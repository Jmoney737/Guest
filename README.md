<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smartphone-Friendly Routine Dashboard</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
        }
        header {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 1rem 0;
        }
        .dashboard-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 1rem;
        }
        .card {
            background-color: white;
            border: 1px solid #ddd;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 300px;
            padding: 1rem;
            text-align: center;
        }
        .card h3 {
            margin: 0.5rem 0;
            color: #333;
        }
        .button-group {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 1rem;
        }
        .button-group button {
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 10px 15px;
            font-size: 1rem;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .button-group button:hover {
            background-color: #45a049;
        }
        footer {
            text-align: center;
            padding: 1rem;
            background-color: #4CAF50;
            color: white;
            margin-top: 2rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>Routine Dashboard</h1>
        <p>Quickly activate your routines below</p>
    </header>

    <div class="dashboard-container">
        <!-- Kitchen Group -->
        <div class="card">
            <h3>Kitchen Group</h3>
            <div class="button-group">
                <button onclick="triggerRoutine('https://www.virtualsmarthome.xyz/url_routine_trigger/activate.php?trigger=5846a7ff-8452-4c2f-81c7-65792b5cfbcb&token=57d238c9-34e8-4bdd-9bd8-76f34bbeb544&response=html')">On</button>
                <button onclick="triggerRoutine('https://www.virtualsmarthome.xyz/url_routine_trigger/activate.php?trigger=f909cd87-e74a-4c94-bf0a-91d88c567111&token=5405bd16-657c-487b-a635-5422deae8015&response=html')">Off</button>
            </div>
        </div>

        <!-- Living Room Group -->
        <div class="card">
            <h3>Living Room Group</h3>
            <div class="button-group">
                <button onclick="triggerRoutine('https://www.virtualsmarthome.xyz/url_routine_trigger/activate.php?trigger=39168a11-14c6-4bfb-8504-a73578a37555&token=a2b9357b-2a6a-4277-b2ac-3fe59fc0a80e&response=html')">On</button>
                <button onclick="triggerRoutine('https://www.virtualsmarthome.xyz/url_routine_trigger/activate.php?trigger=1f805a37-03bd-404d-b781-0d7c4f8a051c&token=f34fc986-2182-4d80-816e-4cb08e3f7578&response=html')">Off</button>
            </div>
        </div>

        <!-- NFC 1 - Living Room On -->
        <div class="card">
            <h3>NFC 1 - Living Room</h3>
            <div class="button-group">
                <button onclick="triggerRoutine('https://www.virtualsmarthome.xyz/url_routine_trigger/activate.php?trigger=43a345bd-7137-4efb-bcf3-d1138b11652f&token=48d2e3a7-60af-4973-b63e-3a183df4b9e8&response=html')">On</button>
            </div>
        </div>

        <!-- Office Group -->
        <div class="card">
            <h3>Office Group</h3>
            <div class="button-group">
                <button onclick="triggerRoutine('https://www.virtualsmarthome.xyz/url_routine_trigger/activate.php?trigger=747403c7-9a9f-4a47-9a80-0f6923b5c4d0&token=50f5e41a-50c5-4802-9d4f-a673d38c2491&response=html')">On</button>
                <button onclick="triggerRoutine('https://www.virtualsmarthome.xyz/url_routine_trigger/activate.php?trigger=e458094d-4c7a-42b8-8d7c-61b0bcaca741&token=1549d5d9-19ef-4a9c-bb1f-9a2f055e6a82&response=html')">Off</button>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 Routine Dashboard</p>
    </footer>

    <script>
        function triggerRoutine(url) {
            alert("Triggering routine...");
            fetch(url)
                .then(response => {
                    if (response.ok) {
                        alert("Routine triggered successfully!");
                    } else {
                        alert("Failed to trigger routine.");
                    }
                })
                .catch(error => {
                    alert("Error triggering routine. Please check your connection.");
                });
        }
    </script>
</body>
</html>
