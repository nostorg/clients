---
layout: home
---

Compendium of nostr clients and known features.

Contribute your findings: <https://github.com/nostorg/clients>

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
- 🟡 : partially supported or nonstandard implementation
- ❌ : mostly not supported
- ⚡ : paid feature
- `?` : reviewed but unclear
- <code>&nbsp;</code> : not yet reviewed

### Criteria for ✅

- macOS: Has a fully native desktop macOS app, not just a mobile app built for Apple Silicon.
- Zaps: Can view who zapped what amounts; can process zaps via QR code or external application.
- Reactions: Can view who reacted with which reactions; can react with any custom emoji.
- Mute List: Uses the kind 10000 list, not a kind 30000 parameterized list.
- Long-form Content: Properly renders markdown; updated events are fully replaced or the update history is clearly indicated.
- User Relays: Shows complete relay list for other users; has an option for disabling write access on each connected relay.
- Event Relays: Shows all connected relays where an event exists.
- Search: On connected relays, returns any existing user by username or NIP-05, and returns any existing note by content.

### Similar projects

- <https://github.com/aljazceru/awesome-nostr>
- <https://github.com/vishalxl/Nostr-Clients-Features-List>
- [Nostr Client Comparison Sheet (Google Docs)](https://docs.google.com/spreadsheets/d/1GjfN_eMiEywqXfKFHZMw4rLnoQLBXYEyl2NCEtsCXWw/edit)
- <https://www.nostrapps.com/>
- <https://nostrapp.link/>
