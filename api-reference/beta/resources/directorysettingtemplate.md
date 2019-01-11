---
title: directorySettingTemplate リソースの種類
description: ディレクトリ設定のテンプレートでは、テナントの使用可能なシステム定義の設定を表します。 ディレクトリの設定は、使用可能な directorySettingTemplates と事前に設定された既定値から変更された値に基づいて作成できます。 ディレクトリ設定のテンプレートを作成、更新または削除することはできません。 これらの設定では、テナント全体の設定を表すことができますか、特定のエンティティの設定を表すことができます。  現在、使用可能な唯一のテンプレートは、Office グループに適用され、ユーザーのグループを作成またはグループのメンバーになることを組織外からのゲストを招待できるかどうかなどの設定が含まれます。
localization_priority: Normal
ms.openlocfilehash: e0df923854059723ee83380f7aa0f6425cf2afb9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806147"
---
# <a name="directorysettingtemplate-resource-type"></a>directorySettingTemplate リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ディレクトリ設定のテンプレートでは、テナントの使用可能なシステム定義の設定を表します。 [ディレクトリの設定](directorysetting.md)は、使用可能な directorySettingTemplates と事前に設定された既定値から変更された値に基づいて作成できます。 ディレクトリ設定のテンプレートを作成、更新または削除することはできません。 これらの設定では、テナント全体の設定を表すことができますか、特定のエンティティの設定を表すことができます。  現在、使用可能な唯一のテンプレートは、Office グループに適用され、ユーザーのグループを作成またはグループのメンバーになることを組織外からのゲストを招待できるかどうかなどの設定が含まれます。

> **注**: directorySettingTemplate リソースの種類の/beta バージョンは、グループにのみ適用されます。 /V1.0 のバージョンは groupSettingTemplate に名前変更されました。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[DirectorySettingTemplate を取得します。](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |システム定義の directorySettingTemplate オブジェクトの 1 つの特定のプロパティを参照します。|
|[リスト directorySettingTemplate](../api/directorysettingtemplate-list.md) | [DirectorySettingTemplate のコレクション](directorysettingtemplate.md) |すべてのシステム定義の directorySettingTemplate オブジェクトの一覧を表示します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|description|文字列|テンプレートの説明です。 読み取り専用です。|
|displayName|string|テンプレートの表示名です。 読み取り専用です。 |
|ID|文字列| テンプレートの一意識別子です。読み取り専用です。|
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
<!-- {
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
