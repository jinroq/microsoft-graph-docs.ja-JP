---
title: groupsetting リソースの種類
description: グループ設定は、グループの表示名のブロックされた単語リスト、ゲストユーザーがグループの所有者になることができるかどうかなどの動作を制御します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e6c0dc0f0ffd48da84023c5e4ff0d97cb446f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570828"
---
# <a name="groupsetting-resource-type"></a>groupsetting リソースの種類

グループ設定は、グループの表示名のブロックされた単語リスト、ゲストユーザーがグループの所有者になることができるかどうかなどの動作を制御します。

グループ設定は、使用可能な[groupsettingtemplates](groupsettingtemplate.md)に基づいて作成し、既定の既定値から変更することができます。 これらの設定は、テナント全体レベルまたは特定のグループに対するグループの動作を管理します。 テナント全体と特定のグループの両方で同じ設定が定義されている場合、グループレベル設定はテナント全体の設定より優先されます。  たとえば、テナント全体の設定では、グループの既存のメンバーによるゲストの招待が許可されることがありますが、個々のグループの設定を上書きして、グループのメンバーに招待されたゲストの招待を許可することはできません。 グループ設定は、Office 365 グループの動作のみを制御します。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[設定を作成する](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |groupsettingtemplate に基づいて設定オブジェクトを作成します。 POST 要求は、テンプレートで定義されているすべての設定の settingvalues を提供する必要があります。 |
|[設定を取得する](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 特定の設定オブジェクトのプロパティを参照します。 |
|[設定を一覧表示する](../api/groupsetting-list.md) | [groupSetting](groupsetting.md) コレクション | すべての設定オブジェクトのプロパティを一覧表示します。 |
|[設定を更新する](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | groupsetting オブジェクトを更新します。 |
|[設定を削除する](../api/groupsetting-delete.md) | なし | 設定オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|displayName|String| 関連付けられたテンプレートに由来する、この設定グループの表示名。 |
|id|String| これらの設定の一意の識別子。 読み取り専用。 |
|templateId|String| この設定のグループを作成するために使用されるテンプレートの一意識別子。 読み取り専用です。 |
|values|[settingvalue](settingvalue.md)コレクション| 名前と値のペアのコレクション。 テンプレートで定義されているすべての設定が含まれていて、設定されている必要があります。 |

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
