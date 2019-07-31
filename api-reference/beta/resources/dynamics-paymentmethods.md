---
title: paymentMethods リソースの種類
description: Dynamics 365 Business Central の支払い方法オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 08cfc864ee670a799a5f1672fa96cf8167ef1423
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006585"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="6ee97-103">paymentMethods リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ee97-103">paymentMethods resource type</span></span>
<span data-ttu-id="6ee97-104">は、PayPal、クレジットカード、銀行口座など、Dynamics 365 Business Central の支払方法を表します。</span><span class="sxs-lookup"><span data-stu-id="6ee97-104">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="6ee97-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ee97-105">Methods</span></span>

| <span data-ttu-id="6ee97-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ee97-106">Method</span></span>                                                          | <span data-ttu-id="6ee97-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6ee97-107">Return Type</span></span>  |<span data-ttu-id="6ee97-108">説明</span><span class="sxs-lookup"><span data-stu-id="6ee97-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="6ee97-109">PaymentMethods を取得する</span><span class="sxs-lookup"><span data-stu-id="6ee97-109">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="6ee97-110">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="6ee97-110">paymentMethods</span></span>|<span data-ttu-id="6ee97-111">支払い方法オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="6ee97-111">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="6ee97-112">Post paymentMethods</span><span class="sxs-lookup"><span data-stu-id="6ee97-112">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="6ee97-113">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="6ee97-113">paymentMethods</span></span>|<span data-ttu-id="6ee97-114">支払い方法オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6ee97-114">Creates a payment method object.</span></span>|
|[<span data-ttu-id="6ee97-115">Patch paymentMethods</span><span class="sxs-lookup"><span data-stu-id="6ee97-115">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="6ee97-116">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="6ee97-116">paymentMethods</span></span>|<span data-ttu-id="6ee97-117">支払い方法オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="6ee97-117">Updates a payment method object.</span></span>|
|[<span data-ttu-id="6ee97-118">PaymentMethods の削除</span><span class="sxs-lookup"><span data-stu-id="6ee97-118">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="6ee97-119">none</span><span class="sxs-lookup"><span data-stu-id="6ee97-119">none</span></span>          |<span data-ttu-id="6ee97-120">支払い方法オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="6ee97-120">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ee97-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ee97-121">Properties</span></span>
| <span data-ttu-id="6ee97-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ee97-122">Property</span></span>           | <span data-ttu-id="6ee97-123">型</span><span class="sxs-lookup"><span data-stu-id="6ee97-123">Type</span></span>   |<span data-ttu-id="6ee97-124">説明</span><span class="sxs-lookup"><span data-stu-id="6ee97-124">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="6ee97-125">id</span><span class="sxs-lookup"><span data-stu-id="6ee97-125">id</span></span>                  |<span data-ttu-id="6ee97-126">GUID</span><span class="sxs-lookup"><span data-stu-id="6ee97-126">GUID</span></span>    |<span data-ttu-id="6ee97-127">PaymentMethods の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="6ee97-127">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="6ee97-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="6ee97-128">Non-editable.</span></span>           |
|<span data-ttu-id="6ee97-129">code</span><span class="sxs-lookup"><span data-stu-id="6ee97-129">code</span></span>                |<span data-ttu-id="6ee97-130">string</span><span class="sxs-lookup"><span data-stu-id="6ee97-130">string</span></span>  |<span data-ttu-id="6ee97-131">支払い方法のコードを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ee97-131">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="6ee97-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6ee97-132">displayName</span></span>         |<span data-ttu-id="6ee97-133">string</span><span class="sxs-lookup"><span data-stu-id="6ee97-133">string</span></span>  |<span data-ttu-id="6ee97-134">支払い方法の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ee97-134">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="6ee97-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ee97-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6ee97-136">datetime</span><span class="sxs-lookup"><span data-stu-id="6ee97-136">datetime</span></span>|<span data-ttu-id="6ee97-137">支払い方法が最後に変更された datetime。</span><span class="sxs-lookup"><span data-stu-id="6ee97-137">The last datetime the payment method was modified.</span></span> <span data-ttu-id="6ee97-138">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6ee97-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="6ee97-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6ee97-139">Relationships</span></span>
<span data-ttu-id="6ee97-140">なし</span><span class="sxs-lookup"><span data-stu-id="6ee97-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ee97-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ee97-141">JSON representation</span></span>

<span data-ttu-id="6ee97-142">PaymentMethods の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6ee97-142">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
