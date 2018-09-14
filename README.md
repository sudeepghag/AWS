# AWS


aws lambda add-permission \
--function-name Gradebook \
--region us-east-1 \
--statement-id gradebook-unique-id \
--action lambda:InvokeFunction \
--principal s3.amazonaws.com \
--source-arn arn:aws:s3:::sudeepghaggradebookexample \
--source-account 360492922278 \
--profile adminuser



aws lambda add-permission --function-name Gradebook --region us-east-1 --statement-id gradebook-unique-id --action lambda:InvokeFunction --principal s3.amazonaws.com --source-arn arn:aws:s3:::sudeepghaggradebookexample --source-account 360492922278 --profile adminuser


aws lambda remove-permission --function-name Gradebook --statement-id gradebook-unique-id

