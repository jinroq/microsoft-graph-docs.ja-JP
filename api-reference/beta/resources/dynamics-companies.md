---
title: 会社のリソースの種類
description: Dynamics 365 Business Central の会社。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: f1faca36af25bc8cb3e9019e0dc5b4460991e70d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365683"
---
# <a name="companies-resource-type"></a><span data-ttu-id="81bd8-103">会社のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="81bd8-103">companies resource type</span></span>
<span data-ttu-id="81bd8-104">Dynamics 365 Business Central の会社のリソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="81bd8-104">Represents a companies resource type in Dynamics 365 Business Central.</span></span> 

## <a name="methods"></a><span data-ttu-id="81bd8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="81bd8-105">Methods</span></span>

| <span data-ttu-id="81bd8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="81bd8-106">Method</span></span>         | <span data-ttu-id="81bd8-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="81bd8-107">Return Type</span></span>  |<span data-ttu-id="81bd8-108">説明</span><span class="sxs-lookup"><span data-stu-id="81bd8-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="81bd8-109">会社を取得する</span><span class="sxs-lookup"><span data-stu-id="81bd8-109">Get companies</span></span>](../api/dynamics-companies-get.md)|<span data-ttu-id="81bd8-110">とっ</span><span class="sxs-lookup"><span data-stu-id="81bd8-110">companies</span></span>|<span data-ttu-id="81bd8-111">会社を取得します。</span><span class="sxs-lookup"><span data-stu-id="81bd8-111">Get a company.</span></span>|

## <a name="properties"></a><span data-ttu-id="81bd8-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81bd8-112">Properties</span></span>
| <span data-ttu-id="81bd8-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81bd8-113">Property</span></span>        | <span data-ttu-id="81bd8-114">型</span><span class="sxs-lookup"><span data-stu-id="81bd8-114">Type</span></span> |<span data-ttu-id="81bd8-115">説明</span><span class="sxs-lookup"><span data-stu-id="81bd8-115">Description</span></span>                             |
|:----------------|:-----|:---------------------------------------|
|<span data-ttu-id="81bd8-116">ID</span><span class="sxs-lookup"><span data-stu-id="81bd8-116">id</span></span>               |<span data-ttu-id="81bd8-117">GUID</span><span class="sxs-lookup"><span data-stu-id="81bd8-117">GUID</span></span>  |<span data-ttu-id="81bd8-118">会社の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="81bd8-118">The unique ID of the company.</span></span> <span data-ttu-id="81bd8-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="81bd8-119">Read-Only.</span></span>|
|<span data-ttu-id="81bd8-120">name</span><span class="sxs-lookup"><span data-stu-id="81bd8-120">name</span></span>             |<span data-ttu-id="81bd8-121">string</span><span class="sxs-lookup"><span data-stu-id="81bd8-121">string</span></span>|<span data-ttu-id="81bd8-122">会社を指定します。</span><span class="sxs-lookup"><span data-stu-id="81bd8-122">Specifies the Company.</span></span>                  |
|<span data-ttu-id="81bd8-123">displayName</span><span class="sxs-lookup"><span data-stu-id="81bd8-123">displayName</span></span>      |<span data-ttu-id="81bd8-124">string</span><span class="sxs-lookup"><span data-stu-id="81bd8-124">string</span></span>|<span data-ttu-id="81bd8-125">会社の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="81bd8-125">Specifies the company display name.</span></span>     |
|<span data-ttu-id="81bd8-126">systemversion</span><span class="sxs-lookup"><span data-stu-id="81bd8-126">systemVersion</span></span>    |<span data-ttu-id="81bd8-127">string</span><span class="sxs-lookup"><span data-stu-id="81bd8-127">string</span></span>|<span data-ttu-id="81bd8-128">会社の内部バージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="81bd8-128">Specifies the internal version of the company.</span></span>|
|<span data-ttu-id="81bd8-129">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="81bd8-129">businessProfileId</span></span>|<span data-ttu-id="81bd8-130">string</span><span class="sxs-lookup"><span data-stu-id="81bd8-130">string</span></span>|<span data-ttu-id="81bd8-131">会社にリンクされているビジネスプロファイル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="81bd8-131">Specifies the Business Profile ID linked to the company.</span></span>|


## <a name="relationships"></a><span data-ttu-id="81bd8-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="81bd8-132">Relationships</span></span>
<span data-ttu-id="81bd8-133">なし</span><span class="sxs-lookup"><span data-stu-id="81bd8-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81bd8-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81bd8-134">JSON representation</span></span>

<span data-ttu-id="81bd8-135">以下は、会社の JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="81bd8-135">Here is a JSON representation of the company.</span></span>

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


