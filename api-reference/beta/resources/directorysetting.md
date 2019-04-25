---
title: directorysetting リソースの種類
description: ディレクトリの設定は、使用可能な directorysettingtemplates に基づいて作成し、既定の既定値から変更することができます。 これらの設定は、テナント全体レベルまたは特定のエンティティレベルで、エンティティまたは機能の動作を制御できます。 テナント全体と特定のエンティティレベルの両方で同じ設定が定義されている場合、特定のエンティティレベルの設定はテナント全体の設定から除外されることがあります。  たとえば、テナント全体の設定では、ゲストがグループの既存のメンバーに招待されることが許可されますが、特定のグループの設定はオプトアウトされ、グループのメンバーによるゲストの招待が許可されない場合があります。 現在、システムで定義されている設定は、Office グループの動作のみを制御します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535240"
---
# <a name="directorysetting-resource-type"></a>directorysetting リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリの設定は、使用可能な[directorysettingtemplates](directorysettingtemplate.md)に基づいて作成し、既定の既定値から変更することができます。 これらの設定は、テナント全体レベルまたは特定のエンティティレベルで、エンティティまたは機能の動作を制御できます。 テナント全体と特定のエンティティレベルの両方で同じ設定が定義されている場合、特定のエンティティレベルの設定はテナント全体の設定から除外されることがあります。  たとえば、テナント全体の設定では、ゲストがグループの既存のメンバーに招待されることが許可されますが、特定のグループの設定はオプトアウトされ、グループのメンバーによるゲストの招待が許可されない場合があります。 現在、システムで定義されている設定は、Office グループの動作のみを制御します。

> **注**: directorysetting リソースの種類の/ベータ版は、グループにのみ適用されます。 /v1.0 のバージョンが groupsetting に変更されました。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[設定を作成する](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |directorysettingtemplate に基づいて設定オブジェクトを作成します。 POST 要求は、テンプレートで定義されているすべての設定の settingvalues を提供する必要があります。|
|[設定を取得する](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |特定の設定オブジェクトのプロパティを参照します。|
|[設定を一覧表示する](../api/directorysetting-list.md) | [directorySetting](directorysetting.md) コレクション |すべての設定オブジェクトのプロパティを一覧表示します。|
|[設定を更新する](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |設定オブジェクトを更新します。 update で変更できるのは、設定値だけです。|
|[設定を削除する](../api/directorysetting-delete.md) | なし |設定オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|string|関連付けられたテンプレートに由来する、この設定グループの表示名。 読み取り専用。|
|id|string| これらの設定の一意の識別子。 読み取り専用。|
|templateId|string| この設定のグループを作成するために使用されるテンプレートの一意識別子。 読み取り専用です。|
|values|[settingvalue](settingvalue.md)コレクション| 名前と値のペアのコレクション。 テンプレートで定義されているすべての設定が含まれていて、設定されている必要があります。|

## <a name="relationships"></a>リレーションシップ
なし


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
