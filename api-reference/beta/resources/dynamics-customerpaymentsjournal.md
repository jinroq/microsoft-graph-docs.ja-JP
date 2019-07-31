---
title: customerPaymentJournals リソースの種類
description: Dynamics 365 Business Central の顧客支払仕訳帳。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 0791fe2b8c36bdff535f7fc56dea54abe1632647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973633"
---
# <a name="customerpaymentsjournals-resource-type"></a><span data-ttu-id="39bdc-103">customerPaymentsJournals リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39bdc-103">customerPaymentsJournals resource type</span></span>
<span data-ttu-id="39bdc-104">Dynamics 365 Business Central の顧客支払仕訳帳を表します。</span><span class="sxs-lookup"><span data-stu-id="39bdc-104">Represents a customer payment journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="39bdc-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="39bdc-105">Methods</span></span>

| <span data-ttu-id="39bdc-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="39bdc-106">Method</span></span>               | <span data-ttu-id="39bdc-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="39bdc-107">Return Type</span></span>             |<span data-ttu-id="39bdc-108">説明</span><span class="sxs-lookup"><span data-stu-id="39bdc-108">Description</span></span>                      |
|:---------------------|:------------------------|:--------------------------------|
|[<span data-ttu-id="39bdc-109">CustomerPaymentJournals を取得する</span><span class="sxs-lookup"><span data-stu-id="39bdc-109">Get customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-get.md)      |<span data-ttu-id="39bdc-110">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="39bdc-110">customerPaymentJournals</span></span>|<span data-ttu-id="39bdc-111">顧客支払仕訳帳を取得します。</span><span class="sxs-lookup"><span data-stu-id="39bdc-111">Gets a customer payment journal.</span></span>   |
|[<span data-ttu-id="39bdc-112">Post customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="39bdc-112">Post customerPaymentJournals</span></span>](../api/dynamics-create-customerpaymentsjournal.md)  |<span data-ttu-id="39bdc-113">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="39bdc-113">customerPaymentJournals</span></span>|<span data-ttu-id="39bdc-114">顧客支払仕訳帳を作成します。</span><span class="sxs-lookup"><span data-stu-id="39bdc-114">Creates a customer payment journal.</span></span>|
|[<span data-ttu-id="39bdc-115">Patch customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="39bdc-115">Patch customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-update.md) |<span data-ttu-id="39bdc-116">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="39bdc-116">customerPaymentJournals</span></span>|<span data-ttu-id="39bdc-117">顧客支払仕訳帳を更新します。</span><span class="sxs-lookup"><span data-stu-id="39bdc-117">Updates a customer payment journal.</span></span>|
|[<span data-ttu-id="39bdc-118">CustomerPaymentJournals の削除</span><span class="sxs-lookup"><span data-stu-id="39bdc-118">Delete customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-delete.md)|<span data-ttu-id="39bdc-119">none</span><span class="sxs-lookup"><span data-stu-id="39bdc-119">none</span></span>                     |<span data-ttu-id="39bdc-120">顧客支払仕訳帳を削除します。</span><span class="sxs-lookup"><span data-stu-id="39bdc-120">Deletes a customer payment journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="39bdc-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39bdc-121">Properties</span></span>
| <span data-ttu-id="39bdc-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39bdc-122">Property</span></span>           | <span data-ttu-id="39bdc-123">型</span><span class="sxs-lookup"><span data-stu-id="39bdc-123">Type</span></span>                  |<span data-ttu-id="39bdc-124">説明</span><span class="sxs-lookup"><span data-stu-id="39bdc-124">Description</span></span>                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|<span data-ttu-id="39bdc-125">id</span><span class="sxs-lookup"><span data-stu-id="39bdc-125">id</span></span>                  |<span data-ttu-id="39bdc-126">GUID</span><span class="sxs-lookup"><span data-stu-id="39bdc-126">GUID</span></span>                   |<span data-ttu-id="39bdc-127">顧客支払仕訳帳の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="39bdc-127">The unique ID of the customer payment journal.</span></span> <span data-ttu-id="39bdc-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="39bdc-128">Non-editable.</span></span>           |
|<span data-ttu-id="39bdc-129">code</span><span class="sxs-lookup"><span data-stu-id="39bdc-129">code</span></span>                |<span data-ttu-id="39bdc-130">文字列、最大サイズ10</span><span class="sxs-lookup"><span data-stu-id="39bdc-130">string, maximum size 10</span></span>| <span data-ttu-id="39bdc-131">顧客支払仕訳帳のコード。</span><span class="sxs-lookup"><span data-stu-id="39bdc-131">The code of the customer payment journal.</span></span>                             |
|<span data-ttu-id="39bdc-132">displayName</span><span class="sxs-lookup"><span data-stu-id="39bdc-132">displayName</span></span>         |<span data-ttu-id="39bdc-133">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="39bdc-133">string, maximum size 50</span></span>| <span data-ttu-id="39bdc-134">顧客支払仕訳帳の表示名。</span><span class="sxs-lookup"><span data-stu-id="39bdc-134">The display name of the customer payment journal.</span></span>                     |
|<span data-ttu-id="39bdc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39bdc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="39bdc-136">datetime</span><span class="sxs-lookup"><span data-stu-id="39bdc-136">datetime</span></span>               |<span data-ttu-id="39bdc-137">顧客支払仕訳帳が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="39bdc-137">The last datetime the customer payment journal was modified.</span></span> <span data-ttu-id="39bdc-138">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="39bdc-138">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39bdc-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39bdc-139">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="39bdc-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39bdc-140">JSON representation</span></span>

<span data-ttu-id="39bdc-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39bdc-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

