# Kingshot Vikings Reinforcement Calculator

Enter your march size, number of marches, bonuses (pet, City Deployment Buff,
castle) and troop counts. The page shows how to fill each reinforcement march
and whether all your infantry can go out.

## Running it

Live at **https://somebodyelsegaming.github.io/ks-vikings-calc/**

One file, `index.html`, with no build step, no backend and no outside links.
Opening it straight from disk works.

## The math

```
march size  = (size of march + pet + castle) × (1 + City Deployment Buff %)
total room  = march size × number of marches
head room   = total room − all infantry and cavalry
```

Each march is filled in order: all infantry first, then cavalry, then archers
in whatever room is left. Each type is capped so a march never goes over its
size. If total infantry is more than the total room, the page says how many
infantry are left behind.

## Credits

Built by Somebody Else, the gnome you know.
