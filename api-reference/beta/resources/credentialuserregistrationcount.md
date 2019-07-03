---
title: credentialUserRegistrationCount リソースの種類
description: 組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証機能を使用するために登録されているユーザーの数の現在の状態を表します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 42c722b04493767d3dbcaf713157d931569d8c32
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485265"
---
# <a name="credentialuserregistrationcount-resource-type"></a>credentialUserRegistrationCount リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証機能を使用するために登録されているユーザーの数の現在の状態を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md) | credentialUserRegistrationCount コレクション | 組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証 (MFA) の機能を使用するために登録されているユーザー数の現在の状態を報告します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| id | String | アクティビティの一意識別子。 読み取り専用です。 |
| totalUserCount | Int64 | テナント内の総ユーザー数を示します。 |
| userRegistrationCounts | [Userregistrationcount](userregistrationcount.md)コレクション | テナント内のユーザーの登録数と状態情報のコレクション。 |

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "totalUserCount" : 23123,
  "userRegistrationCounts" :
  [
    { "registrationStatus":"registered", "registrationCount": 23423 },
    { "registrationStatus":"enabled", "registrationCount": 4234 },
    { "registrationStatus":"capable", "registrationCount": 323 },
    { "registrationStatus":"mfaRegistered", "registrationCount": 33 }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->