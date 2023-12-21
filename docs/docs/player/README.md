# Player



## Constructor

You can access the player object with either the player class, or the [.getPlayer()](../lavalinkmanager/#.getplayer-guildid-string) function from [LavalinkManager](../lavalinkmanager/)

```javascript
const player = client.lavalink.getPlayer(guildId) || await client.lavalink.createPlayer({
    guildId: guildId,
    voiceChannelId: vcId,
    textChannelId: channelId,
    selfDeaf: true,
    selfMute: false,
    // any other options
})

```

##

## <mark style="color:red;">Import</mark>

{% tabs %}
{% tab title="TypeScript / ESM" %}
<pre class="language-javascript"><code class="lang-javascript"><strong>import { Player } from "lavalink-client";
</strong></code></pre>
{% endtab %}

{% tab title="Javascript (cjs)" %}
```javascript
const { Player } = require("lavalink-client");
```
{% endtab %}
{% endtabs %}

## <mark style="color:red;">Overview</mark>



| Properties                               | Methods              | Event Listeners |
| ---------------------------------------- | -------------------- | --------------- |
| [volume](./#.volume)                     | constructor()        |                 |
| [lavalinkVolume](./#.lavalinkvolume)     | set()                |                 |
| [position](./#.position)                 | get()                |                 |
| [lastPosition](./#.lastposition)         | clearData()          |                 |
| [createdTimeStamp](./#.createdtimestamp) | getAllData()         |                 |
| [connected](./#.connected)               | play()               |                 |
| [voice](./#.voice)                       | setVolume()          |                 |
| [guildId](./#.guildid)                   | lavaSearch()         |                 |
| [voiceChannelId](./#.voicechannelid)     | setSponsorBlock()    |                 |
| [textChannelId](./#.textchannelid)       | getSponsorBlock()    |                 |
| [playing](./#.playing)                   | deleteSponsorBlock() |                 |
| [paused](./#.paused)                     | search()             |                 |
| [repeatMode](./#.repeatmode)             | pause()              |                 |
| [ping](./#.ping)                         | resume()             |                 |
|                                          | seek()               |                 |
|                                          | setRepeatMode()      |                 |
|                                          | skip()               |                 |
|                                          | stopPlaying()        |                 |
|                                          | connect()            |                 |
|                                          | changeVoiceState()   |                 |
|                                          | disconnect()         |                 |
|                                          | destroy()            |                 |
|                                          | changeNode()         |                 |
|                                          | toJSON()             |                 |



***

## <mark style="color:blue;">Properties</mark>

### <mark style="color:blue;">.volume</mark>

> The Display Volume

**Type**: [Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)

### <mark style="color:blue;">.lavalinkVolume</mark>

> The Volume Lavalink is actually outputting

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)

### <mark style="color:blue;">.position</mark>

> The current position of the player (calculated)

**Type**: [Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)

### <mark style="color:blue;">.lastPosition</mark>

> The current position of the player (from Lavalink)

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)

### <mark style="color:blue;">.createdTimeStamp</mark>

> When the player was created \[Timestamp in ms] (from Lavalink)

**Type**: [Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)

### <mark style="color:blue;">.connected</mark>

> The players connection state (from Lavalink)

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)

### <mark style="color:blue;">.voice</mark>

> Voice Server Data (from Lavalink)

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[LavalinkPlayerVoiceOptions](../other-utils-and-classes/)

### <mark style="color:blue;">.guildId</mark>

> The Guild Id of the Player

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/String)

### <mark style="color:blue;">.voiceChannelId</mark>

> The Voice Channel Id of the Player

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/String)

### <mark style="color:blue;">.textChannelId</mark>

> The Text Channel Id of the Player

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/String)

### <mark style="color:blue;">.playing</mark>

> States if the bot is supposed to be outputting audio

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)

### <mark style="color:blue;">.paused</mark>

> State if the bot is paused or not

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)

### <mark style="color:blue;">.repeatMode</mark>

> Repeat mode of the player

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[RepeatMode](playertypes/repeatmode.md)

### <mark style="color:blue;">.ping</mark>

> Player's ping

**Type**:[ ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Array)<[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Number)>

