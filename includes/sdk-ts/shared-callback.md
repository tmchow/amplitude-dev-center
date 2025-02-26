All asynchronous API are optionally awaitable through a Promise interface. This also serves as callback interface.

=== "Promise"

    ```ts
    amplitude.track('Button Clicked').promise.then(function(result) {
      result.event; // {...} (The final event object sent to Amplitude)
      result.code; // 200 (The HTTP response status code of the request.
      result.message; // "Event tracked successfully" (The response message)
    });
    ```

=== "async/await"

    ```ts
    // Using async/await
    const results = await amplitude.track('Button Clicked').promise;
    result.event; // {...} (The final event object sent to Amplitude)
    result.code; // 200 (The HTTP response status code of the request.
    result.message; // "Event tracked successfully" (The response message)
    ```
