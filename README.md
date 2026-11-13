# PlayZ Sports — Free multi-sport data

## GitHub Pages
1. Create a GitHub repository.
2. Upload `index.html` to its root.
3. Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.

## Sports data source
Uses SportScore public matches API for football, cricket, basketball and tennis:
`https://sportscore.com/api/widget/matches/?sport=football&limit=50`

The provider's current documentation says its open tier requires no API key, supports CORS, is cached for 60 seconds, and allows about 10,000 requests per 24 hours per IP. A visible dofollow attribution link is included. Please recheck provider documentation/terms before publishing.

## Notes
- “All” combines the four sports currently listed by this endpoint; it does not mean every sport worldwide.
- Match coverage and live-score availability depend on the data provider.
- This is scores/fixtures only, not a video-streaming service.
- Logos display only when logo URLs are present in the API response.
- If the provider changes its JSON schema, adjust `normalize()` in `index.html`.
