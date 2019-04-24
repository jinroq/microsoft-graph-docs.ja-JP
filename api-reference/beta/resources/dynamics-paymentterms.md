---
title: paymentTerms リソースの種類
description: Dynamics 365 Business Central の支払い用語オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507330"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="ee01a-103">paymentTerms リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee01a-103">paymentTerms resource type</span></span>
<span data-ttu-id="ee01a-104">Dynamics 365 Business Central の支払い条件を表します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-104">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ee01a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ee01a-105">Methods</span></span>

| <span data-ttu-id="ee01a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ee01a-106">Method</span></span>                                                      | <span data-ttu-id="ee01a-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ee01a-107">Return Type</span></span>|<span data-ttu-id="ee01a-108">説明</span><span class="sxs-lookup"><span data-stu-id="ee01a-108">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="ee01a-109">paymentTerms を取得する</span><span class="sxs-lookup"><span data-stu-id="ee01a-109">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="ee01a-110">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="ee01a-110">paymentTerms</span></span>|<span data-ttu-id="ee01a-111">支払い用語オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-111">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="ee01a-112">Post paymentTerms</span><span class="sxs-lookup"><span data-stu-id="ee01a-112">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="ee01a-113">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="ee01a-113">paymentTerms</span></span>|<span data-ttu-id="ee01a-114">支払い用語オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-114">Create a payment terms object.</span></span>|
|[<span data-ttu-id="ee01a-115">Patch paymentTerms</span><span class="sxs-lookup"><span data-stu-id="ee01a-115">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="ee01a-116">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="ee01a-116">paymentTerms</span></span>|<span data-ttu-id="ee01a-117">支払い用語オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-117">Update a payment terms object.</span></span>|
|[<span data-ttu-id="ee01a-118">paymentTerms の削除</span><span class="sxs-lookup"><span data-stu-id="ee01a-118">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="ee01a-119">なし</span><span class="sxs-lookup"><span data-stu-id="ee01a-119">none</span></span>        |<span data-ttu-id="ee01a-120">支払い用語オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-120">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee01a-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee01a-121">Properties</span></span>
| <span data-ttu-id="ee01a-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee01a-122">Property</span></span>                     | <span data-ttu-id="ee01a-123">型</span><span class="sxs-lookup"><span data-stu-id="ee01a-123">Type</span></span>     |<span data-ttu-id="ee01a-124">説明</span><span class="sxs-lookup"><span data-stu-id="ee01a-124">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="ee01a-125">id</span><span class="sxs-lookup"><span data-stu-id="ee01a-125">id</span></span>                            |<span data-ttu-id="ee01a-126">GUID</span><span class="sxs-lookup"><span data-stu-id="ee01a-126">GUID</span></span>    |<span data-ttu-id="ee01a-127">paymentTerms の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="ee01a-127">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="ee01a-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="ee01a-128">Non-editable.</span></span>           |
|<span data-ttu-id="ee01a-129">code</span><span class="sxs-lookup"><span data-stu-id="ee01a-129">code</span></span>                          |<span data-ttu-id="ee01a-130">string</span><span class="sxs-lookup"><span data-stu-id="ee01a-130">string</span></span>  |<span data-ttu-id="ee01a-131">支払い条件コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-131">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="ee01a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ee01a-132">displayName</span></span>                   |<span data-ttu-id="ee01a-133">string</span><span class="sxs-lookup"><span data-stu-id="ee01a-133">string</span></span>  |<span data-ttu-id="ee01a-134">支払用語の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-134">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="ee01a-135">dueDateCalculation</span><span class="sxs-lookup"><span data-stu-id="ee01a-135">dueDateCalculation</span></span>            |<span data-ttu-id="ee01a-136">string</span><span class="sxs-lookup"><span data-stu-id="ee01a-136">string</span></span>  |<span data-ttu-id="ee01a-137">支払いが行われる日付の計算に使用される式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-137">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="ee01a-138">discountDateCalculation</span><span class="sxs-lookup"><span data-stu-id="ee01a-138">discountDateCalculation</span></span>       |<span data-ttu-id="ee01a-139">string</span><span class="sxs-lookup"><span data-stu-id="ee01a-139">string</span></span>  |<span data-ttu-id="ee01a-140">値引きを取得するために支払いを行う必要がある日付の計算に使用される式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-140">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="ee01a-141">discountpercent</span><span class="sxs-lookup"><span data-stu-id="ee01a-141">discountPercent</span></span>               |<span data-ttu-id="ee01a-142">decimal</span><span class="sxs-lookup"><span data-stu-id="ee01a-142">decimal</span></span> |<span data-ttu-id="ee01a-143">請求金額の早期支払いに適用される割引率を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-143">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="ee01a-144">calculateDiscountOnCreditMemos</span><span class="sxs-lookup"><span data-stu-id="ee01a-144">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="ee01a-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="ee01a-145">boolean</span></span> |<span data-ttu-id="ee01a-146">クレジットメモに割引を適用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-146">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="ee01a-147">**True**は割引が提供されることを示し、 **false**は割引が与えられないことを示します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-147">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="ee01a-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee01a-148">lastModifiedDateTime</span></span>          |<span data-ttu-id="ee01a-149">datetime</span><span class="sxs-lookup"><span data-stu-id="ee01a-149">datetime</span></span>|<span data-ttu-id="ee01a-150">paymentTerms が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ee01a-150">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="ee01a-151">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ee01a-151">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="ee01a-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ee01a-152">Relationships</span></span>
<span data-ttu-id="ee01a-153">なし</span><span class="sxs-lookup"><span data-stu-id="ee01a-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee01a-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee01a-154">JSON representation</span></span>

<span data-ttu-id="ee01a-155">paymentTerms の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ee01a-155">Here is a JSON representation of the paymentTerms.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
