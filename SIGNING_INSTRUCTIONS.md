1. Install (if you don't have) Keybase (https://keybase.io/) and set up your identity
2. Join `freeai` group - either with Keybase UI or using command
```
keybase team request-access freeai
```
3. Perform the following commands:
```
git clone keybase://team/freeai/freeai-manifesto
cd freeai-manifesto
keybase pgp sign -c -i the_freeai_manifesto.txt -o signatures/`keybase status | grep 'Username:' | awk '{print $2}'`
git add .
git commit -m "Signed by `keybase status | grep 'Username:' | awk '{print $2}'`"
git push
```

Done, you have signed The #FreeAI Manifesto!
