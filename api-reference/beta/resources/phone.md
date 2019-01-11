---
title: 電話リソースの種類
description: 電話番号を表します。
localization_priority: Normal
ms.openlocfilehash: 7397349e1fee1164d3bcde8ebc785edd9402fe75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874180"
---
# <a name="phone-resource-type"></a><span data-ttu-id="bff55-103">電話リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bff55-103">phone resource type</span></span>

> <span data-ttu-id="bff55-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bff55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bff55-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bff55-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bff55-106">電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="bff55-106">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="bff55-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bff55-107">Properties</span></span>
| <span data-ttu-id="bff55-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bff55-108">Property</span></span>     | <span data-ttu-id="bff55-109">種類</span><span class="sxs-lookup"><span data-stu-id="bff55-109">Type</span></span>   |<span data-ttu-id="bff55-110">説明</span><span class="sxs-lookup"><span data-stu-id="bff55-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bff55-111">number</span><span class="sxs-lookup"><span data-stu-id="bff55-111">number</span></span>|<span data-ttu-id="bff55-112">文字列</span><span class="sxs-lookup"><span data-stu-id="bff55-112">string</span></span>|<span data-ttu-id="bff55-113">電話番号。</span><span class="sxs-lookup"><span data-stu-id="bff55-113">The phone number.</span></span>|
|<span data-ttu-id="bff55-114">種類</span><span class="sxs-lookup"><span data-stu-id="bff55-114">type</span></span>|<span data-ttu-id="bff55-115">String</span><span class="sxs-lookup"><span data-stu-id="bff55-115">String</span></span>|<span data-ttu-id="bff55-p102">電話番号の種類。可能な値は、`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio` です。</span><span class="sxs-lookup"><span data-stu-id="bff55-p102">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bff55-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bff55-118">JSON representation</span></span>

<span data-ttu-id="bff55-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bff55-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
