# Cloud9 Setup for Prototyping

Sample script to create Cloud9 environment for rapid prototyping.

## Step-by-Step Guide

1. Open [CloudShell](https://console.aws.amazon.com/cloudshell/home)
2. Clone this repository
```bash
git clone https://github.com/aws-samples/cloud9-setup-for-prototyping
```
3. Move to the directory
```bash
cd cloud9-setup-for-prototyping
```
4. Execute the script with default parameters
```bash
./bin/bootstrap
```
5. Move to [Cloud9](https://console.aws.amazon.com/cloud9/home) and click "Open IDE".

## Cloud9 for Prototyping

- Amazon Linux 2.x on m5.large
- Change instance volume from 10GB to 128GB
- Update AWS CLI version from 1.x to 2.x
- Automatic stop time minutes is 30 min
- Disable managed credentials and attach IAM Role with AdministratorAccess policy.

To change the parameters above, modify params.json and execute `./bin/bootstrap` again.

## Destroy the environment

- Move to [Cloud9](https://console.aws.amazon.com/cloud9/home) and delete the environment
- Move to [IAM Role](https://console.aws.amazon.com/iamv2/home#/roles) and delete the role. The name of the role is same as the instance id.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.
