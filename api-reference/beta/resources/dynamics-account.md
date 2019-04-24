---
title: accounts リソースの種類
description: Dynamics 365 Business Central の account オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507575"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="7b9d7-103">accounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b9d7-103">accounts resource type</span></span>
<span data-ttu-id="7b9d7-104">Dynamics 365 Business Central の account オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-104">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="7b9d7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7b9d7-105">Methods</span></span>

| <span data-ttu-id="7b9d7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7b9d7-106">Method</span></span>       | <span data-ttu-id="7b9d7-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7b9d7-107">Return Type</span></span>  |<span data-ttu-id="7b9d7-108">説明</span><span class="sxs-lookup"><span data-stu-id="7b9d7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b9d7-109">アカウントを取得する</span><span class="sxs-lookup"><span data-stu-id="7b9d7-109">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="7b9d7-110">アカウント</span><span class="sxs-lookup"><span data-stu-id="7b9d7-110">accounts</span></span>|<span data-ttu-id="7b9d7-111">accounts オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-111">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b9d7-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b9d7-112">Properties</span></span>
| <span data-ttu-id="7b9d7-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b9d7-113">Property</span></span>     | <span data-ttu-id="7b9d7-114">型</span><span class="sxs-lookup"><span data-stu-id="7b9d7-114">Type</span></span>   |<span data-ttu-id="7b9d7-115">説明</span><span class="sxs-lookup"><span data-stu-id="7b9d7-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b9d7-116">id</span><span class="sxs-lookup"><span data-stu-id="7b9d7-116">id</span></span>|<span data-ttu-id="7b9d7-117">GUID</span><span class="sxs-lookup"><span data-stu-id="7b9d7-117">GUID</span></span>|<span data-ttu-id="7b9d7-118">アカウントの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-118">The unique ID of the account.</span></span>|
|<span data-ttu-id="7b9d7-119">number</span><span class="sxs-lookup"><span data-stu-id="7b9d7-119">number</span></span>|<span data-ttu-id="7b9d7-120">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="7b9d7-120">string, maximum size 20</span></span>|<span data-ttu-id="7b9d7-121">G/L アカウントの番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-121">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="7b9d7-122">displayName</span><span class="sxs-lookup"><span data-stu-id="7b9d7-122">displayName</span></span>|<span data-ttu-id="7b9d7-123">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="7b9d7-123">string, maximum size 50</span></span>|<span data-ttu-id="7b9d7-124">G/L アカウントの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-124">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="7b9d7-125">category</span><span class="sxs-lookup"><span data-stu-id="7b9d7-125">category</span></span>|<span data-ttu-id="7b9d7-126">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="7b9d7-126">string, maximum size 20</span></span>|<span data-ttu-id="7b9d7-127">G/L アカウントのカテゴリを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-127">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="7b9d7-128">カテゴリー</span><span class="sxs-lookup"><span data-stu-id="7b9d7-128">subCategory</span></span>|<span data-ttu-id="7b9d7-129">文字列、最大サイズ80</span><span class="sxs-lookup"><span data-stu-id="7b9d7-129">string, maximum size 80</span></span>|<span data-ttu-id="7b9d7-130">G/L アカウントのアカウントカテゴリのサブカテゴリを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-130">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="7b9d7-131">ブロック</span><span class="sxs-lookup"><span data-stu-id="7b9d7-131">blocked</span></span>|<span data-ttu-id="7b9d7-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="7b9d7-132">boolean</span></span>|<span data-ttu-id="7b9d7-133">G/L アカウントにエントリを投稿できないことを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-133">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="7b9d7-134">**True**は、アカウントがブロックされ、投稿が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-134">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="7b9d7-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b9d7-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7b9d7-136">datetime</span><span class="sxs-lookup"><span data-stu-id="7b9d7-136">datetime</span></span>|<span data-ttu-id="7b9d7-137">アカウントが最後に変更された日付です。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-137">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7b9d7-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7b9d7-138">Relationships</span></span>
<span data-ttu-id="7b9d7-139">なし</span><span class="sxs-lookup"><span data-stu-id="7b9d7-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b9d7-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b9d7-140">JSON representation</span></span>

<span data-ttu-id="7b9d7-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7b9d7-141">Here is a JSON representation of the resource.</span></span>


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
