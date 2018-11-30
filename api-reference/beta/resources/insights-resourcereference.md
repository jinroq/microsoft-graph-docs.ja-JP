---
title: resourceReference リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
ms.openlocfilehash: d171151a1c3547aa6863a7f70cc3a42ddec13e5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071282"
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

| プロパティ      | 型      | 説明  |
| ------------- |-----------| -------------|
| webUrl        | String    | 参照先の項目に先行する URL です。 |
| id            | String    | アイテムの一意の識別子です。           |
| type          | String    | 文字列値"microsoft.graph.driveItem"など、アイテムの分類に使用できます。 |