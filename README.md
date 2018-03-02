exampleAPI
Simple SAM API and Lambda Function template

Commands:

echo "{}" | sam local invoke ExampleFunction

sam local start-api

sam package --template-file template.yaml --s3-bucket BUCKETNAME --output-template-file packaged.yaml

sam deploy --template-file packaged.yaml --stack-name exampleAPI --capabilities CAPABILITY_IAM
