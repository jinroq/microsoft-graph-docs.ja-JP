---
title: outlookUser リソースの種類
description: ユーザーが利用できる Outlook サービスを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: bf772eb1598b38550797458df955495dafdd4282
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943600"
---
# <a name="outlookuser-resource-type"></a>outlookUser リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザーが利用できる Outlook サービスを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[カテゴリの作成](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。|
|[カテゴリの一覧表示](../api/outlookuser-list-mastercategories.md) | [outlookCategory](outlookcategory.md) コレクション |ユーザーに対して定義されているすべてのカテゴリを取得します。|
|[OutlookTaskFolder を作成します。](../api/outlookuser-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| 既定のタスク グループにタスク フォルダーを作成 (`My Tasks`) ユーザーのメールボックスの。|
|[リスト taskFolders](../api/outlookuser-list-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)コレクション| ユーザーのメールボックス内のすべての Outlook タスク フォルダーを取得します。|
|[OutlookTaskGroup を作成します。](../api/outlookuser-post-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md)| ユーザーのメールボックスに Outlook のタスク グループを作成します。|
|[TaskGroups のリスト](../api/outlookuser-list-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md)コレクション| ユーザーのメールボックス内のすべての Outlook のタスク グループを取得します。|
|[OutlookTask を作成します。](../api/outlookuser-post-tasks.md) |[outlookTask](outlooktask.md)| デフォルトのタスク グループに Outlook のタスクを作成する (`My Tasks`) と既定の作業フォルダー (`Tasks`) ユーザーのメールボックスにします。|
|[List tasks](../api/outlookuser-list-tasks.md) |[outlookTask](outlooktask.md)コレクション| ユーザーのメールボックス内のすべての Outlook タスクを取得します。|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | [localeInfo](localeinfo.md) コレクション | ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。 |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md) コレクション | ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。 |


## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) コレクション| ユーザーに対して定義されているカテゴリのリスト。 | 
|taskFolders|[outlookTaskFolder](outlooktaskfolder.md)コレクション| ユーザーの Outlook の仕事フォルダー。 読み取り専用です。 Null 許容型。|
|taskGroups|[outlookTaskGroup](outlooktaskgroup.md)コレクション| ユーザーの Outlook のタスク グループ。 読み取り専用です。 Null 許容型。|
|tasks|[outlookTask](outlooktask.md)コレクション| ユーザーの Outlook の仕事です。 読み取り専用です。 Null 許容型。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
