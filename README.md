Repo to reproduce an issue with playwright 1.45.x

When extending the test from playwright and using it in tests the report will not have most information on it when the test fails.

Steps to reproduce
- Run `npm -i`
- Run `npx playwright test`
- Check test that is failing and is using baseTest.ts has and mostly empty trace and most steps are missing
- Check that passed test has full trace
- Check that failed test that is not using baseTest.ts, but instead using @playwright/test directly has all trace information
