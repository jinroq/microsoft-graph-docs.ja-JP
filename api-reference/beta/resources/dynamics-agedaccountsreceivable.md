---
title: agedAccountsReceivable リソースの種類
description: Dynamics 365 Business Central の期限切れの売掛金勘定オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: f9589cbb4cb380eececdcc7adf7bd5dd682269f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012675"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="149a0-103">agedAccountsReceivable リソースの種類</span><span class="sxs-lookup"><span data-stu-id="149a0-103">agedAccountsReceivable resource type</span></span>
<span data-ttu-id="149a0-104">Dynamics 365 Business Central の agedAccountsReceivable オブジェクトを表します。これは、顧客アカウントのエージングを示します。</span><span class="sxs-lookup"><span data-stu-id="149a0-104">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="149a0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="149a0-105">Methods</span></span>

| <span data-ttu-id="149a0-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="149a0-106">Method</span></span>         | <span data-ttu-id="149a0-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="149a0-107">Return Type</span></span>  |<span data-ttu-id="149a0-108">説明</span><span class="sxs-lookup"><span data-stu-id="149a0-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="149a0-109">AgedAccountsReceivable を取得する</span><span class="sxs-lookup"><span data-stu-id="149a0-109">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="149a0-110">agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="149a0-110">agedAccountsReceivable</span></span>|<span data-ttu-id="149a0-111">AgedAccountsReceivable オブジェクトを取得する</span><span class="sxs-lookup"><span data-stu-id="149a0-111">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="149a0-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="149a0-112">Properties</span></span>
| <span data-ttu-id="149a0-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="149a0-113">Property</span></span>       | <span data-ttu-id="149a0-114">型</span><span class="sxs-lookup"><span data-stu-id="149a0-114">Type</span></span>    |<span data-ttu-id="149a0-115">説明</span><span class="sxs-lookup"><span data-stu-id="149a0-115">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="149a0-116">Id</span><span class="sxs-lookup"><span data-stu-id="149a0-116">customerId</span></span>      |<span data-ttu-id="149a0-117">GUID</span><span class="sxs-lookup"><span data-stu-id="149a0-117">GUID</span></span>     |<span data-ttu-id="149a0-118">顧客の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="149a0-118">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="149a0-119">顧客番号</span><span class="sxs-lookup"><span data-stu-id="149a0-119">customerNumber</span></span>  |<span data-ttu-id="149a0-120">string</span><span class="sxs-lookup"><span data-stu-id="149a0-120">string</span></span>   |<span data-ttu-id="149a0-121">顧客の番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-121">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="149a0-122">name</span><span class="sxs-lookup"><span data-stu-id="149a0-122">name</span></span>            |<span data-ttu-id="149a0-123">string</span><span class="sxs-lookup"><span data-stu-id="149a0-123">string</span></span>   |<span data-ttu-id="149a0-124">顧客の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-124">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="149a0-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="149a0-125">currencyCode</span></span>    |<span data-ttu-id="149a0-126">string</span><span class="sxs-lookup"><span data-stu-id="149a0-126">string</span></span>   |<span data-ttu-id="149a0-127">通貨を指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-127">Specifies the currency.</span></span>                      |
|<span data-ttu-id="149a0-128">定率</span><span class="sxs-lookup"><span data-stu-id="149a0-128">balanceDue</span></span>      |<span data-ttu-id="149a0-129">数値</span><span class="sxs-lookup"><span data-stu-id="149a0-129">numeric</span></span>  |<span data-ttu-id="149a0-130">顧客の総残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-130">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="149a0-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="149a0-131">currentAmount</span></span>   |<span data-ttu-id="149a0-132">数値</span><span class="sxs-lookup"><span data-stu-id="149a0-132">numeric</span></span>  |<span data-ttu-id="149a0-133">現在のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-133">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="149a0-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="149a0-134">period1Amount</span></span>   |<span data-ttu-id="149a0-135">数値</span><span class="sxs-lookup"><span data-stu-id="149a0-135">numeric</span></span>  |<span data-ttu-id="149a0-136">最初のエイジング期間で残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-136">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="149a0-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="149a0-137">period2Amount</span></span>   |<span data-ttu-id="149a0-138">数値</span><span class="sxs-lookup"><span data-stu-id="149a0-138">numeric</span></span>  |<span data-ttu-id="149a0-139">2番目のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="149a0-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="149a0-140">period3Amount</span></span>   |<span data-ttu-id="149a0-141">数値</span><span class="sxs-lookup"><span data-stu-id="149a0-141">numeric</span></span>  |<span data-ttu-id="149a0-142">3番目のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-142">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="149a0-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="149a0-143">agedAsOfDate</span></span>    |<span data-ttu-id="149a0-144">date</span><span class="sxs-lookup"><span data-stu-id="149a0-144">date</span></span>     |<span data-ttu-id="149a0-145">エイジング期間の計算に使用される期間の開始日を指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="149a0-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="149a0-146">periodLengthFilter</span></span>|<span data-ttu-id="149a0-147">string</span><span class="sxs-lookup"><span data-stu-id="149a0-147">string</span></span> |<span data-ttu-id="149a0-148">期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="149a0-148">Specifies the length of the periods.</span></span> <span data-ttu-id="149a0-149">使用可能な時間の単位は、D、WD、W、M、Q、および Y で、日付に基づく現在の時間単位は、時間単位のプレフィックスとして指定できます。</span><span class="sxs-lookup"><span data-stu-id="149a0-149">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="149a0-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="149a0-150">Relationships</span></span>
<span data-ttu-id="149a0-151">なし</span><span class="sxs-lookup"><span data-stu-id="149a0-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="149a0-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="149a0-152">JSON representation</span></span>

<span data-ttu-id="149a0-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="149a0-153">Here is a JSON representation of the resource.</span></span>


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
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


