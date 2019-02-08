---
title: relatedContact リソースの種類
description: 守護者、援助施設、医師というように情報を提供する、educationUser に関連するレコードにお問い合わせください。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d29cf93154e2c032ac7010372e3f116f2a1dd46c
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694476"
---
# <a name="relatedcontact-resource-type"></a>relatedContact リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

守護者、援助施設、医師というように情報を提供する[educationUser](../resources/educationuser.md)に関連するレコードにお問い合わせください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String|Azure Active Directory 内の連絡先の id。|
|displayName|文字列型 (String)|連絡先の名前です。 必須です。|
|emailAddress|String|連絡先のプライマリ電子メール アドレスです。|
|mobilePhone|String|連絡先の携帯電話番号です。|
|リレーションシップ|`contactRelationship`|ユーザーに関係します。 使用可能な値は、 `parent`、 `relative`、 `aide`、 `doctor`、 `guardian`、 `child`、 `other`、 `unknownFutureValue`。|
|accessConsent|ブール値|受講者用のデータにアクセスするユーザーが同意したされているかどうかを示します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
