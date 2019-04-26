---
title: 履歴項目リソースの種類
description: アプリ内のアクティビティの履歴アイテムを表します。 ユーザーアクティビティは、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなど、アプリ内の単一の場所を表します。 ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す履歴項目として契約が取得されます。 ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: c43a4f0515f8d61625e11abe8bbdbe2464c729f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344081"
---
# <a name="historyitem-resource-type"></a>履歴項目リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリ内の[アクティビティ](projectrome-activity.md)の履歴アイテムを表します。 ユーザーアクティビティは、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなど、アプリ内の単一の場所を表します。 ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す履歴項目として契約が取得されます。 ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。

アプリでセッションを作成するときには、ユーザーの活動期間を反映するために、**履歴項目**オブジェクトを**activity**オブジェクトに追加する必要があります。 ユーザーがアクティビティを再実行するたびに、新しい**履歴アイテム**が、[見越計上] ユーザー契約に追加されます。

## <a name="methods"></a>メソッド

|メソッド | 戻り値の型 | 説明|
|:------|:------------|:-----------|
|[履歴項目を作成または置換する](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | そのアクティビティの既存の**履歴アイテム**を作成または置換します (upsert)。 ID は GUID である必要があります。|
|[履歴項目を削除する](../api/projectrome-delete-historyitem.md) | No Content | そのアクティビティの指定した**履歴アイテム**を削除します。|

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|status | string | サーバーによって設定されます。 有効なオブジェクトを識別するために使用される状態コード。 値: アクティブ、更新済み、削除済み、無視。|
|usertimezone | String | 省略可能。 アクティビティの生成に使用されたユーザーのデバイスがアクティビティの作成時に配置されたタイムゾーン。 クロスプラットフォーム表現をサポートするために olson id として提供される値。|
|createdDateTime | DateTimeOffset | サーバーによって設定されます。 サーバー上でオブジェクトが作成された日時 (UTC)。|
|lastModifiedDateTime | DateTimeOffset | サーバーによって設定されます。 サーバー上のオブジェクトが変更された日時 (UTC)。|
|id | String | 必須。 **履歴項目**オブジェクトのクライアントセット GUID。|
|開始日時 | DateTimeOffset | 必須です。 **履歴アイテム**(アクティビティセッション) が開始された UTC の DateTime。 タイムライン履歴に必要です。|
|lastactivedatetime | DateTimeOffset | 省略可能。 **履歴項目**(アクティビティセッション) が最後にアクティブまたは完了として認識された UTC の DateTime。 null の場合は、**履歴アイテム**の状態が進行中である必要があります。|
|expirationDateTime | DateTimeOffset | 省略可能。 **履歴アイテム**がハード削除されるときの UTC DateTime。 クライアントによって設定できます。|
|activeDurationSeconds | int | 省略可能。 アクティブなユーザー契約の期間。 指定しない場合、これは開始日**** と**lastactivedatetime**から計算されます。|

## <a name="relationships"></a>リレーションシップ

|リレーションシップ | 型 | 説明|
|:------------|:-----|:-----------|
|activity| [アクティビティ](../resources/projectrome-activity.md) | 省略可能。 NavigationProperty/コンテインメント;関連付けられたアクティビティへのナビゲーションプロパティ。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
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
  "suppressions": []
}
-->
