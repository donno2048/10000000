# 10000000

This is the script used to create this repo:

```bash
mkdir 10000000
cd 10000000/
git init
python3 -c "for i in range(10000000):print((\"blob\nmark :1\ndata 1\n\" * (not i)) + f'\ncommit refs/heads/master\nmark :{i + 2}\nauthor donno2048 <just4now666666@gmail.com> 0 +0000\ncommitter donno2048 <just4now666666@gmail.com> 0 +0000\ndata 1\n\n{\"from\" if i else \"M 100644\"} :{i + 1}{\" a\" * (not i)}')" | git fast-import
git remote add origin https://github.com/donno2048/10000000.git
git push origin master
```
