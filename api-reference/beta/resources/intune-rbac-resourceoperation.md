---
title: resourceOperation リソース タイプ
description: テナント組織の役割ベースのアクセス制御 (RBAC) シナリオをサポートする Intune (REST) 用 Microsoft Graph API の resourceoperation リソース (エンティティ) について説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a299247815993a6ac1e99fe11ecead7ab66e2f2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165003"
---
# <a name="resourceoperation-resource-type"></a>resourceOperation リソース タイプ

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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
|id|文字列|リソース操作のキー。 読み取り専用で、自動生成されます。|
|リソース|String|この操作が属するリソースカテゴリ。|
|resourceName|String|この操作が実行されるリソースの名前。|
|actionName|String|この操作が実行するアクションの種類。 actionName は簡潔で、できるだけ少ない単語にする必要があります。|
|説明|String|リソース操作の説明。 Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。|
|enabledforscopevalidation|ブール値|権限が役割の割り当てごとに定義されたスコープに対して検証されているかどうかを判断します。|

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




