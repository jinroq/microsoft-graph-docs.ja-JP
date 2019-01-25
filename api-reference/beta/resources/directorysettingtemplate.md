---
title: directorySettingTemplate リソースの種類
description: ディレクトリ設定のテンプレートでは、テナントの使用可能なシステム定義の設定を表します。 ディレクトリの設定は、使用可能な directorySettingTemplates と事前に設定された既定値から変更された値に基づいて作成できます。 ディレクトリ設定のテンプレートを作成、更新または削除することはできません。 これらの設定では、テナント全体の設定を表すことができますか、特定のエンティティの設定を表すことができます。  現在、使用可能な唯一のテンプレートは、Office グループに適用され、ユーザーのグループを作成またはグループのメンバーになることを組織外からのゲストを招待できるかどうかなどの設定が含まれます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516659"
---
# <a name="directorysettingtemplate-resource-type"></a>directorySettingTemplate リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリ設定のテンプレートでは、テナントの使用可能なシステム定義の設定を表します。 [ディレクトリの設定](directorysetting.md)は、使用可能な directorySettingTemplates と事前に設定された既定値から変更された値に基づいて作成できます。 ディレクトリ設定のテンプレートを作成、更新または削除することはできません。 これらの設定では、テナント全体の設定を表すことができますか、特定のエンティティの設定を表すことができます。  現在、使用可能な唯一のテンプレートは、Office グループに適用され、ユーザーのグループを作成またはグループのメンバーになることを組織外からのゲストを招待できるかどうかなどの設定が含まれます。

> **注**: directorySettingTemplate リソースの種類の/beta バージョンは、グループにのみ適用されます。 /V1.0 のバージョンは groupSettingTemplate に名前変更されました。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[DirectorySettingTemplate を取得します。](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |システム定義の directorySettingTemplate オブジェクトの 1 つの特定のプロパティを参照します。|
|[リスト directorySettingTemplate](../api/directorysettingtemplate-list.md) | [DirectorySettingTemplate のコレクション](directorysettingtemplate.md) |すべてのシステム定義の directorySettingTemplate オブジェクトの一覧を表示します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|説明|string|テンプレートの説明です。 読み取り専用です。|
|displayName|string|テンプレートの表示名です。 読み取り専用。 |
|id|文字列| テンプレートの一意識別子です。読み取り専用です。|
|値|[settingTemplateValue](settingtemplatevalue.md) コレクション| このテンプレートを構成する、一連の利用可能な設定、既定値、種類を一覧表示する settingTemplateValues のコレクションです。  読み取り専用です。 |

## <a name="relationships"></a>リレーションシップ
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
