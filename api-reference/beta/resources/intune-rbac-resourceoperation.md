---
title: resourceOperation リソース タイプ
description: ロールベースのアクセス制御 (RBAC) に関連する Intune ワークフローをサポートする Microsoft Graph API (REST) の resourceOperation リソース (エンティティ) について説明します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b83ad1c902e8455d42ae0e9805bf6881b49ef3b4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369284"
---
# <a name="resourceoperation-resource-type"></a>resourceOperation リソース タイプ

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ロールベースのアクセス制御 (RBAC) に関連する Intune ワークフローをサポートする Microsoft Graph API (REST) の resourceOperation リソース (エンティティ) について説明します。

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
|リソース|String|この操作が属するリソースカテゴリ。|
|resourceName|String|この操作が実行されるリソースの名前。|
|actionName|文字列型 (String)|この操作が実行するアクションの種類。 actionName は簡潔で、できるだけ少ない単語にする必要があります。|
|description|String|リソース操作の説明。 Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。|
|enabledForScopeValidation|Boolean|権限が役割の割り当てごとに定義されたスコープに対して検証されているかどうかを判断します。|

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



