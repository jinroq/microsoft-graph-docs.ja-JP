---
title: accounts リソースの種類
description: Dynamics 365 Business Central の account オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365459"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="8388f-103">accounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8388f-103">accounts resource type</span></span>
<span data-ttu-id="8388f-104">Dynamics 365 Business Central の account オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="8388f-104">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8388f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8388f-105">Methods</span></span>

| <span data-ttu-id="8388f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8388f-106">Method</span></span>       | <span data-ttu-id="8388f-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8388f-107">Return Type</span></span>  |<span data-ttu-id="8388f-108">説明</span><span class="sxs-lookup"><span data-stu-id="8388f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8388f-109">アカウントを取得する</span><span class="sxs-lookup"><span data-stu-id="8388f-109">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="8388f-110">アカウント</span><span class="sxs-lookup"><span data-stu-id="8388f-110">accounts</span></span>|<span data-ttu-id="8388f-111">accounts オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="8388f-111">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8388f-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8388f-112">Properties</span></span>
| <span data-ttu-id="8388f-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8388f-113">Property</span></span>     | <span data-ttu-id="8388f-114">型</span><span class="sxs-lookup"><span data-stu-id="8388f-114">Type</span></span>   |<span data-ttu-id="8388f-115">説明</span><span class="sxs-lookup"><span data-stu-id="8388f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8388f-116">ID</span><span class="sxs-lookup"><span data-stu-id="8388f-116">id</span></span>|<span data-ttu-id="8388f-117">GUID</span><span class="sxs-lookup"><span data-stu-id="8388f-117">GUID</span></span>|<span data-ttu-id="8388f-118">アカウントの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="8388f-118">The unique ID of the account.</span></span>|
|<span data-ttu-id="8388f-119">number</span><span class="sxs-lookup"><span data-stu-id="8388f-119">number</span></span>|<span data-ttu-id="8388f-120">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="8388f-120">string, maximum size 20</span></span>|<span data-ttu-id="8388f-121">G/L アカウントの番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="8388f-121">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="8388f-122">displayName</span><span class="sxs-lookup"><span data-stu-id="8388f-122">displayName</span></span>|<span data-ttu-id="8388f-123">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="8388f-123">string, maximum size 50</span></span>|<span data-ttu-id="8388f-124">G/L アカウントの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="8388f-124">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="8388f-125">category</span><span class="sxs-lookup"><span data-stu-id="8388f-125">category</span></span>|<span data-ttu-id="8388f-126">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="8388f-126">string, maximum size 20</span></span>|<span data-ttu-id="8388f-127">G/L アカウントのカテゴリを指定します。</span><span class="sxs-lookup"><span data-stu-id="8388f-127">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="8388f-128">カテゴリー</span><span class="sxs-lookup"><span data-stu-id="8388f-128">subCategory</span></span>|<span data-ttu-id="8388f-129">文字列、最大サイズ80</span><span class="sxs-lookup"><span data-stu-id="8388f-129">string, maximum size 80</span></span>|<span data-ttu-id="8388f-130">G/L アカウントのアカウントカテゴリのサブカテゴリを指定します。</span><span class="sxs-lookup"><span data-stu-id="8388f-130">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="8388f-131">ブロック</span><span class="sxs-lookup"><span data-stu-id="8388f-131">blocked</span></span>|<span data-ttu-id="8388f-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="8388f-132">boolean</span></span>|<span data-ttu-id="8388f-133">G/L アカウントにエントリを投稿できないことを指定します。</span><span class="sxs-lookup"><span data-stu-id="8388f-133">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="8388f-134">**True**は、アカウントがブロックされ、投稿が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="8388f-134">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="8388f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8388f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8388f-136">datetime</span><span class="sxs-lookup"><span data-stu-id="8388f-136">datetime</span></span>|<span data-ttu-id="8388f-137">アカウントが最後に変更された日付です。</span><span class="sxs-lookup"><span data-stu-id="8388f-137">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8388f-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8388f-138">Relationships</span></span>
<span data-ttu-id="8388f-139">なし</span><span class="sxs-lookup"><span data-stu-id="8388f-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8388f-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8388f-140">JSON representation</span></span>

<span data-ttu-id="8388f-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8388f-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
