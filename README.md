# aws-syncroutes-auto-run
This project is intended to augment the aws syncroutes project:
https://github.com/awslabs/aws-sync-routes/releases

This project uses stepfunctions to schedule repeated calls to the syncroutes lambda.  If you only need to run it less frequently than one minute, you could just schedule that lambda directly.  This project is for running it multiple times per minute, where seconds are the RTO for routes being changes within your environment.
