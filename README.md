# solidus-s3

This repository maps to the AWS bucket named io.flow.solidus-s3 -
providing versioning over the assets available in s3.

# Install the aws cli

http://docs.aws.amazon.com/cli/latest/userguide/installing.html#install-with-pip

    curl https://bootstrap.pypa.io/get-pip.py  > get-pip.py
    sudo -H python get-pip.py
    sudo -H pip install --ignore-installed awscli

    aws configure

# Upload files

    aws s3 sync assets s3://io.flow.solidus-s3/assets --grants read=uri=http://acs.amazonaws.com/groups/global/AllUsers

# Example URL

    https://s3.amazonaws.com/io.flow.solidus-s3/assets/images/logo.png
