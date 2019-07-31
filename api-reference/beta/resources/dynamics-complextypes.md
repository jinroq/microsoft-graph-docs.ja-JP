---
title: 複合型 JSON
description: Dynamics 365 Business Central 用の JSON の複雑なデータ型。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bb61450ab7f1d62d459f525f6341093f25b1686f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012640"
---
# <a name="complex-types-json"></a><span data-ttu-id="dc6c5-103">複合型 JSON</span><span class="sxs-lookup"><span data-stu-id="dc6c5-103">complex types JSON</span></span>
<span data-ttu-id="dc6c5-104">これらは、Dynamics 365 Business Central のさまざまな複合型です。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-104">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="dc6c5-105">これらの複合型の使用方法は、それらを利用するさまざまな個別のメソッドで確認できます。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-105">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="dc6c5-106">郵送先住所</span><span class="sxs-lookup"><span data-stu-id="dc6c5-106">Postal address</span></span>

<span data-ttu-id="dc6c5-107">Dynamics 365 Business Central の郵送先住所の複合型を表します。</span><span class="sxs-lookup"><span data-stu-id="dc6c5-107">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="dc6c5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc6c5-108">Properties</span></span>
| <span data-ttu-id="dc6c5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc6c5-109">Property</span></span>     | <span data-ttu-id="dc6c5-110">型</span><span class="sxs-lookup"><span data-stu-id="dc6c5-110">Type</span></span>       |<span data-ttu-id="dc6c5-111">説明</span><span class="sxs-lookup"><span data-stu-id="dc6c5-111">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="dc6c5-112">street</span><span class="sxs-lookup"><span data-stu-id="dc6c5-112">street</span></span>        |<span data-ttu-id="dc6c5-113">string</span><span class="sxs-lookup"><span data-stu-id="dc6c5-113">string</span></span>    |<span data-ttu-id="dc6c5-114">郵送先住所</span><span class="sxs-lookup"><span data-stu-id="dc6c5-114">Postal address street.</span></span>  |
|<span data-ttu-id="dc6c5-115">city</span><span class="sxs-lookup"><span data-stu-id="dc6c5-115">city</span></span>          |<span data-ttu-id="dc6c5-116">string</span><span class="sxs-lookup"><span data-stu-id="dc6c5-116">string</span></span>    |<span data-ttu-id="dc6c5-117">市町村 (郵送先)</span><span class="sxs-lookup"><span data-stu-id="dc6c5-117">Postal address city.</span></span>    |
|<span data-ttu-id="dc6c5-118">state</span><span class="sxs-lookup"><span data-stu-id="dc6c5-118">state</span></span>         |<span data-ttu-id="dc6c5-119">string</span><span class="sxs-lookup"><span data-stu-id="dc6c5-119">string</span></span>    |<span data-ttu-id="dc6c5-120">都道府県 (郵送先住所)</span><span class="sxs-lookup"><span data-stu-id="dc6c5-120">Postal address state.</span></span>   |
|<span data-ttu-id="dc6c5-121">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="dc6c5-121">countryLetterCode</span></span>|<span data-ttu-id="dc6c5-122">string</span><span class="sxs-lookup"><span data-stu-id="dc6c5-122">string</span></span> |<span data-ttu-id="dc6c5-123">郵送先住所の文字コード (2 文字の単語)</span><span class="sxs-lookup"><span data-stu-id="dc6c5-123">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="dc6c5-124">postalCode</span><span class="sxs-lookup"><span data-stu-id="dc6c5-124">postalCode</span></span>    |<span data-ttu-id="dc6c5-125">string</span><span class="sxs-lookup"><span data-stu-id="dc6c5-125">string</span></span>    |<span data-ttu-id="dc6c5-126">郵便アドレスの post コード</span><span class="sxs-lookup"><span data-stu-id="dc6c5-126">Postal address post code</span></span>|

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

