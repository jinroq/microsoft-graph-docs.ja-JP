---
title: programControl リソースの種類
description: Azure AD access レビュー機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16824c2ed0c053f0cc4f3a0a2903324ff1a2bf5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965636"
---
# <a name="programcontrol-resource-type"></a>programControl リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](accessreviews-root.md)機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ProgramControl を作成する](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   プログラムに programControl を追加します。|
|[ProgramControl の削除](../api/programcontrol-delete.md) |     なし。   |   プログラムから programControl を削除します。|
|[ProgramControls のリスト](../api/programcontrol-list.md) | [Programcontrol](programcontrol.md)コレクション| テナント内のすべてのプログラムでコントロールを一覧表示します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | プログラムとコントロール間のリンクの機能割り当て識別子                                      |
| `programId`              |`String`                | このコントロールが含まれるプログラムの programId。 作成時に必要です。                            |
| `controlId`              |`String`                | コントロールの controlId (特にアクセスレビューの識別子)。 作成時に必要です。                                                |
| `controlTypeId`          |`String`                | ProgramControlType には、プログラムコントロールの種類を指定します。たとえば、ゲストアクセスレビューにリンクしているコントロールがあります。 作成時に必要です。 |
| `displayName`            |`String`                | コントロールの名前を指定します。                                                             |
| `status`                 |`String`                | コントロールのライフサイクル状態。                                                 |
| `createdDateTime`        |`DateTimeOffset`        | プログラムコントロールの作成日時。                                        |
| `owner`                  |[userIdentity](useridentity.md)   | プログラムコントロールを作成したユーザー。                                               |
| `resource`               |`programResource`       | このプログラムコントロールのアクセスレビューによって対象となるリソース、グループ、またはアプリ。                   |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
| `program`                |[アプリケーション](program.md)               | このコントロールが含まれているプログラム。                                                |

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[プログラムの programControls を一覧表示する](../api/program-listcontrols.md) |      [Programcontrol](programcontrol.md)コレクション| プログラムのコントロールのコレクションを取得します。|
|[ProgramControlTypes のリスト](../api/programcontroltype-list.md) | [Programcontroltype](programcontroltype.md)コレクション| プログラムコントロールの種類を一覧表示します。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": {"@odata.type":"microsoft.graph.userIdentity"},
 "resource":{"@odata.type":"microsoft.graph.programResource"}
}

```

## <a name="the-programresource-complex-type"></a>ProgramResource 複合型

Program control オブジェクト内に含まれるプログラムリソースは、アクセスレビューのターゲットであるオブジェクトへの参照を表します。

この型はから`microsoft.graph.identity`継承され、さらに1つのプロパティが追加されています。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `type`               |`String`  | リソースの種類。これは、グループであるかアプリであるかを示します。 |     

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programResource"
}-->

```json
{
 "type": "string"
}

```
<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
