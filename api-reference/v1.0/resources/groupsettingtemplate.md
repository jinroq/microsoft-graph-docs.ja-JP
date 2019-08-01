---
title: groupSettingTemplate リソースの種類
description: グループ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 使用可能な**Groupsettingtemplates**に基づいてグループ設定を作成し、既定の既定値から変更された値を作成できます。 グループ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のグループ設定を表すことができます。 現時点では、使用可能なテンプレートは Office 365 グループにのみ適用され、グループのメンバーになるようにユーザーがグループを作成できるかどうか、または組織外からゲストを招待するかどうかなどの設定を含めることができます。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d0624be1511b542da08e76ed5f9c51e60fe58a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029282"
---
# <a name="groupsettingtemplate-resource-type"></a>groupSettingTemplate リソースの種類

グループ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 使用可能な**Groupsettingtemplates**に基づいて[グループ設定](groupsetting.md)を作成し、既定の既定値から変更された値を作成できます。 グループ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のグループ設定を表すことができます。 現時点では、使用可能なテンプレートは Office 365 グループにのみ適用され、グループのメンバーになるようにユーザーがグループを作成できるかどうか、または組織外からゲストを招待するかどうかなどの設定を含めることができます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[GroupSettingTemplate の取得](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | システム定義のいずれかの groupSettingTemplate オブジェクトの特定のプロパティを読み取ります。 |
|[GroupSettingTemplate の一覧表示](../api/groupsettingtemplate-list.md) | [GroupSettingTemplate のコレクション](groupsettingtemplate.md) |システム定義のすべての groupSettingTemplate オブジェクトを一覧表示します。|

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|description|String| テンプレートの説明。 |
|displayName|String| テンプレートの表示名。 |
|id|文字列| テンプレートの一意識別子。 読み取り専用です。|
|values|[Settingtemplatevalue](settingtemplatevalue.md)コレクション| このテンプレートを構成する、使用可能な設定、既定値、および種類のセットを一覧表示する settingTemplateValues のコレクションです。 |

## <a name="relationships"></a>リレーションシップ

なし。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
