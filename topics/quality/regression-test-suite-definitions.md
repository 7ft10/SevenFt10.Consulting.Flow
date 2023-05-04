# Regression Test Suite Definitions

## Compile (COP)

A suite of fast-running unit and integration tests run for the purpose of fast feedback for a developer who wants to ensure that there are no regression issues introduced into existing functionality as new functionality is being built.

This suite is the primary facilitator of refactoring.

This suite typically takes 1-2 seconds to run.

## Smoke (SMK)

A suite of tests includes the Compile suite as well as a selection of slower-running tests specific to each sprint that provides coverage for functionality introduced by the sprint stories.

This suite can also include slower-running tests that are often breaking in the Build Suite.

This suite provides a developer with confidence that when their feature branch is merged into the main development branch, it will not break when integrated with changes related to other sprint stories.

The Smoke Suite runs much slower than the Compile Suite and trades speed for a broader scope.

Tests that have dependencies on changes to services whose deployments cannot be effected intra-day must not be run in the Smoke Suite. These tests should be part of the System Regression Suite.

The Smoke Suite is emptied of everything except the Compile Suite at the start of each sprint.

The Smoke Suite typically runs in a few minutes or perhaps no longer than it might take the coder to step away from their desk to stretch their legs.

## Build (CI)

A suite of tests that includes the Compile Suite and the Smoke Suite, and all other automated tests that do not have a dependency on code being deployed to a hosted environment that cannot be affected intraday (for example, NXQ, which is only deployed overnight).

The Build Suite runs slower than the Smoke Suite but has broader functional coverage.

This suite provides the end-to-end team with a level of confidence as to the correctness of their (unintegrated) software on the develop branch as feature branches are merged in. It is a scalable, fine-grained approach to determining go-live readiness.

The Smoke Suite typically takes less than 10-15min to run depending on the number of out-of-process visual and acceptance tests that run in the suite.

## System Regression (SRG)

A suite of tests that focus on asserting functionality that is only available once deployed to a hosted environment such as NXI or NXQ.

This suite provides the end-to-end team with a coarse-grained approach to determining go-live readiness through broad functional coverage.

The System Regression suite is the slowest of all suites - automated tests in this suite can typically take minutes to run after the test subjects have been deployed to a fully integrated, hosted environment. A manual System Regression test suite could take hours to complete.

## Production Verification (PVT)

A small suite of tests that focuses on asserting high-risk functionality after a release has been deployed as a high-level check to ensure the deployment has been effected correctly. These tests are run in production and, as such, should not result in the contamination of transactional data for enterprise reporting.

## Disaster Recovery (DR)

A suite of tests that focuses on asserting current release functionality after production has been switched over to a disaster recovery site. These tests are run in the new production environment in the DR site and, as such, should not result in the contamination of transactional data for enterprise reporting.
