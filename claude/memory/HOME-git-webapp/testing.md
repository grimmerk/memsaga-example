---
name: testing
description: How to run webapp's tests
---
Run `npm test -- --runInBand`; parallel runs share one database and flake.
The e2e suite needs `npm run db:up` first.
