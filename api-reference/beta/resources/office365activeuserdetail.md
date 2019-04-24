---
title: office365ActiveUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 192629623b0a0d46453f4dd4f9bfd7f1dc48cccf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505530"
---
# <a name="office365activeuserdetail-resource-type"></a>office365ActiveUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                          | 型              | 説明                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportrefreshdate                 | Date              | コンテンツの最新の日付。          |
| userPrincipalName                 | String            | ユーザーのユーザープリンシパル名 (UPN)。 UPN は、インターネット標準 RFC 822 に基づくユーザーのインターネットスタイルのログイン名です。 規則により、これはユーザーの電子メール名にマップする必要があります。 一般的な形式は、検証済みドメインのテナントのコレクションにドメインが存在する必要がある、エイリアス @ domain です。 このプロパティは、ユーザーの作成時に必要です。 |
| displayName                       | String            | アドレス帳に表示されるユーザーの名前。 これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。 このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。 |
| isDeleted                         | Boolean           | このユーザーが削除されているか、または削除されているか。 |
| deletedDate                       | Date              | 削除操作が発生した日付。 ユーザーが削除されていない場合、既定値は "null" です。 |
| hasExchangeLicense                | Boolean           | ユーザーに Exchange ライセンスが割り当てられているかどうか。 |
| hasOneDriveLicense                | Boolean           | ユーザーに OneDrive ライセンスが割り当てられているかどうか。 |
| hassharepointlicense              | Boolean           | ユーザーに SharePoint ライセンスが割り当てられているかどうか。 |
| hasSkypeForBusinessLicense        | Boolean           | ユーザーに Skype for business ライセンスが割り当てられているかどうか。 |
| hasYammerLicense                  | Boolean           | ユーザーに Yammer ライセンスが割り当てられているかどうか。 |
| hasteamslicense                   | Boolean           | ユーザーに Teams ライセンスが割り当てられているかどうか。 |
| exchangeLastActivityDate          | Date              | ユーザーが最後に電子メールを読んだり送信したりした日付。 |
| oneDriveLastActivityDate          | Date              | ユーザーが最後にファイルを表示または編集した日付、共有ファイルの内部または外部、または同期したファイル。 |
| sharepointlastactivitydate        | Date              | ユーザーが最後にファイルを表示または編集した日付、共有ファイルの内部または外部、同期済みファイル、または SharePoint ページを表示した日付。 |
| skypeforbusinesslastactivitydate  | Date              | ユーザーが会議に最後に開催または参加した日付、またはピアツーピアセッションに参加した日付。 |
| yammerLastActivityDate            | Date              | ユーザーが最後に投稿、閲覧、または「いいね!」のメッセージを最後に投稿した日付。 |
| teamslastactivitydate             | Date              | ユーザーがチームチャネルでメッセージを最後に投稿した日、プライベートチャットセッションでメッセージを送信した、または会議または通話に参加した日付。 |
| exchangeLicenseAssignDate         | Date              | ユーザーが Exchange ライセンスを割り当てられた最後の日付。 |
| oneDriveLicenseAssignDate         | Date              | ユーザーが OneDrive ライセンスを割り当てられた最後の日付。 |
| sharepointlicenseの割り当て日付       | Date              | ユーザーが SharePoint ライセンスを割り当てられた最後の日付。 |
| skypeforbusinesslicenseの割り当て日付 | Date              | ユーザーが Skype for business ライセンスを割り当てられた最後の日付。 |
| yammerLicenseAssignDate           | Date              | ユーザーが Yammer ライセンスを割り当てられた最後の日付。 |
| teamslicenseの割り当て日付            | Date              | ユーザーが Teams ライセンスを割り当てられた最後の日付。 |
| assignedProducts                  | String collection | ユーザーに割り当てられているすべての製品。  |

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
