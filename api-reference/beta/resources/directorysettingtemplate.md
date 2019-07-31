---
title: directorySettingTemplate リソースの種類
description: ディレクトリ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 ディレクトリの設定は、使用可能な directorySettingTemplates に基づいて作成でき、値は事前設定の既定値から変更されます。 ディレクトリ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のエンティティ設定を表すことができます。  現時点では、Office グループに適用できるテンプレートは、ユーザーがグループを作成できるかどうか、または組織外のゲストをグループのメンバーにすることができるかどうかなどの設定が含まれています。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4239a12be5fffbf5c579752c3de4998c88749bd3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012787"
---
# <a name="directorysettingtemplate-resource-type"></a>directorySettingTemplate リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 [ディレクトリの設定](directorysetting.md)は、使用可能な directorySettingTemplates に基づいて作成でき、値は事前設定の既定値から変更されます。 ディレクトリ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のエンティティ設定を表すことができます。  現時点では、Office グループに適用できるテンプレートは、ユーザーがグループを作成できるかどうか、または組織外のゲストをグループのメンバーにすることができるかどうかなどの設定が含まれています。

> **注**: directorySettingTemplate リソースの種類の/ベータ版は、グループにのみ適用されます。 /V1.0 バージョンの名前が groupSettingTemplate に変更されました。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[DirectorySettingTemplate の取得](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |システム定義の directorySettingTemplate オブジェクトのいずれか1つの特定のプロパティを読み取ります。|
|[DirectorySettingTemplate の一覧表示](../api/directorysettingtemplate-list.md) | [DirectorySettingTemplate のコレクション](directorysettingtemplate.md) |システム定義の directorySettingTemplate オブジェクトをすべて一覧表示します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|string|テンプレートの説明。 読み取り専用です。|
|displayName|string|テンプレートの表示名。 読み取り専用です。 |
|id|string| テンプレートの一意識別子。 読み取り専用。|
|values|[Settingtemplatevalue](settingtemplatevalue.md)コレクション| このテンプレートを構成する、使用可能な設定、既定値、および種類のセットを一覧表示する settingTemplateValues のコレクションです。  読み取り専用。 |

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
