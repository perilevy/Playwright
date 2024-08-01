# Playwright

## Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/perilevy/Playwright.git
    cd Playwright
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Install Playwright browsers:**

    ```bash
    npx playwright install
    ```

## Running the Test

1. **Run the Playwright test:**

    ```bash
    npm test
    ```

## Project Structure

- `api-test.spec.js`: Contains the Playwright test

## Instructions

1. **Open the `api-test.spec.js` file:**

2. Write a test that mocks a GET request to the API `https://jsonplaceholder.typicode.com/posts/1`.
The mock should intercept a GET request to /posts/1 and reply with a 200 status and a body containing a title of 'mocked title'.

3. In the same test, perform a GET request to https://jsonplaceholder.typicode.com/posts/1 using the http module from Playwright.

4. Check the title of the response body. It should be 'mocked title', which is the title provided by the mock.

5. Write another command that mocks a PATCH request to the API. The mock should intercept a PATCH request to /posts/1 and reply with a 200 status and a body containing a title of 'new mocked title'.  
6. In the same test, perform a PATCH request to https://jsonplaceholder.typicode.com/posts/1 using the http module from Playwright.
The request body should contain a title of 'new mocked title'.

7. Run `npm test` to see the test passes
