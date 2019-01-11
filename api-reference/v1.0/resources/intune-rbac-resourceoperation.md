---
title: resourceOperation リソース タイプ
description: " AAD のセキュリティ グループに、MobileApp のリソースを割り当てるオペレーションを使用します。  組み込みのロールについては、リソース操作を変更できません。"
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 47dccffe445024e9e6b086b17f87789316db6585
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811852"
---
# <a name="resourceoperation-resource-type"></a>resourceOperation リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune リソース (またはエンティティ) で実行できる操作またはアクションを定義します。  一般的な操作は Read、Delete、Update、Create です。  これらの操作は、基となる Intune リソース自体の基本的な管理を提供します。  場合によっては、リソースにより使われる Intune リソースの操作が、他のリソースとの組み合わせでアクションを実行する場合もあります。  たとえば、Assign 操作は MobileApp リソースを AAD セキュリティ グループに割り当てるために使用されます。  組み込みのロールについては、リソース操作を変更できません。これは、Intune リソース (またはエンティティ) に実行できる操作またはアクションを定義します。  一般的な操作は Get、List、Delete、Update、Create です。  これらの操作は、基となる Intune リソース自体の基本的な管理を提供します。  場合によっては、リソースにより使われる Intune リソースの操作が、他のリソースとの組み合わせでアクションを実行する場合もあります。  たとえば、「Assign」操作は MobileApp リソースを AAD セキュリティ グループに割り当てるために使用されます。  組み込みのロールについては、リソース操作を変更できません。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List resourceOperations](../api/intune-rbac-resourceoperation-list.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md) コレクション|[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get resourceOperation](../api/intune-rbac-resourceoperation-get.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create resourceOperation](../api/intune-rbac-resourceoperation-create.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|新しい [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを作成します。|
|[Delete resourceOperation](../api/intune-rbac-resourceoperation-delete.md)|なし|[resourceOperation](../resources/intune-rbac-resourceoperation.md) を削除します。|
|[Update resourceOperation](../api/intune-rbac-resourceoperation-update.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|リソース操作のキー。 読み取り専用で、自動生成されます。|
|resourceName|String|この操作が実行されるリソースの名前。|
|actionName|String|この操作が実行するアクションの種類。 actionName は簡潔で、できるだけ少ない単語にする必要があります。|
|説明|String|リソース操作の説明。 Azure Portal で操作にカーソルを合わせると、その操作の説明がテキストで表示されます。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```



