1. Install (if you don't have) Keybase from https://keybase.io/. Press Create an account and follow the on screen instructions to create your identity
2. If you don't have PGP at your Keybase, press Prove your identities -> Create PGP key and follow instructions to set up your own key
3. Join `freeai` group - either with Keybase UI or using command
```
keybase team request-access freeai
```
4. Perform the following commands:
```
git clone keybase://team/freeai/freeai-manifesto
cd freeai-manifesto
keybase pgp sign -c -i the_freeai_manifesto.txt -o signatures/`keybase status | grep 'Username:' | awk '{print $2}'`
git add .
git commit -m "Signed by `keybase status | grep 'Username:' | awk '{print $2}'`"
git push
```

Done, you have signed The #FreeAI Manifesto!
