# serverless-poc

IAM_ROLE=VzPol-profile-NonProd-WLS-NP-I2IV-VZIAAS

SECURITY_GROUPS = 
if (AWS_REGION== "us-east-1"){
return ["sg-70da8e0e:selected","sg-0864ea77:selected","sg-8dd4bff3:selected"]
}
else {
return ["sg-95c52cee:selected","sg-c3f7d6b8:selected","sg-e6b9ca9d:selected"]
}

S3

CF_TEMPLATE=middleware/ae_install/I2IV-NP-LAMBDA.json
S3BUCKET= if (AWS_REGION== "us-east-1"){
return ["vz-app-vzw-i2iv-nonprod-actionengine-np-s3-s3bucket"]
}

