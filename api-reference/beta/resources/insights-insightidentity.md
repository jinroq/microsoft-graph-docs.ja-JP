---
title: insightIdentity
description: 共有アイテムのプロパティを格納する複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a263caa68280128a67a027b75682407fd4932605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938938"
---
# <a name="insightidentity"></a>insightIdentity

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

| プロパティ              | 種類          | 説明  |
| -------------         |-----------    | -------------|
| displayName       | String          | アイテムを共有するユーザーの表示名。 |
| id              | String        | アイテムを共有するユーザーの id です。     |
| address             | String      | アイテムを共有するユーザーの電子メール アドレスです。  |
