# Murdoc privacy notice

**Effective date: October 7, 2026.** Published by Phantom Forge Labs.

Murdoc helps authorized workspace members search uploaded documents and
connected Jira and Confluence content, ask questions, inspect citations and
export evidence. This notice describes the application's data handling. A
self-hosted operator also controls its deployment, providers and backups.

## Information processed

Murdoc processes sign-in identifiers, names and email addresses supplied by
the configured identity provider; workspace memberships and roles; uploaded
files; and content synchronized from sources selected by workspace
administrators. Connected content can contain authors, assignees, comments,
worklogs, attachments, mentions and other information about people.

Murdoc stores document originals, synchronized snapshots, extracted passages,
search embeddings, saved questions and answers, cited excerpts and reviewed
diagram observations. It retains account references and retrieval dates for
Atlassian personal-data reporting. Integration credentials are encrypted in
the backend store or supplied through operator-managed secret files; they are
not intentionally returned to browser clients.

Operational audit records identify actors, affected resources and outcomes.
The essential application audit does not record question, answer or source
text. Authentication cookies maintain sign-in sessions. Workspace preferences
may be stored in the browser. This application currently has no built-in
advertising or marketing analytics workflow.

## Purpose and recipients

Information is processed to provide workspace access, synchronize selected
sources, index and retrieve evidence, generate answers, retain private chats,
support exports and operate the application. Workspace members can access
shared documents subject to their roles and live source permissions. Saved
conversations are private to their owners.

Selected content and questions are sent to the chat or embedding providers
configured for the workspace. These may be locally hosted models or external
services; the operator controls that selection and must provide applicable
provider and hosting information to users. Murdoc's application code does not
itself use these documents to train a shared model; configured providers have
their own data-handling terms.

Atlassian receives account references and the age of cached personal data
through its reporting API. It can instruct Murdoc to refresh or erase affected
cached data. The integration requests read access to Jira work and Confluence
pages and spaces and checks source access using each connected user's grant.

## Retention and removal

Data remains until it is removed through the relevant application or operator
process. Removing a synchronized source item can leave an earlier saved answer
with a source-change warning. Deleting a conversation removes its stored
questions, answers and cited excerpts. Unlinking a user's account stops that
grant's access; it does not erase shared content still needed by other
authorized users.

When Atlassian requires refresh or erasure, the privacy maintenance process
removes affected connected snapshots and their dependent conversations before
fresh synchronization. It retries incomplete cleanup and withholds affected
source access. Account erasure also removes the affected grants and retains a
one-way reference tombstone to prevent structured reimport.

Already downloaded evidence is controlled by its recipient. Backups,
application logs and infrastructure retention are controlled by the deployment
operator; they require an appropriate retention and restore policy. This
notice does not promise immediate deletion from independently held exports or
operator-managed backups.

## Requests and contact

For questions, access, correction or erasure requests concerning the Phantom
Forge Labs deployment, contact **kevin.jones@phantom-forge-labs.com**. For a
self-hosted deployment, contact its operator as well. Provide enough context
to locate the workspace and affected content; do not send passwords or tokens.
The operator may need to verify the requester's authority before processing a
request. Free-text references and manually imported copies may require review
beyond automated Atlassian account reporting.

Changes to this notice will be reviewed and dated when adopted.
