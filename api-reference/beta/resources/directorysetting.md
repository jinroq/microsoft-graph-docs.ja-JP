---
title: directorySetting リソースの種類
description: ディレクトリの設定は、使用可能な directorySettingTemplates を基に作成し、事前に設定された既定値から変更できます。 これらの設定には、エンティティまたは機能の動作、テナント全体のレベルまたは特定のエンティティ レベルの両方を管理できます。 テナント全体、特定のエンティティ レベルの両方で同じ設定が定義されると、特定のエンティティ レベルの設定可能性があります脱退テナント全体の設定から。  たとえば、テナント全体の設定は、グループの既存のメンバーから招待されるには、来園者を許可する可能性がありますが、特定のグループの設定可能性があります脱退グループのメンバーから招待されるには、来園者を許可しません。 現在定義されているシステムの設定は Office グループの動作を制御するだけ。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521370"
---
# <a name="directorysetting-resource-type"></a>directorySetting リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリの設定は、使用可能な[directorySettingTemplates](directorysettingtemplate.md)、に基づいて作成し、事前に設定された既定値から変更できます。 これらの設定には、エンティティまたは機能の動作、テナント全体のレベルまたは特定のエンティティ レベルの両方を管理できます。 テナント全体、特定のエンティティ レベルの両方で同じ設定が定義されると、特定のエンティティ レベルの設定可能性があります脱退テナント全体の設定から。  たとえば、テナント全体の設定は、グループの既存のメンバーから招待されるには、来園者を許可する可能性がありますが、特定のグループの設定可能性があります脱退グループのメンバーから招待されるには、来園者を許可しません。 現在定義されているシステムの設定は Office グループの動作を制御するだけ。

> **注**: directorySetting リソースの種類の/beta バージョンは、グループにのみ適用されます。 /V1.0 のバージョンは groupSetting に名前変更されました。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[設定を作成する](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |directorySettingTemplate に基づいて、設定オブジェクトを作成します。 POST 要求は、テンプレートに定義されているすべての設定の settingValues を提供する必要があります。|
|[設定を取得する](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |特定の設定オブジェクトのプロパティを参照します。|
|[設定を一覧表示する](../api/directorysetting-list.md) | [directorySetting](directorysetting.md) コレクション |すべての設定オブジェクトのプロパティを一覧表示します。|
|[設定を更新する](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |設定オブジェクトを更新します。 更新プログラムでは、settingValues のみを変更できます。|
|[設定を削除する](../api/directorysetting-delete.md) | なし |設定オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|string|関連するテンプレートに由来する設定グループの名前を表示します。 読み取り専用です。|
|id|文字列| 設定の一意識別子です。読み取り専用です。|
|templateId|string| 設定グループの作成に使用されるテンプレートの一意識別子です。読み取り専用です。|
|値|[settingValue](settingvalue.md) コレクション| 名前と値の組のコレクションです。テンプレートに定義されているすべての設定を含める必要があります。|

## <a name="relationships"></a>リレーションシップ
None


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
