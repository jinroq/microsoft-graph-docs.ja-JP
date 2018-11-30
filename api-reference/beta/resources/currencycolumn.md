---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 21c95026eb61eb68c98010d8ac288be115e95ec8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074190"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="e6079-102">CurrencyColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6079-102">CurrencyColumn resource type</span></span>

> <span data-ttu-id="e6079-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e6079-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6079-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6079-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6079-105">[columnDefinition](columndefinition.md) リソースの **currencyColumn** は、列の値が通貨を表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="e6079-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6079-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6079-106">JSON representation</span></span>

<span data-ttu-id="e6079-107">以下は、**currencyColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e6079-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="e6079-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6079-108">Properties</span></span>

| <span data-ttu-id="e6079-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e6079-109">Property name</span></span> | <span data-ttu-id="e6079-110">型</span><span class="sxs-lookup"><span data-stu-id="e6079-110">Type</span></span>   | <span data-ttu-id="e6079-111">説明</span><span class="sxs-lookup"><span data-stu-id="e6079-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e6079-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="e6079-112">**locale**</span></span>    | <span data-ttu-id="e6079-113">文字列</span><span class="sxs-lookup"><span data-stu-id="e6079-113">string</span></span> | <span data-ttu-id="e6079-114">通貨記号を推測するロケールを指定します。</span><span class="sxs-lookup"><span data-stu-id="e6079-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
