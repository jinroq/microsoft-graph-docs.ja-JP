---
title: sharingDetail リソースの種類
description: '共有アイテムのプロパティを格納する複合型。 '
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 463ba207d7b160bffb96319a994b82ee82f14b8d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888460"
---
# <a name="sharingdetail-resource-type"></a>sharingDetail リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[共有](insights-shared.md)アイテムのプロパティを格納する複合型。 

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a>プロパティ

| プロパティ              | 種類          | 説明  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| 日付と時刻、ファイルが最後に共有します。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z` 読み取り専用です。  |
| sharingSubject        | String          | ドキュメントを共有している情報カテゴリです。 |
| sharingType             | String        | 方法、ドキュメントが共有されていた、「リンク」、「添付ファイル」、「グループ」、「サイト」であることができますを決定します。     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | ドキュメントを共有するユーザーです。  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |
