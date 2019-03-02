---
title: 複合型 JSON
description: Dynamics 365 Business Central 用の JSON の複雑なデータ型。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366768"
---
# <a name="complex-types-json"></a><span data-ttu-id="96378-103">複合型 JSON</span><span class="sxs-lookup"><span data-stu-id="96378-103">complex types JSON</span></span>
<span data-ttu-id="96378-104">これらは、Dynamics 365 Business Central のさまざまな複合型です。</span><span class="sxs-lookup"><span data-stu-id="96378-104">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="96378-105">これらの複合型の使用方法は、それらを利用するさまざまな個別のメソッドで確認できます。</span><span class="sxs-lookup"><span data-stu-id="96378-105">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="96378-106">郵送先住所</span><span class="sxs-lookup"><span data-stu-id="96378-106">Postal address</span></span>

<span data-ttu-id="96378-107">Dynamics 365 Business Central の郵送先住所の複合型を表します。</span><span class="sxs-lookup"><span data-stu-id="96378-107">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="96378-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96378-108">Properties</span></span>
| <span data-ttu-id="96378-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96378-109">Property</span></span>     | <span data-ttu-id="96378-110">型</span><span class="sxs-lookup"><span data-stu-id="96378-110">Type</span></span>       |<span data-ttu-id="96378-111">説明</span><span class="sxs-lookup"><span data-stu-id="96378-111">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="96378-112">street</span><span class="sxs-lookup"><span data-stu-id="96378-112">street</span></span>        |<span data-ttu-id="96378-113">string</span><span class="sxs-lookup"><span data-stu-id="96378-113">string</span></span>    |<span data-ttu-id="96378-114">郵送先住所</span><span class="sxs-lookup"><span data-stu-id="96378-114">Postal address street.</span></span>  |
|<span data-ttu-id="96378-115">city</span><span class="sxs-lookup"><span data-stu-id="96378-115">city</span></span>          |<span data-ttu-id="96378-116">string</span><span class="sxs-lookup"><span data-stu-id="96378-116">string</span></span>    |<span data-ttu-id="96378-117">市町村 (郵送先)</span><span class="sxs-lookup"><span data-stu-id="96378-117">Postal address city.</span></span>    |
|<span data-ttu-id="96378-118">state</span><span class="sxs-lookup"><span data-stu-id="96378-118">state</span></span>         |<span data-ttu-id="96378-119">string</span><span class="sxs-lookup"><span data-stu-id="96378-119">string</span></span>    |<span data-ttu-id="96378-120">都道府県 (郵送先住所)</span><span class="sxs-lookup"><span data-stu-id="96378-120">Postal address state.</span></span>   |
|<span data-ttu-id="96378-121">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="96378-121">countryLetterCode</span></span>|<span data-ttu-id="96378-122">string</span><span class="sxs-lookup"><span data-stu-id="96378-122">string</span></span> |<span data-ttu-id="96378-123">郵送先住所の文字コード (2 文字の単語)</span><span class="sxs-lookup"><span data-stu-id="96378-123">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="96378-124">postalCode</span><span class="sxs-lookup"><span data-stu-id="96378-124">postalCode</span></span>    |<span data-ttu-id="96378-125">string</span><span class="sxs-lookup"><span data-stu-id="96378-125">string</span></span>    |<span data-ttu-id="96378-126">郵便アドレスの post コード</span><span class="sxs-lookup"><span data-stu-id="96378-126">Postal address post code</span></span>|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```

