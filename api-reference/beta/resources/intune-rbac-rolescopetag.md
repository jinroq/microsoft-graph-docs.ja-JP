---
title: ロール Copetag リソースの種類
description: 役割のスコープタグ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54aa59e99a9697924512da0072e7b4e05e4fa12a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993537"
---
# <a name="rolescopetag-resource-type"></a>ロール Copetag リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

役割のスコープタグ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|[ロール Copetag](../resources/intune-rbac-rolescopetag.md)コレクション|[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ロール Copetag の取得](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ロール Copetag の作成](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|新しい[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。|
|[ロール Copetag の削除](../api/intune-rbac-rolescopetag-delete.md)|None|[ロール Copetag](../resources/intune-rbac-rolescopetag.md)を削除します。|
|[ロール Copetag の更新](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|[ロール Copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。|
|[assign アクション](../api/intune-rbac-rolescopetag-assign.md)|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 これは読み取り専用で、自動生成されます。|
|displayName|String|ロールスコープタグの表示名またはフレンドリ名。|
|description|String|役割の範囲タグの説明。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクション|この役割スコープタグの割り当てのリスト。|

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





