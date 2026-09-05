# Getting a Subdomain

## Fully automatic registration

You do **not** need to fork the repository, create files manually, make a Pull Request, or wait for approval.

1. Open a **Subdomain request** issue.
2. Enter the subdomain you want, for example `alex`.
3. Enter your HTTPS GitHub Pages address, for example `alex.github.io`.
4. Submit the issue.

GitHub Actions will automatically:

- validate the subdomain name;
- reject reserved names;
- verify that the target is an HTTPS `*.github.io` address;
- check whether the subdomain is already registered;
- create `domains/<subdomain>.json`;
- commit the registration to the repository;
- post the final `https://<subdomain>.visitme.qzz.io` link in the issue;
- close the issue automatically.

No manual file creation or Pull Request is required.

## Example

Request:

```text
Subdomain: alex
GitHub Pages URL: alex.github.io
```

The system automatically creates:

```text
domains/alex.json
```

with the target and publishes the resulting address:

```text
https://alex.visitme.qzz.io
```

## Rules

Read `POLICY.md` before submitting a request.
