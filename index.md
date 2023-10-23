---
layout: home
---

Compendium of nostr clients and known features.

Contribute updates on github: <https://github.com/nostorg/clients>

<div class="bigtable">
<h2>Combined Table</h2>
<table>
  <thead>
    <tr>
      <th>Client</th>
      <th>Site</th>
      <th>Repo</th>
      <th>Latest Version</th>
      <th>Purpose</th>
      <th>Web App</th>
      <th>Windows App</th>
      <th>Linux App</th>
      <th>Mac App</th>
      <th>iPhone App</th>
      <th>Android App</th>
      <th>Integrated Wallet</th>
      <th>Multiple Accounts</th>
      <th>Event Relays</th>
      <th>Relay List</th>
      <th>Relay Info</th>
      <th>JSON</th>
      <th>Follow Hashtag</th>
      <th>Local Feeds</th>
      <th>Algorithmic Feeds</th>
      <th>Rebroadcast</th>
      <th>Machine Translation</th>
      <th>Push Notification</th>
      <th>Event Deletion</th>
      <th>Zaps</th>
      <th>Reactions</th>
      <th>Custom Emoji</th>
      <th>Microblogging</th>
      <th>DMS</th>
      <th>Chatrooms</th>
      <th>Communities</th>
      <th>Longform</th>
      <th>Report</th>
      <th>Mute</th>
      <th>Pins</th>
      <th>Bookmarks</th>
      <th>Badges</th>
      <th>Search</th>
      <th>Content Warning</th>
      <th>Subject Tagging</th>
      <th>Livestreaming</th>
      <th>Classifieds</th>
      <th>Calendar Events</th>
      <th>Marketplaces</th>
      <th>WalletConnect</th>
      <th>NostrConnect</th>
      <th>Mnemonic Seeds</th>
      <th>Proof of Work</th>
      <th>Labelling and Reviews</th>
    </tr>
  </thead>
  <tbody>
    {% for data_file in site.data.clients %}
      <!-- The data_file object contains the name and the content -->
      {% assign file_name = data_file[0] %}
      {% assign file_content = data_file[1] %}
        <tr>
            <td>{{ file_content.client }}</td>
            <td>{{ file_content.site }}</td>
            <td>{{ file_content.repo }}</td>
            <td>{{ file_content.latest }}</td>
            <td>{{ file_content.purpose }}</td>
            <td>{{ file_content.webApp }}</td>
            <td>{{ file_content.windowsApp }}</td>
            <td>{{ file_content.linuxApp }}</td>
            <td>{{ file_content.macApp }}</td>
            <td>{{ file_content.iphoneApp }}</td>
            <td>{{ file_content.androidApp }}</td>
            <td>{{ file_content.integratedWallet }}</td>
            <td>{{ file_content.multipleAccounts }}</td>
            <td>{{ file_content.eventRelays }}</td>
            <td>{{ file_content.relayList }}</td>
            <td>{{ file_content.relayInfo }}</td>
            <td>{{ file_content.json }}</td>
            <td>{{ file_content.followHashtag }}</td>
            <td>{{ file_content.localFeeds }}</td>
            <td>{{ file_content.algorithmicFeeds }}</td>
            <td>{{ file_content.rebroadcast }}</td>
            <td>{{ file_content.machineTranslation }}</td>
            <td>{{ file_content.pushNotification }}</td>
            <td>{{ file_content.eventDeletion }}</td>
            <td>{{ file_content.zaps }}</td>
            <td>{{ file_content.reactions }}</td>
            <td>{{ file_content.customEmoji }}</td>
            <td>{{ file_content.microblogging }}</td>
            <td>{{ file_content.dms }}</td>
            <td>{{ file_content.chatrooms }}</td>
            <td>{{ file_content.communities }}</td>
            <td>{{ file_content.longform }}</td>
            <td>{{ file_content.report }}</td>
            <td>{{ file_content.mute }}</td>
            <td>{{ file_content.pins }}</td>
            <td>{{ file_content.bookmarks }}</td>
            <td>{{ file_content.badges }}</td>
            <td>{{ file_content.search }}</td>
            <td>{{ file_content.contentWarning }}</td>
            <td>{{ file_content.subjectTagging }}</td>
            <td>{{ file_content.livestreaming }}</td>
            <td>{{ file_content.classifieds }}</td>
            <td>{{ file_content.calendarEvents }}</td>
            <td>{{ file_content.marketplaces }}</td>
            <td>{{ file_content.walletconnect }}</td>
            <td>{{ file_content.nostrconnect }}</td>
            <td>{{ file_content.mnemonicSeeds }}</td>
            <td>{{ file_content.proofOfWork }}</td>
            <td>{{ file_content.labellingAndReviews }}</td>
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
- <https://www.nostrapps.com/>
- <https://nostrapp.link/>
