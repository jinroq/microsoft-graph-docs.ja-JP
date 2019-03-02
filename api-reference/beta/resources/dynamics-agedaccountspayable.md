---
title: agedaccountspayable リソースの種類
description: Dynamics 365 Business Central にある、期限切れのアカウントの債務オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 679c24b7ef32ef59b34a5885ea745d8c244376b2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365907"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="fd9bd-103">agedaccountspayable リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd9bd-103">agedAccountsPayable resource type</span></span>
<span data-ttu-id="fd9bd-104">Dynamics 365 Business Central の agedaccountspayable オブジェクトを表します。これは、ベンダーアカウントのエイジングを示しています。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-104">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="fd9bd-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd9bd-105">Methods</span></span>

| <span data-ttu-id="fd9bd-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd9bd-106">Method</span></span>         | <span data-ttu-id="fd9bd-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fd9bd-107">Return Type</span></span>  |<span data-ttu-id="fd9bd-108">説明</span><span class="sxs-lookup"><span data-stu-id="fd9bd-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="fd9bd-109">agedaccountspayable を取得する</span><span class="sxs-lookup"><span data-stu-id="fd9bd-109">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="fd9bd-110">agedaccountspayable</span><span class="sxs-lookup"><span data-stu-id="fd9bd-110">agedAccountsPayable</span></span>|<span data-ttu-id="fd9bd-111">agedaccountspayable オブジェクトを取得する</span><span class="sxs-lookup"><span data-stu-id="fd9bd-111">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="fd9bd-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd9bd-112">Properties</span></span>
| <span data-ttu-id="fd9bd-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd9bd-113">Property</span></span>      | <span data-ttu-id="fd9bd-114">型</span><span class="sxs-lookup"><span data-stu-id="fd9bd-114">Type</span></span>     |<span data-ttu-id="fd9bd-115">説明</span><span class="sxs-lookup"><span data-stu-id="fd9bd-115">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="fd9bd-116">vendorId</span><span class="sxs-lookup"><span data-stu-id="fd9bd-116">vendorId</span></span>       |<span data-ttu-id="fd9bd-117">GUID</span><span class="sxs-lookup"><span data-stu-id="fd9bd-117">GUID</span></span>      |<span data-ttu-id="fd9bd-118">ベンダーの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-118">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="fd9bd-119">vendorNumber</span><span class="sxs-lookup"><span data-stu-id="fd9bd-119">vendorNumber</span></span>   |<span data-ttu-id="fd9bd-120">string</span><span class="sxs-lookup"><span data-stu-id="fd9bd-120">string</span></span>    |<span data-ttu-id="fd9bd-121">仕入先の番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-121">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="fd9bd-122">name</span><span class="sxs-lookup"><span data-stu-id="fd9bd-122">name</span></span>           |<span data-ttu-id="fd9bd-123">string</span><span class="sxs-lookup"><span data-stu-id="fd9bd-123">string</span></span>    |<span data-ttu-id="fd9bd-124">ベンダーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-124">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="fd9bd-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="fd9bd-125">currencyCode</span></span>   |<span data-ttu-id="fd9bd-126">string</span><span class="sxs-lookup"><span data-stu-id="fd9bd-126">string</span></span>    |<span data-ttu-id="fd9bd-127">通貨を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-127">Specifies the currency.</span></span>                     |
|<span data-ttu-id="fd9bd-128">定率</span><span class="sxs-lookup"><span data-stu-id="fd9bd-128">balanceDue</span></span>     |<span data-ttu-id="fd9bd-129">numeric</span><span class="sxs-lookup"><span data-stu-id="fd9bd-129">numeric</span></span>   |<span data-ttu-id="fd9bd-130">仕入先による総残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-130">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="fd9bd-131">currentamount</span><span class="sxs-lookup"><span data-stu-id="fd9bd-131">currentAmount</span></span>  |<span data-ttu-id="fd9bd-132">numeric</span><span class="sxs-lookup"><span data-stu-id="fd9bd-132">numeric</span></span>   |<span data-ttu-id="fd9bd-133">最初のエイジング期間より前の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-133">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="fd9bd-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="fd9bd-134">period1Amount</span></span>  |<span data-ttu-id="fd9bd-135">numeric</span><span class="sxs-lookup"><span data-stu-id="fd9bd-135">numeric</span></span>   |<span data-ttu-id="fd9bd-136">最初のエイジング期間で残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-136">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="fd9bd-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="fd9bd-137">period2Amount</span></span>  |<span data-ttu-id="fd9bd-138">numeric</span><span class="sxs-lookup"><span data-stu-id="fd9bd-138">numeric</span></span>   |<span data-ttu-id="fd9bd-139">2番目のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="fd9bd-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="fd9bd-140">period3Amount</span></span>  |<span data-ttu-id="fd9bd-141">numeric</span><span class="sxs-lookup"><span data-stu-id="fd9bd-141">numeric</span></span>   |<span data-ttu-id="fd9bd-142">3番目のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-142">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="fd9bd-143">agedasofdate</span><span class="sxs-lookup"><span data-stu-id="fd9bd-143">agedAsOfDate</span></span>   |<span data-ttu-id="fd9bd-144">日付</span><span class="sxs-lookup"><span data-stu-id="fd9bd-144">date</span></span>|<span data-ttu-id="fd9bd-145">エイジング期間の計算に使用される期間の開始日を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="fd9bd-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="fd9bd-146">periodLengthFilter</span></span>|<span data-ttu-id="fd9bd-147">string</span><span class="sxs-lookup"><span data-stu-id="fd9bd-147">string</span></span> |<span data-ttu-id="fd9bd-148">期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-148">Specifies the length of the periods.</span></span> <span data-ttu-id="fd9bd-149">時間単位に使用できる値は、D、WD、W、M、Q、または .c で、日付に基づく現在の時間単位は、時間単位のプレフィックスとして指定できます。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-149">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="fd9bd-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd9bd-150">Relationships</span></span>
<span data-ttu-id="fd9bd-151">なし</span><span class="sxs-lookup"><span data-stu-id="fd9bd-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd9bd-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd9bd-152">JSON representation</span></span>

<span data-ttu-id="fd9bd-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fd9bd-153">Here is a JSON representation of the resource.</span></span>


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
