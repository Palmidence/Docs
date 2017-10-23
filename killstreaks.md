![](https://i.imgur.com/nXEDmpz.png)

**Killstreaks** is a module that allows you to customize the killstreaks currently enabled within the plugin.
The options that are available for you to change are the `count`, `message`, and the `commands`.

`count` specifies the amount of kills required for the customization to take effect.

>**Example:** Setting `count: 5` would give the ability to change the message once someone gets 5 kills.

`message` specifies what is displayed in chat once the killstreak is attained.

`commands` specifies what commands the server should automatically execute once a player gets the set amount of kills.

>**Example:** `commands: [ "/give @a stone_sword 1 0 {ench:[{id:19,lvl:1}]}" ]` to give everyone in the match a Knockback I stone sword when a player gets a killstreak.

---

Killstreaks are handled by the server automatically, and do not need to be individually coded for each map.

- At **5 kills**, a zombie death sound plays. `execute %killername% ~ ~ ~ playsound entity.zombie.death master @a ~ ~ ~ 3`

- At **10 kills**, an ambient wither sound plays, and a firework spawns.

- At **25 kills**, an enderdragon growl sound plays, and a firework spawns.

- At **50 kills**, a summoned wither sound plays, and a firework spawns.

- At **100 kills**, a custom orb-like sound plays, a firework spawns, and the player is banned.
