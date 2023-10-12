---
layout: home
---

Compendium of nostr clients and known features.

Contribute updates on github: <https://github.com/nostorg/clients>

<div class="breakout" style="overflow-x:auto;">
<table>
  {% for row in site.data.clients %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
</div>

### Legend

- [NIPs](https://github.com/nostr-protocol/nips)
- ✅ : mostly supported
- 🟡 : partially supported
- ❌ : mostly not supported
- ⚡ : paid feature
- `?` : reviewed but inconclusive
- <code>&nbsp;</code> : not yet reviewed

### Criteria for ✅

Any column with at least one 🟡 entry should have some criteria listed here.

- Zaps: Can view who zapped what amounts; can process zaps via integrated wallet, external application, or QR code.
- Reactions: Can view who reacted with which reactions; can react with any custom emoji.
- Local Feeds: Can view all recent notes from connected relays and filter by relay.
- Algorithmic Feeds: Can view custom feeds determined by some open source or configurable algorithm (e.g. "trending").
- Mute List: Uses the kind 10000 list, not a kind 30000 parameterized list.
- Long-form Content: Properly renders markdown; updated events are fully replaced or the update history is clearly indicated.
- User Relays: Shows complete relay list for other users; has an option for disabling write access on each connected relay.
- Event Relays: Shows all connected relays where an event exists.
- Relay Info: Shows all available relay metadata for all connected relays.
- Search: On connected relays, returns any existing user by username or NIP-05, and returns any existing note by content.
- Push Notifications: Received on device without requiring the client software to be actively running.
- Machine Translation: Can do offline translation of notes with configurable language models.
- Multiple Accounts: Saves multiple profiles to switch between views or logins for multiple accounts with public keys, private keys, or extension (NIP-07).
- macOS: Has a fully native desktop macOS app, not just a mobile app that can run on Apple Silicon.

### Similar projects

- <https://github.com/aljazceru/awesome-nostr>
- <https://github.com/vishalxl/Nostr-Clients-Features-List>
- [Nostr Client Comparison Sheet (Google Docs)](https://docs.google.com/spreadsheets/d/1GjfN_eMiEywqXfKFHZMw4rLnoQLBXYEyl2NCEtsCXWw/edit)
- <https://www.nostrapps.com/>
- <https://nostrapp.link/>
