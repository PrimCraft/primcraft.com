# primcraft.com

Static Jekyll site for PrimCraft

## Deployment

The site is deployed automatically on push to `master`:

1. Jekyll builds the site
2. Output is synced to S3
3. CloudFront cache is invalidated

## Setup

Add the following to the GitHub repository:

**Secrets:**
- `AWS_ROLE_ARN`: IAM role ARN for deployer

**Variables:**
- `CLOUDFRONT_DISTRIBUTION_ID`: CloudFront distribution ID

## Local Development

```bash
bundle install
bundle exec jekyll serve
```

Site will be available at http://localhost:4000
