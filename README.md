# pris.ly - Prisma's url shortener

## Adding a short link

To create the shortened url: `http://pris.ly/internet` pointing to `https://tools.ietf.org/html/rfc3271`

1. Open `vercel.json`
2. Add the following object for a redirect:

```
{
  source: '/internet',
  destination: 'https://tools.ietf.org/html/rfc3271'
}
```

> The location shouldn't really matter as long as the first part, i.e. `/internet` is unique.

For more information on Vercel redirects: https://vercel.com/docs/project-configuration#project-configuration/redirects

## Automatic deployment

:warning: The person opening a PR needs to be added to the project. If not added nothing will be deployed after merging.

After merging the PR or after a commit on the main branch, the Vercel deployment will start automatically and will only take a few seconds (~10 seconds) until it's live.
Vercel URL: https://pris-ly.vercel.app/
