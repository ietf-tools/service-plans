## 1 Terms of service

### 1.1 Availability
The Zulip service will be a production service, available to all IETF community members.

### 1.2 Authentication
Login to Zulip is via the Datatracker credentials only.

### 1.3 NoteWell
The NoteWell will apply to all messages in the Zulip service.

As Zulip does not support a welcome message, a stream will be created called #NOTEWELL with restricted posting rights and the NoteWell will be posted in there. #NOTEWELL will be a default stream for all users.

## 2 Streams
Zulip organises content into streams and then topics within those streams. Streams are analagous to an email list and topics to threads within those.

### 2.1 Working Group streams
Any Working Group can elect to utilise Zulip.

Each working group that chooses to utilise to Zulip will initially be configured with two streams:

1. General chat, two-way bridged with the jabber room.
2. One-way mirror of the mailing list, read only.

The mailing list mirror has been split into a separate stream as having it mirror into the general chat stream would mean:

* People who already subscribe to the mailing list would have to scroll through the same messages twice. In this configuration they can choose not to subscribe to the list mirror in zulip or to mute the stream to view or search the mirrored messages without receiving notifications for them.
* The archive of the chat would include the mailing list messages  which is confusing for searching/referencing.
* The jabber channel would also get the mirrored mailing list messages, compounding the problem. 

Working groups will be free to request other streams to split out some work, say for a sub-team or for a specific integration, but they must follow the naming convention below. 

Working Group streams will be named as follows, in order to ensure that streams for the same WG are adjacent in indexes and a 'start of name' search returns all the relevant streams.

| Stream                        | Name        |
| :---------------------------- | :---------- |
| General chat                  | \<wg name\>      |
| Mirror of the mailing list    | \<wg name\>\/mailing-list |
| Sub-teams (if used)       | \<wg name\>\/\<team name\> |
| Specific draft (if used) | \<wg name\>\/\<draft name\>

### 2.2 Non-WG streams
The admins of any existing non-WG mailing list can elect to utilise Zulip, which will be configured similar to WGs with two streams.

### 2.3 Private streams
Private streams will only be allowed under the same terms as private mailing lists (i.e. for the confidential communications of the different groups in IETF leadership).

### 2.4 Stream archiving
A permanent, public, searchable and linkable archive will be achieved by the jabber bridging and the current archiving of jabber messages rather than directly from Zulip.  Later, it is likely that the built-in Zulip archiving tool will be used to directly archive public streams. 

## 3 Messages
The Zulip service is different from the jabber service because all users have IETF accounts and all messages, including direct messages, pass through the IETF server. The policies around messages are likely to develop over time.

### 3.1 Message retention
Initially all Zulip content (messages and attachments) will be retained in Zulip indefinitely.

### 3.2 Direct messages
Direct messages (described as 'private messages' in Zulip) will be allowed, which is a new development for an IETF operated service. The initial plan is that all messages, including direct ones, are covered by the NoteWell. All direct messages will be retained on the Zulip server in line with the general retention plan for this service. Direct messages should not be regarded as private because they will be accessed and shared where required by policy or law.

### 3.3 Editing messages
The Zulip service will be configured to only allow editing of messages for 10 minutes after creation.

## 4 Integrations

### 4.1 Meetecho integration
Initally, integration with Meetecho will be achieved by the two-way jabber bridging.  Later, it is likely that Meetecho will be asked to add support for Zulip.

### 4.2 GitHub integration
Any stream can be optionally configured to receive GitHub notifications.  WGs can decide if these should be received into an existing stream or a separate dedicated stream.

### 4.3 Agenda integration
Zulip provides a URL for each stream. Initially these URLs will be used in the agenda in addition to the jabber rooms links.

### 4.4 Datatracker integration
Potential ways of integrating Zulip with the Datatracker to provide enhanced functionality between the two systems are being investigated.

### Other integrations
Zulip supports integration with most APIs.  While there are no specific plans to use this, any requests will be investigated.
