---
title: office365ActiveUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 14c785069868783b1e248b41a5b339c9adb4710a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929285"
---
# <a name="office365activeuserdetail-resource-type"></a>office365ActiveUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                          | 型              | 説明                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | 日付              | コンテンツの最新の日付。          |
| userPrincipalName                 | String            | ユーザー プリンシパル名 (UPN) のユーザーです。 UPN は、インターネット標準の RFC 822 に基づくユーザーに対して、インターネット スタイルのログイン名です。 規則では、これはユーザーの電子メール名にマップする必要があります。 一般的な形式は、ドメインをドメインの検証済みのテナントのコレクション内に存在する必要があります、alias@domain、です。 このプロパティは、ユーザーの作成時に必要です。 |
| displayName                       | String            | アドレス帳に表示されるユーザーの名前。 これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。 このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。 |
| isDeleted                         | Boolean           | このユーザーが削除されたか、またはソフトをされてかどうかを削除します。 |
| deletedDate                       | 日付              | 削除操作が発生した日付です。 ユーザーが削除されていない場合、既定値は"null です"。 |
| hasExchangeLicense                | Boolean           | かどうか、ユーザーに Exchange のライセンスを割り当てられています。 |
| hasOneDriveLicense                | Boolean           | かどうか、ユーザーに OneDrive のライセンスを割り当てられています。 |
| hasSharePointLicense              | Boolean           | かどうか、ユーザーに SharePoint ライセンスを割り当てられています。 |
| hasSkypeForBusinessLicense        | Boolean           | かどうか、ユーザーに、Skype のビジネス ライセンスを割り当てられています。 |
| hasYammerLicense                  | Boolean           | かどうかユーザーに Yammer のライセンスを割り当てられています。 |
| hasTeamsLicense                   | Boolean           | かどうかユーザーにチームのライセンスを割り当てられています。 |
| exchangeLastActivityDate          | 日付              | ユーザー最後の読み取りまたは日付電子メールを送信します。 |
| oneDriveLastActivityDate          | 日付              | 日付とユーザー最後を表示または編集したファイルを内部または外部でファイルを共有またはファイルを同期します。 |
| sharePointLastActivityDate        | 日付              | ときユーザー最後表示したり編集したり、ファイルの日付はファイルを社内で共有または外部から、ファイルを同期または SharePoint ページを表示します。 |
| skypeForBusinessLastActivityDate  | 日付              | ユーザー最終編成または会議に参加または日付ピア ツー ピア セッションに参加しています。 |
| yammerLastActivityDate            | 日付              | ユーザー最後投稿、読み取り、または日付メッセージを気に入られました。 |
| teamsLastActivityDate             | 日付              | ユーザー最後転記日付のメッセージ、チームのチャンネルでは、プライベート チャットのセッションにメッセージを送信または、会議や通話に参加しています。 |
| exchangeLicenseAssignDate         | 日付              | 最後の日付では、ユーザーが Exchange のライセンスを割り当てられた場合。 |
| oneDriveLicenseAssignDate         | 日付              | 最後の日付では、ユーザーが OneDrive のライセンスを割り当てられた場合。 |
| sharePointLicenseAssignDate       | 日付              | 最後の日付では、ユーザーが SharePoint ライセンスを割り当てられた場合。 |
| skypeForBusinessLicenseAssignDate | 日付              | ユーザーが Skype のビジネス ライセンスを割り当てられたときの最終日。 |
| yammerLicenseAssignDate           | 日付              | Yammer のライセンスをユーザーが割り当てられたときの最終日。 |
| teamsLicenseAssignDate            | 日付              | 最後の日付では、ユーザーがチームのライセンスを割り当てられた場合。 |
| assignedProducts                  | String コレクション | ユーザーに割り当てられているすべての製品です。  |

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
