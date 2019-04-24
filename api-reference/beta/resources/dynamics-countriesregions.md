---
title: countriesRegions リソースの種類
description: Dynamics 365 Business Central の国/地域オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: b6f50ba3046a402f2b8729529675653286808459
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507267"
---
# <a name="countriesregions-resource-type"></a><span data-ttu-id="fa67a-103">countriesRegions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa67a-103">countriesRegions resource type</span></span>
<span data-ttu-id="fa67a-104">countriesRegions オブジェクトを Dynamics 365 Business Central で表します。これは、アドレスの一部です。</span><span class="sxs-lookup"><span data-stu-id="fa67a-104">Represents a countriesRegions object in Dynamics 365 Business Central, which is part of an address.</span></span>

## <a name="methods"></a><span data-ttu-id="fa67a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="fa67a-105">Methods</span></span>

| <span data-ttu-id="fa67a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="fa67a-106">Method</span></span>                                                              | <span data-ttu-id="fa67a-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fa67a-107">Return Type</span></span>    |<span data-ttu-id="fa67a-108">説明</span><span class="sxs-lookup"><span data-stu-id="fa67a-108">Description</span></span>                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[<span data-ttu-id="fa67a-109">countriesRegions を取得する</span><span class="sxs-lookup"><span data-stu-id="fa67a-109">Get countriesRegions</span></span>](../api/dynamics-countriesregions-get.md)      |<span data-ttu-id="fa67a-110">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="fa67a-110">countriesRegions</span></span>|<span data-ttu-id="fa67a-111">国/地域を取得します。</span><span class="sxs-lookup"><span data-stu-id="fa67a-111">Get a Countries/Regions.</span></span>   |
|[<span data-ttu-id="fa67a-112">Post countriesRegions</span><span class="sxs-lookup"><span data-stu-id="fa67a-112">Post countriesRegions</span></span>](../api/dynamics-create-countriesregions.md)  |<span data-ttu-id="fa67a-113">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="fa67a-113">countriesRegions</span></span>|<span data-ttu-id="fa67a-114">国/地域を作成します。</span><span class="sxs-lookup"><span data-stu-id="fa67a-114">Create a Countries/Regions.</span></span>|
|[<span data-ttu-id="fa67a-115">Patch countriesRegions</span><span class="sxs-lookup"><span data-stu-id="fa67a-115">Patch countriesRegions</span></span>](../api/dynamics-countriesregions-update.md) |<span data-ttu-id="fa67a-116">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="fa67a-116">countriesRegions</span></span>|<span data-ttu-id="fa67a-117">国/地域を更新します。</span><span class="sxs-lookup"><span data-stu-id="fa67a-117">Update a Countries/Regions.</span></span>|
|[<span data-ttu-id="fa67a-118">countriesRegions の削除</span><span class="sxs-lookup"><span data-stu-id="fa67a-118">Delete countriesRegions</span></span>](../api/dynamics-countriesregions-delete.md)|<span data-ttu-id="fa67a-119">なし</span><span class="sxs-lookup"><span data-stu-id="fa67a-119">none</span></span>            |<span data-ttu-id="fa67a-120">国/地域を削除します。</span><span class="sxs-lookup"><span data-stu-id="fa67a-120">Delete a Countries/Regions.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa67a-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa67a-121">Properties</span></span>
| <span data-ttu-id="fa67a-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa67a-122">Property</span></span>       | <span data-ttu-id="fa67a-123">型</span><span class="sxs-lookup"><span data-stu-id="fa67a-123">Type</span></span>       |<span data-ttu-id="fa67a-124">説明</span><span class="sxs-lookup"><span data-stu-id="fa67a-124">Description</span></span>                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|<span data-ttu-id="fa67a-125">id</span><span class="sxs-lookup"><span data-stu-id="fa67a-125">id</span></span>              |<span data-ttu-id="fa67a-126">GUID</span><span class="sxs-lookup"><span data-stu-id="fa67a-126">GUID</span></span>        |<span data-ttu-id="fa67a-127">国/地域の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="fa67a-127">The unique ID of the country/region.</span></span> <span data-ttu-id="fa67a-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="fa67a-128">Non-editable.</span></span>           |
|<span data-ttu-id="fa67a-129">code</span><span class="sxs-lookup"><span data-stu-id="fa67a-129">code</span></span>            |<span data-ttu-id="fa67a-130">string</span><span class="sxs-lookup"><span data-stu-id="fa67a-130">string</span></span>      |<span data-ttu-id="fa67a-131">国/地域のコードを指定します。</span><span class="sxs-lookup"><span data-stu-id="fa67a-131">Specifies the code of the country/region.</span></span>                    |
|<span data-ttu-id="fa67a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fa67a-132">displayName</span></span>     |<span data-ttu-id="fa67a-133">string</span><span class="sxs-lookup"><span data-stu-id="fa67a-133">string</span></span>      |<span data-ttu-id="fa67a-134">国/地域の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa67a-134">Specifies the display name of the country/region.</span></span>            |
|<span data-ttu-id="fa67a-135">addressformat</span><span class="sxs-lookup"><span data-stu-id="fa67a-135">addressFormat</span></span>   |<span data-ttu-id="fa67a-136">string</span><span class="sxs-lookup"><span data-stu-id="fa67a-136">string</span></span>      |<span data-ttu-id="fa67a-137">外部向けドキュメントに表示されるアドレスの形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa67a-137">Specifies the format of the address that is displayed on external-facing documents.</span></span> <span data-ttu-id="fa67a-138">住所形式を国/地域コードにリンクして、その国/地域コードを含むカードまたはドキュメントに基づく外部向けのドキュメントで、指定されたアドレス形式を使用するようにします。</span><span class="sxs-lookup"><span data-stu-id="fa67a-138">You link an address format to a country/region code so that external-facing documents based on cards or documents with that country/region code use the specified address format.</span></span>|
|<span data-ttu-id="fa67a-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa67a-139">lastModifiedDateTime</span></span>|<span data-ttu-id="fa67a-140">datetime</span><span class="sxs-lookup"><span data-stu-id="fa67a-140">datetime</span></span>|<span data-ttu-id="fa67a-141">国/地域が変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="fa67a-141">The last datetime the country/region was modified.</span></span> <span data-ttu-id="fa67a-142">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="fa67a-142">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="fa67a-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fa67a-143">Relationships</span></span>
<span data-ttu-id="fa67a-144">なし</span><span class="sxs-lookup"><span data-stu-id="fa67a-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa67a-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa67a-145">JSON representation</span></span>

<span data-ttu-id="fa67a-146">countriesRegions の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa67a-146">Here is a JSON representation of the countriesRegions.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```


