Bugfix: Fix closing a shared document from the office editor

Closing a document or using "Open file location" in the office editor failed
with a private link error for users who had a single file shared with them.
The editor linked to the folder containing the file, which belongs to the
sharer and is not accessible to the sharee. The editor now links to the file
itself, and the web app resolves the right folder, such as "Shared with me",
without reopening the document.

https://github.com/owncloud/ocis/pull/13198
