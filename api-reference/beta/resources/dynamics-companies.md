---
title: 会社のリソースの種類
description: Dynamics 365 Business Central の会社。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 6720a8959ddba79d1face9c91325900c3a35a95c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973731"
---
# <a name="companies-resource-type"></a><span data-ttu-id="b3c73-103">会社のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3c73-103">companies resource type</span></span>
<span data-ttu-id="b3c73-104">Dynamics 365 Business Central の会社のリソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="b3c73-104">Represents a companies resource type in Dynamics 365 Business Central.</span></span> 

## <a name="methods"></a><span data-ttu-id="b3c73-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3c73-105">Methods</span></span>

| <span data-ttu-id="b3c73-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3c73-106">Method</span></span>         | <span data-ttu-id="b3c73-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b3c73-107">Return Type</span></span>  |<span data-ttu-id="b3c73-108">説明</span><span class="sxs-lookup"><span data-stu-id="b3c73-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="b3c73-109">会社名を取得する</span><span class="sxs-lookup"><span data-stu-id="b3c73-109">Get companies</span></span>](../api/dynamics-companies-get.md)|<span data-ttu-id="b3c73-110">companies</span><span class="sxs-lookup"><span data-stu-id="b3c73-110">companies</span></span>|<span data-ttu-id="b3c73-111">会社を取得します。</span><span class="sxs-lookup"><span data-stu-id="b3c73-111">Get a company.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3c73-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3c73-112">Properties</span></span>
| <span data-ttu-id="b3c73-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3c73-113">Property</span></span>        | <span data-ttu-id="b3c73-114">型</span><span class="sxs-lookup"><span data-stu-id="b3c73-114">Type</span></span> |<span data-ttu-id="b3c73-115">説明</span><span class="sxs-lookup"><span data-stu-id="b3c73-115">Description</span></span>                             |
|:----------------|:-----|:---------------------------------------|
|<span data-ttu-id="b3c73-116">id</span><span class="sxs-lookup"><span data-stu-id="b3c73-116">id</span></span>               |<span data-ttu-id="b3c73-117">GUID</span><span class="sxs-lookup"><span data-stu-id="b3c73-117">GUID</span></span>  |<span data-ttu-id="b3c73-118">会社の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="b3c73-118">The unique ID of the company.</span></span> <span data-ttu-id="b3c73-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b3c73-119">Read-Only.</span></span>|
|<span data-ttu-id="b3c73-120">name</span><span class="sxs-lookup"><span data-stu-id="b3c73-120">name</span></span>             |<span data-ttu-id="b3c73-121">string</span><span class="sxs-lookup"><span data-stu-id="b3c73-121">string</span></span>|<span data-ttu-id="b3c73-122">会社を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3c73-122">Specifies the Company.</span></span>                  |
|<span data-ttu-id="b3c73-123">displayName</span><span class="sxs-lookup"><span data-stu-id="b3c73-123">displayName</span></span>      |<span data-ttu-id="b3c73-124">string</span><span class="sxs-lookup"><span data-stu-id="b3c73-124">string</span></span>|<span data-ttu-id="b3c73-125">会社の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3c73-125">Specifies the company display name.</span></span>     |
|<span data-ttu-id="b3c73-126">systemVersion</span><span class="sxs-lookup"><span data-stu-id="b3c73-126">systemVersion</span></span>    |<span data-ttu-id="b3c73-127">string</span><span class="sxs-lookup"><span data-stu-id="b3c73-127">string</span></span>|<span data-ttu-id="b3c73-128">会社の内部バージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="b3c73-128">Specifies the internal version of the company.</span></span>|
|<span data-ttu-id="b3c73-129">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="b3c73-129">businessProfileId</span></span>|<span data-ttu-id="b3c73-130">string</span><span class="sxs-lookup"><span data-stu-id="b3c73-130">string</span></span>|<span data-ttu-id="b3c73-131">会社にリンクされているビジネスプロファイル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3c73-131">Specifies the Business Profile ID linked to the company.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b3c73-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3c73-132">Relationships</span></span>
<span data-ttu-id="b3c73-133">なし</span><span class="sxs-lookup"><span data-stu-id="b3c73-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3c73-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3c73-134">JSON representation</span></span>

<span data-ttu-id="b3c73-135">以下は、会社の JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3c73-135">Here is a JSON representation of the company.</span></span>

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


