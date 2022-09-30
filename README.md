# nouvionp-proton-templates

## Templates

### open-api-support-testing

This is a set of templates used to test the AWS Proton console support for Open API.

#### TAR and Upload

Example:

```
cd open-api-support-testing/environments
ada credentials update --provider=isengard --profile=default --account=$AWS_ACCOUNT_ID --role=Admin --once
```

After saving/committing changes:

```
tar -zcvf open-api-strings-env-template.tar.gz v1
aws s3 cp open-api-strings-env-template.tar.gz s3://$AWS_BUCKET/
```

```
tar -zcvf open-api-integers-env-template.tar.gz v1
aws s3 cp open-api-integers-env-template.tar.gz s3://$AWS_BUCKET/
```

```
tar -zcvf open-api-numbers-env-template.tar.gz v1
aws s3 cp open-api-numbers-env-template.tar.gz s3://$AWS_BUCKET/
```
