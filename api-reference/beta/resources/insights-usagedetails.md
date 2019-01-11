---
title: usageDetails リソースの種類
description: 複合型を使用する項目のプロパティが含まれています。 リソースが最後にアクセスしたときに情報 (表示)、ユーザーが (編集) を変更します。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 8729973c2393a918d26314ec3b27a2c68079dbfd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858955"
---
# <a name="usagedetails-resource-type"></a>usageDetails リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

複合型が[使用されている](insights-used.md)アイテムのプロパティが含まれています。 リソースが最後にアクセスしたときに情報 (表示)、ユーザーが (編集) を変更します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>プロパティ

| プロパティ              | 種類          | 説明  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | 日付と時刻、リソースは、ユーザーが最後にアクセスしました。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z` 読み取り専用です。                      |
| lastModifiedDateTime              | DateTimeOffset        | 日付と時刻、ユーザーによってリソースが最後に修正されました。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z` 読み取り専用です。       |
