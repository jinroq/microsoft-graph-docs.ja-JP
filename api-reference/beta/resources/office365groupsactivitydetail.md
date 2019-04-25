---
title: office365GroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581451"
---
# <a name="office365groupsactivitydetail-resource-type"></a>office365GroupsActivityDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                          | 型    | 説明                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| reportrefreshdate                 | Date    | コンテンツの最新の日付。          |
| groupdisplayname                  | String  | グループの表示名。           |
| isDeleted                         | Boolean | このユーザーが削除されているか、または削除されているか。 |
| ownerPrincipalName                | String  | グループ所有者のプリンシパル名。          |
| lastactivitydate                  | Date    | 次のシナリオの最後のアクティビティの日付: グループメールが受信した電子メール。SharePoint ドキュメントライブラリでユーザーが表示、編集、共有、または同期されたファイル。ユーザーが SharePoint ページを表示した。Yammer グループ内のユーザー投稿、閲覧、またはいいねのメッセージ。 |
| groupType                         | String  | グループの種類。 使用可能な値は、 **Public**または**Private**です。 |
| memberCount                       | Int64   | グループメンバー数。                  |
| externalMemberCount               | Int64   | グループの外部メンバー数。         |
| exchangeReceivedEmailCount        | Int64   | グループメールボックスが受信したメールの数。 |
| sharePointActiveFileCount         | Int64   | SharePoint グループサイト内のアクティブなファイルの数。 |
| yammerPostedMessageCount          | Int64   | Yammer グループに投稿されたメッセージの数。 |
| yammerReadMessageCount            | Int64   | Yammer グループで読み取られたメッセージの数。 |
| yammerLikedMessageCount           | Int64   | Yammer グループに賛同されたメッセージの数。 |
| exchangeMailboxTotalItemCount     | Int64   | グループメールボックス内のアイテムの数。 |
| exchangeMailboxStorageUsedInBytes | Int64   | グループメールボックスで使用されている記憶域。   |
| sharePointTotalFileCount          | Int64   | SharePoint グループサイト内のファイルの合計数。 |
| sharepointsitestorageused inbytes  | Int64   | SharePoint グループサイトで使用される記憶域。 |
| reportperiod                      | String  | レポートの対象となる日数を指定します。    |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```
