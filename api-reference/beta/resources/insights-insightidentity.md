---
title: insightIdentity
description: " リソースの種類"
ms.openlocfilehash: e13d08eb111844896c96b02ab22c52d2f598ce58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071083"
---
# <a name="insightidentity"></a>insightIdentity

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

 リソースの種類

[共有](insights-shared.md)アイテムのプロパティを格納する複合型。 

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ              | 型          | 説明  |
| -------------         |-----------    | -------------|
| displayName       | String          | アイテムを共有するユーザーの表示名。 |
| id              | String        | アイテムを共有するユーザーの id です。     |
| address             | String      | アイテムを共有するユーザーの電子メール アドレスです。  |