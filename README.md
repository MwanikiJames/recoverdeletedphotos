<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Picture Recovery Magic Wand</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/feather-icons"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#3B82F6', // Blue as primary color
                        secondary: '#10B981', // Green as secondary color
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-gray-100">
    <div class="min-h-screen flex flex-col items-center justify-center p-4">
        <div class="bg-white shadow-lg rounded-lg p-8 max-w-md w-full text-center">
            <i data-feather="camera" class="w-16 h-16 text-primary mx-auto"></i>
            <h1 class="text-3xl font-bold mt-4 text-gray-800">Recover Deleted Pictures</h1>
            <p class="mt-2 text-gray-600">Use our magic wand to recover your precious memories.</p>
            <div class="mt-6">
                <input type="file" class="hidden" id="fileInput">
                <label for="fileInput" class="cursor-pointer inline-flex items-center justify-center px-6 py-3 border border-transparent text-base font-medium rounded-md text-white bg-primary hover:bg-primary-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-primary">
                    <i data-feather="upload" class="w-5 h-5 mr-2"></i>
                    Upload Phone Backup
                </label>
            </div>
            <div class="mt-6">
                <button class="inline-flex items-center justify-center px-6 py-3 border border-transparent text-base font-medium rounded-md text-white bg-secondary hover:bg-secondary-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-secondary">
                    <i data-feather="wand" class="w-5 h-5 mr-2"></i>
                    Start Recovery
                </button>
            </div>
            <div class="mt-6 text-sm text-gray-500">
                <p>Note: This tool works best with recent backups.</p>
            </div>
        </div>
    </div>
    <script>
        feather.replace();
    </script>
</body>
</html>
