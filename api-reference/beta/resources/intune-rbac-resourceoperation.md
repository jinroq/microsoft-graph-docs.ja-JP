---
title: resourceOperation リソース タイプ
description: " AAD のセキュリティ グループに、MobileApp のリソースを割り当てるオペレーションを使用します。  組み込みのロールについては、リソース操作を変更できません。"
ms.openlocfilehash: 2aed25c7558d674abb39fdb4147b722afe69c0f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067562"
---
# <a name="resourceoperation-resource-type"></a>resourceOperation リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
|[getScopesForUser 関数](../api/intune-rbac-resourceoperation-getscopesforuser.md)|String コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|リソース操作のキー。 読み取り専用で、自動生成されます。|
|resource|String|この操作が所属しているリソースのカテゴリです。|
|resourceName|String|この操作が実行されるリソースの名前。|
|actionName|String|この操作が実行するアクションの種類。 actionName は簡潔で、できるだけ少ない単語にする必要があります。|
|説明|String|リソース操作の説明。 Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。|
|enabledForScopeValidation|ブール値|ロールの割り当てごとに定義されたスコープのアクセス許可を検証するかどうかを決定します。|

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
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": true
}
```





