---
title: office365ActiveUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 9e58e0d4613118cd8ceecfcae318982bc2035917
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009497"
---
# <a name="office365activeuserdetail-resource-type"></a>office365ActiveUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                          | 型              | 説明                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | 日付              | コンテンツの最新の日付。          |
| userPrincipalName                 | String            | ユーザーのユーザープリンシパル名 (UPN)。 UPN は、インターネット標準 RFC 822 に基づくユーザーのインターネットスタイルのログイン名です。 規則により、これはユーザーの電子メール名にマップする必要があります。 一般的な形式は、検証済みドメインのテナントのコレクションにドメインが存在する必要がある、エイリアス @ domain です。 このプロパティは、ユーザーの作成時に必要です。 |
| displayName                       | 文字列            | アドレス帳に表示されるユーザーの名前。 これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。 このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。 |
| isDeleted                         | Boolean           | このユーザーが削除されているか、または削除されているか。 |
| deletedDate                       | 日付              | 削除操作が発生した日付。 ユーザーが削除されていない場合、既定値は "null" です。 |
| hasExchangeLicense                | Boolean           | ユーザーに Exchange ライセンスが割り当てられているかどうか。 |
| hasOneDriveLicense                | Boolean           | ユーザーに OneDrive ライセンスが割り当てられているかどうか。 |
| hasSharePointLicense              | Boolean           | ユーザーに SharePoint ライセンスが割り当てられているかどうか。 |
| hasSkypeForBusinessLicense        | Boolean           | ユーザーに Skype For Business ライセンスが割り当てられているかどうか。 |
| hasYammerLicense                  | Boolean           | ユーザーに Yammer ライセンスが割り当てられているかどうか。 |
| hasTeamsLicense                   | Boolean           | ユーザーに Teams ライセンスが割り当てられているかどうか。 |
| exchangeLastActivityDate          | 日付              | ユーザーが最後に電子メールを読んだり送信したりした日付。 |
| oneDriveLastActivityDate          | 日付              | ユーザーが最後にファイルを表示または編集した日付、共有ファイルの内部または外部、または同期したファイル。 |
| sharePointLastActivityDate        | 日付              | ユーザーが最後にファイルを表示または編集した日付、共有ファイルの内部または外部、同期済みファイル、または SharePoint ページを表示した日付。 |
| skypeForBusinessLastActivityDate  | 日付              | ユーザーが会議に最後に開催または参加した日付、またはピアツーピアセッションに参加した日付。 |
| yammerLastActivityDate            | 日付              | ユーザーが最後に投稿、閲覧、または「いいね!」のメッセージを最後に投稿した日付。 |
| teamsLastActivityDate             | 日付              | ユーザーがチームチャネルでメッセージを最後に投稿した日、プライベートチャットセッションでメッセージを送信した、または会議または通話に参加した日付。 |
| exchangeLicenseAssignDate         | 日付              | ユーザーが Exchange ライセンスを割り当てられた最後の日付。 |
| oneDriveLicenseAssignDate         | 日付              | ユーザーが OneDrive ライセンスを割り当てられた最後の日付。 |
| Sharepointlicenseの割り当て日付       | 日付              | ユーザーが SharePoint ライセンスを割り当てられた最後の日付。 |
| Skypeforbusinesslicenseの割り当て日付 | 日付              | ユーザーが Skype For Business ライセンスを割り当てられた最後の日付。 |
| yammerLicenseAssignDate           | 日付              | ユーザーが Yammer ライセンスを割り当てられた最後の日付。 |
| Teamslicenseの割り当て日付            | 日付              | ユーザーが Teams ライセンスを割り当てられた最後の日付。 |
| assignedProducts                  | 文字列コレクション | ユーザーに割り当てられているすべての製品。  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "hasExchangeLicense": true, 
  "hasOneDriveLicense": true, 
  "hasSharePointLicense": true, 
  "hasSkypeForBusinessLicense": true, 
  "hasYammerLicense": true, 
  "hasTeamsLicense": true, 
  "exchangeLastActivityDate": "Date", 
  "oneDriveLastActivityDate": "Date", 
  "sharePointLastActivityDate": "Date", 
  "skypeForBusinessLastActivityDate": "Date", 
  "yammerLastActivityDate": "Date", 
  "teamsLastActivityDate": "Date", 
  "exchangeLicenseAssignDate": "Date", 
  "oneDriveLicenseAssignDate": "Date", 
  "sharePointLicenseAssignDate": "Date", 
  "skypeForBusinessLicenseAssignDate": "Date", 
  "yammerLicenseAssignDate": "Date", 
  "teamsLicenseAssignDate": "Date", 
  "assignedProducts": ["String"]
}
```
