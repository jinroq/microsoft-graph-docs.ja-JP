---
title: directorysettingtemplate リソースの種類
description: ディレクトリ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 ディレクトリの設定は、使用可能な directorysettingtemplates に基づいて作成でき、値は事前設定の既定値から変更されます。 ディレクトリ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のエンティティ設定を表すことができます。  現時点では、Office グループに適用できるテンプレートは、ユーザーがグループを作成できるかどうか、または組織外のゲストをグループのメンバーにすることができるかどうかなどの設定が含まれています。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543253"
---
# <a name="directorysettingtemplate-resource-type"></a>directorysettingtemplate リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリ設定テンプレートは、テナントで使用可能なシステム定義の設定を表します。 [ディレクトリの設定](directorysetting.md)は、使用可能な directorysettingtemplates に基づいて作成でき、値は事前設定の既定値から変更されます。 ディレクトリ設定テンプレートを作成、更新、または削除することはできません。 これらの設定は、テナント全体の設定、または特定のエンティティ設定を表すことができます。  現時点では、Office グループに適用できるテンプレートは、ユーザーがグループを作成できるかどうか、または組織外のゲストをグループのメンバーにすることができるかどうかなどの設定が含まれています。

> **注**: directorysettingtemplate リソースの種類の/ベータ版は、グループにのみ適用されます。 /v1.0 バージョンの名前が groupsettingtemplate に変更されました。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[directorysettingtemplate の取得](../api/directorysettingtemplate-get.md) | [directorysettingtemplate](directorysettingtemplate.md) |システム定義の directorysettingtemplate オブジェクトのいずれか1つの特定のプロパティを読み取ります。|
|[directorysettingtemplate の一覧表示](../api/directorysettingtemplate-list.md) | [directorysettingtemplate のコレクション](directorysettingtemplate.md) |システム定義の directorysettingtemplate オブジェクトをすべて一覧表示します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|string|テンプレートの説明。 読み取り専用です。|
|displayName|string|テンプレートの表示名。 読み取り専用。 |
|id|string| テンプレートの一意識別子。 読み取り専用です。|
|values|[settingtemplatevalue](settingtemplatevalue.md)コレクション| このテンプレートを構成する、使用可能な設定、既定値、および種類のセットを一覧表示する settingtemplatevalues のコレクションです。  読み取り専用。 |

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysettingtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
