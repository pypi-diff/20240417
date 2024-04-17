# Comparing `tmp/netbluemind5-5.0.7152.tar.gz` & `tmp/netbluemind5-5.0.7187.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbluemind5-5.0.7152.tar", last modified: Thu Apr 11 14:30:48 2024, max compression
+gzip compressed data, was "netbluemind5-5.0.7187.tar", last modified: Wed Apr 17 12:54:02 2024, max compression
```

## Comparing `netbluemind5-5.0.7152.tar` & `netbluemind5-5.0.7187.tar`

### file list

```diff
@@ -1,670 +1,672 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.843433 netbluemind5-5.0.7152/
--rw-r--r--   0 root         (0) root         (0)     2232 2024-04-11 14:29:52.000000 netbluemind5-5.0.7152/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-11 14:30:48.843433 netbluemind5-5.0.7152/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      461 2024-04-11 14:29:52.000000 netbluemind5-5.0.7152/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.755431 netbluemind5-5.0.7152/netbluemind/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.755431 netbluemind5-5.0.7152/netbluemind/addressbook/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/addressbook/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.767431 netbluemind5-5.0.7152/netbluemind/addressbook/api/
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/AddressBookDescriptor.py
--rw-r--r--   0 root         (0) root         (0)    24040 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/IAddressBook.py
--rw-r--r--   0 root         (0) root         (0)     3064 2024-04-11 14:30:15.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/IAddressBookUids.py
--rw-r--r--   0 root         (0) root         (0)     2156 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/IAddressBooks.py
--rw-r--r--   0 root         (0) root         (0)     7034 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/IAddressBooksMgmt.py
--rw-r--r--   0 root         (0) root         (0)     2734 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/IVCardService.py
--rw-r--r--   0 root         (0) root         (0)     6805 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCard.py
--rw-r--r--   0 root         (0) root         (0)     2204 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardBasicAttribute.py
--rw-r--r--   0 root         (0) root         (0)     3405 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardChanges.py
--rw-r--r--   0 root         (0) root         (0)     2218 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1515 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2227 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     4211 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunications.py
--rw-r--r--   0 root         (0) root         (0)     1705 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunicationsEmail.py
--rw-r--r--   0 root         (0) root         (0)     1702 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunicationsImpp.py
--rw-r--r--   0 root         (0) root         (0)     1702 2024-04-11 14:30:15.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunicationsLang.py
--rw-r--r--   0 root         (0) root         (0)     1894 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunicationsTel.py
--rw-r--r--   0 root         (0) root         (0)     2085 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardDeliveryAddressing.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardDeliveryAddressingAddress.py
--rw-r--r--   0 root         (0) root         (0)     2750 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardExplanatory.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardExplanatoryUrl.py
--rw-r--r--   0 root         (0) root         (0)     5236 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentification.py
--rw-r--r--   0 root         (0) root         (0)     1726 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentificationFormatedName.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentificationGender.py
--rw-r--r--   0 root         (0) root         (0)     3023 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentificationName.py
--rw-r--r--   0 root         (0) root         (0)     1714 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentificationNickname.py
--rw-r--r--   0 root         (0) root         (0)     4030 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardInfo.py
--rw-r--r--   0 root         (0) root         (0)     1140 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardKind.py
--rw-r--r--   0 root         (0) root         (0)     3115 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardOrganizational.py
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardOrganizationalMember.py
--rw-r--r--   0 root         (0) root         (0)     2049 2024-04-11 14:30:16.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardOrganizationalOrg.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-04-11 14:30:15.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardParameter.py
--rw-r--r--   0 root         (0) root         (0)     2788 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardQuery.py
--rw-r--r--   0 root         (0) root         (0)     1136 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardQueryOrderBy.py
--rw-r--r--   0 root         (0) root         (0)     1992 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardRelated.py
--rw-r--r--   0 root         (0) root         (0)     1939 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardSecurity.py
--rw-r--r--   0 root         (0) root         (0)     1681 2024-04-11 14:30:15.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardSecurityKey.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/addressbook/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.767431 netbluemind5-5.0.7152/netbluemind/attachment/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/attachment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.767431 netbluemind5-5.0.7152/netbluemind/attachment/api/
--rw-r--r--   0 root         (0) root         (0)     2228 2024-04-11 14:30:38.000000 netbluemind5-5.0.7152/netbluemind/attachment/api/AttachedFile.py
--rw-r--r--   0 root         (0) root         (0)     2196 2024-04-11 14:30:37.000000 netbluemind5-5.0.7152/netbluemind/attachment/api/Configuration.py
--rw-r--r--   0 root         (0) root         (0)     3699 2024-04-11 14:30:38.000000 netbluemind5-5.0.7152/netbluemind/attachment/api/IAttachment.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/attachment/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.767431 netbluemind5-5.0.7152/netbluemind/authentication/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/authentication/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.771431 netbluemind5-5.0.7152/netbluemind/authentication/api/
--rw-r--r--   0 root         (0) root         (0)     2214 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/APIKey.py
--rw-r--r--   0 root         (0) root         (0)     4622 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/AccessTokenInfo.py
--rw-r--r--   0 root         (0) root         (0)     1205 2024-04-11 14:30:41.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/AccessTokenInfoTokenStatus.py
--rw-r--r--   0 root         (0) root         (0)     3330 2024-04-11 14:30:41.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/AuthUser.py
--rw-r--r--   0 root         (0) root         (0)     3891 2024-04-11 14:30:41.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/IAPIKeys.py
--rw-r--r--   0 root         (0) root         (0)     6122 2024-04-11 14:30:41.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/IAuthentication.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-04-11 14:30:41.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/ISecurityToken.py
--rw-r--r--   0 root         (0) root         (0)     1387 2024-04-11 14:30:41.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/ISudoSupport.py
--rw-r--r--   0 root         (0) root         (0)     2334 2024-04-11 14:30:41.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/IUserAccessToken.py
--rw-r--r--   0 root         (0) root         (0)     3151 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/LoginResponse.py
--rw-r--r--   0 root         (0) root         (0)     1132 2024-04-11 14:30:41.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/LoginResponseStatus.py
--rw-r--r--   0 root         (0) root         (0)     1193 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/ValidationKind.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/authentication/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.771431 netbluemind5-5.0.7152/netbluemind/backend/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.771431 netbluemind5-5.0.7152/netbluemind/backend/mail/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.779431 netbluemind5-5.0.7152/netbluemind/backend/mail/api/
--rw-r--r--   0 root         (0) root         (0)     2669 2024-04-11 14:30:45.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/Conversation.py
--rw-r--r--   0 root         (0) root         (0)     1987 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/ConversationMessageRef.py
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/DispositionType.py
--rw-r--r--   0 root         (0) root         (0)    10594 2024-04-11 14:30:45.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IBaseMailboxFolders.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IItemsTransfer.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailConversation.py
--rw-r--r--   0 root         (0) root         (0)     6827 2024-04-11 14:30:44.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailConversationActions.py
--rw-r--r--   0 root         (0) root         (0)    19038 2024-04-11 14:30:44.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailboxFolders.py
--rw-r--r--   0 root         (0) root         (0)    19188 2024-04-11 14:30:46.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailboxFoldersByContainer.py
--rw-r--r--   0 root         (0) root         (0)    20565 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailboxItems.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IOutbox.py
--rw-r--r--   0 root         (0) root         (0)    10805 2024-04-11 14:30:45.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IReadOnlyMailboxFolders.py
--rw-r--r--   0 root         (0) root         (0)     1579 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/IUserInbox.py
--rw-r--r--   0 root         (0) root         (0)     1759 2024-04-11 14:30:46.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImapAck.py
--rw-r--r--   0 root         (0) root         (0)     1884 2024-04-11 14:30:44.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImapItemIdentifier.py
--rw-r--r--   0 root         (0) root         (0)     2751 2024-04-11 14:30:46.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemSet.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemSetMailboxItemId.py
--rw-r--r--   0 root         (0) root         (0)     3090 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemsStatus.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportStatus.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-04-11 14:30:42.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportedMailboxItem.py
--rw-r--r--   0 root         (0) root         (0)     2219 2024-04-11 14:30:46.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MailboxFolder.py
--rw-r--r--   0 root         (0) root         (0)     2397 2024-04-11 14:30:44.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MailboxFolderSearchQuery.py
--rw-r--r--   0 root         (0) root         (0)     2723 2024-04-11 14:30:46.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MailboxItem.py
--rw-r--r--   0 root         (0) root         (0)     5744 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBody.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBodyHeader.py
--rw-r--r--   0 root         (0) root         (0)     4943 2024-04-11 14:30:44.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBodyPart.py
--rw-r--r--   0 root         (0) root         (0)     2397 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBodyRecipient.py
--rw-r--r--   0 root         (0) root         (0)     1239 2024-04-11 14:30:42.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBodyRecipientKind.py
--rw-r--r--   0 root         (0) root         (0)     4966 2024-04-11 14:30:42.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageSearchResult.py
--rw-r--r--   0 root         (0) root         (0)     2088 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageSearchResultMbox.py
--rw-r--r--   0 root         (0) root         (0)     5250 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQuery.py
--rw-r--r--   0 root         (0) root         (0)     1569 2024-04-11 14:30:44.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQueryFolderScope.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-04-11 14:30:44.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQueryHeader.py
--rw-r--r--   0 root         (0) root         (0)     2800 2024-04-11 14:30:44.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQueryHeaderQuery.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-11 14:30:45.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQueryLogicalOperator.py
--rw-r--r--   0 root         (0) root         (0)     2360 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQuerySearchScope.py
--rw-r--r--   0 root         (0) root         (0)     2563 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchResult.py
--rw-r--r--   0 root         (0) root         (0)     2030 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchSort.py
--rw-r--r--   0 root         (0) root         (0)     1100 2024-04-11 14:30:42.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchSortOrder.py
--rw-r--r--   0 root         (0) root         (0)     2118 2024-04-11 14:30:43.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchSortSortCriteria.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.783431 netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/ConversationFlagUpdate.py
--rw-r--r--   0 root         (0) root         (0)     2274 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/FlagUpdate.py
--rw-r--r--   0 root         (0) root         (0)     2340 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/ImportMailboxConversationSet.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/MailboxItemFlag.py
--rw-r--r--   0 root         (0) root         (0)     1196 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/MailboxItemFlagSystem.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.783431 netbluemind5-5.0.7152/netbluemind/calendar/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.791432 netbluemind5-5.0.7152/netbluemind/calendar/api/
--rw-r--r--   0 root         (0) root         (0)     2788 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     3116 2024-04-11 14:30:25.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarLookupResponse.py
--rw-r--r--   0 root         (0) root         (0)     1145 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarLookupResponseType.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-04-11 14:30:27.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarSettingsData.py
--rw-r--r--   0 root         (0) root         (0)     1188 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarSettingsDataDay.py
--rw-r--r--   0 root         (0) root         (0)     2770 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarView.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-04-11 14:30:24.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewCalendarViewType.py
--rw-r--r--   0 root         (0) root         (0)     3600 2024-04-11 14:30:24.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewChanges.py
--rw-r--r--   0 root         (0) root         (0)     2066 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1536 2024-04-11 14:30:27.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2075 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarsVEventQuery.py
--rw-r--r--   0 root         (0) root         (0)    23442 2024-04-11 14:30:25.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendar.py
--rw-r--r--   0 root         (0) root         (0)     2750 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarAutocomplete.py
--rw-r--r--   0 root         (0) root         (0)     2440 2024-04-11 14:30:27.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarSettings.py
--rw-r--r--   0 root         (0) root         (0)     2496 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarUids.py
--rw-r--r--   0 root         (0) root         (0)     6957 2024-04-11 14:30:27.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarView.py
--rw-r--r--   0 root         (0) root         (0)     1467 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarViewUids.py
--rw-r--r--   0 root         (0) root         (0)     3049 2024-04-11 14:30:24.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendars.py
--rw-r--r--   0 root         (0) root         (0)     4943 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarsMgmt.py
--rw-r--r--   0 root         (0) root         (0)     3067 2024-04-11 14:30:24.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/IFreebusyMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1448 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/IFreebusyUids.py
--rw-r--r--   0 root         (0) root         (0)     1752 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/IPrint.py
--rw-r--r--   0 root         (0) root         (0)     3473 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/IPublicFreebusy.py
--rw-r--r--   0 root         (0) root         (0)     3665 2024-04-11 14:30:25.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/IPublishCalendar.py
--rw-r--r--   0 root         (0) root         (0)    13473 2024-04-11 14:30:27.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/IUserCalendarViews.py
--rw-r--r--   0 root         (0) root         (0)     2596 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/IVEvent.py
--rw-r--r--   0 root         (0) root         (0)     2623 2024-04-11 14:30:25.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/IVFreebusy.py
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/PrintData.py
--rw-r--r--   0 root         (0) root         (0)     5946 2024-04-11 14:30:24.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptions.py
--rw-r--r--   0 root         (0) root         (0)     1746 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptionsCalendarMetadata.py
--rw-r--r--   0 root         (0) root         (0)     1156 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptionsPrintFormat.py
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptionsPrintLayout.py
--rw-r--r--   0 root         (0) root         (0)     1160 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptionsPrintView.py
--rw-r--r--   0 root         (0) root         (0)     1100 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/PublishMode.py
--rw-r--r--   0 root         (0) root         (0)     2821 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEvent.py
--rw-r--r--   0 root         (0) root         (0)     2695 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventAttendeeQuery.py
--rw-r--r--   0 root         (0) root         (0)     3402 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventChanges.py
--rw-r--r--   0 root         (0) root         (0)     2375 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-04-11 14:30:27.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2384 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     2667 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventCounter.py
--rw-r--r--   0 root         (0) root         (0)     1815 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventCounterCounterOriginator.py
--rw-r--r--   0 root         (0) root         (0)     2112 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventOccurrence.py
--rw-r--r--   0 root         (0) root         (0)     4230 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventQuery.py
--rw-r--r--   0 root         (0) root         (0)     3935 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventSeries.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VEventTransparency.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-04-11 14:30:25.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VFreebusy.py
--rw-r--r--   0 root         (0) root         (0)     2996 2024-04-11 14:30:26.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VFreebusyQuery.py
--rw-r--r--   0 root         (0) root         (0)     3128 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VFreebusySlot.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-04-11 14:30:27.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/VFreebusyType.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/calendar/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.791432 netbluemind5-5.0.7152/netbluemind/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.795432 netbluemind5-5.0.7152/netbluemind/core/api/
--rw-r--r--   0 root         (0) root         (0)     2011 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/api/Email.py
--rw-r--r--   0 root         (0) root         (0)     1736 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/api/ImportStats.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/api/ListResult.py
--rw-r--r--   0 root         (0) root         (0)     2211 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/api/VersionInfo.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/core/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.795432 netbluemind5-5.0.7152/netbluemind/core/api/date/
--rw-r--r--   0 root         (0) root         (0)     2417 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/api/date/BmDateTime.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/api/date/BmDateTimePrecision.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/core/api/date/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.795432 netbluemind5-5.0.7152/netbluemind/core/api/fault/
--rw-r--r--   0 root         (0) root         (0)     5200 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/api/fault/ErrorCode.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/core/api/fault/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.795432 netbluemind5-5.0.7152/netbluemind/core/container/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/core/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.795432 netbluemind5-5.0.7152/netbluemind/core/container/api/
--rw-r--r--   0 root         (0) root         (0)     1735 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/Ack.py
--rw-r--r--   0 root         (0) root         (0)     2318 2024-04-11 14:30:32.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerHierarchyNode.py
--rw-r--r--   0 root         (0) root         (0)     2906 2024-04-11 14:30:33.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerQuery.py
--rw-r--r--   0 root         (0) root         (0)     1158 2024-04-11 14:30:33.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerSettingsKeys.py
--rw-r--r--   0 root         (0) root         (0)     2113 2024-04-11 14:30:34.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerSubscription.py
--rw-r--r--   0 root         (0) root         (0)     2460 2024-04-11 14:30:32.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerSubscriptionDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     2762 2024-04-11 14:30:33.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerSubscriptionModel.py
--rw-r--r--   0 root         (0) root         (0)     1478 2024-04-11 14:30:32.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/Count.py
--rw-r--r--   0 root         (0) root         (0)     5503 2024-04-11 14:30:32.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IChangelogSupport.py
--rw-r--r--   0 root         (0) root         (0)    11391 2024-04-11 14:30:34.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IContainerManagement.py
--rw-r--r--   0 root         (0) root         (0)     2974 2024-04-11 14:30:34.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IContainerSync.py
--rw-r--r--   0 root         (0) root         (0)    12400 2024-04-11 14:30:33.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IContainers.py
--rw-r--r--   0 root         (0) root         (0)    10022 2024-04-11 14:30:32.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IContainersFlatHierarchy.py
--rw-r--r--   0 root         (0) root         (0)     1788 2024-04-11 14:30:33.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/ICountingSupport.py
--rw-r--r--   0 root         (0) root         (0)     1529 2024-04-11 14:30:32.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IFlatHierarchyUids.py
--rw-r--r--   0 root         (0) root         (0)     1799 2024-04-11 14:30:33.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IOfflineMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1543 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IOwnerSubscriptionUids.py
--rw-r--r--   0 root         (0) root         (0)    11454 2024-04-11 14:30:33.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IOwnerSubscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1667 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/ISortingSupport.py
--rw-r--r--   0 root         (0) root         (0)     1763 2024-04-11 14:30:34.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/IdRange.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/core/container/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.799432 netbluemind5-5.0.7152/netbluemind/core/container/model/
--rw-r--r--   0 root         (0) root         (0)     4694 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/BaseContainerDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     3777 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ChangeLogEntry.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ChangeLogEntryType.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerChangelog.py
--rw-r--r--   0 root         (0) root         (0)     2477 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerChangeset.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     2105 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerModifiableDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     2861 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerSyncResult.py
--rw-r--r--   0 root         (0) root         (0)     3156 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerSyncStatus.py
--rw-r--r--   0 root         (0) root         (0)     1140 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerSyncStatusStatus.py
--rw-r--r--   0 root         (0) root         (0)     3489 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerUpdatesResult.py
--rw-r--r--   0 root         (0) root         (0)     2320 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerUpdatesResultInError.py
--rw-r--r--   0 root         (0) root         (0)     1188 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/CountFastPath.py
--rw-r--r--   0 root         (0) root         (0)     2677 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/IdQuery.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemChangeLogEntry.py
--rw-r--r--   0 root         (0) root         (0)     2006 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemChangelog.py
--rw-r--r--   0 root         (0) root         (0)     3737 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemContainerValue.py
--rw-r--r--   0 root         (0) root         (0)     4056 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemFlag.py
--rw-r--r--   0 root         (0) root         (0)     3131 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemFlagFilter.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemIdentifier.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemUri.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemValue.py
--rw-r--r--   0 root         (0) root         (0)     1941 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/ItemVersion.py
--rw-r--r--   0 root         (0) root         (0)     2610 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/SortDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/SortDescriptorDirection.py
--rw-r--r--   0 root         (0) root         (0)     2196 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/SortDescriptorField.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.799432 netbluemind5-5.0.7152/netbluemind/core/container/model/acl/
--rw-r--r--   0 root         (0) root         (0)     2037 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/acl/AccessControlEntry.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-11 14:30:31.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/acl/Verb.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:12.000000 netbluemind5-5.0.7152/netbluemind/core/container/model/acl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.799432 netbluemind5-5.0.7152/netbluemind/core/task/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/core/task/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.803432 netbluemind5-5.0.7152/netbluemind/core/task/api/
--rw-r--r--   0 root         (0) root         (0)     2471 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/task/api/ITask.py
--rw-r--r--   0 root         (0) root         (0)     1461 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/task/api/TaskRef.py
--rw-r--r--   0 root         (0) root         (0)     2808 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/task/api/TaskStatus.py
--rw-r--r--   0 root         (0) root         (0)     1174 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/core/task/api/TaskStatusState.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/core/task/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.803432 netbluemind5-5.0.7152/netbluemind/cti/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/cti/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.803432 netbluemind5-5.0.7152/netbluemind/cti/api/
--rw-r--r--   0 root         (0) root         (0)     4038 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/cti/api/IComputerTelephonyIntegration.py
--rw-r--r--   0 root         (0) root         (0)     2610 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/cti/api/Status.py
--rw-r--r--   0 root         (0) root         (0)     1219 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/cti/api/StatusPhoneState.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/cti/api/StatusType.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/cti/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.803432 netbluemind5-5.0.7152/netbluemind/dataprotect/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.803432 netbluemind5-5.0.7152/netbluemind/dataprotect/api/
--rw-r--r--   0 root         (0) root         (0)     3500 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/DataProtectGeneration.py
--rw-r--r--   0 root         (0) root         (0)     4139 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/GenerationContent.py
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/GenerationStatus.py
--rw-r--r--   0 root         (0) root         (0)     8292 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/IDataProtect.py
--rw-r--r--   0 root         (0) root         (0)     4132 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/PartGeneration.py
--rw-r--r--   0 root         (0) root         (0)     2878 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/Restorable.py
--rw-r--r--   0 root         (0) root         (0)     1229 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/RestorableKind.py
--rw-r--r--   0 root         (0) root         (0)     2507 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/RestoreDefinition.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/RestoreOperation.py
--rw-r--r--   0 root         (0) root         (0)     1947 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/RetentionPolicy.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/dataprotect/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.803432 netbluemind5-5.0.7152/netbluemind/device/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/device/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.803432 netbluemind5-5.0.7152/netbluemind/device/api/
--rw-r--r--   0 root         (0) root         (0)     4714 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/device/api/Device.py
--rw-r--r--   0 root         (0) root         (0)     8584 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/device/api/IDevice.py
--rw-r--r--   0 root         (0) root         (0)     1440 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/device/api/IDeviceUids.py
--rw-r--r--   0 root         (0) root         (0)     1498 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/device/api/IDevices.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/device/api/WipeMode.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/device/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.803432 netbluemind5-5.0.7152/netbluemind/directory/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/directory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.807432 netbluemind5-5.0.7152/netbluemind/directory/api/
--rw-r--r--   0 root         (0) root         (0)     3091 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/directory/api/BaseDirEntry.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/directory/api/BaseDirEntryAccountType.py
--rw-r--r--   0 root         (0) root         (0)     1301 2024-04-11 14:30:12.000000 netbluemind5-5.0.7152/netbluemind/directory/api/BaseDirEntryKind.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/directory/api/DirBaseValue.py
--rw-r--r--   0 root         (0) root         (0)     4364 2024-04-11 14:30:12.000000 netbluemind5-5.0.7152/netbluemind/directory/api/DirEntry.py
--rw-r--r--   0 root         (0) root         (0)     7466 2024-04-11 14:30:12.000000 netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQuery.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-04-11 14:30:12.000000 netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQueryDir.py
--rw-r--r--   0 root         (0) root         (0)     2469 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQueryOrder.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQueryOrderBy.py
--rw-r--r--   0 root         (0) root         (0)     1157 2024-04-11 14:30:12.000000 netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQueryStateFilter.py
--rw-r--r--   0 root         (0) root         (0)     2719 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/directory/api/IDirEntryMaintenance.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/directory/api/IDirEntryPath.py
--rw-r--r--   0 root         (0) root         (0)    13515 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/directory/api/IDirectory.py
--rw-r--r--   0 root         (0) root         (0)     9387 2024-04-11 14:30:12.000000 netbluemind5-5.0.7152/netbluemind/directory/api/IOrgUnits.py
--rw-r--r--   0 root         (0) root         (0)     1839 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/directory/api/MaintenanceOperation.py
--rw-r--r--   0 root         (0) root         (0)     1728 2024-04-11 14:30:12.000000 netbluemind5-5.0.7152/netbluemind/directory/api/OrgUnit.py
--rw-r--r--   0 root         (0) root         (0)     2228 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/directory/api/OrgUnitPath.py
--rw-r--r--   0 root         (0) root         (0)     2632 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/directory/api/OrgUnitQuery.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/directory/api/RepairConfig.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/directory/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.807432 netbluemind5-5.0.7152/netbluemind/document/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/document/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.807432 netbluemind5-5.0.7152/netbluemind/document/api/
--rw-r--r--   0 root         (0) root         (0)     2146 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/document/api/Document.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/document/api/DocumentMetadata.py
--rw-r--r--   0 root         (0) root         (0)     5027 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/document/api/IDocument.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/document/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.807432 netbluemind5-5.0.7152/netbluemind/documentfolder/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/documentfolder/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.807432 netbluemind5-5.0.7152/netbluemind/documentfolder/api/
--rw-r--r--   0 root         (0) root         (0)     1695 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/documentfolder/api/DocumentFolder.py
--rw-r--r--   0 root         (0) root         (0)     4166 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/documentfolder/api/IDocumentFolder.py
--rw-r--r--   0 root         (0) root         (0)     1482 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/documentfolder/api/IDocumentFolderUids.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/documentfolder/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.807432 netbluemind5-5.0.7152/netbluemind/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.807432 netbluemind5-5.0.7152/netbluemind/domain/api/
--rw-r--r--   0 root         (0) root         (0)     3063 2024-04-11 14:30:37.000000 netbluemind5-5.0.7152/netbluemind/domain/api/Domain.py
--rw-r--r--   0 root         (0) root         (0)     2076 2024-04-11 14:30:37.000000 netbluemind5-5.0.7152/netbluemind/domain/api/IDomainSettings.py
--rw-r--r--   0 root         (0) root         (0)     8758 2024-04-11 14:30:37.000000 netbluemind5-5.0.7152/netbluemind/domain/api/IDomains.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/domain/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.807432 netbluemind5-5.0.7152/netbluemind/eas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/eas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.811432 netbluemind5-5.0.7152/netbluemind/eas/api/
--rw-r--r--   0 root         (0) root         (0)     1728 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/eas/api/Account.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/eas/api/FolderSyncVersions.py
--rw-r--r--   0 root         (0) root         (0)     1739 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/eas/api/Heartbeat.py
--rw-r--r--   0 root         (0) root         (0)     7128 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/eas/api/IEas.py
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/eas/api/SentItem.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/eas/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.811432 netbluemind5-5.0.7152/netbluemind/externaluser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/externaluser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.811432 netbluemind5-5.0.7152/netbluemind/externaluser/api/
--rw-r--r--   0 root         (0) root         (0)     2153 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/externaluser/api/ExternalUser.py
--rw-r--r--   0 root         (0) root         (0)     6976 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/externaluser/api/IExternalUser.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/externaluser/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.811432 netbluemind5-5.0.7152/netbluemind/filehosting/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/filehosting/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.811432 netbluemind5-5.0.7152/netbluemind/filehosting/api/
--rw-r--r--   0 root         (0) root         (0)     1835 2024-04-11 14:30:36.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/Configuration.py
--rw-r--r--   0 root         (0) root         (0)     2599 2024-04-11 14:30:36.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/FileHostingInfo.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-11 14:30:37.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/FileHostingInfoType.py
--rw-r--r--   0 root         (0) root         (0)     3011 2024-04-11 14:30:36.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/FileHostingItem.py
--rw-r--r--   0 root         (0) root         (0)     1802 2024-04-11 14:30:36.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/FileHostingPublicLink.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-11 14:30:36.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/FileType.py
--rw-r--r--   0 root         (0) root         (0)     6927 2024-04-11 14:30:37.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/IFileHosting.py
--rw-r--r--   0 root         (0) root         (0)     8672 2024-04-11 14:30:36.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/IInternalBMFileSystem.py
--rw-r--r--   0 root         (0) root         (0)     1686 2024-04-11 14:30:36.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/Metadata.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/filehosting/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.811432 netbluemind5-5.0.7152/netbluemind/group/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/group/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.811432 netbluemind5-5.0.7152/netbluemind/group/api/
--rw-r--r--   0 root         (0) root         (0)     3205 2024-04-11 14:30:35.000000 netbluemind5-5.0.7152/netbluemind/group/api/Group.py
--rw-r--r--   0 root         (0) root         (0)     1826 2024-04-11 14:30:35.000000 netbluemind5-5.0.7152/netbluemind/group/api/GroupSearchQuery.py
--rw-r--r--   0 root         (0) root         (0)    17530 2024-04-11 14:30:35.000000 netbluemind5-5.0.7152/netbluemind/group/api/IGroup.py
--rw-r--r--   0 root         (0) root         (0)     2253 2024-04-11 14:30:34.000000 netbluemind5-5.0.7152/netbluemind/group/api/IGroupMember.py
--rw-r--r--   0 root         (0) root         (0)     1965 2024-04-11 14:30:34.000000 netbluemind5-5.0.7152/netbluemind/group/api/Member.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-11 14:30:35.000000 netbluemind5-5.0.7152/netbluemind/group/api/MemberType.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/group/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.811432 netbluemind5-5.0.7152/netbluemind/icalendar/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/icalendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.815432 netbluemind5-5.0.7152/netbluemind/icalendar/api/
--rw-r--r--   0 root         (0) root         (0)    11482 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElement.py
--rw-r--r--   0 root         (0) root         (0)     6703 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementAttendee.py
--rw-r--r--   0 root         (0) root         (0)     1205 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementCUType.py
--rw-r--r--   0 root         (0) root         (0)     1191 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementClassification.py
--rw-r--r--   0 root         (0) root         (0)     2199 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementOrganizer.py
--rw-r--r--   0 root         (0) root         (0)     1294 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementParticipationStatus.py
--rw-r--r--   0 root         (0) root         (0)     6113 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementRRule.py
--rw-r--r--   0 root         (0) root         (0)     1273 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementRRuleFrequency.py
--rw-r--r--   0 root         (0) root         (0)     1749 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementRRuleWeekDay.py
--rw-r--r--   0 root         (0) root         (0)     1235 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementRole.py
--rw-r--r--   0 root         (0) root         (0)     1259 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementStatus.py
--rw-r--r--   0 root         (0) root         (0)     3218 2024-04-11 14:30:30.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementVAlarm.py
--rw-r--r--   0 root         (0) root         (0)     1169 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementVAlarmAction.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/icalendar/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.815432 netbluemind5-5.0.7152/netbluemind/mailbox/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.815432 netbluemind5-5.0.7152/netbluemind/mailbox/api/
--rw-r--r--   0 root         (0) root         (0)     1444 2024-04-11 14:30:08.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/IMailboxAclUids.py
--rw-r--r--   0 root         (0) root         (0)     7069 2024-04-11 14:30:08.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/IMailboxMgmt.py
--rw-r--r--   0 root         (0) root         (0)    19281 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/IMailboxes.py
--rw-r--r--   0 root         (0) root         (0)     3235 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/MailFilter.py
--rw-r--r--   0 root         (0) root         (0)     2069 2024-04-11 14:30:08.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/MailFilterForwarding.py
--rw-r--r--   0 root         (0) root         (0)     2616 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/MailFilterVacation.py
--rw-r--r--   0 root         (0) root         (0)     4279 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/Mailbox.py
--rw-r--r--   0 root         (0) root         (0)     1788 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/MailboxConfig.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/MailboxQuota.py
--rw-r--r--   0 root         (0) root         (0)     1133 2024-04-11 14:30:08.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/MailboxRouting.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-11 14:30:08.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/MailboxType.py
--rw-r--r--   0 root         (0) root         (0)     2940 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/ShardStats.py
--rw-r--r--   0 root         (0) root         (0)     1814 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/ShardStatsMailboxStats.py
--rw-r--r--   0 root         (0) root         (0)     1160 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/ShardStatsState.py
--rw-r--r--   0 root         (0) root         (0)     3617 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/SimpleShardStats.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.815432 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/
--rw-r--r--   0 root         (0) root         (0)     2770 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/DelegationRule.py
--rw-r--r--   0 root         (0) root         (0)     5633 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/MailFilterRule.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/MailFilterRuleTrigger.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/MailFilterRuleType.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.819432 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/
--rw-r--r--   0 root         (0) root         (0)     2390 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleAction.py
--rw-r--r--   0 root         (0) root         (0)     2031 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionAddHeaders.py
--rw-r--r--   0 root         (0) root         (0)     1831 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCategorize.py
--rw-r--r--   0 root         (0) root         (0)     2368 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCopy.py
--rw-r--r--   0 root         (0) root         (0)     2263 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCustom.py
--rw-r--r--   0 root         (0) root         (0)     1763 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionDeferredAction.py
--rw-r--r--   0 root         (0) root         (0)     1742 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionDiscard.py
--rw-r--r--   0 root         (0) root         (0)     1824 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsDeleted.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsImportant.py
--rw-r--r--   0 root         (0) root         (0)     1815 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsRead.py
--rw-r--r--   0 root         (0) root         (0)     2368 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMove.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionName.py
--rw-r--r--   0 root         (0) root         (0)     1831 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionPrioritize.py
--rw-r--r--   0 root         (0) root         (0)     2260 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionRedirect.py
--rw-r--r--   0 root         (0) root         (0)     2091 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionRemoveHeaders.py
--rw-r--r--   0 root         (0) root         (0)     2456 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionReply.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionSetFlags.py
--rw-r--r--   0 root         (0) root         (0)     2538 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionTransfer.py
--rw-r--r--   0 root         (0) root         (0)     1861 2024-04-11 14:30:09.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionUncategorize.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionUnfollow.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.819432 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/
--rw-r--r--   0 root         (0) root         (0)     4268 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleCondition.py
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleConditionOperator.py
--rw-r--r--   0 root         (0) root         (0)     2370 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilter.py
--rw-r--r--   0 root         (0) root         (0)     3837 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContains.py
--rw-r--r--   0 root         (0) root         (0)     1215 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContainsComparator.py
--rw-r--r--   0 root         (0) root         (0)     1263 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContainsModifier.py
--rw-r--r--   0 root         (0) root         (0)     2018 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterEquals.py
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterExists.py
--rw-r--r--   0 root         (0) root         (0)     2021 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterMatches.py
--rw-r--r--   0 root         (0) root         (0)     2509 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterRange.py
--rw-r--r--   0 root         (0) root         (0)     1213 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleOperatorName.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.819432 netbluemind5-5.0.7152/netbluemind/mailbox/identity/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailbox/identity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.819432 netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/
--rw-r--r--   0 root         (0) root         (0)     5175 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/IMailboxIdentity.py
--rw-r--r--   0 root         (0) root         (0)     3330 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/Identity.py
--rw-r--r--   0 root         (0) root         (0)     3421 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/IdentityDescription.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/SignatureFormat.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.819432 netbluemind5-5.0.7152/netbluemind/mailflow/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.819432 netbluemind5-5.0.7152/netbluemind/mailflow/common/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailflow/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.823433 netbluemind5-5.0.7152/netbluemind/mailflow/common/api/
--rw-r--r--   0 root         (0) root         (0)     2218 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/mailflow/common/api/AssignmentActionMapping.py
--rw-r--r--   0 root         (0) root         (0)     2849 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/mailflow/common/api/Message.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/mailflow/common/api/Recipient.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/mailflow/common/api/RecipientAddressType.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/mailflow/common/api/RecipientRecipientType.py
--rw-r--r--   0 root         (0) root         (0)     1714 2024-04-11 14:30:47.000000 netbluemind5-5.0.7152/netbluemind/mailflow/common/api/SendingAs.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailflow/common/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.823433 netbluemind5-5.0.7152/netbluemind/mailmessage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailmessage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.823433 netbluemind5-5.0.7152/netbluemind/mailmessage/api/
--rw-r--r--   0 root         (0) root         (0)     1928 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/mailmessage/api/IMailTip.py
--rw-r--r--   0 root         (0) root         (0)     1755 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTip.py
--rw-r--r--   0 root         (0) root         (0)     2531 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTipContext.py
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTipFilter.py
--rw-r--r--   0 root         (0) root         (0)     1138 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTipFilterFilterType.py
--rw-r--r--   0 root         (0) root         (0)     2519 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTips.py
--rw-r--r--   0 root         (0) root         (0)     3062 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind/mailmessage/api/MessageContext.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailmessage/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.823433 netbluemind5-5.0.7152/netbluemind/mailshare/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailshare/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.823433 netbluemind5-5.0.7152/netbluemind/mailshare/api/
--rw-r--r--   0 root         (0) root         (0)     6859 2024-04-11 14:30:42.000000 netbluemind5-5.0.7152/netbluemind/mailshare/api/IMailshare.py
--rw-r--r--   0 root         (0) root         (0)     3056 2024-04-11 14:30:42.000000 netbluemind5-5.0.7152/netbluemind/mailshare/api/Mailshare.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/mailshare/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.823433 netbluemind5-5.0.7152/netbluemind/notes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/notes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.823433 netbluemind5-5.0.7152/netbluemind/notes/api/
--rw-r--r--   0 root         (0) root         (0)    19136 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/notes/api/INote.py
--rw-r--r--   0 root         (0) root         (0)     2192 2024-04-11 14:30:39.000000 netbluemind5-5.0.7152/netbluemind/notes/api/INoteIndexMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1942 2024-04-11 14:30:39.000000 netbluemind5-5.0.7152/netbluemind/notes/api/INoteUids.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-04-11 14:30:38.000000 netbluemind5-5.0.7152/netbluemind/notes/api/INotes.py
--rw-r--r--   0 root         (0) root         (0)     3598 2024-04-11 14:30:39.000000 netbluemind5-5.0.7152/netbluemind/notes/api/VNote.py
--rw-r--r--   0 root         (0) root         (0)     3333 2024-04-11 14:30:38.000000 netbluemind5-5.0.7152/netbluemind/notes/api/VNoteChanges.py
--rw-r--r--   0 root         (0) root         (0)     2290 2024-04-11 14:30:39.000000 netbluemind5-5.0.7152/netbluemind/notes/api/VNoteChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1842 2024-04-11 14:30:39.000000 netbluemind5-5.0.7152/netbluemind/notes/api/VNoteChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2526 2024-04-11 14:30:39.000000 netbluemind5-5.0.7152/netbluemind/notes/api/VNoteChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-11 14:30:39.000000 netbluemind5-5.0.7152/netbluemind/notes/api/VNoteColor.py
--rw-r--r--   0 root         (0) root         (0)     2169 2024-04-11 14:30:39.000000 netbluemind5-5.0.7152/netbluemind/notes/api/VNoteQuery.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-04-11 14:30:40.000000 netbluemind5-5.0.7152/netbluemind/notes/api/VNotesQuery.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/notes/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.827432 netbluemind5-5.0.7152/netbluemind/python/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 17:44:48.000000 netbluemind5-5.0.7152/netbluemind/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4632 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/python/client.py
--rw-r--r--   0 root         (0) root         (0)     4129 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/python/serder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.827432 netbluemind5-5.0.7152/netbluemind/resource/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/resource/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.827432 netbluemind5-5.0.7152/netbluemind/resource/api/
--rw-r--r--   0 root         (0) root         (0)     1281 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/resource/api/EventInfo.py
--rw-r--r--   0 root         (0) root         (0)     7985 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/resource/api/IResources.py
--rw-r--r--   0 root         (0) root         (0)     3991 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/resource/api/ResourceDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/resource/api/ResourceDescriptorPropertyValue.py
--rw-r--r--   0 root         (0) root         (0)     1204 2024-04-11 14:30:10.000000 netbluemind5-5.0.7152/netbluemind/resource/api/ResourceReservationMode.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/resource/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.827432 netbluemind5-5.0.7152/netbluemind/resource/api/type/
--rw-r--r--   0 root         (0) root         (0)     1458 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/resource/api/type/IResourceTypeUids.py
--rw-r--r--   0 root         (0) root         (0)     5685 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/resource/api/type/IResourceTypes.py
--rw-r--r--   0 root         (0) root         (0)     1761 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/resource/api/type/ResourceType.py
--rw-r--r--   0 root         (0) root         (0)     2692 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/resource/api/type/ResourceTypeDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     2526 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/resource/api/type/ResourceTypeDescriptorProperty.py
--rw-r--r--   0 root         (0) root         (0)     1191 2024-04-11 14:30:11.000000 netbluemind5-5.0.7152/netbluemind/resource/api/type/ResourceTypeDescriptorPropertyType.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/resource/api/type/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.827432 netbluemind5-5.0.7152/netbluemind/role/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/role/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.827432 netbluemind5-5.0.7152/netbluemind/role/api/
--rw-r--r--   0 root         (0) root         (0)     2151 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/role/api/IRoles.py
--rw-r--r--   0 root         (0) root         (0)     5403 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/role/api/RoleDescriptor.py
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/role/api/RolesCategory.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/role/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.827432 netbluemind5-5.0.7152/netbluemind/scheduledjob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.827432 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/
--rw-r--r--   0 root         (0) root         (0)     7252 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/IJob.py
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/Job.py
--rw-r--r--   0 root         (0) root         (0)     2095 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobDomainStatus.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobExecution.py
--rw-r--r--   0 root         (0) root         (0)     3201 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobExecutionQuery.py
--rw-r--r--   0 root         (0) root         (0)     1252 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobExitStatus.py
--rw-r--r--   0 root         (0) root         (0)     1096 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobKind.py
--rw-r--r--   0 root         (0) root         (0)     2961 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobPlanification.py
--rw-r--r--   0 root         (0) root         (0)     2367 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobQuery.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobRec.py
--rw-r--r--   0 root         (0) root         (0)     2734 2024-04-11 14:30:18.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/LogEntry.py
--rw-r--r--   0 root         (0) root         (0)     1133 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/LogLevel.py
--rw-r--r--   0 root         (0) root         (0)     1135 2024-04-11 14:30:17.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/PlanKind.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/scheduledjob/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.831433 netbluemind5-5.0.7152/netbluemind/server/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.831433 netbluemind5-5.0.7152/netbluemind/server/api/
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-11 14:30:35.000000 netbluemind5-5.0.7152/netbluemind/server/api/Assignment.py
--rw-r--r--   0 root         (0) root         (0)     2093 2024-04-11 14:30:35.000000 netbluemind5-5.0.7152/netbluemind/server/api/CommandStatus.py
--rw-r--r--   0 root         (0) root         (0)    12045 2024-04-11 14:30:36.000000 netbluemind5-5.0.7152/netbluemind/server/api/IServer.py
--rw-r--r--   0 root         (0) root         (0)     2108 2024-04-11 14:30:36.000000 netbluemind5-5.0.7152/netbluemind/server/api/Server.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:14.000000 netbluemind5-5.0.7152/netbluemind/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.831433 netbluemind5-5.0.7152/netbluemind/system/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.835433 netbluemind5-5.0.7152/netbluemind/system/api/
--rw-r--r--   0 root         (0) root         (0)     3513 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/CertData.py
--rw-r--r--   0 root         (0) root         (0)     1192 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/CertDataCertificateDomainEngine.py
--rw-r--r--   0 root         (0) root         (0)     4088 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/CloneConfiguration.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/system/api/CloneConfigurationMode.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/ConnectionTestStatus.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/system/api/CustomLogo.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplate.py
--rw-r--r--   0 root         (0) root         (0)     2195 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplateDescription.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplateDescriptionI18NDescription.py
--rw-r--r--   0 root         (0) root         (0)     2858 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplateKind.py
--rw-r--r--   0 root         (0) root         (0)     2999 2024-04-11 14:30:21.000000 netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplateTag.py
--rw-r--r--   0 root         (0) root         (0)     2812 2024-04-11 14:30:21.000000 netbluemind5-5.0.7152/netbluemind/system/api/ExternalSystem.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/ExternalSystemAuthKind.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-04-11 14:30:21.000000 netbluemind5-5.0.7152/netbluemind/system/api/ICacheMgmt.py
--rw-r--r--   0 root         (0) root         (0)     2464 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/ICustomTheme.py
--rw-r--r--   0 root         (0) root         (0)     1545 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/IDomainTemplate.py
--rw-r--r--   0 root         (0) root         (0)     4877 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/IExternalSystem.py
--rw-r--r--   0 root         (0) root         (0)     2369 2024-04-11 14:30:21.000000 netbluemind5-5.0.7152/netbluemind/system/api/IGlobalSettings.py
--rw-r--r--   0 root         (0) root         (0)    17451 2024-04-11 14:30:21.000000 netbluemind5-5.0.7152/netbluemind/system/api/IInstallation.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/system/api/IInternalFirewallMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/IMailDeliveryMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1497 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/system/api/ISchemaMgmt.py
--rw-r--r--   0 root         (0) root         (0)     3421 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/ISecurityMgmt.py
--rw-r--r--   0 root         (0) root         (0)     2092 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/ISystemConfiguration.py
--rw-r--r--   0 root         (0) root         (0)     2488 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/system/api/InstallationVersion.py
--rw-r--r--   0 root         (0) root         (0)     2155 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/system/api/PublicInfos.py
--rw-r--r--   0 root         (0) root         (0)     1965 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/SchemaCheckInfo.py
--rw-r--r--   0 root         (0) root         (0)     7282 2024-04-11 14:30:21.000000 netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformations.py
--rw-r--r--   0 root         (0) root         (0)     3048 2024-04-11 14:30:21.000000 netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsInstallationIndicator.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-04-11 14:30:21.000000 netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsInstallationIndicatorKind.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsKind.py
--rw-r--r--   0 root         (0) root         (0)     3108 2024-04-11 14:30:21.000000 netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsMessage.py
--rw-r--r--   0 root         (0) root         (0)     1248 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsMessageCode.py
--rw-r--r--   0 root         (0) root         (0)     1170 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsMessageKind.py
--rw-r--r--   0 root         (0) root         (0)     1555 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/system/api/SystemConf.py
--rw-r--r--   0 root         (0) root         (0)     1492 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/SystemState.py
--rw-r--r--   0 root         (0) root         (0)     2684 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/UpgradeReport.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/UpgradeReportStatus.py
--rw-r--r--   0 root         (0) root         (0)     1945 2024-04-11 14:30:20.000000 netbluemind5-5.0.7152/netbluemind/system/api/UpgradeReportUpgraderReport.py
--rw-r--r--   0 root         (0) root         (0)     2115 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/UpgradeStatus.py
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-11 14:30:19.000000 netbluemind5-5.0.7152/netbluemind/system/api/UpgradeStatusState.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/system/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.835433 netbluemind5-5.0.7152/netbluemind/system/api/hot/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.835433 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/
--rw-r--r--   0 root         (0) root         (0)     2466 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeProgress.py
--rw-r--r--   0 root         (0) root         (0)     2677 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeStepEvent.py
--rw-r--r--   0 root         (0) root         (0)     1204 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeStepEventStatus.py
--rw-r--r--   0 root         (0) root         (0)     6020 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeTask.py
--rw-r--r--   0 root         (0) root         (0)     1140 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeTaskExecutionMode.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeTaskFilter.py
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-11 14:30:23.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeTaskStatus.py
--rw-r--r--   0 root         (0) root         (0)     3211 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/IHotUpgrade.py
--rw-r--r--   0 root         (0) root         (0)     5213 2024-04-11 14:30:22.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/IInternalHotUpgrade.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.835433 netbluemind5-5.0.7152/netbluemind/tag/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/tag/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.839433 netbluemind5-5.0.7152/netbluemind/tag/api/
--rw-r--r--   0 root         (0) root         (0)     1423 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/tag/api/ITagUids.py
--rw-r--r--   0 root         (0) root         (0)     7268 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/tag/api/ITags.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/tag/api/Tag.py
--rw-r--r--   0 root         (0) root         (0)     3243 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/tag/api/TagChanges.py
--rw-r--r--   0 root         (0) root         (0)     1929 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/tag/api/TagChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-04-11 14:30:14.000000 netbluemind5-5.0.7152/netbluemind/tag/api/TagChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/tag/api/TagChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     2205 2024-04-11 14:30:13.000000 netbluemind5-5.0.7152/netbluemind/tag/api/TagRef.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/tag/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.839433 netbluemind5-5.0.7152/netbluemind/todolist/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/todolist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.839433 netbluemind5-5.0.7152/netbluemind/todolist/api/
--rw-r--r--   0 root         (0) root         (0)    21970 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/ITodoList.py
--rw-r--r--   0 root         (0) root         (0)     3303 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/ITodoLists.py
--rw-r--r--   0 root         (0) root         (0)     2196 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/ITodoListsMgmt.py
--rw-r--r--   0 root         (0) root         (0)     1957 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/ITodoUids.py
--rw-r--r--   0 root         (0) root         (0)     2634 2024-04-11 14:30:28.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/IVTodo.py
--rw-r--r--   0 root         (0) root         (0)     2410 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/TodoListsVTodoQuery.py
--rw-r--r--   0 root         (0) root         (0)     3104 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/VTodo.py
--rw-r--r--   0 root         (0) root         (0)     3369 2024-04-11 14:30:28.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoChanges.py
--rw-r--r--   0 root         (0) root         (0)     2302 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoChangesItemAdd.py
--rw-r--r--   0 root         (0) root         (0)     1842 2024-04-11 14:30:29.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoChangesItemDelete.py
--rw-r--r--   0 root         (0) root         (0)     2538 2024-04-11 14:30:28.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoChangesItemModify.py
--rw-r--r--   0 root         (0) root         (0)     3482 2024-04-11 14:30:27.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoQuery.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/todolist/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.839433 netbluemind5-5.0.7152/netbluemind/user/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/user/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.839433 netbluemind5-5.0.7152/netbluemind/user/api/
--rw-r--r--   0 root         (0) root         (0)     1879 2024-04-11 14:30:06.000000 netbluemind5-5.0.7152/netbluemind/user/api/ChangePassword.py
--rw-r--r--   0 root         (0) root         (0)    17255 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/user/api/IUser.py
--rw-r--r--   0 root         (0) root         (0)     4869 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/user/api/IUserExternalAccount.py
--rw-r--r--   0 root         (0) root         (0)     5750 2024-04-11 14:30:06.000000 netbluemind5-5.0.7152/netbluemind/user/api/IUserMailIdentities.py
--rw-r--r--   0 root         (0) root         (0)     3402 2024-04-11 14:30:06.000000 netbluemind5-5.0.7152/netbluemind/user/api/IUserSettings.py
--rw-r--r--   0 root         (0) root         (0)     4879 2024-04-11 14:30:05.000000 netbluemind5-5.0.7152/netbluemind/user/api/IUserSubscription.py
--rw-r--r--   0 root         (0) root         (0)     5804 2024-04-11 14:30:06.000000 netbluemind5-5.0.7152/netbluemind/user/api/User.py
--rw-r--r--   0 root         (0) root         (0)     2159 2024-04-11 14:30:05.000000 netbluemind5-5.0.7152/netbluemind/user/api/UserAccount.py
--rw-r--r--   0 root         (0) root         (0)     1925 2024-04-11 14:30:07.000000 netbluemind5-5.0.7152/netbluemind/user/api/UserAccountInfo.py
--rw-r--r--   0 root         (0) root         (0)     1861 2024-04-11 14:30:06.000000 netbluemind5-5.0.7152/netbluemind/user/api/UserMailIdentity.py
--rw-r--r--   0 root         (0) root         (0)     1561 2024-04-11 14:30:06.000000 netbluemind5-5.0.7152/netbluemind/user/api/UserSettings.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/user/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.839433 netbluemind5-5.0.7152/netbluemind/webappdata/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/webappdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.839433 netbluemind5-5.0.7152/netbluemind/webappdata/api/
--rw-r--r--   0 root         (0) root         (0)    12898 2024-04-11 14:30:38.000000 netbluemind5-5.0.7152/netbluemind/webappdata/api/IWebAppData.py
--rw-r--r--   0 root         (0) root         (0)     1464 2024-04-11 14:30:38.000000 netbluemind5-5.0.7152/netbluemind/webappdata/api/IWebAppDataUids.py
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-11 14:30:38.000000 netbluemind5-5.0.7152/netbluemind/webappdata/api/WebAppData.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 09:55:16.000000 netbluemind5-5.0.7152/netbluemind/webappdata/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:30:48.843433 netbluemind5-5.0.7152/netbluemind5.egg-info/
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind5.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    26888 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind5.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind5.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind5.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/netbluemind5.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-11 14:30:48.843433 netbluemind5-5.0.7152/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      758 2024-04-11 14:30:48.000000 netbluemind5-5.0.7152/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.411362 netbluemind5-5.0.7187/
+-rw-r--r--   0 root         (0) root         (0)     2232 2024-04-17 12:52:28.000000 netbluemind5-5.0.7187/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-17 12:54:02.415362 netbluemind5-5.0.7187/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2024-04-17 12:52:28.000000 netbluemind5-5.0.7187/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.291360 netbluemind5-5.0.7187/netbluemind/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.291360 netbluemind5-5.0.7187/netbluemind/addressbook/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/addressbook/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.299360 netbluemind5-5.0.7187/netbluemind/addressbook/api/
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/AddressBookDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)    24040 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/IAddressBook.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/IAddressBookUids.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/IAddressBooks.py
+-rw-r--r--   0 root         (0) root         (0)     7034 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/IAddressBooksMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/IVCardService.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCard.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardBasicAttribute.py
+-rw-r--r--   0 root         (0) root         (0)     3405 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     4211 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunications.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunicationsEmail.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunicationsImpp.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunicationsLang.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunicationsTel.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardDeliveryAddressing.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardDeliveryAddressingAddress.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardExplanatory.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardExplanatoryUrl.py
+-rw-r--r--   0 root         (0) root         (0)     5236 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentification.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentificationFormatedName.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentificationGender.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentificationName.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentificationNickname.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardKind.py
+-rw-r--r--   0 root         (0) root         (0)     3115 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardOrganizational.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardOrganizationalMember.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-04-17 12:53:30.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardOrganizationalOrg.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardParameter.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardQueryOrderBy.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardRelated.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardSecurity.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardSecurityKey.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/addressbook/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.299360 netbluemind5-5.0.7187/netbluemind/attachment/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/attachment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.303360 netbluemind5-5.0.7187/netbluemind/attachment/api/
+-rw-r--r--   0 root         (0) root         (0)     2228 2024-04-17 12:53:51.000000 netbluemind5-5.0.7187/netbluemind/attachment/api/AttachedFile.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-17 12:53:51.000000 netbluemind5-5.0.7187/netbluemind/attachment/api/Configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2024-04-17 12:53:51.000000 netbluemind5-5.0.7187/netbluemind/attachment/api/IAttachment.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/attachment/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.303360 netbluemind5-5.0.7187/netbluemind/authentication/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/authentication/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.303360 netbluemind5-5.0.7187/netbluemind/authentication/api/
+-rw-r--r--   0 root         (0) root         (0)     2214 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/APIKey.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/AccessTokenInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/AccessTokenInfoTokenStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/AuthUser.py
+-rw-r--r--   0 root         (0) root         (0)     3891 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/IAPIKeys.py
+-rw-r--r--   0 root         (0) root         (0)     6122 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/IAuthentication.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-04-17 12:53:55.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/ISecurityToken.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2024-04-17 12:53:55.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/ISudoSupport.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-04-17 12:53:55.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/IUserAccessToken.py
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/LoginResponse.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/LoginResponseStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/ValidationKind.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/authentication/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.303360 netbluemind5-5.0.7187/netbluemind/backend/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.303360 netbluemind5-5.0.7187/netbluemind/backend/mail/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.311360 netbluemind5-5.0.7187/netbluemind/backend/mail/api/
+-rw-r--r--   0 root         (0) root         (0)     2669 2024-04-17 12:53:59.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/Conversation.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/ConversationMessageRef.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/DispositionType.py
+-rw-r--r--   0 root         (0) root         (0)    10594 2024-04-17 12:53:59.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IBaseMailboxFolders.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IItemsTransfer.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailConversation.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2024-04-17 12:53:58.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailConversationActions.py
+-rw-r--r--   0 root         (0) root         (0)    19038 2024-04-17 12:53:57.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailboxFolders.py
+-rw-r--r--   0 root         (0) root         (0)    19188 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailboxFoldersByContainer.py
+-rw-r--r--   0 root         (0) root         (0)    20565 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailboxItems.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IOutbox.py
+-rw-r--r--   0 root         (0) root         (0)    10805 2024-04-17 12:53:58.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IReadOnlyMailboxFolders.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/IUserInbox.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImapAck.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-04-17 12:53:58.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImapItemIdentifier.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemSet.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemSetMailboxItemId.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemsStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-17 12:53:55.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportedMailboxItem.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MailboxFolder.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2024-04-17 12:53:57.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MailboxFolderSearchQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MailboxItem.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBody.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBodyHeader.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2024-04-17 12:53:58.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBodyPart.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBodyRecipient.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-04-17 12:53:55.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBodyRecipientKind.py
+-rw-r--r--   0 root         (0) root         (0)     4966 2024-04-17 12:53:55.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageSearchResult.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageSearchResultMbox.py
+-rw-r--r--   0 root         (0) root         (0)     5250 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2024-04-17 12:53:58.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQueryFolderScope.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-04-17 12:53:58.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQueryHeader.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2024-04-17 12:53:57.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQueryHeaderQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-17 12:53:58.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQueryLogicalOperator.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQuerySearchScope.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2024-04-17 12:53:56.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchResult.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-17 12:53:57.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchSort.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-04-17 12:53:55.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchSortOrder.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2024-04-17 12:53:57.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchSortSortCriteria.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.315360 netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/ConversationFlagUpdate.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/FlagUpdate.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/ImportMailboxConversationSet.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/MailboxItemFlag.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-04-17 12:54:00.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/MailboxItemFlagSystem.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.315360 netbluemind5-5.0.7187/netbluemind/calendar/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.323360 netbluemind5-5.0.7187/netbluemind/calendar/api/
+-rw-r--r--   0 root         (0) root         (0)     2788 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2024-04-17 12:53:39.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarLookupResponse.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarLookupResponseType.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarSettingsData.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-17 12:53:40.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarSettingsDataDay.py
+-rw-r--r--   0 root         (0) root         (0)     2770 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarView.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewCalendarViewType.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarsVEventQuery.py
+-rw-r--r--   0 root         (0) root         (0)    23442 2024-04-17 12:53:39.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendar.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2024-04-17 12:53:40.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarAutocomplete.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarSettings.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-17 12:53:40.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarUids.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarView.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarViewUids.py
+-rw-r--r--   0 root         (0) root         (0)     3049 2024-04-17 12:53:38.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendars.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2024-04-17 12:53:39.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarsMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/IFreebusyMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/IFreebusyUids.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/IPrint.py
+-rw-r--r--   0 root         (0) root         (0)     3473 2024-04-17 12:53:39.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/IPublicFreebusy.py
+-rw-r--r--   0 root         (0) root         (0)     3665 2024-04-17 12:53:39.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/IPublishCalendar.py
+-rw-r--r--   0 root         (0) root         (0)    13473 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/IUserCalendarViews.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/IVEvent.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2024-04-17 12:53:39.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/IVFreebusy.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/PrintData.py
+-rw-r--r--   0 root         (0) root         (0)     5946 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptions.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptionsCalendarMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptionsPrintFormat.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptionsPrintLayout.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-17 12:53:40.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptionsPrintView.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/PublishMode.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEvent.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventAttendeeQuery.py
+-rw-r--r--   0 root         (0) root         (0)     3402 2024-04-17 12:53:40.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2024-04-17 12:53:40.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventCounter.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventCounterCounterOriginator.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventOccurrence.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2024-04-17 12:53:40.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventQuery.py
+-rw-r--r--   0 root         (0) root         (0)     3935 2024-04-17 12:53:40.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventSeries.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-17 12:53:39.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VEventTransparency.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-04-17 12:53:39.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VFreebusy.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-04-17 12:53:39.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VFreebusyQuery.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2024-04-17 12:53:37.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VFreebusySlot.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/VFreebusyType.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/calendar/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.323360 netbluemind5-5.0.7187/netbluemind/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.327360 netbluemind5-5.0.7187/netbluemind/core/api/
+-rw-r--r--   0 root         (0) root         (0)     2011 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/api/Email.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/api/ImportStats.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/api/ListResult.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/api/VersionInfo.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/core/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.327360 netbluemind5-5.0.7187/netbluemind/core/api/date/
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/api/date/BmDateTime.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/api/date/BmDateTimePrecision.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/core/api/date/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.327360 netbluemind5-5.0.7187/netbluemind/core/api/fault/
+-rw-r--r--   0 root         (0) root         (0)     5200 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/api/fault/ErrorCode.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:14.000000 netbluemind5-5.0.7187/netbluemind/core/api/fault/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.327360 netbluemind5-5.0.7187/netbluemind/core/container/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/core/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.331360 netbluemind5-5.0.7187/netbluemind/core/container/api/
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-04-17 12:53:45.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/Ack.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2024-04-17 12:53:46.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerHierarchyNode.py
+-rw-r--r--   0 root         (0) root         (0)     2906 2024-04-17 12:53:47.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2024-04-17 12:53:47.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerSettingsKeys.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-04-17 12:53:48.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerSubscription.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2024-04-17 12:53:46.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerSubscriptionDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2024-04-17 12:53:47.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerSubscriptionModel.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2024-04-17 12:53:46.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/Count.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2024-04-17 12:53:45.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IChangelogSupport.py
+-rw-r--r--   0 root         (0) root         (0)    11391 2024-04-17 12:53:48.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IContainerManagement.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2024-04-17 12:53:47.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IContainerSync.py
+-rw-r--r--   0 root         (0) root         (0)    12400 2024-04-17 12:53:46.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IContainers.py
+-rw-r--r--   0 root         (0) root         (0)    10022 2024-04-17 12:53:46.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IContainersFlatHierarchy.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2024-04-17 12:53:47.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/ICountingSupport.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-04-17 12:53:46.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IFlatHierarchyUids.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2024-04-17 12:53:47.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IOfflineMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2024-04-17 12:53:45.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IOwnerSubscriptionUids.py
+-rw-r--r--   0 root         (0) root         (0)    11454 2024-04-17 12:53:47.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IOwnerSubscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2024-04-17 12:53:45.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/ISortingSupport.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-04-17 12:53:47.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/IdRange.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/core/container/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.335361 netbluemind5-5.0.7187/netbluemind/core/container/model/
+-rw-r--r--   0 root         (0) root         (0)     4694 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/BaseContainerDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     3777 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ChangeLogEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ChangeLogEntryType.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerChangelog.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerChangeset.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerModifiableDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2861 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerSyncResult.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerSyncStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerSyncStatusStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3489 2024-04-17 12:53:45.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerUpdatesResult.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerUpdatesResultInError.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/CountFastPath.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/IdQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemChangeLogEntry.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemChangelog.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2024-04-17 12:53:45.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemContainerValue.py
+-rw-r--r--   0 root         (0) root         (0)     4056 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemFlag.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemFlagFilter.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemIdentifier.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemUri.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemValue.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/ItemVersion.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-04-17 12:53:45.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/SortDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/SortDescriptorDirection.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/SortDescriptorField.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.339361 netbluemind5-5.0.7187/netbluemind/core/container/model/acl/
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-17 12:53:45.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/acl/AccessControlEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-17 12:53:45.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/acl/Verb.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/core/container/model/acl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.339361 netbluemind5-5.0.7187/netbluemind/core/task/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/core/task/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.339361 netbluemind5-5.0.7187/netbluemind/core/task/api/
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-04-17 12:53:44.000000 netbluemind5-5.0.7187/netbluemind/core/task/api/ITask.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/core/task/api/TaskRef.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/core/task/api/TaskStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/core/task/api/TaskStatusState.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/core/task/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.339361 netbluemind5-5.0.7187/netbluemind/cti/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/cti/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.339361 netbluemind5-5.0.7187/netbluemind/cti/api/
+-rw-r--r--   0 root         (0) root         (0)     4038 2024-04-17 12:54:02.000000 netbluemind5-5.0.7187/netbluemind/cti/api/IComputerTelephonyIntegration.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-04-17 12:54:02.000000 netbluemind5-5.0.7187/netbluemind/cti/api/Status.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-04-17 12:54:02.000000 netbluemind5-5.0.7187/netbluemind/cti/api/StatusPhoneState.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/cti/api/StatusType.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/cti/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.339361 netbluemind5-5.0.7187/netbluemind/dataprotect/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.343361 netbluemind5-5.0.7187/netbluemind/dataprotect/api/
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/DataProtectGeneration.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/GenerationContent.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/GenerationStatus.py
+-rw-r--r--   0 root         (0) root         (0)     8292 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/IDataProtect.py
+-rw-r--r--   0 root         (0) root         (0)     4132 2024-04-17 12:53:32.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/PartGeneration.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/Restorable.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/RestorableKind.py
+-rw-r--r--   0 root         (0) root         (0)     2507 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/RestoreDefinition.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/RestoreOperation.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/RetentionPolicy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/dataprotect/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.343361 netbluemind5-5.0.7187/netbluemind/device/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/device/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.343361 netbluemind5-5.0.7187/netbluemind/device/api/
+-rw-r--r--   0 root         (0) root         (0)     4714 2024-04-17 12:53:32.000000 netbluemind5-5.0.7187/netbluemind/device/api/Device.py
+-rw-r--r--   0 root         (0) root         (0)     8584 2024-04-17 12:53:32.000000 netbluemind5-5.0.7187/netbluemind/device/api/IDevice.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2024-04-17 12:53:32.000000 netbluemind5-5.0.7187/netbluemind/device/api/IDeviceUids.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-04-17 12:53:32.000000 netbluemind5-5.0.7187/netbluemind/device/api/IDevices.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-17 12:53:32.000000 netbluemind5-5.0.7187/netbluemind/device/api/WipeMode.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/device/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.343361 netbluemind5-5.0.7187/netbluemind/directory/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/directory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.347361 netbluemind5-5.0.7187/netbluemind/directory/api/
+-rw-r--r--   0 root         (0) root         (0)     3091 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/BaseDirEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/directory/api/BaseDirEntryAccountType.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/BaseDirEntryKind.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/DirBaseValue.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2024-04-17 12:53:26.000000 netbluemind5-5.0.7187/netbluemind/directory/api/DirEntry.py
+-rw-r--r--   0 root         (0) root         (0)     7466 2024-04-17 12:53:26.000000 netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQueryDir.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQueryOrder.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQueryOrderBy.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQueryStateFilter.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/IDirEntryMaintenance.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/directory/api/IDirEntryPath.py
+-rw-r--r--   0 root         (0) root         (0)    13515 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/directory/api/IDirectory.py
+-rw-r--r--   0 root         (0) root         (0)     9387 2024-04-17 12:53:26.000000 netbluemind5-5.0.7187/netbluemind/directory/api/IOrgUnits.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/directory/api/MaintenanceOperation.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/OrgUnit.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/directory/api/OrgUnitPath.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/directory/api/OrgUnitQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/directory/api/RepairConfig.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/directory/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.347361 netbluemind5-5.0.7187/netbluemind/document/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/document/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.347361 netbluemind5-5.0.7187/netbluemind/document/api/
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/document/api/Document.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/document/api/DocumentMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/document/api/IDocument.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/document/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.347361 netbluemind5-5.0.7187/netbluemind/documentfolder/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/documentfolder/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.351361 netbluemind5-5.0.7187/netbluemind/documentfolder/api/
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/documentfolder/api/DocumentFolder.py
+-rw-r--r--   0 root         (0) root         (0)     4166 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/documentfolder/api/IDocumentFolder.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2024-04-17 12:53:28.000000 netbluemind5-5.0.7187/netbluemind/documentfolder/api/IDocumentFolderUids.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/documentfolder/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.351361 netbluemind5-5.0.7187/netbluemind/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.351361 netbluemind5-5.0.7187/netbluemind/domain/api/
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-04-17 12:53:50.000000 netbluemind5-5.0.7187/netbluemind/domain/api/Domain.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2024-04-17 12:53:51.000000 netbluemind5-5.0.7187/netbluemind/domain/api/IDomainSettings.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2024-04-17 12:53:51.000000 netbluemind5-5.0.7187/netbluemind/domain/api/IDomains.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/domain/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.351361 netbluemind5-5.0.7187/netbluemind/eas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/eas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.351361 netbluemind5-5.0.7187/netbluemind/eas/api/
+-rw-r--r--   0 root         (0) root         (0)     1728 2024-04-17 12:53:53.000000 netbluemind5-5.0.7187/netbluemind/eas/api/Account.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/eas/api/FolderSyncVersions.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-04-17 12:53:53.000000 netbluemind5-5.0.7187/netbluemind/eas/api/Heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/eas/api/IEas.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-17 12:53:54.000000 netbluemind5-5.0.7187/netbluemind/eas/api/SentItem.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/eas/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.351361 netbluemind5-5.0.7187/netbluemind/externaluser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/externaluser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.351361 netbluemind5-5.0.7187/netbluemind/externaluser/api/
+-rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/externaluser/api/ExternalUser.py
+-rw-r--r--   0 root         (0) root         (0)     6976 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/externaluser/api/IExternalUser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/externaluser/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.351361 netbluemind5-5.0.7187/netbluemind/filehosting/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/filehosting/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.355361 netbluemind5-5.0.7187/netbluemind/filehosting/api/
+-rw-r--r--   0 root         (0) root         (0)     1835 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/Configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/FileHostingInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-17 12:53:50.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/FileHostingInfoType.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2024-04-17 12:53:50.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/FileHostingItem.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2024-04-17 12:53:50.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/FileHostingPublicLink.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/FileType.py
+-rw-r--r--   0 root         (0) root         (0)     6927 2024-04-17 12:53:50.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/IFileHosting.py
+-rw-r--r--   0 root         (0) root         (0)     8672 2024-04-17 12:53:50.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/IInternalBMFileSystem.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2024-04-17 12:53:50.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/Metadata.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/filehosting/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.355361 netbluemind5-5.0.7187/netbluemind/group/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/group/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.355361 netbluemind5-5.0.7187/netbluemind/group/api/
+-rw-r--r--   0 root         (0) root         (0)     3205 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/group/api/Group.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/group/api/GroupSearchQuery.py
+-rw-r--r--   0 root         (0) root         (0)    17530 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/group/api/IGroup.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-17 12:53:48.000000 netbluemind5-5.0.7187/netbluemind/group/api/IGroupMember.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2024-04-17 12:53:48.000000 netbluemind5-5.0.7187/netbluemind/group/api/Member.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/group/api/MemberType.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/group/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.355361 netbluemind5-5.0.7187/netbluemind/icalendar/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/icalendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.359361 netbluemind5-5.0.7187/netbluemind/icalendar/api/
+-rw-r--r--   0 root         (0) root         (0)    11482 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElement.py
+-rw-r--r--   0 root         (0) root         (0)     6703 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementAttendee.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementCUType.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementOrganizer.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementParticipationStatus.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementRRule.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementRRuleFrequency.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementRRuleWeekDay.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementRole.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3218 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementVAlarm.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementVAlarmAction.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:16.000000 netbluemind5-5.0.7187/netbluemind/icalendar/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.359361 netbluemind5-5.0.7187/netbluemind/mailbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.363361 netbluemind5-5.0.7187/netbluemind/mailbox/api/
+-rw-r--r--   0 root         (0) root         (0)     1444 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/IMailboxAclUids.py
+-rw-r--r--   0 root         (0) root         (0)     7069 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/IMailboxMgmt.py
+-rw-r--r--   0 root         (0) root         (0)    29554 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/IMailboxes.py
+-rw-r--r--   0 root         (0) root         (0)     3235 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/MailFilter.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/MailFilterForwarding.py
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/MailFilterVacation.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/Mailbox.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/MailboxConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/MailboxQuota.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/MailboxRouting.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/MailboxType.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/ShardStats.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/ShardStatsMailboxStats.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/ShardStatsState.py
+-rw-r--r--   0 root         (0) root         (0)     3617 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/SimpleShardStats.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.363361 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/
+-rw-r--r--   0 root         (0) root         (0)     2770 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/DelegationRule.py
+-rw-r--r--   0 root         (0) root         (0)     5815 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/MailFilterRule.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/MailFilterRuleTrigger.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/MailFilterRuleType.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/RuleMoveDirection.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/RuleMoveRelativePosition.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.367361 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleAction.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionAddHeaders.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCategorize.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCopy.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCustom.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionDeferredAction.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionDiscard.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsDeleted.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsImportant.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsRead.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMove.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionName.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionPrioritize.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionRedirect.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionRemoveHeaders.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionReply.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionSetFlags.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionTransfer.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionUncategorize.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-04-17 12:53:23.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionUnfollow.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.371361 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/
+-rw-r--r--   0 root         (0) root         (0)     4268 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleCondition.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleConditionOperator.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilter.py
+-rw-r--r--   0 root         (0) root         (0)     3837 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContains.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContainsComparator.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContainsModifier.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterEquals.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterExists.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterMatches.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterRange.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleOperatorName.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.371361 netbluemind5-5.0.7187/netbluemind/mailbox/identity/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailbox/identity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.371361 netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/
+-rw-r--r--   0 root         (0) root         (0)     5175 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/IMailboxIdentity.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2024-04-17 12:53:20.000000 netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/Identity.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2024-04-17 12:53:21.000000 netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/IdentityDescription.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-04-17 12:53:20.000000 netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/SignatureFormat.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.371361 netbluemind5-5.0.7187/netbluemind/mailflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.371361 netbluemind5-5.0.7187/netbluemind/mailflow/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailflow/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.371361 netbluemind5-5.0.7187/netbluemind/mailflow/common/api/
+-rw-r--r--   0 root         (0) root         (0)     2218 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailflow/common/api/AssignmentActionMapping.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailflow/common/api/Message.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailflow/common/api/Recipient.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailflow/common/api/RecipientAddressType.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailflow/common/api/RecipientRecipientType.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailflow/common/api/SendingAs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailflow/common/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.371361 netbluemind5-5.0.7187/netbluemind/mailmessage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailmessage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.375362 netbluemind5-5.0.7187/netbluemind/mailmessage/api/
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailmessage/api/IMailTip.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTip.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTipContext.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTipFilter.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTipFilterFilterType.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTips.py
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-04-17 12:54:01.000000 netbluemind5-5.0.7187/netbluemind/mailmessage/api/MessageContext.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailmessage/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.375362 netbluemind5-5.0.7187/netbluemind/mailshare/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailshare/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.375362 netbluemind5-5.0.7187/netbluemind/mailshare/api/
+-rw-r--r--   0 root         (0) root         (0)     6859 2024-04-17 12:53:55.000000 netbluemind5-5.0.7187/netbluemind/mailshare/api/IMailshare.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2024-04-17 12:53:55.000000 netbluemind5-5.0.7187/netbluemind/mailshare/api/Mailshare.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/mailshare/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.375362 netbluemind5-5.0.7187/netbluemind/notes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/notes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.379362 netbluemind5-5.0.7187/netbluemind/notes/api/
+-rw-r--r--   0 root         (0) root         (0)    19136 2024-04-17 12:53:53.000000 netbluemind5-5.0.7187/netbluemind/notes/api/INote.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/INoteIndexMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/INoteUids.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/INotes.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/VNote.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/VNoteChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/VNoteChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/VNoteChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/VNoteChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/VNoteColor.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/notes/api/VNoteQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-17 12:53:53.000000 netbluemind5-5.0.7187/netbluemind/notes/api/VNotesQuery.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/notes/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.379362 netbluemind5-5.0.7187/netbluemind/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 17:44:48.000000 netbluemind5-5.0.7187/netbluemind/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/python/client.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/python/serder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.379362 netbluemind5-5.0.7187/netbluemind/resource/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/resource/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.383362 netbluemind5-5.0.7187/netbluemind/resource/api/
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/resource/api/EventInfo.py
+-rw-r--r--   0 root         (0) root         (0)     7985 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/resource/api/IResources.py
+-rw-r--r--   0 root         (0) root         (0)     3991 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/resource/api/ResourceDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/resource/api/ResourceDescriptorPropertyValue.py
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-17 12:53:24.000000 netbluemind5-5.0.7187/netbluemind/resource/api/ResourceReservationMode.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/resource/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.383362 netbluemind5-5.0.7187/netbluemind/resource/api/type/
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/resource/api/type/IResourceTypeUids.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/resource/api/type/IResourceTypes.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/resource/api/type/ResourceType.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/resource/api/type/ResourceTypeDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/resource/api/type/ResourceTypeDescriptorProperty.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-04-17 12:53:25.000000 netbluemind5-5.0.7187/netbluemind/resource/api/type/ResourceTypeDescriptorPropertyType.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/resource/api/type/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.383362 netbluemind5-5.0.7187/netbluemind/role/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/role/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.383362 netbluemind5-5.0.7187/netbluemind/role/api/
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-04-17 12:53:32.000000 netbluemind5-5.0.7187/netbluemind/role/api/IRoles.py
+-rw-r--r--   0 root         (0) root         (0)     5403 2024-04-17 12:53:32.000000 netbluemind5-5.0.7187/netbluemind/role/api/RoleDescriptor.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/role/api/RolesCategory.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/role/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.383362 netbluemind5-5.0.7187/netbluemind/scheduledjob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.387362 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/
+-rw-r--r--   0 root         (0) root         (0)     7252 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/IJob.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/Job.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobDomainStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobExecution.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobExecutionQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobExitStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobKind.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobPlanification.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobQuery.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobRec.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/LogEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/LogLevel.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-04-17 12:53:31.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/PlanKind.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/scheduledjob/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.387362 netbluemind5-5.0.7187/netbluemind/server/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.387362 netbluemind5-5.0.7187/netbluemind/server/api/
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/server/api/Assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/server/api/CommandStatus.py
+-rw-r--r--   0 root         (0) root         (0)    12045 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/server/api/IServer.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-17 12:53:49.000000 netbluemind5-5.0.7187/netbluemind/server/api/Server.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.391362 netbluemind5-5.0.7187/netbluemind/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/system/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.399362 netbluemind5-5.0.7187/netbluemind/system/api/
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/CertData.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2024-04-17 12:53:34.000000 netbluemind5-5.0.7187/netbluemind/system/api/CertDataCertificateDomainEngine.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/CloneConfiguration.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/CloneConfigurationMode.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/ConnectionTestStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/CustomLogo.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplate.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-04-17 12:53:34.000000 netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplateDescription.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-17 12:53:34.000000 netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplateDescriptionI18NDescription.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2024-04-17 12:53:34.000000 netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplateKind.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplateTag.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/ExternalSystem.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/ExternalSystemAuthKind.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/ICacheMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/ICustomTheme.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/IDomainTemplate.py
+-rw-r--r--   0 root         (0) root         (0)     4877 2024-04-17 12:53:34.000000 netbluemind5-5.0.7187/netbluemind/system/api/IExternalSystem.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/IGlobalSettings.py
+-rw-r--r--   0 root         (0) root         (0)    17451 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/IInstallation.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/IInternalFirewallMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-17 12:53:34.000000 netbluemind5-5.0.7187/netbluemind/system/api/IMailDeliveryMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/ISchemaMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/ISecurityMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/ISystemConfiguration.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/InstallationVersion.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/PublicInfos.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/SchemaCheckInfo.py
+-rw-r--r--   0 root         (0) root         (0)     7282 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformations.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsInstallationIndicator.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsInstallationIndicatorKind.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsKind.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsMessage.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-04-17 12:53:34.000000 netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsMessageCode.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2024-04-17 12:53:34.000000 netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsMessageKind.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/SystemConf.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/SystemState.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2024-04-17 12:53:34.000000 netbluemind5-5.0.7187/netbluemind/system/api/UpgradeReport.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/UpgradeReportStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/UpgradeReportUpgraderReport.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-17 12:53:35.000000 netbluemind5-5.0.7187/netbluemind/system/api/UpgradeStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-17 12:53:33.000000 netbluemind5-5.0.7187/netbluemind/system/api/UpgradeStatusState.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/system/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.399362 netbluemind5-5.0.7187/netbluemind/system/api/hot/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.403362 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeProgress.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeStepEvent.py
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeStepEventStatus.py
+-rw-r--r--   0 root         (0) root         (0)     6020 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeTask.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeTaskExecutionMode.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeTaskFilter.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeTaskStatus.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/IHotUpgrade.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2024-04-17 12:53:36.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/IInternalHotUpgrade.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.403362 netbluemind5-5.0.7187/netbluemind/tag/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/tag/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.403362 netbluemind5-5.0.7187/netbluemind/tag/api/
+-rw-r--r--   0 root         (0) root         (0)     1423 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/tag/api/ITagUids.py
+-rw-r--r--   0 root         (0) root         (0)     7268 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/tag/api/ITags.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/tag/api/Tag.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/tag/api/TagChanges.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/tag/api/TagChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/tag/api/TagChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/tag/api/TagChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2024-04-17 12:53:27.000000 netbluemind5-5.0.7187/netbluemind/tag/api/TagRef.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/tag/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.403362 netbluemind5-5.0.7187/netbluemind/todolist/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/todolist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.407362 netbluemind5-5.0.7187/netbluemind/todolist/api/
+-rw-r--r--   0 root         (0) root         (0)    21970 2024-04-17 12:53:42.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/ITodoList.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/ITodoLists.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/ITodoListsMgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/ITodoUids.py
+-rw-r--r--   0 root         (0) root         (0)     2634 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/IVTodo.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/TodoListsVTodoQuery.py
+-rw-r--r--   0 root         (0) root         (0)     3104 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/VTodo.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoChanges.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-17 12:53:42.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoChangesItemAdd.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2024-04-17 12:53:43.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoChangesItemDelete.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoChangesItemModify.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-04-17 12:53:41.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoQuery.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/todolist/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.407362 netbluemind5-5.0.7187/netbluemind/user/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/user/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.411362 netbluemind5-5.0.7187/netbluemind/user/api/
+-rw-r--r--   0 root         (0) root         (0)     1879 2024-04-17 12:53:19.000000 netbluemind5-5.0.7187/netbluemind/user/api/ChangePassword.py
+-rw-r--r--   0 root         (0) root         (0)    17255 2024-04-17 12:53:20.000000 netbluemind5-5.0.7187/netbluemind/user/api/IUser.py
+-rw-r--r--   0 root         (0) root         (0)     4869 2024-04-17 12:53:20.000000 netbluemind5-5.0.7187/netbluemind/user/api/IUserExternalAccount.py
+-rw-r--r--   0 root         (0) root         (0)     5750 2024-04-17 12:53:19.000000 netbluemind5-5.0.7187/netbluemind/user/api/IUserMailIdentities.py
+-rw-r--r--   0 root         (0) root         (0)     3402 2024-04-17 12:53:19.000000 netbluemind5-5.0.7187/netbluemind/user/api/IUserSettings.py
+-rw-r--r--   0 root         (0) root         (0)     4879 2024-04-17 12:53:19.000000 netbluemind5-5.0.7187/netbluemind/user/api/IUserSubscription.py
+-rw-r--r--   0 root         (0) root         (0)     5804 2024-04-17 12:53:19.000000 netbluemind5-5.0.7187/netbluemind/user/api/User.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2024-04-17 12:53:19.000000 netbluemind5-5.0.7187/netbluemind/user/api/UserAccount.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2024-04-17 12:53:20.000000 netbluemind5-5.0.7187/netbluemind/user/api/UserAccountInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2024-04-17 12:53:19.000000 netbluemind5-5.0.7187/netbluemind/user/api/UserMailIdentity.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2024-04-17 12:53:19.000000 netbluemind5-5.0.7187/netbluemind/user/api/UserSettings.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/user/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.411362 netbluemind5-5.0.7187/netbluemind/webappdata/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/webappdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.411362 netbluemind5-5.0.7187/netbluemind/webappdata/api/
+-rw-r--r--   0 root         (0) root         (0)    12898 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/webappdata/api/IWebAppData.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/webappdata/api/IWebAppDataUids.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-17 12:53:52.000000 netbluemind5-5.0.7187/netbluemind/webappdata/api/WebAppData.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 08:39:18.000000 netbluemind5-5.0.7187/netbluemind/webappdata/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:54:02.411362 netbluemind5-5.0.7187/netbluemind5.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-17 12:54:02.000000 netbluemind5-5.0.7187/netbluemind5.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    26997 2024-04-17 12:54:02.000000 netbluemind5-5.0.7187/netbluemind5.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 12:54:02.000000 netbluemind5-5.0.7187/netbluemind5.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-17 12:54:02.000000 netbluemind5-5.0.7187/netbluemind5.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-17 12:54:02.000000 netbluemind5-5.0.7187/netbluemind5.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-17 12:54:02.415362 netbluemind5-5.0.7187/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-17 12:54:02.000000 netbluemind5-5.0.7187/setup.py
```

### Comparing `netbluemind5-5.0.7152/LICENSE.txt` & `netbluemind5-5.0.7187/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/AddressBookDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/AddressBookDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/IAddressBook.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/IAddressBook.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAddressBook_VERSION = "5.0.7152"
+IAddressBook_VERSION = "5.0.7187"
 
 
 class IAddressBook(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/addressbooks/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/IAddressBookUids.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/IAddressBookUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAddressBookUids_VERSION = "5.0.7152"
+IAddressBookUids_VERSION = "5.0.7187"
 
 
 class IAddressBookUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/addressbook/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/IAddressBooks.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/IAddressBooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAddressBooks_VERSION = "5.0.7152"
+IAddressBooks_VERSION = "5.0.7187"
 
 
 class IAddressBooks(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/addressbooks'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/IAddressBooksMgmt.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/IAddressBooksMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAddressBooksMgmt_VERSION = "5.0.7152"
+IAddressBooksMgmt_VERSION = "5.0.7187"
 
 
 class IAddressBooksMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/addressbooks'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/IVCardService.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/IVCardService.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IVCardService_VERSION = "5.0.7152"
+IVCardService_VERSION = "5.0.7187"
 
 
 class IVCardService(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/addressbooks/vcards/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCard.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCard.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardBasicAttribute.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardBasicAttribute.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardChanges.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardChangesItemAdd.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardChangesItemDelete.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardChangesItemModify.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunications.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunications.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunicationsEmail.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunicationsEmail.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunicationsImpp.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunicationsImpp.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunicationsLang.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunicationsLang.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardCommunicationsTel.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardCommunicationsTel.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardDeliveryAddressing.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardDeliveryAddressing.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardDeliveryAddressingAddress.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardDeliveryAddressingAddress.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardExplanatory.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardExplanatory.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardExplanatoryUrl.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardExplanatoryUrl.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentification.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentification.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentificationFormatedName.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentificationFormatedName.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentificationGender.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentificationGender.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentificationName.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentificationName.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardIdentificationNickname.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardIdentificationNickname.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardInfo.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardKind.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardOrganizational.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardOrganizational.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardOrganizationalMember.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardOrganizationalMember.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardOrganizationalOrg.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardOrganizationalOrg.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardParameter.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardParameter.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardQuery.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardQueryOrderBy.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardQueryOrderBy.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardRelated.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardRelated.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardSecurity.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardSecurity.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/addressbook/api/VCardSecurityKey.py` & `netbluemind5-5.0.7187/netbluemind/addressbook/api/VCardSecurityKey.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/attachment/api/AttachedFile.py` & `netbluemind5-5.0.7187/netbluemind/attachment/api/AttachedFile.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/attachment/api/Configuration.py` & `netbluemind5-5.0.7187/netbluemind/attachment/api/Configuration.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/attachment/api/IAttachment.py` & `netbluemind5-5.0.7187/netbluemind/attachment/api/IAttachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAttachment_VERSION = "5.0.7152"
+IAttachment_VERSION = "5.0.7187"
 
 
 class IAttachment(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/attachment/{domainUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/APIKey.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/APIKey.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/AccessTokenInfo.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/AccessTokenInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/AccessTokenInfoTokenStatus.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/AccessTokenInfoTokenStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/AuthUser.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/AuthUser.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/IAPIKeys.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/IAPIKeys.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAPIKeys_VERSION = "5.0.7152"
+IAPIKeys_VERSION = "5.0.7187"
 
 
 class IAPIKeys(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth/keys'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/IAuthentication.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/IAuthentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IAuthentication_VERSION = "5.0.7152"
+IAuthentication_VERSION = "5.0.7187"
 
 
 class IAuthentication(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/ISecurityToken.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/ISecurityToken.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISecurityToken_VERSION = "5.0.7152"
+ISecurityToken_VERSION = "5.0.7187"
 
 
 class ISecurityToken(BaseEndpoint):
     def __init__(self, apiKey, url, sessionIdentifier):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth/token/{sessionIdentifier}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/ISudoSupport.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/ISudoSupport.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISudoSupport_VERSION = "5.0.7152"
+ISudoSupport_VERSION = "5.0.7187"
 
 
 class ISudoSupport(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth/sudo_support'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/IUserAccessToken.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/IUserAccessToken.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserAccessToken_VERSION = "5.0.7152"
+IUserAccessToken_VERSION = "5.0.7187"
 
 
 class IUserAccessToken(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/auth/access_token'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/LoginResponse.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/LoginResponse.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/LoginResponseStatus.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/LoginResponseStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/authentication/api/ValidationKind.py` & `netbluemind5-5.0.7187/netbluemind/authentication/api/ValidationKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/Conversation.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/Conversation.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/ConversationMessageRef.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/ConversationMessageRef.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/DispositionType.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/DispositionType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IBaseMailboxFolders.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IBaseMailboxFolders.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IBaseMailboxFolders_VERSION = "5.0.7152"
+IBaseMailboxFolders_VERSION = "5.0.7187"
 
 
 class IBaseMailboxFolders(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IItemsTransfer.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IItemsTransfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IItemsTransfer_VERSION = "5.0.7152"
+IItemsTransfer_VERSION = "5.0.7187"
 
 
 class IItemsTransfer(BaseEndpoint):
     def __init__(self, apiKey, url, fromMailboxUid, toMailboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + \
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailConversation.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailConversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailConversation_VERSION = "5.0.7152"
+IMailConversation_VERSION = "5.0.7187"
 
 
 class IMailConversation(BaseEndpoint):
     def __init__(self, apiKey, url, subtreeContainer):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mail_conversation/{subtreeContainer}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailConversationActions.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailConversationActions.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailConversationActions_VERSION = "5.0.7152"
+IMailConversationActions_VERSION = "5.0.7187"
 
 
 class IMailConversationActions(BaseEndpoint):
     def __init__(self, apiKey, url, conversationContainer, replicatedMailboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + \
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailboxFolders.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailboxFolders.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxFolders_VERSION = "5.0.7152"
+IMailboxFolders_VERSION = "5.0.7187"
 
 
 class IMailboxFolders(BaseEndpoint):
     def __init__(self, apiKey, url, partition, mailboxRoot):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mail_folders/{partition}/{mailboxRoot}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailboxFoldersByContainer.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailboxFoldersByContainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxFoldersByContainer_VERSION = "5.0.7152"
+IMailboxFoldersByContainer_VERSION = "5.0.7187"
 
 
 class IMailboxFoldersByContainer(BaseEndpoint):
     def __init__(self, apiKey, url, container):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mail_folders_container/{container}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IMailboxItems.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IMailboxItems.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxItems_VERSION = "5.0.7152"
+IMailboxItems_VERSION = "5.0.7187"
 
 
 class IMailboxItems(BaseEndpoint):
     def __init__(self, apiKey, url, replicatedMailboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mail_items/{replicatedMailboxUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IOutbox.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IOutbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOutbox_VERSION = "5.0.7152"
+IOutbox_VERSION = "5.0.7187"
 
 
 class IOutbox(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, mailboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/outbox/{domainUid}/{mailboxUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IReadOnlyMailboxFolders.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IReadOnlyMailboxFolders.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IReadOnlyMailboxFolders_VERSION = "5.0.7152"
+IReadOnlyMailboxFolders_VERSION = "5.0.7187"
 
 
 class IReadOnlyMailboxFolders(BaseEndpoint):
     def __init__(self, apiKey, url, container):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/db_replicated_mailboxes_folders/{container}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/IUserInbox.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/IUserInbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserInbox_VERSION = "5.0.7152"
+IUserInbox_VERSION = "5.0.7187"
 
 
 class IUserInbox(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/inbox/{domainUid}/{userUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImapAck.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImapAck.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImapItemIdentifier.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImapItemIdentifier.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemSet.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemSet.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemSetMailboxItemId.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemSetMailboxItemId.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemsStatus.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemsStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportStatus.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportedMailboxItem.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/ImportMailboxItemsStatusImportedMailboxItem.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MailboxFolder.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MailboxFolder.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MailboxFolderSearchQuery.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MailboxFolderSearchQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MailboxItem.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MailboxItem.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBody.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBody.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBodyHeader.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBodyHeader.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBodyPart.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBodyPart.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBodyRecipient.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBodyRecipient.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageBodyRecipientKind.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageBodyRecipientKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageSearchResult.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageSearchResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/MessageSearchResultMbox.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/MessageSearchResultMbox.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQuery.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQueryFolderScope.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQueryFolderScope.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQueryHeader.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQueryHeader.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQueryHeaderQuery.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQueryHeaderQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQueryLogicalOperator.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQueryLogicalOperator.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchQuerySearchScope.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchQuerySearchScope.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchResult.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchSort.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchSort.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchSortOrder.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchSortOrder.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/SearchSortSortCriteria.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/SearchSortSortCriteria.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/ConversationFlagUpdate.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/ConversationFlagUpdate.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/FlagUpdate.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/FlagUpdate.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/ImportMailboxConversationSet.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/ImportMailboxConversationSet.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/MailboxItemFlag.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/MailboxItemFlag.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/backend/mail/api/flags/MailboxItemFlagSystem.py` & `netbluemind5-5.0.7187/netbluemind/backend/mail/api/flags/MailboxItemFlagSystem.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarLookupResponse.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarLookupResponse.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarLookupResponseType.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarLookupResponseType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarSettingsData.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarSettingsData.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarSettingsDataDay.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarSettingsDataDay.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarView.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarView.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewCalendarViewType.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewCalendarViewType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewChanges.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewChangesItemAdd.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewChangesItemDelete.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarViewChangesItemModify.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarViewChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/CalendarsVEventQuery.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/CalendarsVEventQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendar.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendar_VERSION = "5.0.7152"
+ICalendar_VERSION = "5.0.7187"
 
 
 class ICalendar(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarAutocomplete.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarAutocomplete.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarAutocomplete_VERSION = "5.0.7152"
+ICalendarAutocomplete_VERSION = "5.0.7187"
 
 
 class ICalendarAutocomplete(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendar/autocomplete'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarSettings.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarSettings_VERSION = "5.0.7152"
+ICalendarSettings_VERSION = "5.0.7187"
 
 
 class ICalendarSettings(BaseEndpoint):
     def __init__(self, apiKey, url, calendarUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/{calendarUid}/_config'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarUids.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarUids.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarUids_VERSION = "5.0.7152"
+ICalendarUids_VERSION = "5.0.7187"
 
 
 class ICalendarUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendar/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarView.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarView.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarView_VERSION = "5.0.7152"
+ICalendarView_VERSION = "5.0.7187"
 
 
 class ICalendarView(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/view/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarViewUids.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarViewUids.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarViewUids_VERSION = "5.0.7152"
+ICalendarViewUids_VERSION = "5.0.7187"
 
 
 class ICalendarViewUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendarview/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendars.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendars.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendars_VERSION = "5.0.7152"
+ICalendars_VERSION = "5.0.7187"
 
 
 class ICalendars(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/ICalendarsMgmt.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/ICalendarsMgmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICalendarsMgmt_VERSION = "5.0.7152"
+ICalendarsMgmt_VERSION = "5.0.7187"
 
 
 class ICalendarsMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/calendars'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/IFreebusyMgmt.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/IFreebusyMgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IFreebusyMgmt_VERSION = "5.0.7152"
+IFreebusyMgmt_VERSION = "5.0.7187"
 
 
 class IFreebusyMgmt(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/freebusy/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/IFreebusyUids.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/IFreebusyUids.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IFreebusyUids_VERSION = "5.0.7152"
+IFreebusyUids_VERSION = "5.0.7187"
 
 
 class IFreebusyUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/freebusy/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/IPrint.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/IPrint.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IPrint_VERSION = "5.0.7152"
+IPrint_VERSION = "5.0.7187"
 
 
 class IPrint(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/print'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/IPublicFreebusy.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/IPublicFreebusy.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IPublicFreebusy_VERSION = "5.0.7152"
+IPublicFreebusy_VERSION = "5.0.7187"
 
 
 class IPublicFreebusy(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/sfreebusy'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/IPublishCalendar.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/IPublishCalendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IPublishCalendar_VERSION = "5.0.7152"
+IPublishCalendar_VERSION = "5.0.7187"
 
 
 class IPublishCalendar(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/publish/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/IUserCalendarViews.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/IUserCalendarViews.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserCalendarViews_VERSION = "5.0.7152"
+IUserCalendarViews_VERSION = "5.0.7187"
 
 
 class IUserCalendarViews(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{domainUid}/{userUid}/calendar-views'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/IVEvent.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/IVEvent.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IVEvent_VERSION = "5.0.7152"
+IVEvent_VERSION = "5.0.7187"
 
 
 class IVEvent(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/vevent/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/IVFreebusy.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/IVFreebusy.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IVFreebusy_VERSION = "5.0.7152"
+IVFreebusy_VERSION = "5.0.7187"
 
 
 class IVFreebusy(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/calendars/vfreebusy/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/PrintData.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/PrintData.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptions.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptions.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptionsCalendarMetadata.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptionsCalendarMetadata.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptionsPrintFormat.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptionsPrintFormat.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptionsPrintLayout.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptionsPrintLayout.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/PrintOptionsPrintView.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/PrintOptionsPrintView.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/PublishMode.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/PublishMode.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEvent.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEvent.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventAttendeeQuery.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventAttendeeQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventChanges.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventChangesItemAdd.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventChangesItemDelete.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventChangesItemModify.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventCounter.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventCounter.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventCounterCounterOriginator.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventCounterCounterOriginator.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventOccurrence.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventOccurrence.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventQuery.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventSeries.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventSeries.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VEventTransparency.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VEventTransparency.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VFreebusy.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VFreebusy.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VFreebusyQuery.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VFreebusyQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VFreebusySlot.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VFreebusySlot.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/calendar/api/VFreebusyType.py` & `netbluemind5-5.0.7187/netbluemind/calendar/api/VFreebusyType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/api/Email.py` & `netbluemind5-5.0.7187/netbluemind/core/api/Email.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/api/ImportStats.py` & `netbluemind5-5.0.7187/netbluemind/core/api/ImportStats.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/api/ListResult.py` & `netbluemind5-5.0.7187/netbluemind/core/api/ListResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/api/VersionInfo.py` & `netbluemind5-5.0.7187/netbluemind/core/api/VersionInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/api/date/BmDateTime.py` & `netbluemind5-5.0.7187/netbluemind/core/api/date/BmDateTime.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/api/date/BmDateTimePrecision.py` & `netbluemind5-5.0.7187/netbluemind/core/api/date/BmDateTimePrecision.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/api/fault/ErrorCode.py` & `netbluemind5-5.0.7187/netbluemind/core/api/fault/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/Ack.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/Ack.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerHierarchyNode.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerHierarchyNode.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerQuery.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerSettingsKeys.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerSettingsKeys.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerSubscription.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerSubscription.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerSubscriptionDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerSubscriptionDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/ContainerSubscriptionModel.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/ContainerSubscriptionModel.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/Count.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/Count.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IChangelogSupport.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IChangelogSupport.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IChangelogSupport_VERSION = "5.0.7152"
+IChangelogSupport_VERSION = "5.0.7187"
 
 
 class IChangelogSupport(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IContainerManagement.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IContainerManagement.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IContainerManagement_VERSION = "5.0.7152"
+IContainerManagement_VERSION = "5.0.7187"
 
 
 class IContainerManagement(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_manage/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IContainerSync.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IContainerSync.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IContainerSync_VERSION = "5.0.7152"
+IContainerSync_VERSION = "5.0.7187"
 
 
 class IContainerSync(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_sync/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IContainers.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IContainers.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IContainers_VERSION = "5.0.7152"
+IContainers_VERSION = "5.0.7187"
 
 
 class IContainers(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_manage'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IContainersFlatHierarchy.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IContainersFlatHierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IContainersFlatHierarchy_VERSION = "5.0.7152"
+IContainersFlatHierarchy_VERSION = "5.0.7187"
 
 
 class IContainersFlatHierarchy(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, ownerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_hierarchy/{domainUid}/{ownerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/ICountingSupport.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/ICountingSupport.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICountingSupport_VERSION = "5.0.7152"
+ICountingSupport_VERSION = "5.0.7187"
 
 
 class ICountingSupport(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IFlatHierarchyUids.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IFlatHierarchyUids.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IFlatHierarchyUids_VERSION = "5.0.7152"
+IFlatHierarchyUids_VERSION = "5.0.7187"
 
 
 class IFlatHierarchyUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/flat_hierarchy/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IOfflineMgmt.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IOfflineMgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOfflineMgmt_VERSION = "5.0.7152"
+IOfflineMgmt_VERSION = "5.0.7187"
 
 
 class IOfflineMgmt(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, ownerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/offline/{domainUid}/{ownerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IOwnerSubscriptionUids.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IOwnerSubscriptionUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOwnerSubscriptionUids_VERSION = "5.0.7152"
+IOwnerSubscriptionUids_VERSION = "5.0.7187"
 
 
 class IOwnerSubscriptionUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/owner_subscriptions/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IOwnerSubscriptions.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IOwnerSubscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOwnerSubscriptions_VERSION = "5.0.7152"
+IOwnerSubscriptions_VERSION = "5.0.7187"
 
 
 class IOwnerSubscriptions(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, ownerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/containers/_subscriptions/{domainUid}/{ownerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/ISortingSupport.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/ISortingSupport.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISortingSupport_VERSION = "5.0.7152"
+ISortingSupport_VERSION = "5.0.7187"
 
 
 class ISortingSupport(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/api/IdRange.py` & `netbluemind5-5.0.7187/netbluemind/core/container/api/IdRange.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/BaseContainerDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/BaseContainerDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ChangeLogEntry.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ChangeLogEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ChangeLogEntryType.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ChangeLogEntryType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerChangelog.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerChangelog.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerChangeset.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerChangeset.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerModifiableDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerModifiableDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerSyncResult.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerSyncResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerSyncStatus.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerSyncStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerSyncStatusStatus.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerSyncStatusStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerUpdatesResult.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerUpdatesResult.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ContainerUpdatesResultInError.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ContainerUpdatesResultInError.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/CountFastPath.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/CountFastPath.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/IdQuery.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/IdQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemChangeLogEntry.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemChangeLogEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemChangelog.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemChangelog.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemContainerValue.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemContainerValue.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemFlag.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemFlag.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemFlagFilter.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemFlagFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemIdentifier.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemIdentifier.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemUri.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemUri.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemValue.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemValue.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/ItemVersion.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/ItemVersion.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/SortDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/SortDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/SortDescriptorDirection.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/SortDescriptorDirection.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/SortDescriptorField.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/SortDescriptorField.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/acl/AccessControlEntry.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/acl/AccessControlEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/container/model/acl/Verb.py` & `netbluemind5-5.0.7187/netbluemind/core/container/model/acl/Verb.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/task/api/ITask.py` & `netbluemind5-5.0.7187/netbluemind/core/task/api/ITask.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITask_VERSION = "5.0.7152"
+ITask_VERSION = "5.0.7187"
 
 
 class ITask(BaseEndpoint):
     def __init__(self, apiKey, url, taskId):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/tasks/{taskId}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/core/task/api/TaskRef.py` & `netbluemind5-5.0.7187/netbluemind/core/task/api/TaskRef.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/task/api/TaskStatus.py` & `netbluemind5-5.0.7187/netbluemind/core/task/api/TaskStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/core/task/api/TaskStatusState.py` & `netbluemind5-5.0.7187/netbluemind/core/task/api/TaskStatusState.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/cti/api/IComputerTelephonyIntegration.py` & `netbluemind5-5.0.7187/netbluemind/cti/api/IComputerTelephonyIntegration.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IComputerTelephonyIntegration_VERSION = "5.0.7152"
+IComputerTelephonyIntegration_VERSION = "5.0.7187"
 
 
 class IComputerTelephonyIntegration(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/cti/{domainUid}/{userUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/cti/api/Status.py` & `netbluemind5-5.0.7187/netbluemind/cti/api/Status.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/cti/api/StatusPhoneState.py` & `netbluemind5-5.0.7187/netbluemind/cti/api/StatusPhoneState.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/cti/api/StatusType.py` & `netbluemind5-5.0.7187/netbluemind/cti/api/StatusType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/DataProtectGeneration.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/DataProtectGeneration.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/GenerationContent.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/GenerationContent.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/GenerationStatus.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/GenerationStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/IDataProtect.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/IDataProtect.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDataProtect_VERSION = "5.0.7152"
+IDataProtect_VERSION = "5.0.7187"
 
 
 class IDataProtect(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/dataprotect'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/PartGeneration.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/PartGeneration.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/Restorable.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/Restorable.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/RestorableKind.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/RestorableKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/RestoreDefinition.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/RestoreDefinition.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/RestoreOperation.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/RestoreOperation.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/dataprotect/api/RetentionPolicy.py` & `netbluemind5-5.0.7187/netbluemind/dataprotect/api/RetentionPolicy.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/device/api/Device.py` & `netbluemind5-5.0.7187/netbluemind/device/api/Device.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/device/api/IDevice.py` & `netbluemind5-5.0.7187/netbluemind/device/api/IDevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDevice_VERSION = "5.0.7152"
+IDevice_VERSION = "5.0.7187"
 
 
 class IDevice(BaseEndpoint):
     def __init__(self, apiKey, url, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/devices/{userUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/device/api/IDeviceUids.py` & `netbluemind5-5.0.7187/netbluemind/tag/api/ITagUids.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDeviceUids_VERSION = "5.0.7152"
+ITagUids_VERSION = "5.0.7187"
 
 
-class IDeviceUids(BaseEndpoint):
+class ITagUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
-        self.base = url + '/device/uids'
+        self.base = url + '/tags/uids'
 
-    def getDefaultUserDevices(self, uid):
-        postUri = "/{uid}/_default_devices"
+    def getDefaultUserTags(self, uid):
+        postUri = "/{uid}/_default_tags"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IDeviceUids_VERSION}, data=__encoded__)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': ITagUids_VERSION}, data=__encoded__)
         return self.handleResult__(serder.STRING, response)
```

### Comparing `netbluemind5-5.0.7152/netbluemind/device/api/IDevices.py` & `netbluemind5-5.0.7187/netbluemind/device/api/IDevices.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDevices_VERSION = "5.0.7152"
+IDevices_VERSION = "5.0.7187"
 
 
 class IDevices(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/devices'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/device/api/WipeMode.py` & `netbluemind5-5.0.7187/netbluemind/device/api/WipeMode.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/BaseDirEntry.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/BaseDirEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/BaseDirEntryAccountType.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/BaseDirEntryAccountType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/BaseDirEntryKind.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/BaseDirEntryKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/DirBaseValue.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/DirBaseValue.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/DirEntry.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/DirEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQuery.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQueryDir.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQueryDir.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQueryOrder.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQueryOrder.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQueryOrderBy.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQueryOrderBy.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/DirEntryQueryStateFilter.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/DirEntryQueryStateFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/IDirEntryMaintenance.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/IDirEntryMaintenance.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDirEntryMaintenance_VERSION = "5.0.7152"
+IDirEntryMaintenance_VERSION = "5.0.7187"
 
 
 class IDirEntryMaintenance(BaseEndpoint):
     def __init__(self, apiKey, url, domain, entryUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/directory/{domain}/{entryUid}/mgmt'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/IDirEntryPath.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/IDirEntryPath.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDirEntryPath_VERSION = "5.0.7152"
+IDirEntryPath_VERSION = "5.0.7187"
 
 
 class IDirEntryPath(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/directory/path'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/IDirectory.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/IDirectory.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDirectory_VERSION = "5.0.7152"
+IDirectory_VERSION = "5.0.7187"
 
 
 class IDirectory(BaseEndpoint):
     def __init__(self, apiKey, url, domain):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/directory/{domain}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/IOrgUnits.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/IOrgUnits.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IOrgUnits_VERSION = "5.0.7152"
+IOrgUnits_VERSION = "5.0.7187"
 
 
 class IOrgUnits(BaseEndpoint):
     def __init__(self, apiKey, url, domain):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/directory/_ou/{domain}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/MaintenanceOperation.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/MaintenanceOperation.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/OrgUnit.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/OrgUnit.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/OrgUnitPath.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/OrgUnitPath.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/OrgUnitQuery.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/OrgUnitQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/directory/api/RepairConfig.py` & `netbluemind5-5.0.7187/netbluemind/directory/api/RepairConfig.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/document/api/Document.py` & `netbluemind5-5.0.7187/netbluemind/document/api/Document.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/document/api/DocumentMetadata.py` & `netbluemind5-5.0.7187/netbluemind/document/api/DocumentMetadata.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/document/api/IDocument.py` & `netbluemind5-5.0.7187/netbluemind/document/api/IDocument.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDocument_VERSION = "5.0.7152"
+IDocument_VERSION = "5.0.7187"
 
 
 class IDocument(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid, itemUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/document/{containerUid}/{itemUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/documentfolder/api/DocumentFolder.py` & `netbluemind5-5.0.7187/netbluemind/documentfolder/api/DocumentFolder.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/documentfolder/api/IDocumentFolder.py` & `netbluemind5-5.0.7187/netbluemind/documentfolder/api/IDocumentFolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDocumentFolder_VERSION = "5.0.7152"
+IDocumentFolder_VERSION = "5.0.7187"
 
 
 class IDocumentFolder(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/document/{containerUid}/'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/documentfolder/api/IDocumentFolderUids.py` & `netbluemind5-5.0.7187/netbluemind/documentfolder/api/IDocumentFolderUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDocumentFolderUids_VERSION = "5.0.7152"
+IDocumentFolderUids_VERSION = "5.0.7187"
 
 
 class IDocumentFolderUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/document/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/domain/api/Domain.py` & `netbluemind5-5.0.7187/netbluemind/domain/api/Domain.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/domain/api/IDomainSettings.py` & `netbluemind5-5.0.7187/netbluemind/domain/api/IDomainSettings.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDomainSettings_VERSION = "5.0.7152"
+IDomainSettings_VERSION = "5.0.7187"
 
 
 class IDomainSettings(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/domains/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/domain/api/IDomains.py` & `netbluemind5-5.0.7187/netbluemind/domain/api/IDomains.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDomains_VERSION = "5.0.7152"
+IDomains_VERSION = "5.0.7187"
 
 
 class IDomains(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/domains'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/eas/api/Account.py` & `netbluemind5-5.0.7187/netbluemind/eas/api/Account.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/eas/api/FolderSyncVersions.py` & `netbluemind5-5.0.7187/netbluemind/eas/api/FolderSyncVersions.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/eas/api/Heartbeat.py` & `netbluemind5-5.0.7187/netbluemind/eas/api/Heartbeat.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/eas/api/IEas.py` & `netbluemind5-5.0.7187/netbluemind/eas/api/IEas.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IEas_VERSION = "5.0.7152"
+IEas_VERSION = "5.0.7187"
 
 
 class IEas(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/eas'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/eas/api/SentItem.py` & `netbluemind5-5.0.7187/netbluemind/eas/api/SentItem.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/externaluser/api/ExternalUser.py` & `netbluemind5-5.0.7187/netbluemind/externaluser/api/ExternalUser.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/externaluser/api/IExternalUser.py` & `netbluemind5-5.0.7187/netbluemind/externaluser/api/IExternalUser.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IExternalUser_VERSION = "5.0.7152"
+IExternalUser_VERSION = "5.0.7187"
 
 
 class IExternalUser(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/externaluser/{domainUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/filehosting/api/Configuration.py` & `netbluemind5-5.0.7187/netbluemind/filehosting/api/Configuration.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/filehosting/api/FileHostingInfo.py` & `netbluemind5-5.0.7187/netbluemind/filehosting/api/FileHostingInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/filehosting/api/FileHostingInfoType.py` & `netbluemind5-5.0.7187/netbluemind/filehosting/api/FileHostingInfoType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/filehosting/api/FileHostingItem.py` & `netbluemind5-5.0.7187/netbluemind/filehosting/api/FileHostingItem.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/filehosting/api/FileHostingPublicLink.py` & `netbluemind5-5.0.7187/netbluemind/filehosting/api/FileHostingPublicLink.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/filehosting/api/FileType.py` & `netbluemind5-5.0.7187/netbluemind/filehosting/api/FileType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/filehosting/api/IFileHosting.py` & `netbluemind5-5.0.7187/netbluemind/filehosting/api/IFileHosting.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IFileHosting_VERSION = "5.0.7152"
+IFileHosting_VERSION = "5.0.7187"
 
 
 class IFileHosting(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/filehosting/{domainUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/filehosting/api/IInternalBMFileSystem.py` & `netbluemind5-5.0.7187/netbluemind/filehosting/api/IInternalBMFileSystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IInternalBMFileSystem_VERSION = "5.0.7152"
+IInternalBMFileSystem_VERSION = "5.0.7187"
 
 
 class IInternalBMFileSystem(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/bmfilehosting'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/filehosting/api/Metadata.py` & `netbluemind5-5.0.7187/netbluemind/filehosting/api/Metadata.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/group/api/Group.py` & `netbluemind5-5.0.7187/netbluemind/group/api/Group.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/group/api/GroupSearchQuery.py` & `netbluemind5-5.0.7187/netbluemind/group/api/GroupSearchQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/group/api/IGroup.py` & `netbluemind5-5.0.7187/netbluemind/group/api/IGroup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IGroup_VERSION = "5.0.7152"
+IGroup_VERSION = "5.0.7187"
 
 
 class IGroup(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/groups/{domainUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/group/api/IGroupMember.py` & `netbluemind5-5.0.7187/netbluemind/group/api/IGroupMember.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IGroupMember_VERSION = "5.0.7152"
+IGroupMember_VERSION = "5.0.7187"
 
 
 class IGroupMember(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind5-5.0.7152/netbluemind/group/api/Member.py` & `netbluemind5-5.0.7187/netbluemind/group/api/Member.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/group/api/MemberType.py` & `netbluemind5-5.0.7187/netbluemind/group/api/MemberType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElement.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElement.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementAttendee.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementAttendee.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementCUType.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementCUType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementClassification.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementClassification.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementOrganizer.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementOrganizer.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementParticipationStatus.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementParticipationStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementRRule.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementRRule.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementRRuleFrequency.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementRRuleFrequency.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementRRuleWeekDay.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementRRuleWeekDay.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementRole.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementRole.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementStatus.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementVAlarm.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementVAlarm.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/icalendar/api/ICalendarElementVAlarmAction.py` & `netbluemind5-5.0.7187/netbluemind/icalendar/api/ICalendarElementVAlarmAction.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/IMailboxAclUids.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/IMailboxAclUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxAclUids_VERSION = "5.0.7152"
+IMailboxAclUids_VERSION = "5.0.7187"
 
 
 class IMailboxAclUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailbox/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/IMailboxMgmt.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/IMailboxMgmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxMgmt_VERSION = "5.0.7152"
+IMailboxMgmt_VERSION = "5.0.7187"
 
 
 class IMailboxMgmt(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/mailbox/{domainUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/IMailboxes.py` & `netbluemind5-5.0.7187/netbluemind/user/api/IUser.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,363 +18,350 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxes_VERSION = "5.0.7152"
+IUser_VERSION = "5.0.7187"
 
 
-class IMailboxes(BaseEndpoint):
+class IUser(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
-        self.base = url + '/mailboxes/{domainUid}'
+        self.base = url + '/users/{domainUid}'
         self.domainUid_ = domainUid
         self.base = self.base.replace('{domainUid}', domainUid)
 
-    def byEmail(self, email):
-        postUri = "/_byemail"
+    def allUids(self):
+        postUri = "/_alluids"
         __data__ = None
         __encoded__ = None
-        queryParams = {'email': email}
+        queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.Mailbox import Mailbox
-        from netbluemind.mailbox.api.Mailbox import __MailboxSerDer__
-        from netbluemind.core.container.model.ItemValue import ItemValue
-        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(__ItemValueSerDer__(__MailboxSerDer__()), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        return self.handleResult__(serder.ListSerDer(serder.STRING), response)
 
-    def byName(self, name):
-        postUri = "/_byname"
+    def byEmail(self, email):
+        postUri = "/byEmail/{email}"
         __data__ = None
         __encoded__ = None
-        queryParams = {'name': name}
+        postUri = postUri.replace("{email}", email)
+        queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.Mailbox import Mailbox
-        from netbluemind.mailbox.api.Mailbox import __MailboxSerDer__
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        from netbluemind.user.api.User import User
+        from netbluemind.user.api.User import __UserSerDer__
         from netbluemind.core.container.model.ItemValue import ItemValue
         from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(__ItemValueSerDer__(__MailboxSerDer__()), response)
+        return self.handleResult__(__ItemValueSerDer__(__UserSerDer__()), response)
 
-    def byRouting(self, email):
-        postUri = "/_byRouting"
+    def byExtId(self, extid):
+        postUri = "/byExtId/{extid}"
         __data__ = None
         __encoded__ = None
-        queryParams = {'email': email}
+        postUri = postUri.replace("{extid}", extid)
+        queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.ListSerDer(serder.STRING), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        from netbluemind.user.api.User import User
+        from netbluemind.user.api.User import __UserSerDer__
+        from netbluemind.core.container.model.ItemValue import ItemValue
+        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
+        return self.handleResult__(__ItemValueSerDer__(__UserSerDer__()), response)
 
-    def byType(self, email):
-        postUri = "/_byType"
+    def byLogin(self, login):
+        postUri = "/byLogin/{login}"
         __data__ = None
         __encoded__ = None
-        queryParams = {'email': email}
+        postUri = postUri.replace("{login}", login)
+        queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.ListSerDer(serder.STRING), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        from netbluemind.user.api.User import User
+        from netbluemind.user.api.User import __UserSerDer__
+        from netbluemind.core.container.model.ItemValue import ItemValue
+        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
+        return self.handleResult__(__ItemValueSerDer__(__UserSerDer__()), response)
 
-    def create(self, uid, mailbox):
+    def create(self, uid, user):
         postUri = "/{uid}"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
-        from netbluemind.mailbox.api.Mailbox import Mailbox
-        from netbluemind.mailbox.api.Mailbox import __MailboxSerDer__
-        __data__ = __MailboxSerDer__().encode(mailbox)
+        from netbluemind.user.api.User import User
+        from netbluemind.user.api.User import __UserSerDer__
+        __data__ = __UserSerDer__().encode(user)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.put(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
         return self.handleResult__(None, response)
 
-    def delete(self, uid):
-        postUri = "/{uid}"
+    def createWithExtId(self, uid, extid, user):
+        postUri = "/{uid}/{extid}/createwithextid"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
+        postUri = postUri.replace("{extid}", extid)
+        from netbluemind.user.api.User import User
+        from netbluemind.user.api.User import __UserSerDer__
+        __data__ = __UserSerDer__().encode(user)
+        __encoded__ = json.dumps(__data__)
         queryParams = {}
 
-        response = requests.delete(self.base + postUri, params=queryParams, verify=False, headers={
-                                   'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
+        response = requests.put(self.base + postUri, params=queryParams, verify=False, headers={
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
         return self.handleResult__(None, response)
 
-    def getComplete(self, uid):
-        postUri = "/{uid}/complete"
+    def delete(self, uid):
+        postUri = "/{uid}"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.Mailbox import Mailbox
-        from netbluemind.mailbox.api.Mailbox import __MailboxSerDer__
-        from netbluemind.core.container.model.ItemValue import ItemValue
-        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(__ItemValueSerDer__(__MailboxSerDer__()), response)
+        response = requests.delete(self.base + postUri, params=queryParams, verify=False, headers={
+                                   'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        from netbluemind.core.task.api.TaskRef import TaskRef
+        from netbluemind.core.task.api.TaskRef import __TaskRefSerDer__
+        return self.handleResult__(__TaskRefSerDer__(), response)
 
-    def getDomainFilter(self):
-        postUri = "/_filter"
+    def deletePhoto(self, uid):
+        postUri = "/{uid}/photo"
         __data__ = None
         __encoded__ = None
+        postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.MailFilter import MailFilter
-        from netbluemind.mailbox.api.MailFilter import __MailFilterSerDer__
-        return self.handleResult__(__MailFilterSerDer__(), response)
+        response = requests.delete(self.base + postUri, params=queryParams, verify=False, headers={
+                                   'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        return self.handleResult__(None, response)
 
-    def getMailboxAccessControlList(self, mailboxUid):
-        postUri = "/{mailboxUid}/_acls"
+    def enablePerUserLog(self, userUid, endpoint, enable):
+        postUri = "/{userUid}/_logging/{endpoint}"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{mailboxUid}", mailboxUid)
+        postUri = postUri.replace("{userUid}", userUid)
+        postUri = postUri.replace("{endpoint}", endpoint)
+        __data__ = serder.BOOLEAN.encode(enable)
+        __encoded__ = json.dumps(__data__)
         queryParams = {}
 
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.core.container.model.acl.AccessControlEntry import AccessControlEntry
-        from netbluemind.core.container.model.acl.AccessControlEntry import __AccessControlEntrySerDer__
-        return self.handleResult__(serder.ListSerDer(__AccessControlEntrySerDer__()), response)
+        response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        return self.handleResult__(None, response)
 
-    def getMailboxConfig(self, uid):
-        postUri = "/{uid}/_config"
+    def getComplete(self, uid):
+        postUri = "/{uid}/complete"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.MailboxConfig import MailboxConfig
-        from netbluemind.mailbox.api.MailboxConfig import __MailboxConfigSerDer__
-        return self.handleResult__(__MailboxConfigSerDer__(), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        from netbluemind.user.api.User import User
+        from netbluemind.user.api.User import __UserSerDer__
+        from netbluemind.core.container.model.ItemValue import ItemValue
+        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
+        return self.handleResult__(__ItemValueSerDer__(__UserSerDer__()), response)
 
-    def getMailboxDelegationRule(self, mailboxUid):
-        postUri = "/{mailboxUid}/_delegationRule"
+    def getIcon(self, uid):
+        postUri = "/{uid}/icon"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{mailboxUid}", mailboxUid)
+        postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.rules.DelegationRule import DelegationRule
-        from netbluemind.mailbox.api.rules.DelegationRule import __DelegationRuleSerDer__
-        return self.handleResult__(__DelegationRuleSerDer__(), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        return self.handleResult__(serder.ByteArraySerDer, response)
 
-    def getMailboxFilter(self, mailboxUid):
-        postUri = "/{mailboxUid}/_filter"
+    def getPhoto(self, uid):
+        postUri = "/{uid}/photo"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{mailboxUid}", mailboxUid)
+        postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.MailFilter import MailFilter
-        from netbluemind.mailbox.api.MailFilter import __MailFilterSerDer__
-        return self.handleResult__(__MailFilterSerDer__(), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        return self.handleResult__(serder.ByteArraySerDer, response)
 
-    def getMailboxQuota(self, uid):
-        postUri = "/{uid}/_quota"
+    def getResolvedRoles(self, uid):
+        postUri = "/{uid}/roles_resolved"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.MailboxQuota import MailboxQuota
-        from netbluemind.mailbox.api.MailboxQuota import __MailboxQuotaSerDer__
-        return self.handleResult__(__MailboxQuotaSerDer__(), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        return self.handleResult__(serder.SetSerDer(serder.STRING), response)
 
-    def getMailboxRules(self, mailboxUid):
-        postUri = "/{mailboxUid}/_rules"
+    def getRoles(self, uid):
+        postUri = "/{uid}/roles"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{mailboxUid}", mailboxUid)
+        postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.rules.MailFilterRule import MailFilterRule
-        from netbluemind.mailbox.api.rules.MailFilterRule import __MailFilterRuleSerDer__
-        return self.handleResult__(serder.ListSerDer(__MailFilterRuleSerDer__()), response)
-
-    def getMailboxRulesByClient(self, mailboxUid, client):
-        postUri = "/{mailboxUid}/_rulesByClient"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{mailboxUid}", mailboxUid)
-        queryParams = {'client': client}
-
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.rules.MailFilterRule import MailFilterRule
-        from netbluemind.mailbox.api.rules.MailFilterRule import __MailFilterRuleSerDer__
-        return self.handleResult__(serder.ListSerDer(__MailFilterRuleSerDer__()), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        return self.handleResult__(serder.SetSerDer(serder.STRING), response)
 
-    def getMailboxVacation(self, mailboxUid):
-        postUri = "/{mailboxUid}/_vacation"
+    def getUsersWithRoles(self, roles):
+        postUri = "/_roleusers"
         __data__ = None
         __encoded__ = None
-        __data__ = serder.STRING.encode(mailboxUid)
+        __data__ = serder.ListSerDer(serder.STRING).encode(roles)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.MailFilterVacation import MailFilterVacation
-        from netbluemind.mailbox.api.MailFilterVacation import __MailFilterVacationSerDer__
-        return self.handleResult__(__MailFilterVacationSerDer__(), response)
+        response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        return self.handleResult__(serder.SetSerDer(serder.STRING), response)
 
-    def getUnreadMessagesCount(self):
-        postUri = "/_unread"
+    def getVCard(self, uid):
+        postUri = "/{uid}/vcard"
         __data__ = None
         __encoded__ = None
+        postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.INT, response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        from netbluemind.addressbook.api.VCard import VCard
+        from netbluemind.addressbook.api.VCard import __VCardSerDer__
+        return self.handleResult__(__VCardSerDer__(), response)
 
-    def list(self):
-        postUri = "/_list"
+    def memberOf(self, uid):
+        postUri = "/{uid}/groups"
         __data__ = None
         __encoded__ = None
+        postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.Mailbox import Mailbox
-        from netbluemind.mailbox.api.Mailbox import __MailboxSerDer__
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        from netbluemind.group.api.Group import Group
+        from netbluemind.group.api.Group import __GroupSerDer__
         from netbluemind.core.container.model.ItemValue import ItemValue
         from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(serder.ListSerDer(__ItemValueSerDer__(__MailboxSerDer__())), response)
+        return self.handleResult__(serder.ListSerDer(__ItemValueSerDer__(__GroupSerDer__())), response)
 
-    def listUids(self):
-        postUri = "/_listUids"
+    def memberOfGroups(self, uid):
+        postUri = "/{uid}/groupUids"
         __data__ = None
         __encoded__ = None
+        postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
         return self.handleResult__(serder.ListSerDer(serder.STRING), response)
 
-    def multipleGet(self, uids):
-        postUri = "/_mget"
+    def setExtId(self, uid, arg1):
+        postUri = "/{uid}/_extId"
         __data__ = None
         __encoded__ = None
-        __data__ = serder.ListSerDer(serder.STRING).encode(uids)
+        postUri = postUri.replace("{uid}", uid)
+        __data__ = serder.STRING.encode(arg1)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
-        from netbluemind.mailbox.api.Mailbox import Mailbox
-        from netbluemind.mailbox.api.Mailbox import __MailboxSerDer__
-        from netbluemind.core.container.model.ItemValue import ItemValue
-        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(serder.ListSerDer(__ItemValueSerDer__(__MailboxSerDer__())), response)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+        return self.handleResult__(None, response)
 
-    def setDomainFilter(self, filter):
-        postUri = "/_filter"
+    def setPassword(self, uid, password):
+        postUri = "/{uid}/password_"
         __data__ = None
         __encoded__ = None
-        from netbluemind.mailbox.api.MailFilter import MailFilter
-        from netbluemind.mailbox.api.MailFilter import __MailFilterSerDer__
-        __data__ = __MailFilterSerDer__().encode(filter)
+        postUri = postUri.replace("{uid}", uid)
+        from netbluemind.user.api.ChangePassword import ChangePassword
+        from netbluemind.user.api.ChangePassword import __ChangePasswordSerDer__
+        __data__ = __ChangePasswordSerDer__().encode(password)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
         return self.handleResult__(None, response)
 
-    def setMailboxAccessControlList(self, mailboxUid, accessControlEntries):
-        postUri = "/{mailboxUid}/_acls"
+    def setPhoto(self, uid, arg1):
+        postUri = "/{uid}/photo"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{mailboxUid}", mailboxUid)
-        from netbluemind.core.container.model.acl.AccessControlEntry import AccessControlEntry
-        from netbluemind.core.container.model.acl.AccessControlEntry import __AccessControlEntrySerDer__
-        __data__ = serder.ListSerDer(
-            __AccessControlEntrySerDer__()).encode(accessControlEntries)
+        postUri = postUri.replace("{uid}", uid)
+        __data__ = serder.ByteArraySerDer.encode(arg1)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
         return self.handleResult__(None, response)
 
-    def setMailboxDelegationRule(self, mailboxUid, delegationRule):
-        postUri = "/{mailboxUid}/_delegationRule"
+    def setRoles(self, uid, roles):
+        postUri = "/{uid}/roles"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{mailboxUid}", mailboxUid)
-        from netbluemind.mailbox.api.rules.DelegationRule import DelegationRule
-        from netbluemind.mailbox.api.rules.DelegationRule import __DelegationRuleSerDer__
-        __data__ = __DelegationRuleSerDer__().encode(delegationRule)
+        postUri = postUri.replace("{uid}", uid)
+        __data__ = serder.SetSerDer(serder.STRING).encode(roles)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
         return self.handleResult__(None, response)
 
-    def setMailboxFilter(self, mailboxUid, filter):
-        postUri = "/{mailboxUid}/_filter"
+    def update(self, uid, user):
+        postUri = "/{uid}"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{mailboxUid}", mailboxUid)
-        from netbluemind.mailbox.api.MailFilter import MailFilter
-        from netbluemind.mailbox.api.MailFilter import __MailFilterSerDer__
-        __data__ = __MailFilterSerDer__().encode(filter)
+        postUri = postUri.replace("{uid}", uid)
+        from netbluemind.user.api.User import User
+        from netbluemind.user.api.User import __UserSerDer__
+        __data__ = __UserSerDer__().encode(user)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
         return self.handleResult__(None, response)
 
-    def setMailboxVacation(self, mailboxUid, vacation):
-        postUri = "/{mailboxUid}/_vacation"
+    def updateAccountType(self, uid, accountType):
+        postUri = "/_updateAccountType/{uid}"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{mailboxUid}", mailboxUid)
-        from netbluemind.mailbox.api.MailFilterVacation import MailFilterVacation
-        from netbluemind.mailbox.api.MailFilterVacation import __MailFilterVacationSerDer__
-        __data__ = __MailFilterVacationSerDer__().encode(vacation)
+        postUri = postUri.replace("{uid}", uid)
+        from netbluemind.directory.api.BaseDirEntryAccountType import BaseDirEntryAccountType
+        from netbluemind.directory.api.BaseDirEntryAccountType import __BaseDirEntryAccountTypeSerDer__
+        __data__ = __BaseDirEntryAccountTypeSerDer__().encode(accountType)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
         return self.handleResult__(None, response)
 
-    def update(self, uid, mailbox):
-        postUri = "/{uid}"
+    def updateVCard(self, uid, userVCard):
+        postUri = "/{uid}/vcard"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
-        from netbluemind.mailbox.api.Mailbox import Mailbox
-        from netbluemind.mailbox.api.Mailbox import __MailboxSerDer__
-        __data__ = __MailboxSerDer__().encode(mailbox)
+        from netbluemind.addressbook.api.VCard import VCard
+        from netbluemind.addressbook.api.VCard import __VCardSerDer__
+        __data__ = __VCardSerDer__().encode(userVCard)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IMailboxes_VERSION}, data=__encoded__)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
         return self.handleResult__(None, response)
```

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/MailFilter.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/MailFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/MailFilterForwarding.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/MailFilterForwarding.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/MailFilterVacation.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/MailFilterVacation.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/Mailbox.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/Mailbox.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/MailboxConfig.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/MailboxConfig.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/MailboxQuota.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/MailboxQuota.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/MailboxRouting.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/MailboxRouting.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/MailboxType.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/MailboxType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/ShardStats.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/ShardStats.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/ShardStatsMailboxStats.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/ShardStatsMailboxStats.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/ShardStatsState.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/ShardStatsState.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/SimpleShardStats.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/SimpleShardStats.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/DelegationRule.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/DelegationRule.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/MailFilterRule.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/MailFilterRule.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #
 import requests
 from netbluemind.python import serder
 
 
 class MailFilterRule:
     def __init__(self):
+        self.id = None
         self.client = None
         self.type = None
         self.trigger = None
         self.deferred = None
         self.active = None
         self.name = None
         self.clientProperties = None
@@ -45,14 +46,16 @@
             return None
         instance = MailFilterRule()
 
         self.parseInternal(value, instance)
         return instance
 
     def parseInternal(self, value, instance):
+        idValue = value['id']
+        instance.id = serder.LONG.parse(idValue)
         clientValue = value['client']
         instance.client = serder.STRING.parse(clientValue)
         from netbluemind.mailbox.api.rules.MailFilterRuleType import MailFilterRuleType
         from netbluemind.mailbox.api.rules.MailFilterRuleType import __MailFilterRuleTypeSerDer__
         typeValue = value['type']
         instance.type = __MailFilterRuleTypeSerDer__().parse(typeValue)
         from netbluemind.mailbox.api.rules.MailFilterRuleTrigger import MailFilterRuleTrigger
@@ -87,14 +90,16 @@
             return None
         instance = dict()
         self.encodeInternal(value, instance)
         return instance
 
     def encodeInternal(self, value, instance):
 
+        idValue = value.id
+        instance["id"] = serder.LONG.encode(idValue)
         clientValue = value.client
         instance["client"] = serder.STRING.encode(clientValue)
         from netbluemind.mailbox.api.rules.MailFilterRuleType import MailFilterRuleType
         from netbluemind.mailbox.api.rules.MailFilterRuleType import __MailFilterRuleTypeSerDer__
         typeValue = value.type
         instance["type"] = __MailFilterRuleTypeSerDer__().encode(typeValue)
         from netbluemind.mailbox.api.rules.MailFilterRuleTrigger import MailFilterRuleTrigger
```

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/MailFilterRuleTrigger.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/MailFilterRuleTrigger.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/MailFilterRuleType.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/MailFilterRuleType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleAction.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleAction.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionAddHeaders.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionAddHeaders.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCategorize.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCategorize.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCopy.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCopy.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCustom.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCustom.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionDeferredAction.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionDeferredAction.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionDiscard.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionDiscard.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsDeleted.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsDeleted.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsImportant.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsImportant.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsRead.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMarkAsRead.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMove.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionMove.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionName.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionName.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionPrioritize.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionPrioritize.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionRedirect.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionRedirect.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionRemoveHeaders.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionRemoveHeaders.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionReply.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionReply.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionSetFlags.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionSetFlags.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionTransfer.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionTransfer.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionUncategorize.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionUncategorize.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionUnfollow.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/actions/MailFilterRuleActionUnfollow.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleCondition.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleCondition.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleConditionOperator.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleConditionOperator.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilter.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContains.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContains.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContainsComparator.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContainsComparator.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContainsModifier.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterContainsModifier.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterEquals.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterEquals.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterExists.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterExists.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterMatches.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterMatches.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterRange.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleFilterRange.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/api/rules/conditions/MailFilterRuleOperatorName.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/conditions/MailFilterRuleOperatorName.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/IMailboxIdentity.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/IMailboxIdentity.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailboxIdentity_VERSION = "5.0.7152"
+IMailboxIdentity_VERSION = "5.0.7187"
 
 
 class IMailboxIdentity(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, mboxUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailboxes/{domainUid}/identity/{mboxUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/Identity.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/Identity.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/IdentityDescription.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/IdentityDescription.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailbox/identity/api/SignatureFormat.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/identity/api/SignatureFormat.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailflow/common/api/AssignmentActionMapping.py` & `netbluemind5-5.0.7187/netbluemind/mailflow/common/api/AssignmentActionMapping.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailflow/common/api/Message.py` & `netbluemind5-5.0.7187/netbluemind/mailflow/common/api/Message.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailflow/common/api/Recipient.py` & `netbluemind5-5.0.7187/netbluemind/mailflow/common/api/Recipient.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailflow/common/api/RecipientAddressType.py` & `netbluemind5-5.0.7187/netbluemind/mailflow/common/api/RecipientAddressType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailflow/common/api/RecipientRecipientType.py` & `netbluemind5-5.0.7187/netbluemind/mailflow/common/api/RecipientRecipientType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailflow/common/api/SendingAs.py` & `netbluemind5-5.0.7187/netbluemind/mailflow/common/api/SendingAs.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailmessage/api/IMailTip.py` & `netbluemind5-5.0.7187/netbluemind/mailmessage/api/IMailTip.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailTip_VERSION = "5.0.7152"
+IMailTip_VERSION = "5.0.7187"
 
 
 class IMailTip(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailtip/{domainUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTip.py` & `netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTip.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTipContext.py` & `netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTipContext.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTipFilter.py` & `netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTipFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTipFilterFilterType.py` & `netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTipFilterFilterType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailmessage/api/MailTips.py` & `netbluemind5-5.0.7187/netbluemind/mailmessage/api/MailTips.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailmessage/api/MessageContext.py` & `netbluemind5-5.0.7187/netbluemind/mailmessage/api/MessageContext.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/mailshare/api/IMailshare.py` & `netbluemind5-5.0.7187/netbluemind/mailshare/api/IMailshare.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailshare_VERSION = "5.0.7152"
+IMailshare_VERSION = "5.0.7187"
 
 
 class IMailshare(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailshares/{domainUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/mailshare/api/Mailshare.py` & `netbluemind5-5.0.7187/netbluemind/mailshare/api/Mailshare.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/INote.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/INote.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-INote_VERSION = "5.0.7152"
+INote_VERSION = "5.0.7187"
 
 
 class INote(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/notes/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/INoteIndexMgmt.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/INoteIndexMgmt.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-INoteIndexMgmt_VERSION = "5.0.7152"
+INoteIndexMgmt_VERSION = "5.0.7187"
 
 
 class INoteIndexMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/notes'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/INoteUids.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/INoteUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-INoteUids_VERSION = "5.0.7152"
+INoteUids_VERSION = "5.0.7187"
 
 
 class INoteUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/notes/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/INotes.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/INotes.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-INotes_VERSION = "5.0.7152"
+INotes_VERSION = "5.0.7187"
 
 
 class INotes(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/notes'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/VNote.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/VNote.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/VNoteChanges.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/VNoteChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/VNoteChangesItemAdd.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/VNoteChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/VNoteChangesItemDelete.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/VNoteChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/VNoteChangesItemModify.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/VNoteChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/VNoteColor.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/VNoteColor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/VNoteQuery.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/VNoteQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/notes/api/VNotesQuery.py` & `netbluemind5-5.0.7187/netbluemind/notes/api/VNotesQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/python/client.py` & `netbluemind5-5.0.7187/netbluemind/python/client.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/python/serder.py` & `netbluemind5-5.0.7187/netbluemind/python/serder.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/EventInfo.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/EventInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/IResources.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/IResources.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IResources_VERSION = "5.0.7152"
+IResources_VERSION = "5.0.7187"
 
 
 class IResources(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/resources/{domainUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/ResourceDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/ResourceDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/ResourceDescriptorPropertyValue.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/ResourceDescriptorPropertyValue.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/ResourceReservationMode.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/ResourceReservationMode.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/type/IResourceTypeUids.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/type/IResourceTypeUids.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IResourceTypeUids_VERSION = "5.0.7152"
+IResourceTypeUids_VERSION = "5.0.7187"
 
 
 class IResourceTypeUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mailbox/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/type/IResourceTypes.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/type/IResourceTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IResourceTypes_VERSION = "5.0.7152"
+IResourceTypes_VERSION = "5.0.7187"
 
 
 class IResourceTypes(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/resources/{domainUid}/type'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/type/ResourceType.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/type/ResourceType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/type/ResourceTypeDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/type/ResourceTypeDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/type/ResourceTypeDescriptorProperty.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/type/ResourceTypeDescriptorProperty.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/resource/api/type/ResourceTypeDescriptorPropertyType.py` & `netbluemind5-5.0.7187/netbluemind/resource/api/type/ResourceTypeDescriptorPropertyType.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/role/api/IRoles.py` & `netbluemind5-5.0.7187/netbluemind/role/api/IRoles.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IRoles_VERSION = "5.0.7152"
+IRoles_VERSION = "5.0.7187"
 
 
 class IRoles(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/roles'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/role/api/RoleDescriptor.py` & `netbluemind5-5.0.7187/netbluemind/role/api/RoleDescriptor.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/role/api/RolesCategory.py` & `netbluemind5-5.0.7187/netbluemind/role/api/RolesCategory.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/IJob.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/IJob.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IJob_VERSION = "5.0.7152"
+IJob_VERSION = "5.0.7187"
 
 
 class IJob(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/scheduledjobs'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/Job.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/Job.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobDomainStatus.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobDomainStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobExecution.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobExecution.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobExecutionQuery.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobExecutionQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobExitStatus.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobExitStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobKind.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobPlanification.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobPlanification.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobQuery.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/JobRec.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/JobRec.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/LogEntry.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/LogEntry.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/LogLevel.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/LogLevel.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/scheduledjob/api/PlanKind.py` & `netbluemind5-5.0.7187/netbluemind/scheduledjob/api/PlanKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/server/api/Assignment.py` & `netbluemind5-5.0.7187/netbluemind/server/api/Assignment.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/server/api/CommandStatus.py` & `netbluemind5-5.0.7187/netbluemind/server/api/CommandStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/server/api/IServer.py` & `netbluemind5-5.0.7187/netbluemind/server/api/IServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IServer_VERSION = "5.0.7152"
+IServer_VERSION = "5.0.7187"
 
 
 class IServer(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/servers/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/server/api/Server.py` & `netbluemind5-5.0.7187/netbluemind/server/api/Server.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/CertData.py` & `netbluemind5-5.0.7187/netbluemind/system/api/CertData.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/CertDataCertificateDomainEngine.py` & `netbluemind5-5.0.7187/netbluemind/system/api/CertDataCertificateDomainEngine.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/CloneConfiguration.py` & `netbluemind5-5.0.7187/netbluemind/system/api/CloneConfiguration.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/CloneConfigurationMode.py` & `netbluemind5-5.0.7187/netbluemind/system/api/CloneConfigurationMode.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/ConnectionTestStatus.py` & `netbluemind5-5.0.7187/netbluemind/system/api/ConnectionTestStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/CustomLogo.py` & `netbluemind5-5.0.7187/netbluemind/system/api/CustomLogo.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplate.py` & `netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplate.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplateDescription.py` & `netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplateDescription.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplateDescriptionI18NDescription.py` & `netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplateDescriptionI18NDescription.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplateKind.py` & `netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplateKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/DomainTemplateTag.py` & `netbluemind5-5.0.7187/netbluemind/system/api/DomainTemplateTag.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/ExternalSystem.py` & `netbluemind5-5.0.7187/netbluemind/system/api/ExternalSystem.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/ExternalSystemAuthKind.py` & `netbluemind5-5.0.7187/netbluemind/system/api/ExternalSystemAuthKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/ICacheMgmt.py` & `netbluemind5-5.0.7187/netbluemind/system/api/ICacheMgmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICacheMgmt_VERSION = "5.0.7152"
+ICacheMgmt_VERSION = "5.0.7187"
 
 
 class ICacheMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/cache'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/ICustomTheme.py` & `netbluemind5-5.0.7187/netbluemind/system/api/ICustomTheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ICustomTheme_VERSION = "5.0.7152"
+ICustomTheme_VERSION = "5.0.7187"
 
 
 class ICustomTheme(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + ''
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/IDomainTemplate.py` & `netbluemind5-5.0.7187/netbluemind/system/api/IDomainTemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IDomainTemplate_VERSION = "5.0.7152"
+IDomainTemplate_VERSION = "5.0.7187"
 
 
 class IDomainTemplate(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/domaintemplate'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/IExternalSystem.py` & `netbluemind5-5.0.7187/netbluemind/system/api/IExternalSystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IExternalSystem_VERSION = "5.0.7152"
+IExternalSystem_VERSION = "5.0.7187"
 
 
 class IExternalSystem(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/external'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/IGlobalSettings.py` & `netbluemind5-5.0.7187/netbluemind/system/api/IGlobalSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IGlobalSettings_VERSION = "5.0.7152"
+IGlobalSettings_VERSION = "5.0.7187"
 
 
 class IGlobalSettings(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/global_settings'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/IInstallation.py` & `netbluemind5-5.0.7187/netbluemind/system/api/IInstallation.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IInstallation_VERSION = "5.0.7152"
+IInstallation_VERSION = "5.0.7187"
 
 
 class IInstallation(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/installation'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/IInternalFirewallMgmt.py` & `netbluemind5-5.0.7187/netbluemind/system/api/IInternalFirewallMgmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IInternalFirewallMgmt_VERSION = "5.0.7152"
+IInternalFirewallMgmt_VERSION = "5.0.7187"
 
 
 class IInternalFirewallMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/firewall'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/IMailDeliveryMgmt.py` & `netbluemind5-5.0.7187/netbluemind/system/api/IMailDeliveryMgmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IMailDeliveryMgmt_VERSION = "5.0.7152"
+IMailDeliveryMgmt_VERSION = "5.0.7187"
 
 
 class IMailDeliveryMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/maildelivery/mgmt'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/ISchemaMgmt.py` & `netbluemind5-5.0.7187/netbluemind/system/api/ISchemaMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISchemaMgmt_VERSION = "5.0.7152"
+ISchemaMgmt_VERSION = "5.0.7187"
 
 
 class ISchemaMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/schema'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/ISecurityMgmt.py` & `netbluemind5-5.0.7187/netbluemind/system/api/ISecurityMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISecurityMgmt_VERSION = "5.0.7152"
+ISecurityMgmt_VERSION = "5.0.7187"
 
 
 class ISecurityMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/system/security'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/ISystemConfiguration.py` & `netbluemind5-5.0.7187/netbluemind/system/api/ISystemConfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ISystemConfiguration_VERSION = "5.0.7152"
+ISystemConfiguration_VERSION = "5.0.7187"
 
 
 class ISystemConfiguration(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/configuration'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/InstallationVersion.py` & `netbluemind5-5.0.7187/netbluemind/system/api/InstallationVersion.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/PublicInfos.py` & `netbluemind5-5.0.7187/netbluemind/system/api/PublicInfos.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SchemaCheckInfo.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SchemaCheckInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformations.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformations.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsInstallationIndicator.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsInstallationIndicator.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsInstallationIndicatorKind.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsInstallationIndicatorKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsKind.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsMessage.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsMessage.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsMessageCode.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsMessageCode.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SubscriptionInformationsMessageKind.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SubscriptionInformationsMessageKind.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SystemConf.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SystemConf.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/SystemState.py` & `netbluemind5-5.0.7187/netbluemind/system/api/SystemState.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/UpgradeReport.py` & `netbluemind5-5.0.7187/netbluemind/system/api/UpgradeReport.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/UpgradeReportStatus.py` & `netbluemind5-5.0.7187/netbluemind/system/api/UpgradeReportStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/UpgradeReportUpgraderReport.py` & `netbluemind5-5.0.7187/netbluemind/system/api/UpgradeReportUpgraderReport.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/UpgradeStatus.py` & `netbluemind5-5.0.7187/netbluemind/system/api/UpgradeStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/UpgradeStatusState.py` & `netbluemind5-5.0.7187/netbluemind/system/api/UpgradeStatusState.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeProgress.py` & `netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeProgress.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeStepEvent.py` & `netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeStepEvent.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeStepEventStatus.py` & `netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeStepEventStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeTask.py` & `netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeTask.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeTaskExecutionMode.py` & `netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeTaskExecutionMode.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeTaskFilter.py` & `netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeTaskFilter.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/HotUpgradeTaskStatus.py` & `netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/HotUpgradeTaskStatus.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/IHotUpgrade.py` & `netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/IHotUpgrade.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IHotUpgrade_VERSION = "5.0.7152"
+IHotUpgrade_VERSION = "5.0.7187"
 
 
 class IHotUpgrade(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/hot_upgrade'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/system/api/hot/upgrade/IInternalHotUpgrade.py` & `netbluemind5-5.0.7187/netbluemind/system/api/hot/upgrade/IInternalHotUpgrade.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IInternalHotUpgrade_VERSION = "5.0.7152"
+IInternalHotUpgrade_VERSION = "5.0.7187"
 
 
 class IInternalHotUpgrade(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/hot_upgrade'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/tag/api/ITagUids.py` & `netbluemind5-5.0.7187/netbluemind/mailbox/api/rules/RuleMoveRelativePosition.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,30 +14,31 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 #
 #  See LICENSE.txt
 #  END LICENSE
 #
 import requests
-import json
 from netbluemind.python import serder
-from netbluemind.python.client import BaseEndpoint
+from enum import Enum
 
-ITagUids_VERSION = "5.0.7152"
 
+class RuleMoveRelativePosition(Enum):
+    BEFORE = 'BEFORE'
+    AFTER = 'AFTER'
 
-class ITagUids(BaseEndpoint):
-    def __init__(self, apiKey, url):
-        self.url = url
-        self.apiKey = apiKey
-        self.base = url + '/tags/uids'
-
-    def getDefaultUserTags(self, uid):
-        postUri = "/{uid}/_default_tags"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        queryParams = {}
-
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': ITagUids_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.STRING, response)
+
+class __RuleMoveRelativePositionSerDer__:
+    def __init__(self):
+        pass
+
+    def parse(self, value):
+        if (value == None):
+            return None
+        instance = RuleMoveRelativePosition[value]
+        return instance
+
+    def encode(self, value):
+        if (value == None):
+            return None
+        instance = value.value
+        return instance
```

### Comparing `netbluemind5-5.0.7152/netbluemind/tag/api/ITags.py` & `netbluemind5-5.0.7187/netbluemind/tag/api/ITags.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITags_VERSION = "5.0.7152"
+ITags_VERSION = "5.0.7187"
 
 
 class ITags(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/tags/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/tag/api/Tag.py` & `netbluemind5-5.0.7187/netbluemind/tag/api/Tag.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/tag/api/TagChanges.py` & `netbluemind5-5.0.7187/netbluemind/tag/api/TagChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/tag/api/TagChangesItemAdd.py` & `netbluemind5-5.0.7187/netbluemind/tag/api/TagChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/tag/api/TagChangesItemDelete.py` & `netbluemind5-5.0.7187/netbluemind/tag/api/TagChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/tag/api/TagChangesItemModify.py` & `netbluemind5-5.0.7187/netbluemind/tag/api/TagChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/tag/api/TagRef.py` & `netbluemind5-5.0.7187/netbluemind/tag/api/TagRef.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/ITodoList.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/ITodoList.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITodoList_VERSION = "5.0.7152"
+ITodoList_VERSION = "5.0.7187"
 
 
 class ITodoList(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/todolist/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/ITodoLists.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/ITodoLists.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITodoLists_VERSION = "5.0.7152"
+ITodoLists_VERSION = "5.0.7187"
 
 
 class ITodoLists(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/todolists'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/ITodoListsMgmt.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/ITodoListsMgmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITodoListsMgmt_VERSION = "5.0.7152"
+ITodoListsMgmt_VERSION = "5.0.7187"
 
 
 class ITodoListsMgmt(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/mgmt/todolists'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/ITodoUids.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/ITodoUids.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-ITodoUids_VERSION = "5.0.7152"
+ITodoUids_VERSION = "5.0.7187"
 
 
 class ITodoUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/todolist/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/IVTodo.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/IVTodo.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IVTodo_VERSION = "5.0.7152"
+IVTodo_VERSION = "5.0.7187"
 
 
 class IVTodo(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/todolists/vtodos/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/TodoListsVTodoQuery.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/TodoListsVTodoQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/VTodo.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/VTodo.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoChanges.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoChanges.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoChangesItemAdd.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoChangesItemAdd.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoChangesItemDelete.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoChangesItemDelete.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoChangesItemModify.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoChangesItemModify.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/todolist/api/VTodoQuery.py` & `netbluemind5-5.0.7187/netbluemind/todolist/api/VTodoQuery.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/ChangePassword.py` & `netbluemind5-5.0.7187/netbluemind/user/api/ChangePassword.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/IUser.py` & `netbluemind5-5.0.7187/netbluemind/webappdata/api/IWebAppData.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,350 +18,237 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUser_VERSION = "5.0.7152"
+IWebAppData_VERSION = "5.0.7187"
 
 
-class IUser(BaseEndpoint):
-    def __init__(self, apiKey, url, domainUid):
+class IWebAppData(BaseEndpoint):
+    def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
-        self.base = url + '/users/{domainUid}'
-        self.domainUid_ = domainUid
-        self.base = self.base.replace('{domainUid}', domainUid)
+        self.base = url + '/webappdata/{containerUid}'
+        self.containerUid_ = containerUid
+        self.base = self.base.replace('{containerUid}', containerUid)
 
-    def allUids(self):
-        postUri = "/_alluids"
+    def allIds(self, filter, knownContainerVersion, limit, offset):
+        postUri = "/_itemIds"
         __data__ = None
         __encoded__ = None
-        queryParams = {}
+        queryParams = {'filter': filter, 'knownContainerVersion':
+                       knownContainerVersion, 'limit': limit, 'offset': offset}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.ListSerDer(serder.STRING), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.core.api.ListResult import ListResult
+        from netbluemind.core.api.ListResult import __ListResultSerDer__
+        return self.handleResult__(__ListResultSerDer__(serder.LONG), response)
 
-    def byEmail(self, email):
-        postUri = "/byEmail/{email}"
+    def allUids(self):
+        postUri = "/_alluids"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{email}", email)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        from netbluemind.user.api.User import User
-        from netbluemind.user.api.User import __UserSerDer__
-        from netbluemind.core.container.model.ItemValue import ItemValue
-        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(__ItemValueSerDer__(__UserSerDer__()), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        return self.handleResult__(serder.ListSerDer(serder.STRING), response)
 
-    def byExtId(self, extid):
-        postUri = "/byExtId/{extid}"
+    def changeset(self, since):
+        postUri = "/_changeset"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{extid}", extid)
-        queryParams = {}
+        queryParams = {'since': since}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        from netbluemind.user.api.User import User
-        from netbluemind.user.api.User import __UserSerDer__
-        from netbluemind.core.container.model.ItemValue import ItemValue
-        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(__ItemValueSerDer__(__UserSerDer__()), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.core.container.model.ContainerChangeset import ContainerChangeset
+        from netbluemind.core.container.model.ContainerChangeset import __ContainerChangesetSerDer__
+        return self.handleResult__(__ContainerChangesetSerDer__(serder.STRING), response)
 
-    def byLogin(self, login):
-        postUri = "/byLogin/{login}"
+    def changesetById(self, since):
+        postUri = "/_changesetById"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{login}", login)
-        queryParams = {}
+        queryParams = {'since': since}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        from netbluemind.user.api.User import User
-        from netbluemind.user.api.User import __UserSerDer__
-        from netbluemind.core.container.model.ItemValue import ItemValue
-        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(__ItemValueSerDer__(__UserSerDer__()), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.core.container.model.ContainerChangeset import ContainerChangeset
+        from netbluemind.core.container.model.ContainerChangeset import __ContainerChangesetSerDer__
+        return self.handleResult__(__ContainerChangesetSerDer__(serder.LONG), response)
 
-    def create(self, uid, user):
-        postUri = "/{uid}"
+    def create(self, uid, arg1):
+        postUri = "/uid/{uid}"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
-        from netbluemind.user.api.User import User
-        from netbluemind.user.api.User import __UserSerDer__
-        __data__ = __UserSerDer__().encode(user)
+        from netbluemind.webappdata.api.WebAppData import WebAppData
+        from netbluemind.webappdata.api.WebAppData import __WebAppDataSerDer__
+        __data__ = __WebAppDataSerDer__().encode(arg1)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.put(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
-
-    def createWithExtId(self, uid, extid, user):
-        postUri = "/{uid}/{extid}/createwithextid"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        postUri = postUri.replace("{extid}", extid)
-        from netbluemind.user.api.User import User
-        from netbluemind.user.api.User import __UserSerDer__
-        __data__ = __UserSerDer__().encode(user)
-        __encoded__ = json.dumps(__data__)
-        queryParams = {}
-
-        response = requests.put(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.core.container.api.Ack import Ack
+        from netbluemind.core.container.api.Ack import __AckSerDer__
+        return self.handleResult__(__AckSerDer__(), response)
 
     def delete(self, uid):
-        postUri = "/{uid}"
+        postUri = "/uid/{uid}"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.delete(self.base + postUri, params=queryParams, verify=False, headers={
-                                   'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        from netbluemind.core.task.api.TaskRef import TaskRef
-        from netbluemind.core.task.api.TaskRef import __TaskRefSerDer__
-        return self.handleResult__(__TaskRefSerDer__(), response)
+                                   'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        return self.handleResult__(None, response)
 
-    def deletePhoto(self, uid):
-        postUri = "/{uid}/photo"
+    def deleteAll(self):
+        postUri = "/_deleteAll"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.delete(self.base + postUri, params=queryParams, verify=False, headers={
-                                   'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
+                                   'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
         return self.handleResult__(None, response)
 
-    def enablePerUserLog(self, userUid, endpoint, enable):
-        postUri = "/{userUid}/_logging/{endpoint}"
+    def filteredChangesetById(self, since, arg1):
+        postUri = "/_filteredChangesetById"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{userUid}", userUid)
-        postUri = postUri.replace("{endpoint}", endpoint)
-        __data__ = serder.BOOLEAN.encode(enable)
+        from netbluemind.core.container.model.ItemFlagFilter import ItemFlagFilter
+        from netbluemind.core.container.model.ItemFlagFilter import __ItemFlagFilterSerDer__
+        __data__ = __ItemFlagFilterSerDer__().encode(arg1)
         __encoded__ = json.dumps(__data__)
-        queryParams = {}
+        queryParams = {'since': since}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.core.container.model.ItemVersion import ItemVersion
+        from netbluemind.core.container.model.ItemVersion import __ItemVersionSerDer__
+        from netbluemind.core.container.model.ContainerChangeset import ContainerChangeset
+        from netbluemind.core.container.model.ContainerChangeset import __ContainerChangesetSerDer__
+        return self.handleResult__(__ContainerChangesetSerDer__(__ItemVersionSerDer__()), response)
 
-    def getComplete(self, uid):
-        postUri = "/{uid}/complete"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        queryParams = {}
-
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        from netbluemind.user.api.User import User
-        from netbluemind.user.api.User import __UserSerDer__
-        from netbluemind.core.container.model.ItemValue import ItemValue
-        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(__ItemValueSerDer__(__UserSerDer__()), response)
-
-    def getIcon(self, uid):
-        postUri = "/{uid}/icon"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        queryParams = {}
-
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.ByteArraySerDer, response)
-
-    def getPhoto(self, uid):
-        postUri = "/{uid}/photo"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        queryParams = {}
-
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.ByteArraySerDer, response)
-
-    def getResolvedRoles(self, uid):
-        postUri = "/{uid}/roles_resolved"
+    def getByKey(self, key):
+        postUri = "/key/{key}"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
+        postUri = postUri.replace("{key}", key)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.SetSerDer(serder.STRING), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.webappdata.api.WebAppData import WebAppData
+        from netbluemind.webappdata.api.WebAppData import __WebAppDataSerDer__
+        return self.handleResult__(__WebAppDataSerDer__(), response)
 
-    def getRoles(self, uid):
-        postUri = "/{uid}/roles"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        queryParams = {}
-
-        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.SetSerDer(serder.STRING), response)
-
-    def getUsersWithRoles(self, roles):
-        postUri = "/_roleusers"
-        __data__ = None
-        __encoded__ = None
-        __data__ = serder.ListSerDer(serder.STRING).encode(roles)
-        __encoded__ = json.dumps(__data__)
-        queryParams = {}
-
-        response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.SetSerDer(serder.STRING), response)
-
-    def getVCard(self, uid):
-        postUri = "/{uid}/vcard"
+    def getComplete(self, uid):
+        postUri = "/uid/{uid}"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        from netbluemind.addressbook.api.VCard import VCard
-        from netbluemind.addressbook.api.VCard import __VCardSerDer__
-        return self.handleResult__(__VCardSerDer__(), response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.webappdata.api.WebAppData import WebAppData
+        from netbluemind.webappdata.api.WebAppData import __WebAppDataSerDer__
+        from netbluemind.core.container.model.ItemValue import ItemValue
+        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
+        return self.handleResult__(__ItemValueSerDer__(__WebAppDataSerDer__()), response)
 
-    def memberOf(self, uid):
-        postUri = "/{uid}/groups"
+    def getCompleteById(self, id):
+        postUri = "/{id}/completeById"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
+        postUri = postUri.replace("{id}", id)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        from netbluemind.group.api.Group import Group
-        from netbluemind.group.api.Group import __GroupSerDer__
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.webappdata.api.WebAppData import WebAppData
+        from netbluemind.webappdata.api.WebAppData import __WebAppDataSerDer__
         from netbluemind.core.container.model.ItemValue import ItemValue
         from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
-        return self.handleResult__(serder.ListSerDer(__ItemValueSerDer__(__GroupSerDer__())), response)
+        return self.handleResult__(__ItemValueSerDer__(__WebAppDataSerDer__()), response)
 
-    def memberOfGroups(self, uid):
-        postUri = "/{uid}/groupUids"
+    def getVersion(self):
+        postUri = "/_version"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
         queryParams = {}
 
         response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
-                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(serder.ListSerDer(serder.STRING), response)
-
-    def setExtId(self, uid, arg1):
-        postUri = "/{uid}/_extId"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        __data__ = serder.STRING.encode(arg1)
-        __encoded__ = json.dumps(__data__)
-        queryParams = {}
-
-        response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
-
-    def setPassword(self, uid, password):
-        postUri = "/{uid}/password_"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        from netbluemind.user.api.ChangePassword import ChangePassword
-        from netbluemind.user.api.ChangePassword import __ChangePasswordSerDer__
-        __data__ = __ChangePasswordSerDer__().encode(password)
-        __encoded__ = json.dumps(__data__)
-        queryParams = {}
-
-        response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
-
-    def setPhoto(self, uid, arg1):
-        postUri = "/{uid}/photo"
-        __data__ = None
-        __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        __data__ = serder.ByteArraySerDer.encode(arg1)
-        __encoded__ = json.dumps(__data__)
-        queryParams = {}
-
-        response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        return self.handleResult__(serder.LONG, response)
 
-    def setRoles(self, uid, roles):
-        postUri = "/{uid}/roles"
+    def itemChangelog(self, uid, arg1):
+        postUri = "/{uid}/_itemchangelog"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
-        __data__ = serder.SetSerDer(serder.STRING).encode(roles)
+        __data__ = serder.LONG.encode(arg1)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
-        response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
+        response = requests.get(self.base + postUri, params=queryParams, verify=False, headers={
+                                'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.core.container.model.ItemChangelog import ItemChangelog
+        from netbluemind.core.container.model.ItemChangelog import __ItemChangelogSerDer__
+        return self.handleResult__(__ItemChangelogSerDer__(), response)
 
-    def update(self, uid, user):
-        postUri = "/{uid}"
+    def multipleGet(self, arg0):
+        postUri = "/uid/_mget"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        from netbluemind.user.api.User import User
-        from netbluemind.user.api.User import __UserSerDer__
-        __data__ = __UserSerDer__().encode(user)
+        __data__ = serder.ListSerDer(serder.STRING).encode(arg0)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.webappdata.api.WebAppData import WebAppData
+        from netbluemind.webappdata.api.WebAppData import __WebAppDataSerDer__
+        from netbluemind.core.container.model.ItemValue import ItemValue
+        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
+        return self.handleResult__(serder.ListSerDer(__ItemValueSerDer__(__WebAppDataSerDer__())), response)
 
-    def updateAccountType(self, uid, accountType):
-        postUri = "/_updateAccountType/{uid}"
+    def multipleGetById(self, arg0):
+        postUri = "/_mgetById"
         __data__ = None
         __encoded__ = None
-        postUri = postUri.replace("{uid}", uid)
-        from netbluemind.directory.api.BaseDirEntryAccountType import BaseDirEntryAccountType
-        from netbluemind.directory.api.BaseDirEntryAccountType import __BaseDirEntryAccountTypeSerDer__
-        __data__ = __BaseDirEntryAccountTypeSerDer__().encode(accountType)
+        __data__ = serder.ListSerDer(serder.LONG).encode(arg0)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.webappdata.api.WebAppData import WebAppData
+        from netbluemind.webappdata.api.WebAppData import __WebAppDataSerDer__
+        from netbluemind.core.container.model.ItemValue import ItemValue
+        from netbluemind.core.container.model.ItemValue import __ItemValueSerDer__
+        return self.handleResult__(serder.ListSerDer(__ItemValueSerDer__(__WebAppDataSerDer__())), response)
 
-    def updateVCard(self, uid, userVCard):
-        postUri = "/{uid}/vcard"
+    def update(self, uid, arg1):
+        postUri = "/uid/{uid}"
         __data__ = None
         __encoded__ = None
         postUri = postUri.replace("{uid}", uid)
-        from netbluemind.addressbook.api.VCard import VCard
-        from netbluemind.addressbook.api.VCard import __VCardSerDer__
-        __data__ = __VCardSerDer__().encode(userVCard)
+        from netbluemind.webappdata.api.WebAppData import WebAppData
+        from netbluemind.webappdata.api.WebAppData import __WebAppDataSerDer__
+        __data__ = __WebAppDataSerDer__().encode(arg1)
         __encoded__ = json.dumps(__data__)
         queryParams = {}
 
         response = requests.post(self.base + postUri, params=queryParams, verify=False, headers={
-                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IUser_VERSION}, data=__encoded__)
-        return self.handleResult__(None, response)
+                                 'X-BM-ApiKey': self.apiKey, 'Accept': 'application/json', 'X-BM-ClientVersion': IWebAppData_VERSION}, data=__encoded__)
+        from netbluemind.core.container.api.Ack import Ack
+        from netbluemind.core.container.api.Ack import __AckSerDer__
+        return self.handleResult__(__AckSerDer__(), response)
```

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/IUserExternalAccount.py` & `netbluemind5-5.0.7187/netbluemind/user/api/IUserExternalAccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserExternalAccount_VERSION = "5.0.7152"
+IUserExternalAccount_VERSION = "5.0.7187"
 
 
 class IUserExternalAccount(BaseEndpoint):
     def __init__(self, apiKey, url, domain, uid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{domain}/{uid}/accounts'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/IUserMailIdentities.py` & `netbluemind5-5.0.7187/netbluemind/user/api/IUserMailIdentities.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserMailIdentities_VERSION = "5.0.7152"
+IUserMailIdentities_VERSION = "5.0.7187"
 
 
 class IUserMailIdentities(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid, userUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{domainUid}/{userUid}/identity'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/IUserSettings.py` & `netbluemind5-5.0.7187/netbluemind/user/api/IUserSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserSettings_VERSION = "5.0.7152"
+IUserSettings_VERSION = "5.0.7187"
 
 
 class IUserSettings(BaseEndpoint):
     def __init__(self, apiKey, url, containerUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{containerUid}'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/IUserSubscription.py` & `netbluemind5-5.0.7187/netbluemind/user/api/IUserSubscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IUserSubscription_VERSION = "5.0.7152"
+IUserSubscription_VERSION = "5.0.7187"
 
 
 class IUserSubscription(BaseEndpoint):
     def __init__(self, apiKey, url, domainUid):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/users/{domainUid}/subscriptions'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/User.py` & `netbluemind5-5.0.7187/netbluemind/user/api/User.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/UserAccount.py` & `netbluemind5-5.0.7187/netbluemind/user/api/UserAccount.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/UserAccountInfo.py` & `netbluemind5-5.0.7187/netbluemind/user/api/UserAccountInfo.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/UserMailIdentity.py` & `netbluemind5-5.0.7187/netbluemind/user/api/UserMailIdentity.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/user/api/UserSettings.py` & `netbluemind5-5.0.7187/netbluemind/user/api/UserSettings.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind/webappdata/api/IWebAppDataUids.py` & `netbluemind5-5.0.7187/netbluemind/webappdata/api/IWebAppDataUids.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  END LICENSE
 #
 import requests
 import json
 from netbluemind.python import serder
 from netbluemind.python.client import BaseEndpoint
 
-IWebAppDataUids_VERSION = "5.0.7152"
+IWebAppDataUids_VERSION = "5.0.7187"
 
 
 class IWebAppDataUids(BaseEndpoint):
     def __init__(self, apiKey, url):
         self.url = url
         self.apiKey = apiKey
         self.base = url + '/webappdata/uids'
```

### Comparing `netbluemind5-5.0.7152/netbluemind/webappdata/api/WebAppData.py` & `netbluemind5-5.0.7187/netbluemind/webappdata/api/WebAppData.py`

 * *Files identical despite different names*

### Comparing `netbluemind5-5.0.7152/netbluemind5.egg-info/SOURCES.txt` & `netbluemind5-5.0.7187/netbluemind5.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,16 @@
 netbluemind/mailbox/api/ShardStatsState.py
 netbluemind/mailbox/api/SimpleShardStats.py
 netbluemind/mailbox/api/__init__.py
 netbluemind/mailbox/api/rules/DelegationRule.py
 netbluemind/mailbox/api/rules/MailFilterRule.py
 netbluemind/mailbox/api/rules/MailFilterRuleTrigger.py
 netbluemind/mailbox/api/rules/MailFilterRuleType.py
+netbluemind/mailbox/api/rules/RuleMoveDirection.py
+netbluemind/mailbox/api/rules/RuleMoveRelativePosition.py
 netbluemind/mailbox/api/rules/__init__.py
 netbluemind/mailbox/api/rules/actions/MailFilterRuleAction.py
 netbluemind/mailbox/api/rules/actions/MailFilterRuleActionAddHeaders.py
 netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCategorize.py
 netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCopy.py
 netbluemind/mailbox/api/rules/actions/MailFilterRuleActionCustom.py
 netbluemind/mailbox/api/rules/actions/MailFilterRuleActionDeferredAction.py
```

### Comparing `netbluemind5-5.0.7152/setup.py` & `netbluemind5-5.0.7187/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 install_requires = ['requests']
 if sys.version_info < (3, 4):
     install_requires.append('enum34')
 
 setup(
     name = 'netbluemind5',
     packages = find_packages(),
-    version = '5.0.7152',
+    version = '5.0.7187',
     description = 'Automatically generated client for BlueMind >= 5 REST API. Check netbluemind4 for older releases',
     author = 'BlueMind team',
     author_email = 'contact@bluemind.net',
     url = 'http://gitlab.bluemind.net/',
     keywords = ['bluemind', 'rest', 'api', 'mail', 'groupware'],
     classifiers = [
         'Development Status :: 5 - Production/Stable',
```

