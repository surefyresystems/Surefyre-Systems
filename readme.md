tool used to create doc site: https://github.com/djacquel/WikiToJekyll

## updating docs
1. Sidebar is manually updated in \_include/sidebar.md
2. Pull \_wiki submodule to make sure it is up to date
3. `rake wikibuild`
4. sync with docs.surefyre.co s3 bucket (`aws s3 sync _site/ s3://docs.surefyre.co/ --acl public-read`)

