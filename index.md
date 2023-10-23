---
layout: home
---

Compendium of nostr clients and known features.

Contribute on github: <{{ site.github.repository_url }}>

<div class="bigtable">
<table>
  <thead>
    {% assign spec = site.data.spec %}
    <tr>
      <th>{{ spec.client }}</th>
      <th>{{ spec.site }}</th>
      <th>{{ spec.repo }}</th>
      <th>{{ spec.latest }}</th>
      <th>{{ spec.purpose }}</th>
      <th>{{ spec.webApp }}</th>
      <th>{{ spec.windowsApp }}</th>
      <th>{{ spec.linuxApp }}</th>
      <th>{{ spec.macApp }}</th>
      <th>{{ spec.iphoneApp }}</th>
      <th>{{ spec.androidApp }}</th>
      <th>{{ spec.integratedWallet }}</th>
      <th>{{ spec.multipleAccounts }}</th>
      <th>{{ spec.eventRelays }}</th>
      <th>{{ spec.relayList }}</th>
      <th>{{ spec.relayInfo }}</th>
      <th>{{ spec.json }}</th>
      <th>{{ spec.followHashtag }}</th>
      <th>{{ spec.localFeeds }}</th>
      <th>{{ spec.algorithmicFeeds }}</th>
      <th>{{ spec.rebroadcast }}</th>
      <th>{{ spec.machineTranslation }}</th>
      <th>{{ spec.pushNotification }}</th>
      <th>{{ spec.eventDeletion }}</th>
      <th>{{ spec.zaps }}</th>
      <th>{{ spec.reactions }}</th>
      <th>{{ spec.customEmoji }}</th>
      <th>{{ spec.microblogging }}</th>
      <th>{{ spec.dms }}</th>
      <th>{{ spec.chatrooms }}</th>
      <th>{{ spec.communities }}</th>
      <th>{{ spec.longform }}</th>
      <th>{{ spec.report }}</th>
      <th>{{ spec.mute }}</th>
      <th>{{ spec.pins }}</th>
      <th>{{ spec.bookmarks }}</th>
      <th>{{ spec.badges }}</th>
      <th>{{ spec.search }}</th>
      <th>{{ spec.contentWarning }}</th>
      <th>{{ spec.subjectTagging }}</th>
      <th>{{ spec.livestreaming }}</th>
      <th>{{ spec.classifieds }}</th>
      <th>{{ spec.calendarEvents }}</th>
      <th>{{ spec.marketplaces }}</th>
      <th>{{ spec.walletconnect }}</th>
      <th>{{ spec.nostrconnect }}</th>
      <th>{{ spec.mnemonicSeeds }}</th>
      <th>{{ spec.proofOfWork }}</th>
      <th>{{ spec.labellingAndReviews }}</th>
    </tr>
  </thead>
  <tbody>
    {% for client_hash in site.data.clients %}
      {% assign client = client_hash[1] %}
      <tr>
        <td>{{ client.client }}</td>
        <td>{{ client.site }}</td>
        <td>{{ client.repo }}</td>
        <td>{{ client.latest }}</td>
        <td>{{ client.purpose }}</td>
        <td>{{ client.webApp }}</td>
        <td>{{ client.windowsApp }}</td>
        <td>{{ client.linuxApp }}</td>
        <td>{{ client.macApp }}</td>
        <td>{{ client.iphoneApp }}</td>
        <td>{{ client.androidApp }}</td>
        <td>{{ client.integratedWallet }}</td>
        <td>{{ client.multipleAccounts }}</td>
        <td>{{ client.eventRelays }}</td>
        <td>{{ client.relayList }}</td>
        <td>{{ client.relayInfo }}</td>
        <td>{{ client.json }}</td>
        <td>{{ client.followHashtag }}</td>
        <td>{{ client.localFeeds }}</td>
        <td>{{ client.algorithmicFeeds }}</td>
        <td>{{ client.rebroadcast }}</td>
        <td>{{ client.machineTranslation }}</td>
        <td>{{ client.pushNotification }}</td>
        <td>{{ client.eventDeletion }}</td>
        <td>{{ client.zaps }}</td>
        <td>{{ client.reactions }}</td>
        <td>{{ client.customEmoji }}</td>
        <td>{{ client.microblogging }}</td>
        <td>{{ client.dms }}</td>
        <td>{{ client.chatrooms }}</td>
        <td>{{ client.communities }}</td>
        <td>{{ client.longform }}</td>
        <td>{{ client.report }}</td>
        <td>{{ client.mute }}</td>
        <td>{{ client.pins }}</td>
        <td>{{ client.bookmarks }}</td>
        <td>{{ client.badges }}</td>
        <td>{{ client.search }}</td>
        <td>{{ client.contentWarning }}</td>
        <td>{{ client.subjectTagging }}</td>
        <td>{{ client.livestreaming }}</td>
        <td>{{ client.classifieds }}</td>
        <td>{{ client.calendarEvents }}</td>
        <td>{{ client.marketplaces }}</td>
        <td>{{ client.walletconnect }}</td>
        <td>{{ client.nostrconnect }}</td>
        <td>{{ client.mnemonicSeeds }}</td>
        <td>{{ client.proofOfWork }}</td>
        <td>{{ client.labellingAndReviews }}</td>
      </tr>
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
- macOS: Has a fully native desktop macOS app, not just a mobile app that can run on Apple Silicon.

## Similar projects

- <https://github.com/aljazceru/awesome-nostr>
- <https://github.com/vishalxl/Nostr-Clients-Features-List>
- [Nostr Client Comparison Sheet (Google Docs)](https://docs.google.com/spreadsheets/d/1GjfN_eMiEywqXfKFHZMw4rLnoQLBXYEyl2NCEtsCXWw/edit)
- <https://nostr.info/resources/>
- <https://nostr.com/clients>
- <https://www.nostrapps.com/>
- <https://nostrapp.link/>
