# Deploying Updates to AmslerGr.id

## Quick Deploy

From the `amsler-grid-website/` directory:

```bash
git add -A
git commit -m "Your change description"
git push
```

Changes go live within 1-2 minutes at https://amslergr.id

## Verify Deployment

Check build status:
```bash
gh api repos/mullman11/amslergr.id/pages/builds --jq '.[0].status'
```

## Regenerate PDF

If you update the grid PDF:
```bash
python3 gen_pdf.py
```
Then commit and push as above.
