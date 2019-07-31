---
title: agedAccountsPayable リソースの種類
description: Dynamics 365 Business Central にある、期限切れのアカウントの債務オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a135627804e2d6c5be4203c0ee0c229642c70c65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973745"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="435d5-103">agedAccountsPayable リソースの種類</span><span class="sxs-lookup"><span data-stu-id="435d5-103">agedAccountsPayable resource type</span></span>
<span data-ttu-id="435d5-104">Dynamics 365 Business Central の agedAccountsPayable オブジェクトを表します。これは、ベンダーアカウントのエイジングを示しています。</span><span class="sxs-lookup"><span data-stu-id="435d5-104">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="435d5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="435d5-105">Methods</span></span>

| <span data-ttu-id="435d5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="435d5-106">Method</span></span>         | <span data-ttu-id="435d5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="435d5-107">Return Type</span></span>  |<span data-ttu-id="435d5-108">説明</span><span class="sxs-lookup"><span data-stu-id="435d5-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="435d5-109">AgedAccountsPayable を取得する</span><span class="sxs-lookup"><span data-stu-id="435d5-109">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="435d5-110">agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="435d5-110">agedAccountsPayable</span></span>|<span data-ttu-id="435d5-111">AgedAccountsPayable オブジェクトを取得する</span><span class="sxs-lookup"><span data-stu-id="435d5-111">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="435d5-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="435d5-112">Properties</span></span>
| <span data-ttu-id="435d5-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="435d5-113">Property</span></span>      | <span data-ttu-id="435d5-114">型</span><span class="sxs-lookup"><span data-stu-id="435d5-114">Type</span></span>     |<span data-ttu-id="435d5-115">説明</span><span class="sxs-lookup"><span data-stu-id="435d5-115">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="435d5-116">vendorId</span><span class="sxs-lookup"><span data-stu-id="435d5-116">vendorId</span></span>       |<span data-ttu-id="435d5-117">GUID</span><span class="sxs-lookup"><span data-stu-id="435d5-117">GUID</span></span>      |<span data-ttu-id="435d5-118">ベンダーの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="435d5-118">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="435d5-119">vendorNumber</span><span class="sxs-lookup"><span data-stu-id="435d5-119">vendorNumber</span></span>   |<span data-ttu-id="435d5-120">string</span><span class="sxs-lookup"><span data-stu-id="435d5-120">string</span></span>    |<span data-ttu-id="435d5-121">仕入先の番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-121">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="435d5-122">name</span><span class="sxs-lookup"><span data-stu-id="435d5-122">name</span></span>           |<span data-ttu-id="435d5-123">string</span><span class="sxs-lookup"><span data-stu-id="435d5-123">string</span></span>    |<span data-ttu-id="435d5-124">ベンダーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-124">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="435d5-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="435d5-125">currencyCode</span></span>   |<span data-ttu-id="435d5-126">string</span><span class="sxs-lookup"><span data-stu-id="435d5-126">string</span></span>    |<span data-ttu-id="435d5-127">通貨を指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-127">Specifies the currency.</span></span>                     |
|<span data-ttu-id="435d5-128">定率</span><span class="sxs-lookup"><span data-stu-id="435d5-128">balanceDue</span></span>     |<span data-ttu-id="435d5-129">数値</span><span class="sxs-lookup"><span data-stu-id="435d5-129">numeric</span></span>   |<span data-ttu-id="435d5-130">仕入先による総残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-130">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="435d5-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="435d5-131">currentAmount</span></span>  |<span data-ttu-id="435d5-132">数値</span><span class="sxs-lookup"><span data-stu-id="435d5-132">numeric</span></span>   |<span data-ttu-id="435d5-133">最初のエイジング期間より前の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-133">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="435d5-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="435d5-134">period1Amount</span></span>  |<span data-ttu-id="435d5-135">数値</span><span class="sxs-lookup"><span data-stu-id="435d5-135">numeric</span></span>   |<span data-ttu-id="435d5-136">最初のエイジング期間で残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-136">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="435d5-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="435d5-137">period2Amount</span></span>  |<span data-ttu-id="435d5-138">数値</span><span class="sxs-lookup"><span data-stu-id="435d5-138">numeric</span></span>   |<span data-ttu-id="435d5-139">2番目のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="435d5-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="435d5-140">period3Amount</span></span>  |<span data-ttu-id="435d5-141">数値</span><span class="sxs-lookup"><span data-stu-id="435d5-141">numeric</span></span>   |<span data-ttu-id="435d5-142">3番目のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-142">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="435d5-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="435d5-143">agedAsOfDate</span></span>   |<span data-ttu-id="435d5-144">date</span><span class="sxs-lookup"><span data-stu-id="435d5-144">date</span></span>|<span data-ttu-id="435d5-145">エイジング期間の計算に使用される期間の開始日を指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="435d5-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="435d5-146">periodLengthFilter</span></span>|<span data-ttu-id="435d5-147">string</span><span class="sxs-lookup"><span data-stu-id="435d5-147">string</span></span> |<span data-ttu-id="435d5-148">期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="435d5-148">Specifies the length of the periods.</span></span> <span data-ttu-id="435d5-149">時間単位に使用できる値は、D、WD、W、M、Q、または .C で、日付に基づく現在の時間単位は、時間単位のプレフィックスとして指定できます。</span><span class="sxs-lookup"><span data-stu-id="435d5-149">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="435d5-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="435d5-150">Relationships</span></span>
<span data-ttu-id="435d5-151">なし</span><span class="sxs-lookup"><span data-stu-id="435d5-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="435d5-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="435d5-152">JSON representation</span></span>

<span data-ttu-id="435d5-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="435d5-153">Here is a JSON representation of the resource.</span></span>


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```
