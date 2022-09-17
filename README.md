
# build
kubectl crossplane build configuration

# login
aws ecr-public get-login-password --region us-east-1 | docker login --username AWS --password-stdin public.ecr.aws

# Push
kubectl crossplane push configuration $REGISTRY/$PACKAGE:$VERSION
