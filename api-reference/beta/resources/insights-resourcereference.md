---
title: resourceReference リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 23a05a362ea57c84dceecbd9523c2620edc21fbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966287"
---
# <a name="resourcereference-resource-type"></a>resourceReference リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

複合型のプロパティ[情報](insights.md)にはが含まれています。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ      | 種類      | 説明  |
| ------------- |-----------| -------------|
| webUrl        | String    | 参照先の項目に先行する URL です。 |
| id            | String    | アイテムの一意の識別子です。           |
| type          | String    | 文字列値"microsoft.graph.driveItem"など、アイテムの分類に使用できます。 |
