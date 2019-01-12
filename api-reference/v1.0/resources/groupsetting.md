---
title: groupSetting リソースの種類
description: グループ設定は、グループ表示名でブロックする単語の一覧や、ゲスト ユーザーがグループの所有者になることを許可するか、といった動作を制御します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e6c0dc0f0ffd48da84023c5e4ff0d97cb446f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911694"
---
# <a name="groupsetting-resource-type"></a>groupSetting リソースの種類

グループ設定は、グループ表示名でブロックする単語の一覧や、ゲスト ユーザーがグループの所有者になることを許可するか、といった動作を制御します。

グループ設定は、使用可能な [groupSettingTemplates](groupsettingtemplate.md) に基づいて作成することができ、事前設定された既定値を変更することができます。これらの設定は、テナント全体のレベルまたは特定のグループのグループ基本動作を制御します。テナント全体および特定のグループの両方で同じ設定が定義されている場合、グループ レベルの設定がテナント全体の設定よりも優先されます。たとえば、テナント全体の設定では、ゲストは既存のグループのメンバーによって招待されることがありますが、個別のグループ設定を優先することができ、その場合は、グループのメンバーはゲストを招待することができません。グループ設定は、Office 365 グループの動作のみを制御します。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[設定を作成する](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |groupSettingTemplate に基づいて、設定オブジェクトを作成します。POST 要求は、テンプレートに定義されているすべての設定の settingValues を提供する必要があります。 |
|[設定を取得する](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 特定の設定オブジェクトのプロパティを参照します。 |
|[設定を一覧表示する](../api/groupsetting-list.md) | [groupSetting](groupsetting.md) コレクション | すべての設定オブジェクトのプロパティを一覧表示します。 |
|[設定を更新する](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Groupsetting オブジェクトを更新します。 |
|[設定を削除する](../api/groupsetting-delete.md) | なし | 設定オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:---------------|:--------|:----------|
|displayName|文字列| 関連するテンプレートに由来する設定グループの名前を表示します。 |
|id|文字列| 設定の一意識別子です。読み取り専用です。 |
|templateId|文字列| 設定グループの作成に使用されるテンプレートの一意識別子です。読み取り専用です。 |
|値|[settingValue](settingvalue.md) コレクション| 名前と値の組のコレクションです。テンプレートに定義されているすべての設定を含める必要があります。 |

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
