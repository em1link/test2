<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amazon Link Redirect</title>
</head>
<body>
    <h1>Redirecting...</h1>

    <script>
        function redirect() {
            var appUrl = "com.amazon.mobile.shopping.web://amazon.de/PUMA-Fashion-Trainers-Sneakers-BLACK-PUMA/dp/B077MKHLCN/";
            var webUrl = "https://www.amazon.de/PUMA-Fashion-Trainers-Sneakers-BLACK-PUMA/dp/B077MKHLCN/";
            
            // Try to open the app
            window.location.href = appUrl;
            
            // Wait 2 seconds and then redirect to the web link
            setTimeout(function() {
                window.location.href = webUrl;
            }, 2000);
        }

        // Execute the redirect once the page is loaded
        window.onload = redirect;
    </script>
</body>
</html>
