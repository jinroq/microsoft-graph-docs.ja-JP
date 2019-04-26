---
title: outlookUser リソースの種類
description: ユーザーが利用できる Outlook サービスを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a649de502728bbc51ac53e072c08d95291d20853
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568597"
---
# <a name="outlookuser-resource-type"></a>outlookUser リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーが利用できる Outlook サービスを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[カテゴリの作成](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。|
|[カテゴリの一覧表示](../api/outlookuser-list-mastercategories.md) | [outlookCategory](outlookcategory.md) コレクション |ユーザーに対して定義されているすべてのカテゴリを取得します。|
|[outlooktaskfolder の作成](../api/outlookuser-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) にタスクフォルダーを作成します。|
|[taskfolders を一覧表示する](../api/outlookuser-list-taskfolders.md) |[outlooktaskfolder](outlooktaskfolder.md)コレクション| ユーザーのメールボックス内のすべての Outlook タスクフォルダーを取得します。|
|[outlooktaskgroup の作成](../api/outlookuser-post-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md)| ユーザーのメールボックスに Outlook のタスクグループを作成します。|
|[taskgroups を一覧表示する](../api/outlookuser-list-taskgroups.md) |[outlooktaskgroup](outlooktaskgroup.md)コレクション| ユーザーのメールボックス内のすべての Outlook タスクグループを取得します。|
|[outlooktask の作成](../api/outlookuser-post-tasks.md) |[outlookTask](outlooktask.md)| ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) および既定のタスクフォルダー`Tasks`() に Outlook のタスクを作成します。|
|[タスクを一覧表示する](../api/outlookuser-list-tasks.md) |[outlookTask](outlooktask.md) コレクション| ユーザーのメールボックス内のすべての Outlook タスクを取得します。|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | [localeInfo](localeinfo.md) コレクション | ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。 |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md) コレクション | ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。 |


## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) コレクション| ユーザーに対して定義されているカテゴリのリスト。 | 
|taskfolders|[outlooktaskfolder](outlooktaskfolder.md)コレクション| ユーザーの Outlook タスクフォルダー。 読み取り専用。 Null 許容型。|
|taskGroups|[outlooktaskgroup](outlooktaskgroup.md)コレクション| ユーザーの Outlook タスクグループ。 読み取り専用。 Null 許容型。|
|tasks|[outlookTask](outlooktask.md) コレクション| ユーザーの Outlook タスク。 読み取り専用。 Null 許容型。|

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
