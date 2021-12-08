## S3 bucket pillaging
#### Brute force bucket names
- https://github.com/initstring/cloud_enum
```
python3 cloud_enum.py -k <KEYWORD>
```

#### Use the AWS CLI to list the files of the s3 bucket
```
sudo aws s3 ls s3://<BUCKET> --profile <PROFILE>
```

#### Use the AWS CLI to download the files of the s3 bucket
```
sudo aws s3 sync s3://<BUCKET> s3-files-dir --profile <PROFILE>
```

## Git secrets
- https://github.com/zricethezav/gitleaks
#### Search for secrets
```
./gitleaks detect -v source ~/tools/gitleaks/
```

#### Use web browser to view the commit
```
https://github.com/[git account]/[repo name]/commit/[commit ID]
```
