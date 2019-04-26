---
title: programcontrol リソースの種類
description: Azure AD access レビュー機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。
localization_priority: Normal
ms.openlocfilehash: 7d194f3e80f44eb57be0deb7d2ffd71624c385d7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344023"
---
# <a name="programcontrol-resource-type"></a>programcontrol リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](accessreviews-root.md)機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[programcontrol を作成する](../api/programcontrol-create.md) |     [programcontrol](programcontrol.md) |   プログラムに programcontrol を追加します。|
|[programcontrol の削除](../api/programcontrol-delete.md) |     なし。   |   プログラムから programcontrol を削除します。|
|[programcontrols のリスト](../api/programcontrol-list.md) | [programcontrol](programcontrol.md)コレクション| テナント内のすべてのプログラムでコントロールを一覧表示します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | プログラムとコントロール間のリンクの機能割り当て識別子                                      |
| `programId`              |`String`                | このコントロールが含まれるプログラムの programid。 作成時に必要です。                            |
| `controlId`              |`String`                | コントロールの controlId (特にアクセスレビューの識別子)。 作成時に必要です。                                                |
| `controlTypeId`          |`String`                | programcontroltype には、プログラムコントロールの種類を指定します。たとえば、ゲストアクセスレビューにリンクしているコントロールがあります。 作成時に必要です。 |
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
|[プログラムの programcontrols を一覧表示する](../api/program-listcontrols.md) |      [programcontrol](programcontrol.md)コレクション| プログラムのコントロールのコレクションを取得します。|
|[programcontroltypes のリスト](../api/programcontroltype-list.md) | [programcontroltype](programcontroltype.md)コレクション| プログラムコントロールの種類を一覧表示します。 |

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

## <a name="the-programresource-complex-type"></a>programresource 複合型

program control オブジェクト内に含まれるプログラムリソースは、アクセスレビューのターゲットであるオブジェクトへの参照を表します。

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
