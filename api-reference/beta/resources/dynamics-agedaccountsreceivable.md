---
title: agedAccountsReceivable リソースの種類
description: Dynamics 365 Business Central の期限切れの売掛金勘定オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507617"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="a5a72-103">agedAccountsReceivable リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a5a72-103">agedAccountsReceivable resource type</span></span>
<span data-ttu-id="a5a72-104">Dynamics 365 Business Central の agedAccountsReceivable オブジェクトを表します。これは、顧客アカウントのエージングを示します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-104">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="a5a72-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5a72-105">Methods</span></span>

| <span data-ttu-id="a5a72-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5a72-106">Method</span></span>         | <span data-ttu-id="a5a72-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a5a72-107">Return Type</span></span>  |<span data-ttu-id="a5a72-108">説明</span><span class="sxs-lookup"><span data-stu-id="a5a72-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="a5a72-109">agedAccountsReceivable を取得する</span><span class="sxs-lookup"><span data-stu-id="a5a72-109">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="a5a72-110">agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="a5a72-110">agedAccountsReceivable</span></span>|<span data-ttu-id="a5a72-111">agedAccountsReceivable オブジェクトを取得する</span><span class="sxs-lookup"><span data-stu-id="a5a72-111">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="a5a72-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5a72-112">Properties</span></span>
| <span data-ttu-id="a5a72-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5a72-113">Property</span></span>       | <span data-ttu-id="a5a72-114">型</span><span class="sxs-lookup"><span data-stu-id="a5a72-114">Type</span></span>    |<span data-ttu-id="a5a72-115">説明</span><span class="sxs-lookup"><span data-stu-id="a5a72-115">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="a5a72-116">id</span><span class="sxs-lookup"><span data-stu-id="a5a72-116">customerId</span></span>      |<span data-ttu-id="a5a72-117">GUID</span><span class="sxs-lookup"><span data-stu-id="a5a72-117">GUID</span></span>     |<span data-ttu-id="a5a72-118">顧客の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="a5a72-118">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="a5a72-119">顧客番号</span><span class="sxs-lookup"><span data-stu-id="a5a72-119">customerNumber</span></span>  |<span data-ttu-id="a5a72-120">string</span><span class="sxs-lookup"><span data-stu-id="a5a72-120">string</span></span>   |<span data-ttu-id="a5a72-121">顧客の番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-121">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="a5a72-122">name</span><span class="sxs-lookup"><span data-stu-id="a5a72-122">name</span></span>            |<span data-ttu-id="a5a72-123">string</span><span class="sxs-lookup"><span data-stu-id="a5a72-123">string</span></span>   |<span data-ttu-id="a5a72-124">顧客の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-124">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="a5a72-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="a5a72-125">currencyCode</span></span>    |<span data-ttu-id="a5a72-126">string</span><span class="sxs-lookup"><span data-stu-id="a5a72-126">string</span></span>   |<span data-ttu-id="a5a72-127">通貨を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-127">Specifies the currency.</span></span>                      |
|<span data-ttu-id="a5a72-128">定率</span><span class="sxs-lookup"><span data-stu-id="a5a72-128">balanceDue</span></span>      |<span data-ttu-id="a5a72-129">数値</span><span class="sxs-lookup"><span data-stu-id="a5a72-129">numeric</span></span>  |<span data-ttu-id="a5a72-130">顧客の総残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-130">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="a5a72-131">currentamount</span><span class="sxs-lookup"><span data-stu-id="a5a72-131">currentAmount</span></span>   |<span data-ttu-id="a5a72-132">数値</span><span class="sxs-lookup"><span data-stu-id="a5a72-132">numeric</span></span>  |<span data-ttu-id="a5a72-133">現在のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-133">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="a5a72-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="a5a72-134">period1Amount</span></span>   |<span data-ttu-id="a5a72-135">数値</span><span class="sxs-lookup"><span data-stu-id="a5a72-135">numeric</span></span>  |<span data-ttu-id="a5a72-136">最初のエイジング期間で残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-136">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="a5a72-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="a5a72-137">period2Amount</span></span>   |<span data-ttu-id="a5a72-138">数値</span><span class="sxs-lookup"><span data-stu-id="a5a72-138">numeric</span></span>  |<span data-ttu-id="a5a72-139">2番目のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="a5a72-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="a5a72-140">period3Amount</span></span>   |<span data-ttu-id="a5a72-141">数値</span><span class="sxs-lookup"><span data-stu-id="a5a72-141">numeric</span></span>  |<span data-ttu-id="a5a72-142">3番目のエイジング期間の残高を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-142">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="a5a72-143">agedasofdate</span><span class="sxs-lookup"><span data-stu-id="a5a72-143">agedAsOfDate</span></span>    |<span data-ttu-id="a5a72-144">日付</span><span class="sxs-lookup"><span data-stu-id="a5a72-144">date</span></span>     |<span data-ttu-id="a5a72-145">エイジング期間の計算に使用される期間の開始日を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="a5a72-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="a5a72-146">periodLengthFilter</span></span>|<span data-ttu-id="a5a72-147">string</span><span class="sxs-lookup"><span data-stu-id="a5a72-147">string</span></span> |<span data-ttu-id="a5a72-148">期間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a5a72-148">Specifies the length of the periods.</span></span> <span data-ttu-id="a5a72-149">使用可能な時間の単位は、D、WD、W、M、Q、および Y で、日付に基づく現在の時間単位は、時間単位のプレフィックスとして指定できます。</span><span class="sxs-lookup"><span data-stu-id="a5a72-149">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="a5a72-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a5a72-150">Relationships</span></span>
<span data-ttu-id="a5a72-151">なし</span><span class="sxs-lookup"><span data-stu-id="a5a72-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5a72-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a5a72-152">JSON representation</span></span>

<span data-ttu-id="a5a72-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a5a72-153">Here is a JSON representation of the resource.</span></span>


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


