---
title: groupsettingtemplate リソースの種類
description: グループ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 使用可能な**groupsettingtemplates**に基づいてグループ設定を作成し、既定の既定値から変更された値を作成できます。 グループ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のグループ設定を表すことができます。 現時点では、使用可能なテンプレートは Office 365 グループにのみ適用され、グループのメンバーになるようにユーザーがグループを作成できるかどうか、または組織外からゲストを招待するかどうかなどの設定を含めることができます。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b9b95303b72bc111f045010e71459f541e9a9b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570793"
---
# <a name="groupsettingtemplate-resource-type"></a>groupsettingtemplate リソースの種類

グループ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 使用可能な**groupsettingtemplates**に基づいて[グループ設定](groupsetting.md)を作成し、既定の既定値から変更された値を作成できます。 グループ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のグループ設定を表すことができます。 現時点では、使用可能なテンプレートは Office 365 グループにのみ適用され、グループのメンバーになるようにユーザーがグループを作成できるかどうか、または組織外からゲストを招待するかどうかなどの設定を含めることができます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[groupsettingtemplate の取得](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | システム定義のいずれかの groupsettingtemplate オブジェクトの特定のプロパティを読み取ります。 |
|[groupsettingtemplate の一覧表示](../api/groupsettingtemplate-list.md) | [groupsettingtemplate のコレクション](groupsettingtemplate.md) |システム定義のすべての groupsettingtemplate オブジェクトを一覧表示します。|

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|description|String| テンプレートの説明。 |
|displayName|String| テンプレートの表示名。 |
|id|String| テンプレートの一意識別子。 読み取り専用です。|
|values|[settingtemplatevalue](settingtemplatevalue.md)コレクション| このテンプレートを構成する、使用可能な設定、既定値、および種類のセットを一覧表示する settingtemplatevalues のコレクションです。 |

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
