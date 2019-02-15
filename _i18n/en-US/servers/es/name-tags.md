Rather than writing a long and messy description right next to your name, we designed a short scheme to capture and display the basic player info. It follows the format of `<[Position1][Position2]Position3> ChatContent`, and here is a list of labels and colors that can be applied to each position.

| Label        | Posotion | Color                                     | Meaning                                     |
|--------------|----------|-------------------------------------------|---------------------------------------------|
| [M]          | 1        | <span class ="minecraft-text-2">§2</span> | MainWorld / OverWorld                       |
| [N]          | 1        | <span class ="minecraft-text-c">§c</span> | Nether                                      |
| [E]          | 1        | <span class ="minecraft-text-e">§e</span> | The End                                     |
| [R]          | 1        | <span class ="minecraft-text-a">§a</span> | Resource World                              |
| [#]          | 1        | <span class ="minecraft-text-9">§9</span> | Discord (Not in game)                       |
| [Admin]      | 2        | <span class ="minecraft-text-c">§c</span> | Admin, label text may be customized         |
| [Builder]    | 2        | <span class ="minecraft-text-e">§e</span> | Builder, label text may be customized       |
| [Mod]        | 2        | <span class ="minecraft-text-6">§6</span> | Moderator, label text may be customized     |
|              | 2        | <span class ="minecraft-text-b">§b</span> | Sponsor, label text may be customized       |
| [Player]     | 2        | <span class ="minecraft-text-a">§a</span> | Player                                      |
| [Unverified] | 2        | <span class ="minecraft-text-a">§9</span> | Unverified Discord user                     |
|              | 3        | <span class ="minecraft-text-b">§b</span> | Admin Team, label text is the player's name |
|              | 3        | <span class ="minecraft-text-6">§6</span> | Builders, label text is the player's name   |
|              | 3        | <span class ="minecraft-text-2">§2</span> | Players, label text is the player's name    |
|              | 3        | <span class ="minecraft-text-3">§3</span> | Discord users                               |

Simply speaking, position1 is the abbreviation of the world the player located, position2 is the player's permission group, and position3 is the player's role.


## Examples
### General usage
<ul class="bg-dark list-unstyled minecraft-text p-1">
    <li>&lt;<span class ="minecraft-text-2">[M]</span><span class ="minecraft-text-c">[Admin]</span><span class ="minecraft-text-b">Soniji</span>&gt; Meow</li>
    <li>&lt;<span class ="minecraft-text-c">[N]</span><span class ="minecraft-text-6">[Mod]</span><span class ="minecraft-text-b">Whitebai_</span>&gt; Hi</li>
    <li>&lt;<span class ="minecraft-text-e">[E]</span><span class ="minecraft-text-a">[Player]</span><span class ="minecraft-text-2">Dinnerbone</span>&gt; 🙃</li>
    <li>&lt;<span class ="minecraft-text-a">[R]</span><span class ="minecraft-text-e">[Builder]</span><span class ="minecraft-text-6">bk_owenk</span>&gt; Build!</li>
    <li><span class ="minecraft-text-7">&lt;<span class ="minecraft-text-9">[#]</span><span class ="minecraft-text-8">[Unverified]</span><span class ="minecraft-text-3">some one</span>&gt; SPAM! I mean musubi..</span></li>
    <li>&lt;<span class ="minecraft-text-9">[#]</span><span class ="minecraft-text-c">[Admin]</span><span class ="minecraft-text-3">Soniji</span>&gt; hmm...</li>
</ul>
A line by line explanation of the chat messages above:
- An admin called Soniji meowed in the over world.
- Moderator Whitebai_ said Hi in the nether.
- Player Dinnerbone posted a upside-down face in the end.
- Builder bk_owenk said Build! in the resource world.
- A Discord user whoes account has not been linked to their minecraft account said "SPAM! I mean musubi.." from Discord
- Admin Soniji said hmm... from Discord

### Multiple Roles
It is possible for a player to have multiple groups/roles in this server. In this case, the labeling process follows the rules below:
- Admin Team always displays a cyan (<span class ="minecraft-text-b">§b</span>) player name (position 3).
- No role other than Builders can have a bule (<span class ="minecraft-text-9">§9</span>) player name (position 3).
- Players always display a green (<span class ="minecraft-text-2">§2</span>) player name (position 3).
- Admin Team never displays the sponsor cyan color (<span class ="minecraft-text-b">§b</span>) at position 2.
- When a player is both a builder and a moderator, position 2 displays the player as a builder.
- When a player is both a builder and an admin, position 2 displays the player as an admin (Admin already has the permission of a builder).

More examples!:
<ul class="bg-dark list-unstyled minecraft-text p-1">
    <li>&lt;<span class ="minecraft-text-2">[M]</span><span class ="minecraft-text-3">[Builder]</span><span class ="minecraft-text-b">Soniji</span>&gt; Builder and Mod</li>
    <li>&lt;<span class ="minecraft-text-e">[E]</span><span class ="minecraft-text-3">[I Am Cat]</span><span class ="minecraft-text-b">Soniji</span>&gt; Customized Builder and Mod</li>
    <li>&lt;<span class ="minecraft-text-e">[E]</span><span class ="minecraft-text-6">[I Am Cat]</span><span class ="minecraft-text-b">Soniji</span>&gt; Customized Mod</li>
    <li>&lt;<span class ="minecraft-text-c">[N]</span><span class ="minecraft-text-b">[Player]</span><span class ="minecraft-text-2">Soniji</span>&gt; Sponser</li>
    <li>&lt;<span class ="minecraft-text-a">[R]</span><span class ="minecraft-text-b">[I am Cat]</span><span class ="minecraft-text-2">Soniji</span>&gt; Customized Sponser</li>
    <li>&lt;<span class ="minecraft-text-2">[M]</span><span class ="minecraft-text-b">[Builder]</span><span class ="minecraft-text-6">Soniji</span>&gt; Builder and Sponser</li>
    <li>&lt;<span class ="minecraft-text-2">[M]</span><span class ="minecraft-text-b">[I am Cat]</span><span class ="minecraft-text-6">Soniji</span>&gt; Customized Builder and Sponser</li>
</ul>
The corresponding groups/roles are:
- Builder and moderator
- Builder, moderator, and sponsor (because only sponsors can customize their label)
- Moderator and sponsor (because only sponsors can customize their label)
- Sponsor and player
- Sponsor and player
- Sponsor and builder
- Sponsor and builder
