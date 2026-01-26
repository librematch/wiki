# Polling

The polling stage checks for updated data frequently. [huey](https://huey.readthedocs.io/en/latest/) as a task scheduler/queue takes over triggering our polling jobs.
Data queried from the authenticated endpoints get a separate job.
These endpoints need special treatment, as in only query what's essential.
