---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 179c0bb1e5c82d7f2af17dcbcae08be8726f2ecd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888936"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="8adee-102">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8adee-102">CurrencyColumn resource type</span></span>

> <span data-ttu-id="8adee-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8adee-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8adee-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8adee-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8adee-105">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="8adee-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8adee-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8adee-106">JSON representation</span></span>

<span data-ttu-id="8adee-107">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8adee-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="8adee-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8adee-108">Properties</span></span>

| <span data-ttu-id="8adee-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8adee-109">Property name</span></span> | <span data-ttu-id="8adee-110">Type</span><span class="sxs-lookup"><span data-stu-id="8adee-110">Type</span></span>   | <span data-ttu-id="8adee-111">説明</span><span class="sxs-lookup"><span data-stu-id="8adee-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8adee-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="8adee-112">**locale**</span></span>    | <span data-ttu-id="8adee-113">文字列</span><span class="sxs-lookup"><span data-stu-id="8adee-113">string</span></span> | <span data-ttu-id="8adee-114">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="8adee-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
