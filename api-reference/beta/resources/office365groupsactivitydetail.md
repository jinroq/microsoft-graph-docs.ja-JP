---
title: office365GroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: a849932d646be61f3cedec76ecdafdaca941baaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067253"
---
# <a name="office365groupsactivitydetail-resource-type"></a>office365GroupsActivityDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                          | 型    | 説明                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| reportRefreshDate                 | Date    | コンテンツの最新の日付。          |
| groupDisplayName                  | String  | グループの表示名。           |
| isDeleted                         | ブール値 | このユーザーが削除されたか、またはソフトをされてかどうかを削除します。 |
| ownerPrincipalName                | String  | グループの所有者のプリンシパル名です。          |
| lastActivityDate                  | Date    | 次のシナリオの最後のアクティビティの日付: グループのメールボックスに受信した電子メールです。ユーザーを表示、編集、共有、または SharePoint ドキュメント ライブラリ内のファイルの同期ユーザーが SharePoint ページを表示ユーザーは、投稿、読み取り、または、Yammer グループ内のメッセージを気に入られました。 |
| groupType                         | String  | グループの種類。 使用可能な値:**パブリック**または**プライベート**です。 |
| membercount プロパティ                       | Int64   | グループ メンバーの数です。                  |
| externalMemberCount               | Int64   | グループ外部のメンバーの数です。         |
| exchangeReceivedEmailCount        | Int64   | グループのメールボックスで受信した電子メールの数。 |
| sharePointActiveFileCount         | Int64   | SharePoint グループのサイト内のアクティブなファイルの数です。 |
| yammerPostedMessageCount          | Int64   | Yammer のグループに投稿されたメッセージの数です。 |
| yammerReadMessageCount            | Int64   | Yammer グループでメッセージの数を読み取る。 |
| yammerLikedMessageCount           | Int64   | Yammer グループに賛同のメッセージの数です。 |
| exchangeMailboxTotalItemCount     | Int64   | グループ メールボックス内のアイテムの数です。 |
| exchangeMailboxStorageUsedInBytes | Int64   | ・ ストレージ ・ グループのメールボックスのために使用します。   |
| sharePointTotalFileCount          | Int64   | SharePoint グループのサイト内のファイルの合計数です。 |
| sharePointSiteStorageUsedInBytes  | Int64   | ・ ストレージ ・ グループを SharePoint サイトで使用されます。 |
| reportPeriod                      | String  | レポートの対象日数です。    |

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
