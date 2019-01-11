---
title: recentNotebook リソース型
description: 最近アクセスした OneNote ノートブック。 **recentNotebook** は、notebook と類似していますが、より少ないプロパティを持ちます。
localization_priority: Normal
ms.openlocfilehash: 67c707043e5b6ca65cd72ddc323b5a484f0f2959
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889224"
---
# <a name="recentnotebook-resource-type"></a>recentNotebook リソース型

最近アクセスした OneNote ノートブック。 **recentNotebook** は、[notebook](notebook.md) と類似していますが、より少ないプロパティを持ちます。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|displayName|String|ノートブックの名前。|
|lastAccessedTime|DateTimeOffset|ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。|
|リンク|[recentNotebookLinks](recentnotebooklinks.md)|ノートブックを開くためのリンク。 `oneNoteClientURL` リンクは、OneNote クライアントでノートブックを開きます (インストールされている場合)。 `oneNoteWebURL` リンクは、OneNote Online でノートブックを開きます。|
|sourceService|onenoteSourceService|ノートブックが存在するバックエンド ストア (`OneDriveForBusiness` または `OneDrive` のいずれか)。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}
```

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | [ノートブック](notebook.md) コレクション | ユーザーの最近アクセスしたノートブックのコレクションを取得します。 |
