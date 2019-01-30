---
title: outlookUser リソースの種類
description: ユーザーが利用できる Outlook サービスを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a649de502728bbc51ac53e072c08d95291d20853
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643546"
---
# <a name="outlookuser-resource-type"></a>outlookUser リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|[List tasks](../api/outlookuser-list-tasks.md) |[outlookTask](outlooktask.md) コレクション| ユーザーのメールボックス内のすべての Outlook タスクを取得します。|
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
|tasks|[outlookTask](outlooktask.md) コレクション| ユーザーの Outlook の仕事です。 読み取り専用です。 Null 許容型。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
