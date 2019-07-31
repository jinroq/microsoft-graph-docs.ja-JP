---
title: trialBalance リソースの種類
description: Dynamics 365 Business Central の試算表オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 02e4f039411c992cd1d7335fc2463d660b8ff181
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972874"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="2924c-103">trialBalance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2924c-103">trialBalance resource type</span></span>
<span data-ttu-id="2924c-104">Dynamics 365 Business Central の試算表を表します。</span><span class="sxs-lookup"><span data-stu-id="2924c-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="2924c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2924c-105">Methods</span></span>

| <span data-ttu-id="2924c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2924c-106">Method</span></span>       | <span data-ttu-id="2924c-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2924c-107">Return Type</span></span>  |<span data-ttu-id="2924c-108">説明</span><span class="sxs-lookup"><span data-stu-id="2924c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2924c-109">TrialBalance の取得</span><span class="sxs-lookup"><span data-stu-id="2924c-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="2924c-110">trialBalance</span><span class="sxs-lookup"><span data-stu-id="2924c-110">trialBalance</span></span>|<span data-ttu-id="2924c-111">試算表オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="2924c-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2924c-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2924c-112">Properties</span></span>
| <span data-ttu-id="2924c-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2924c-113">Property</span></span>     | <span data-ttu-id="2924c-114">型</span><span class="sxs-lookup"><span data-stu-id="2924c-114">Type</span></span>   |<span data-ttu-id="2924c-115">説明</span><span class="sxs-lookup"><span data-stu-id="2924c-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2924c-116">番号</span><span class="sxs-lookup"><span data-stu-id="2924c-116">number</span></span>|<span data-ttu-id="2924c-117">string</span><span class="sxs-lookup"><span data-stu-id="2924c-117">string</span></span>|<span data-ttu-id="2924c-118">TrialBalance アイテムの G/L アカウント番号</span><span class="sxs-lookup"><span data-stu-id="2924c-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="2924c-119">accountId</span><span class="sxs-lookup"><span data-stu-id="2924c-119">accountId</span></span>|<span data-ttu-id="2924c-120">GUID</span><span class="sxs-lookup"><span data-stu-id="2924c-120">GUID</span></span>|<span data-ttu-id="2924c-121">レコードの G/L アカウントの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="2924c-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="2924c-122">accountType</span><span class="sxs-lookup"><span data-stu-id="2924c-122">accountType</span></span>|<span data-ttu-id="2924c-123">string</span><span class="sxs-lookup"><span data-stu-id="2924c-123">string</span></span>|<span data-ttu-id="2924c-124">レコードの G/L アカウントのアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="2924c-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="2924c-125">ディスプレイ</span><span class="sxs-lookup"><span data-stu-id="2924c-125">display</span></span>|<span data-ttu-id="2924c-126">string</span><span class="sxs-lookup"><span data-stu-id="2924c-126">string</span></span>|<span data-ttu-id="2924c-127">TrialBalance アイテムの G/L アカウント名。</span><span class="sxs-lookup"><span data-stu-id="2924c-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="2924c-128">totalDebit</span><span class="sxs-lookup"><span data-stu-id="2924c-128">totalDebit</span></span>|<span data-ttu-id="2924c-129">string</span><span class="sxs-lookup"><span data-stu-id="2924c-129">string</span></span>|<span data-ttu-id="2924c-130">G/L アカウントの借方金額の合計を表します。</span><span class="sxs-lookup"><span data-stu-id="2924c-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="2924c-131">totalCredit</span><span class="sxs-lookup"><span data-stu-id="2924c-131">totalCredit</span></span>|<span data-ttu-id="2924c-132">string</span><span class="sxs-lookup"><span data-stu-id="2924c-132">string</span></span>|<span data-ttu-id="2924c-133">G/L アカウントの合計クレジット金額を表します。</span><span class="sxs-lookup"><span data-stu-id="2924c-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="2924c-134">定率</span><span class="sxs-lookup"><span data-stu-id="2924c-134">balanceAtDateDebit</span></span>|<span data-ttu-id="2924c-135">string</span><span class="sxs-lookup"><span data-stu-id="2924c-135">string</span></span>|<span data-ttu-id="2924c-136">G/L アカウントの日付の金額での正の残高を表します。</span><span class="sxs-lookup"><span data-stu-id="2924c-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="2924c-137">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="2924c-137">balanceAtDateCredit</span></span>|<span data-ttu-id="2924c-138">string</span><span class="sxs-lookup"><span data-stu-id="2924c-138">string</span></span>|<span data-ttu-id="2924c-139">G/L アカウントの日付の金額での負の残高を表します。</span><span class="sxs-lookup"><span data-stu-id="2924c-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="2924c-140">dateFilter</span><span class="sxs-lookup"><span data-stu-id="2924c-140">dateFilter</span></span>|<span data-ttu-id="2924c-141">date</span><span class="sxs-lookup"><span data-stu-id="2924c-141">date</span></span>|<span data-ttu-id="2924c-142">TrialBalance のアイテムを計算するために使用される日付フィルター。</span><span class="sxs-lookup"><span data-stu-id="2924c-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2924c-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2924c-143">Relationships</span></span>
<span data-ttu-id="2924c-144">なし</span><span class="sxs-lookup"><span data-stu-id="2924c-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2924c-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2924c-145">JSON representation</span></span>

<span data-ttu-id="2924c-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2924c-146">Here is a JSON representation of the resource.</span></span>


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

