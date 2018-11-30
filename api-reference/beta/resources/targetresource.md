---
title: targetResource リソースの種類
description: Audit アクティビティに関連付けられているターゲット ・ リソースの種類のコレクションを表します。 各ターゲット リソースの種類は、次の手順は、このリソースからプロパティを継承します。
ms.openlocfilehash: ba3bee7ce89f73ed97610d62676c22d14488ed9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066895"
---
# <a name="targetresource-resource-type"></a>targetResource リソースの種類
Audit アクティビティに関連付けられているターゲット ・ リソースの種類のコレクションを表します。 各ターゲット リソースの種類は、次の手順は、このリソースからプロパティを継承します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|次のターゲット リソースの種類] の下に記載されているリソースの表示名を示します。|
|id|String|リソースの一意の Id を示します (例: ユーザー Id、AppId を RoleId。)。|
|modifiedProperties|[modifiedProperty](modifiedproperty.md)コレクション|名前、変更前の値と変更された各属性の新しい値を示します。 これは、「更新プログラム」のすべてのアクティビティの適用|

### <a name="target-resource-types"></a>ターゲット リソースの種類

ターゲット リソースの種類は、基になるリソースによって異なります。

|リソース名| リファレンス|
|-------------|----------|
デバイス|[targetResourceDevice](targetresourcedevice.md)
ディレクトリ|[targetResourceDirectory](targetresourcedirectory.md]
グループ化|[targetResourceGroup](targetresourcegroup.md)
ポリシー|[targetResourcePolicy](targetresourcepolicy.md)
Role|[targetResourceRole](targetresourcerole.md)
サービス ・ プリンシパル|[targetResourceServicePrincipal](targetresourceserviceprincipal.md)
User|[targetResourceUser](targetresourceuser.md)
その他|[targetResourceOther](targetresourceother.md)

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->