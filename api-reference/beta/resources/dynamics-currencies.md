---
title: 通貨リソースの種類
description: Dynamics 365 Business Central の currency オブジェクト
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ba8ad750831394e2a84fab7ca87d76754838db60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012619"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="c328c-103">通貨リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c328c-103">currencies resource type</span></span>
<span data-ttu-id="c328c-104">Dynamics 365 Business Central で使用されている通貨を表します。</span><span class="sxs-lookup"><span data-stu-id="c328c-104">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="c328c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c328c-105">Methods</span></span>
| <span data-ttu-id="c328c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c328c-106">Method</span></span>                                                  |<span data-ttu-id="c328c-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c328c-107">Return Type</span></span>|<span data-ttu-id="c328c-108">説明</span><span class="sxs-lookup"><span data-stu-id="c328c-108">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="c328c-109">通貨を取得する</span><span class="sxs-lookup"><span data-stu-id="c328c-109">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="c328c-110">外貨</span><span class="sxs-lookup"><span data-stu-id="c328c-110">currencies</span></span> |<span data-ttu-id="c328c-111">通貨を取得します。</span><span class="sxs-lookup"><span data-stu-id="c328c-111">Get a Currency.</span></span>   |
|[<span data-ttu-id="c328c-112">通貨の転記</span><span class="sxs-lookup"><span data-stu-id="c328c-112">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="c328c-113">外貨</span><span class="sxs-lookup"><span data-stu-id="c328c-113">currencies</span></span> |<span data-ttu-id="c328c-114">通貨を作成します。</span><span class="sxs-lookup"><span data-stu-id="c328c-114">Create a Currency.</span></span>|
|[<span data-ttu-id="c328c-115">パッチ通貨</span><span class="sxs-lookup"><span data-stu-id="c328c-115">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="c328c-116">外貨</span><span class="sxs-lookup"><span data-stu-id="c328c-116">currencies</span></span> |<span data-ttu-id="c328c-117">通貨を更新します。</span><span class="sxs-lookup"><span data-stu-id="c328c-117">Update a Currency.</span></span>|
|[<span data-ttu-id="c328c-118">通貨を削除する</span><span class="sxs-lookup"><span data-stu-id="c328c-118">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="c328c-119">none</span><span class="sxs-lookup"><span data-stu-id="c328c-119">none</span></span>       |<span data-ttu-id="c328c-120">通貨を削除します。</span><span class="sxs-lookup"><span data-stu-id="c328c-120">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="c328c-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c328c-121">Properties</span></span>
| <span data-ttu-id="c328c-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c328c-122">Property</span></span>              | <span data-ttu-id="c328c-123">型</span><span class="sxs-lookup"><span data-stu-id="c328c-123">Type</span></span>   |<span data-ttu-id="c328c-124">説明</span><span class="sxs-lookup"><span data-stu-id="c328c-124">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="c328c-125">id</span><span class="sxs-lookup"><span data-stu-id="c328c-125">id</span></span>                     |<span data-ttu-id="c328c-126">GUID</span><span class="sxs-lookup"><span data-stu-id="c328c-126">GUID</span></span>    |<span data-ttu-id="c328c-127">通貨の一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="c328c-127">The unique ID of the currency.</span></span> <span data-ttu-id="c328c-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="c328c-128">Non-editable.</span></span>                  |
|<span data-ttu-id="c328c-129">code</span><span class="sxs-lookup"><span data-stu-id="c328c-129">code</span></span>                   |<span data-ttu-id="c328c-130">string</span><span class="sxs-lookup"><span data-stu-id="c328c-130">string</span></span>  |<span data-ttu-id="c328c-131">通貨コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="c328c-131">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="c328c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c328c-132">displayName</span></span>            |<span data-ttu-id="c328c-133">string</span><span class="sxs-lookup"><span data-stu-id="c328c-133">string</span></span>  |<span data-ttu-id="c328c-134">通貨の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="c328c-134">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="c328c-135">疑問符</span><span class="sxs-lookup"><span data-stu-id="c328c-135">symbol</span></span>                 |<span data-ttu-id="c328c-136">string</span><span class="sxs-lookup"><span data-stu-id="c328c-136">string</span></span>  |<span data-ttu-id="c328c-137">小切手に表示されるこの通貨の記号を指定します。</span><span class="sxs-lookup"><span data-stu-id="c328c-137">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="c328c-138">amountDecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="c328c-138">amountDecimalPlaces</span></span>    |<span data-ttu-id="c328c-139">string</span><span class="sxs-lookup"><span data-stu-id="c328c-139">string</span></span>  |<span data-ttu-id="c328c-140">この通貨の金額で、システムが表示される小数点以下の桁数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c328c-140">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="c328c-141">amountRoundingPrecision</span><span class="sxs-lookup"><span data-stu-id="c328c-141">amountRoundingPrecision</span></span>|<span data-ttu-id="c328c-142">decimal</span><span class="sxs-lookup"><span data-stu-id="c328c-142">decimal</span></span> |<span data-ttu-id="c328c-143">この通貨の金額を丸めるときに使用する間隔のサイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="c328c-143">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="c328c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c328c-144">lastModifiedDateTime</span></span>   |<span data-ttu-id="c328c-145">datetime</span><span class="sxs-lookup"><span data-stu-id="c328c-145">datetime</span></span>|<span data-ttu-id="c328c-146">通貨が最後に変更された datetime。</span><span class="sxs-lookup"><span data-stu-id="c328c-146">The last datetime the currency was modified.</span></span> <span data-ttu-id="c328c-147">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c328c-147">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="c328c-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c328c-148">Relationships</span></span>
<span data-ttu-id="c328c-149">なし</span><span class="sxs-lookup"><span data-stu-id="c328c-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c328c-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c328c-150">JSON representation</span></span>

<span data-ttu-id="c328c-151">以下は、通貨の JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c328c-151">Here is a JSON representation of the currencies.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

