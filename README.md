# Unhandled Exception During JSON Decoding in Dart

This repository demonstrates a common error in Dart: neglecting to handle potential exceptions when decoding JSON responses from an API.  The `bug.dart` file shows the flawed code, while `bugSolution.dart` provides a corrected version that gracefully handles potential `FormatException` errors during JSON decoding.  This is crucial for robust error handling in asynchronous operations.

**Problem:** The original code fails to explicitly catch the `FormatException` that can occur if the server returns malformed JSON. This leads to unexpected crashes or app instability.

**Solution:** The corrected code includes a `try-catch` block specifically to handle the `FormatException`, providing a more user-friendly error message and preventing app crashes.