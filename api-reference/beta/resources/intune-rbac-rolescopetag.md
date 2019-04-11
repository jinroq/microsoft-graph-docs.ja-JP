---
title: ロール copetag リソースの種類
description: 役割のスコープタグ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6916521c8edef1b1decfb6b006779a372d3ab4e5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781954"
---
# <a name="rolescopetag-resource-type"></a>ロール copetag リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

役割のスコープタグ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|[ロール copetag](../resources/intune-rbac-rolescopetag.md)コレクション|[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ロール copetag の取得](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ロール copetag の作成](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|新しい[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。|
|[ロール copetag の削除](../api/intune-rbac-rolescopetag-delete.md)|なし|[ロール copetag](../resources/intune-rbac-rolescopetag.md)を削除します。|
|[ロール copetag の更新](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 これは読み取り専用で、自動生成されます。|
|displayName|String|ロールスコープタグの表示名またはフレンドリ名。|
|説明|String|役割の範囲タグの説明。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```





