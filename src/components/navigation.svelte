<script>
    import {
        List,
        ListItem
    } from 'framework7-svelte'

    let navigationItems = [
        {
            link:"#",
            header:"Nouveautés",
            title:"iOS 15",
            footer:"11 astuces",
            imgUrl:"https://touch1.hhi.co.kr/deploy/resources/images/content/ios-logo1.png",
        },
        {
            link:"#",
            header:"Bienvenue sur l'iPhone",
            title:"Faire connaissance avec l'iPhone",
            footer:"9 astuces",
            imgUrl:"https://support.apple.com/library/content/dam/edam/applecare/images/fr_FR/iOS/ios13-iphone-xs-iphone-disabled-passcode.jpg",
        },
        {
            link:"#",
            header:"Indispensables",
            title:"Des fonctionnalités à découvrir absolument et que vous adorerez",
            footer:"10 astuces",
            imgUrl:"https://cdn.framework7.io/placeholder/people-160x160-2.jpg",
        },
    ]
    
</script>

<List>
    {#each navigationItems as {link, header, title, footer, imgUrl}}
    <ListItem link="{link}" header="{header}" title="{title}" footer="{footer}">
      <img alt="" slot="media" src="{imgUrl}" width="80" />
    </ListItem>
    {/each}
</List>