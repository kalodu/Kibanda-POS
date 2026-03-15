# Contributing to KibandaPOS

<p align="center">
<strong><a href="#setup">Setup</a></strong> |
<strong><a href="#running-tests">Running Tests</a></strong> |
<strong><a href="#writing-tests">Writing Tests</a></strong> |
<strong><a href="#debugging-code">Debugging</a></strong> |
<strong><a href="#internals">Internals</a></strong> |
<strong><a href="#code-of-conduct">Code of Conduct</a></strong>
</p>

---

## Setup

1. Fork & clone the repository:

```bash
git clone https://github.com/<your-username>/KibandaPOS
cd KibandaPOS
```

2. Install dependencies:

```bash
npm install
```

3. Run the development server:

```bash
npm run dev
```

## Running Tests

```bash
# Run all tests
npm test

# Run a specific test file
npm test -- --testPathPattern=testname
```

## Writing Tests

Place tests in tests/ folder with test_<module>.py naming.

Example:

```javascript
function test_login(client) {
    response = client.post("/login", data={"username": "user", "password": "pass"});
    assert response.status_code === 200;
}
```

## Debugging Code

Use browser developer tools or VS Code debugging.

## Internals

- App.jsx – React entry point
- context/AppContext.jsx – State management
- pages/ – Page components
- components/ – Reusable components

## Creating a New Feature

1. Fork repository & create a branch.
2. Implement your changes.
3. Add tests.
4. Ensure all tests pass.
5. Submit a pull request describing your feature.

## Code of Conduct

Be respectful, welcoming, and constructive.

No harassment, personal attacks, or sharing private info.

Maintain professionalism in all interactions.

Enforcement Contact: mwakidenice@gmail.com
