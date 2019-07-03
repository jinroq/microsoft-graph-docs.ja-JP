---
title: credentialUserRegistrationDetails リソースの種類
description: 登録されているすべてのユーザーに対して、セルフサービスのパスワードのリセットと多要素認証 (MFA) の使用法の詳細を表します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 414cd6977f4e3c15ab7b82bd88329e9e3549f137
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527085"
---
# <a name="credentialuserregistrationdetails-resource-type"></a>credentialUserRegistrationDetails リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

登録されているすべてのユーザーに対して、セルフサービスのパスワードのリセットと多要素認証 (MFA) の使用法の詳細を表します。 詳細には、ユーザー情報、登録の状態、使用される認証方法が含まれます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [CredentialUserRegistrationDetails を一覧表示する](../api/reportroot-list-credentialuserregistrationdetails.md) | credentialUserRegistrationDetails コレクション | 指定したテナントの[Credentialuserregistrationdetails](../resources/credentialuserregistrationdetails.md)オブジェクトの一覧を取得します。
 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| authMethods | registrationAuthMethod コレクション | ユーザーが使用した認証方法を表します。 可能な値は`email`、 `mobilePhone` `officePhone`、、 `securityQuestion` 、(セルフサービスのパスワードのリセットにのみ使用`appNotification`) `appCode`、、 `alternateMobilePhone` 、および (登録でのみサポートされます) です。 |
| id | 文字列 | アクティビティの一意識別子。 読み取り専用です。|
| isCapable | Boolean | ユーザーがセルフサービスのパスワードのリセットまたは MFA を実行する準備ができているかどうかを示します。 |
| isEnabled | Boolean | ユーザーがセルフサービスのパスワードのリセットの実行を有効にしたかどうかを Indiciates します。 |
| isMfaRegistered | Boolean | ユーザーが MFA 用に登録されているかどうかを Indiciates します。 |
| isRegistered | Boolean | ユーザーがセルフサービスのパスワードのリセットのために認証方法を登録しているかどうかを示します。 |
| userDisplayName | String | 対応するユーザーのユーザー名を提供します。 |
| userPrincipalName | String | 対応するユーザーのユーザープリンシパル名を提供します。 |

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "authMethods": ["string"],
  "isRegistered" : false,
  "isEnabled" : true,
  "isCapable" : false,
  "isMfaRegistered" : true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->