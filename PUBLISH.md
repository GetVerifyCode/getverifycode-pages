# Publish getverifycode.pages.dev

Static site for pack item #4. Different content from github.io (OTP delivery playbook, not the checklist).

## Deploy

```bash
cd _backlink-assets/getverifycode-pages
CLOUDFLARE_ACCOUNT_ID=fc8aa53945db3e466b0fce0758eccfac \
  npx wrangler@4 pages deploy . --project-name=getverifycode --commit-dirty=true
```

Project already exists on Sajeel's Cloudflare account (`fc8aa539…`). Live URL: https://getverifycode.pages.dev/

## Verify

1. HTTP 200 on https://getverifycode.pages.dev/
2. View Source: links to https://getverifycode.com/ must not have `rel="nofollow"`
