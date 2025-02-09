# Unhandled JSON Decoding Exception in Dart HTTP Request

This repository demonstrates a common error in Dart code that handles HTTP requests and JSON responses. The `bug.dart` file contains code that fetches data from an API but fails to explicitly handle `FormatException` during JSON decoding.  The `bugSolution.dart` file provides a corrected version with improved error handling.

## Bug
The original code lacks robust error handling, specifically for `FormatException` when the JSON response is malformed.

## Solution
The solution adds a more specific `catch` block to handle `FormatException` separately. This allows for more informative error messages and better recovery strategies.