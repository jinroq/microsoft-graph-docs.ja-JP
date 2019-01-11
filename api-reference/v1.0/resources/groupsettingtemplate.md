---
title: groupSettingTemplate リソースの種類
description: グループ設定テンプレートは、テナントが使用できるシステム定義の設定を表します。グループ設定は、使用可能な **groupSettingTemplates** に基づいて作成することができ、値は事前設定された既定値から変更することができます。グループ設定テンプレートの作成、更新、削除はできません。これらの設定は、テナント全体の設定または特定のグループ設定を表すことができます。現時点では、利用可能なテンプレートは Office 365 グループのみに適用され、そこでユーザーがグループを作成したり、組織外からゲストをグループのメンバーに招待できるかどうかなどの設定をすることができます。
localization_priority: Normal
ms.openlocfilehash: c2e6b465226b8c1c69438fab37d874735e89ac52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859347"
---
# <a name="groupsettingtemplate-resource-type"></a>groupSettingTemplate リソースの種類

グループ設定テンプレートは、テナントが使用できるシステム定義の設定を表します。[グループ設定](groupsetting.md)は、使用可能な **groupSettingTemplates** に基づいて作成することができ、値は事前設定された既定値から変更することができます。グループ設定テンプレートの作成、更新、削除はできません。これらの設定は、テナント全体の設定または特定のグループ設定を表すことができます。現時点では、利用可能なテンプレートは Office 365 グループのみに適用され、そこでユーザーがグループを作成したり、組織外からゲストをグループのメンバーに招待できるかどうかなどの設定をすることができます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[groupSettingTemplate の取得](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | システムで定義された groupSettingTemplate オブジェクトの特定のプロパティを読み込みます。 |
|[groupSettingTemplate のリスト](../api/groupsettingtemplate-list.md) | [GroupSettingTemplate のコレクション](groupsettingtemplate.md) |システムで定義された groupSettingTemplate オブジェクトをすべて一覧表示します。|

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:---------------|:--------|:----------|
|説明|文字列| テンプレートの説明です。 |
|displayName|文字列| テンプレートの表示名です。 |
|id|文字列| テンプレートの一意識別子です。読み取り専用です。|
|値|[settingTemplateValue](settingtemplatevalue.md) コレクション| このテンプレートを構成する、一連の利用可能な設定、既定値、種類を一覧表示する settingTemplateValues のコレクションです。 |

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
