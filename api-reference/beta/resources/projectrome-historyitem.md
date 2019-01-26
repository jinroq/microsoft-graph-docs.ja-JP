---
title: historyItem リソースの種類
description: アプリケーション内のアクティビティの履歴項目を表します。 ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 582cfe71ab85602efc087d5e39005d5a9763394d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576305"
---
# <a name="historyitem-resource-type"></a>historyItem リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーション内の[アクティビティ](projectrome-activity.md)の履歴項目を表します。 ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。

アプリケーションは、セッションを作成するときは、ユーザー契約の期間を反映するように**アクティビティ**オブジェクトに**historyItem**オブジェクトを追加する必要があります。 ユーザーは、再活動と連携して、たびに、新しい**historyItem**がユーザーの活動を見越計上するアクティビティに追加されます。

## <a name="methods"></a>メソッド

|メソッド | 戻り値の型 | 説明|
|:------|:------------|:-----------|
|[作成または置換 historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | 作成するか、その活動 (アップサート) の既存の**historyItem**に置き換えられます。 ID は GUID である必要があります。|
|[HistoryItem を削除します。](../api/projectrome-delete-historyitem.md) | 内容なし | そのアクティビティに指定された**historyItem**を削除します。|

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|status | 列挙型文字列 | サーバーで設定します。 有効なオブジェクトを識別するために使用する状態コードです。 値: アクティブな場合、更新、削除、無視されます。|
|userTimezone | String | 省略可能。 活動の作成時に配置されましたユーザーのデバイスのアクティビティを生成するために使用するタイム ゾーンです。 クロスプラット フォーム形式をサポートするために、Olson の Id として指定された値です。|
|createdDateTime | DateTimeOffset | サーバーで設定します。 サーバー上にオブジェクトが作成されたときの utc 日時。|
|lastModifiedDateTime | DateTimeOffset | サーバーで設定します。 サーバー上にオブジェクトが変更されたときの utc 日時。|
|id | String | 必須。 **HistoryItem**オブジェクトの GUID をクライアントに設定します。|
|startedDateTime | DateTimeOffset | 必須です。 **HistoryItem** (アクティビティ セッション) が開始されたときの UTC 日時。 タイムラインの履歴が必要です。|
|lastActiveDateTime | DateTimeOffset | 省略可能。 **HistoryItem** (アクティビティ セッション) がアクティブまたは終了の null の場合、 **historyItem**の状態として理解された最後のときの UTC 日時は、継続中にする必要があります。|
|expirationDateTime | DateTimeOffset | 省略可能。 **HistoryItem**がハード削除を行うときの UTC 日時。 クライアントによって設定できます。|
|activeDurationSeconds | int | 省略可能。 アクティブなユーザーの活動の期間です。 指定されなかった場合、この**startedDateTime**と**lastActiveDateTime**から計算されます。|

## <a name="relationships"></a>関係

|リレーションシップ | 型 | 説明|
|:------------|:-----|:-----------|
|activity| [アクティビティ](../resources/projectrome-activity.md) | 省略可能。 受け取りますおよび抑制ソリューションです。ナビゲーション プロパティに関連する活動です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "enum-string",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-historyitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
