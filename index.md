---
layout: home
---

Compendium of nostr clients and known features.

Contribute on github: <{{ site.github.repository_url }}>

<div class="bigtable">
<table>
  <thead>
    <tr>
      <!-- Basic Info -->
      <th>Client \ Feature (NIP) [Kind]</th>
      <th>Source Repository</th>
      <th>Last Reviewed Version/Date</th>
      <th>Primary Purpose</th>
      <!-- Features -->
      {% for feature in site.data.features %}
      <th>{{ feature[1] }}</th>
      {% endfor %}
    </tr>
  </thead>
  <tbody>
    {% for client_order in site.data.order %}
    {% for client_hash in site.data.clients %}
    {% if client_hash[0] == client_order %}
    {% assign client = client_hash[1] %}
    <tr>
      <!-- Basic Info -->
      {% if client.site %}
      <td><a href="{{ client.site }}">{{ client.alias }}</a></td>
      {% else %}
      <td>{{ client.alias }}</td>
      {% endif %}
      <td><a href="{{ client.repo }}">
        <img alt="" src="https://img.shields.io/github/last-commit/{{ client.repo | split: '/' | slice: -2, 2 | join: '/' }}/main">
        <img alt="" src="https://img.shields.io/github/last-commit/{{ client.repo | split: '/' | slice: -2, 2 | join: '/' }}/master">
        </a></td>
      <td>{{ client.latest }}</td>
      <td>{{ client.purpose }}</td>
      <!-- Features -->
      {% for feature_head in site.data.features %}
      <td>
      {% for feature_client in client.features %}
      {% if feature_client[0] == feature_head[0] %}
      {{ feature_client[1] }}
      {% endif %}
      {% endfor %}
      </td>
      {% endfor %}
    </tr>
    {% endif %}
    {% endfor %}
    {% endfor %}
  </tbody>
</table>
</div>

## Legend

- [NIPs](https://github.com/nostr-protocol/nips)
- ✅ : mostly supported
- 🟡 : partially supported
- ❌ : mostly not supported
- ⚡ : paid feature
- `?` : reviewed but inconclusive
- <code>&nbsp;</code> : not yet reviewed

## Criteria for ✅

Any column with at least one 🟡 entry should have some criteria listed here.

- Zaps: Can view who zapped what amounts on notes; can zap notes and profiles via integrated wallet, external application, or QR code.
- Reactions: Can view who reacted with which reactions; can react with any unicode emoji.
- Event Deletion: Can delete own notes and undo reactions by deletion.
- Direct Messages: Can view and decrypt all past conversations; can encrypt and send new messages.
- Local Feeds: Can view all recent notes from connected relays and filter by relay.
- Algorithmic Feeds: Can view custom feeds determined by some open source or configurable algorithm (e.g. "trending").
- Mute List: Reads from and writes to the kind 10000 list, not a kind 30000 parameterized list.
- Pins: Reads from and writes to the kind 10001 list, not a kind 30001 parameterized list.
- Bookmarks: Reads from and writes to a kind 30001 parameterized list.
- Relay List: Reads from and writes to the kind 10002 relay list; DOES NOT write relay list changes to the kind 3 contact list; shows relay lists for other users; can toggle read/write access for each connected relay.
- Event Relays: Shows all connected relays where an event exists.
- Relay Info: Shows all available relay metadata for all connected relays.
- Long-form Content: Properly renders markdown; updated events are fully replaced or the update history is clearly indicated.
- Search: On connected relays, returns any existing user by username or NIP-05, and returns any existing note by content.
- Push Notifications: Received on device without requiring the client software to be actively running.
- Machine Translation: Can do offline translation of notes with configurable language models.
- Multiple Accounts: Saves multiple profiles to switch between views or logins for multiple accounts with public keys, private keys, or extension (NIP-07).

Has a fully native desktop macOS app, not just a mobile app that can run on Apple Silicon.

## Similar projects

- <https://github.com/aljazceru/awesome-nostr>
- <https://github.com/vishalxl/Nostr-Clients-Features-List>
- [Nostr Client Comparison Sheet (Google Docs)](https://docs.google.com/spreadsheets/d/1GjfN_eMiEywqXfKFHZMw4rLnoQLBXYEyl2NCEtsCXWw/edit)
- <https://nostr.info/resources/>
- <https://nostr.com/clients>
- <https://www.nostrapps.com/>
- <https://nostrapp.link/>
