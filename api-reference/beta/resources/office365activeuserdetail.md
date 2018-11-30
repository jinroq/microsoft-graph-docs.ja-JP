---
title: office365ActiveUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 95912e736459894a69f8e2e1a18c2aaf672a19a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069177"
---
# <a name="office365activeuserdetail-resource-type"></a>office365ActiveUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                          | 型              | 説明                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Date              | コンテンツの最新の日付。          |
| userPrincipalName                 | String            | ユーザー プリンシパル名 (UPN) のユーザーです。 UPN は、インターネット標準の RFC 822 に基づくユーザーに対して、インターネット スタイルのログイン名です。 規則では、これはユーザーの電子メール名にマップする必要があります。 一般的な形式は、ドメインをドメインの検証済みのテナントのコレクション内に存在する必要があります、alias@domain、です。 このプロパティは、ユーザーの作成時に必要です。 |
| displayName                       | String            | アドレス帳に表示されるユーザーの名前。 これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。 このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。 |
| isDeleted                         | ブール値           | このユーザーが削除されたか、またはソフトをされてかどうかを削除します。 |
| deletedDate                       | Date              | 削除操作が発生した日付です。 ユーザーが削除されていない場合、既定値は"null です"。 |
| hasExchangeLicense                | ブール値           | かどうか、ユーザーに Exchange のライセンスを割り当てられています。 |
| hasOneDriveLicense                | ブール値           | かどうか、ユーザーに OneDrive のライセンスを割り当てられています。 |
| hasSharePointLicense              | ブール値           | かどうか、ユーザーに SharePoint ライセンスを割り当てられています。 |
| hasSkypeForBusinessLicense        | ブール値           | かどうか、ユーザーに、Skype のビジネス ライセンスを割り当てられています。 |
| hasYammerLicense                  | ブール値           | かどうかユーザーに Yammer のライセンスを割り当てられています。 |
| hasTeamsLicense                   | ブール値           | かどうかユーザーにチームのライセンスを割り当てられています。 |
| exchangeLastActivityDate          | Date              | ユーザー最後の読み取りまたは日付電子メールを送信します。 |
| oneDriveLastActivityDate          | Date              | 日付とユーザー最後を表示または編集したファイルを内部または外部でファイルを共有またはファイルを同期します。 |
| sharePointLastActivityDate        | Date              | ときユーザー最後表示したり編集したり、ファイルの日付はファイルを社内で共有または外部から、ファイルを同期または SharePoint ページを表示します。 |
| skypeForBusinessLastActivityDate  | Date              | ユーザー最終編成または会議に参加または日付ピア ツー ピア セッションに参加しています。 |
| yammerLastActivityDate            | Date              | ユーザー最後投稿、読み取り、または日付メッセージを気に入られました。 |
| teamsLastActivityDate             | Date              | ユーザー最後転記日付のメッセージ、チームのチャンネルでは、プライベート チャットのセッションにメッセージを送信または、会議や通話に参加しています。 |
| exchangeLicenseAssignDate         | Date              | 最後の日付では、ユーザーが Exchange のライセンスを割り当てられた場合。 |
| oneDriveLicenseAssignDate         | Date              | 最後の日付では、ユーザーが OneDrive のライセンスを割り当てられた場合。 |
| sharePointLicenseAssignDate       | Date              | 最後の日付では、ユーザーが SharePoint ライセンスを割り当てられた場合。 |
| skypeForBusinessLicenseAssignDate | Date              | ユーザーが Skype のビジネス ライセンスを割り当てられたときの最終日。 |
| yammerLicenseAssignDate           | Date              | Yammer のライセンスをユーザーが割り当てられたときの最終日。 |
| teamsLicenseAssignDate            | Date              | 最後の日付では、ユーザーがチームのライセンスを割り当てられた場合。 |
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
