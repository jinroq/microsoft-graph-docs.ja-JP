---
title: trialbalance リソースの種類
description: Dynamics 365 Business Central の試算表オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534851"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="1a497-103">trialbalance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a497-103">trialBalance resource type</span></span>
<span data-ttu-id="1a497-104">Dynamics 365 Business Central の試算表を表します。</span><span class="sxs-lookup"><span data-stu-id="1a497-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="1a497-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a497-105">Methods</span></span>

| <span data-ttu-id="1a497-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a497-106">Method</span></span>       | <span data-ttu-id="1a497-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1a497-107">Return Type</span></span>  |<span data-ttu-id="1a497-108">説明</span><span class="sxs-lookup"><span data-stu-id="1a497-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a497-109">trialbalance の取得</span><span class="sxs-lookup"><span data-stu-id="1a497-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="1a497-110">trialbalance</span><span class="sxs-lookup"><span data-stu-id="1a497-110">trialBalance</span></span>|<span data-ttu-id="1a497-111">試算表オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="1a497-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a497-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a497-112">Properties</span></span>
| <span data-ttu-id="1a497-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a497-113">Property</span></span>     | <span data-ttu-id="1a497-114">型</span><span class="sxs-lookup"><span data-stu-id="1a497-114">Type</span></span>   |<span data-ttu-id="1a497-115">説明</span><span class="sxs-lookup"><span data-stu-id="1a497-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a497-116">番号</span><span class="sxs-lookup"><span data-stu-id="1a497-116">number</span></span>|<span data-ttu-id="1a497-117">string</span><span class="sxs-lookup"><span data-stu-id="1a497-117">string</span></span>|<span data-ttu-id="1a497-118">trialbalance アイテムの G/L アカウント番号</span><span class="sxs-lookup"><span data-stu-id="1a497-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="1a497-119">accountId</span><span class="sxs-lookup"><span data-stu-id="1a497-119">accountId</span></span>|<span data-ttu-id="1a497-120">GUID</span><span class="sxs-lookup"><span data-stu-id="1a497-120">GUID</span></span>|<span data-ttu-id="1a497-121">レコードの G/L アカウントの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1a497-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="1a497-122">accountType</span><span class="sxs-lookup"><span data-stu-id="1a497-122">accountType</span></span>|<span data-ttu-id="1a497-123">string</span><span class="sxs-lookup"><span data-stu-id="1a497-123">string</span></span>|<span data-ttu-id="1a497-124">レコードの G/L アカウントのアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="1a497-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="1a497-125">ディスプレイ</span><span class="sxs-lookup"><span data-stu-id="1a497-125">display</span></span>|<span data-ttu-id="1a497-126">string</span><span class="sxs-lookup"><span data-stu-id="1a497-126">string</span></span>|<span data-ttu-id="1a497-127">trialbalance アイテムの G/L アカウント名。</span><span class="sxs-lookup"><span data-stu-id="1a497-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="1a497-128">totaldebit</span><span class="sxs-lookup"><span data-stu-id="1a497-128">totalDebit</span></span>|<span data-ttu-id="1a497-129">string</span><span class="sxs-lookup"><span data-stu-id="1a497-129">string</span></span>|<span data-ttu-id="1a497-130">G/L アカウントの借方金額の合計を表します。</span><span class="sxs-lookup"><span data-stu-id="1a497-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="1a497-131">totalcredit</span><span class="sxs-lookup"><span data-stu-id="1a497-131">totalCredit</span></span>|<span data-ttu-id="1a497-132">string</span><span class="sxs-lookup"><span data-stu-id="1a497-132">string</span></span>|<span data-ttu-id="1a497-133">G/L アカウントの合計クレジット金額を表します。</span><span class="sxs-lookup"><span data-stu-id="1a497-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="1a497-134">定率</span><span class="sxs-lookup"><span data-stu-id="1a497-134">balanceAtDateDebit</span></span>|<span data-ttu-id="1a497-135">string</span><span class="sxs-lookup"><span data-stu-id="1a497-135">string</span></span>|<span data-ttu-id="1a497-136">G/L アカウントの日付の金額での正の残高を表します。</span><span class="sxs-lookup"><span data-stu-id="1a497-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="1a497-137">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="1a497-137">balanceAtDateCredit</span></span>|<span data-ttu-id="1a497-138">string</span><span class="sxs-lookup"><span data-stu-id="1a497-138">string</span></span>|<span data-ttu-id="1a497-139">G/L アカウントの日付の金額での負の残高を表します。</span><span class="sxs-lookup"><span data-stu-id="1a497-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="1a497-140">datefilter</span><span class="sxs-lookup"><span data-stu-id="1a497-140">dateFilter</span></span>|<span data-ttu-id="1a497-141">日付</span><span class="sxs-lookup"><span data-stu-id="1a497-141">date</span></span>|<span data-ttu-id="1a497-142">trialbalance のアイテムを計算するために使用される日付フィルター。</span><span class="sxs-lookup"><span data-stu-id="1a497-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1a497-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a497-143">Relationships</span></span>
<span data-ttu-id="1a497-144">なし</span><span class="sxs-lookup"><span data-stu-id="1a497-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a497-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a497-145">JSON representation</span></span>

<span data-ttu-id="1a497-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a497-146">Here is a JSON representation of the resource.</span></span>


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```

