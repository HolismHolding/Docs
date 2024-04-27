# Create a project

- `sudo mkdir /ProjectName`
- `sudo chmod 777 /ProjectName`
- `cd /ProjectName`
- `mkdir ApiOrPanelOrSite`
    - API = `AdminApi` or `SiteApi` or `AreaApi`
    - Panel = `AdminPanel` or `ClientPanel` or `AreaPanel`
    - Site = `SiteQwik` or `SiteNext`
        - `SiteQwik` uses [Qwik from Builder.io](https://qwik.builder.io)
        - `SiteNext` uses [Next.js from Vercel](https://nextjs.org)
- Go inside the API or Panel or Site directory
- Run `Start`

If the default domain is not suitable for you, then

- Go to `/ProjectName/ApiOrPanelOrSiteDirectory`
- `micro Host`
- Write your custom domain
    - It should end with `.local`
