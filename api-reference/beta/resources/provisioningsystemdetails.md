---
title: 入力システムの詳細リソースの種類
description: ユーザーがプロビジョニングされたシステムを表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e84af77ac7d2b14fb25ce07939bc1a542102fb19
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349423"
---
# <a name="provisioningsystemdetails-resource-type"></a>入力システムの詳細リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーがプロビジョニングされたシステムを表します。 たとえば、Azure Active Directory (Azure AD) から ServiceNow にユーザーをプロビジョニングするときに、ソースシステムが Azure AD で、ターゲットシステムが ServiceNow であるとします。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|詳細|[詳細情報](detailsinfo.md)|システムの詳細。|
|displayName|String|ユーザーがプロビジョニングされたシステムの名前。|
|id|文字列|ユーザーがプロビジョニングされたシステムの識別子。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystemDetails",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningSystemDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
