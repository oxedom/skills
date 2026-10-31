# Security research

Map what the frontend reveals about the application's architecture, exposed interfaces, and security assumptions. Aim for evidence that helps someone plan an authorized security review.

## Questions to answer

- Which technologies and services does the application rely on?
- Which pages, API endpoints, and data flows are visible?
- How does the client handle sign-in, sessions, roles, and permissions?
- Does application code reveal sensitive configuration or potentially unsafe behavior?

Follow relevant request handling, storage, configuration, and permission logic. Describe endpoint methods and inputs when visible. For a potential weakness, explain the observed behavior, why it could matter, and the conditions that would need to hold for it to become a real issue.

Keep findings specific to application behavior. Generic library capabilities and security-related keywords alone are not vulnerabilities. Frontend permission checks do not establish whether equivalent checks exist on the server.

## Shape the report

Start with the architecture and exposed surface, then explain authentication and access patterns. Present potential weaknesses with supporting evidence, uncertainty, and useful next verification steps within the user's authorized scope.

Separate confirmed observations from hypotheses. Do not describe an issue as exploitable based only on a suggestive string or client-side pattern. This mode studies the downloaded material; active testing requires an appropriate user request and scope.
