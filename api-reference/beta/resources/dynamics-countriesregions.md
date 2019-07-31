---
title: countriesRegions リソースの種類
description: Dynamics 365 Business Central の国/地域オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 73f60a48e1b7b3564851271209e195ecbbf171e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012633"
---
# <a name="countriesregions-resource-type"></a><span data-ttu-id="88fd0-103">countriesRegions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88fd0-103">countriesRegions resource type</span></span>
<span data-ttu-id="88fd0-104">CountriesRegions オブジェクトを Dynamics 365 Business Central で表します。これは、アドレスの一部です。</span><span class="sxs-lookup"><span data-stu-id="88fd0-104">Represents a countriesRegions object in Dynamics 365 Business Central, which is part of an address.</span></span>

## <a name="methods"></a><span data-ttu-id="88fd0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="88fd0-105">Methods</span></span>

| <span data-ttu-id="88fd0-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="88fd0-106">Method</span></span>                                                              | <span data-ttu-id="88fd0-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="88fd0-107">Return Type</span></span>    |<span data-ttu-id="88fd0-108">説明</span><span class="sxs-lookup"><span data-stu-id="88fd0-108">Description</span></span>                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[<span data-ttu-id="88fd0-109">CountriesRegions を取得する</span><span class="sxs-lookup"><span data-stu-id="88fd0-109">Get countriesRegions</span></span>](../api/dynamics-countriesregions-get.md)      |<span data-ttu-id="88fd0-110">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="88fd0-110">countriesRegions</span></span>|<span data-ttu-id="88fd0-111">国/地域を取得します。</span><span class="sxs-lookup"><span data-stu-id="88fd0-111">Get a Countries/Regions.</span></span>   |
|[<span data-ttu-id="88fd0-112">Post countriesRegions</span><span class="sxs-lookup"><span data-stu-id="88fd0-112">Post countriesRegions</span></span>](../api/dynamics-create-countriesregions.md)  |<span data-ttu-id="88fd0-113">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="88fd0-113">countriesRegions</span></span>|<span data-ttu-id="88fd0-114">国/地域を作成します。</span><span class="sxs-lookup"><span data-stu-id="88fd0-114">Create a Countries/Regions.</span></span>|
|[<span data-ttu-id="88fd0-115">Patch countriesRegions</span><span class="sxs-lookup"><span data-stu-id="88fd0-115">Patch countriesRegions</span></span>](../api/dynamics-countriesregions-update.md) |<span data-ttu-id="88fd0-116">countriesRegions</span><span class="sxs-lookup"><span data-stu-id="88fd0-116">countriesRegions</span></span>|<span data-ttu-id="88fd0-117">国/地域を更新します。</span><span class="sxs-lookup"><span data-stu-id="88fd0-117">Update a Countries/Regions.</span></span>|
|[<span data-ttu-id="88fd0-118">CountriesRegions の削除</span><span class="sxs-lookup"><span data-stu-id="88fd0-118">Delete countriesRegions</span></span>](../api/dynamics-countriesregions-delete.md)|<span data-ttu-id="88fd0-119">none</span><span class="sxs-lookup"><span data-stu-id="88fd0-119">none</span></span>            |<span data-ttu-id="88fd0-120">国/地域を削除します。</span><span class="sxs-lookup"><span data-stu-id="88fd0-120">Delete a Countries/Regions.</span></span>|

## <a name="properties"></a><span data-ttu-id="88fd0-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88fd0-121">Properties</span></span>
| <span data-ttu-id="88fd0-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88fd0-122">Property</span></span>       | <span data-ttu-id="88fd0-123">型</span><span class="sxs-lookup"><span data-stu-id="88fd0-123">Type</span></span>       |<span data-ttu-id="88fd0-124">説明</span><span class="sxs-lookup"><span data-stu-id="88fd0-124">Description</span></span>                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|<span data-ttu-id="88fd0-125">id</span><span class="sxs-lookup"><span data-stu-id="88fd0-125">id</span></span>              |<span data-ttu-id="88fd0-126">GUID</span><span class="sxs-lookup"><span data-stu-id="88fd0-126">GUID</span></span>        |<span data-ttu-id="88fd0-127">国/地域の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="88fd0-127">The unique ID of the country/region.</span></span> <span data-ttu-id="88fd0-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="88fd0-128">Non-editable.</span></span>           |
|<span data-ttu-id="88fd0-129">code</span><span class="sxs-lookup"><span data-stu-id="88fd0-129">code</span></span>            |<span data-ttu-id="88fd0-130">string</span><span class="sxs-lookup"><span data-stu-id="88fd0-130">string</span></span>      |<span data-ttu-id="88fd0-131">国/地域のコードを指定します。</span><span class="sxs-lookup"><span data-stu-id="88fd0-131">Specifies the code of the country/region.</span></span>                    |
|<span data-ttu-id="88fd0-132">displayName</span><span class="sxs-lookup"><span data-stu-id="88fd0-132">displayName</span></span>     |<span data-ttu-id="88fd0-133">string</span><span class="sxs-lookup"><span data-stu-id="88fd0-133">string</span></span>      |<span data-ttu-id="88fd0-134">国/地域の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="88fd0-134">Specifies the display name of the country/region.</span></span>            |
|<span data-ttu-id="88fd0-135">addressFormat</span><span class="sxs-lookup"><span data-stu-id="88fd0-135">addressFormat</span></span>   |<span data-ttu-id="88fd0-136">string</span><span class="sxs-lookup"><span data-stu-id="88fd0-136">string</span></span>      |<span data-ttu-id="88fd0-137">外部向けドキュメントに表示されるアドレスの形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="88fd0-137">Specifies the format of the address that is displayed on external-facing documents.</span></span> <span data-ttu-id="88fd0-138">住所形式を国/地域コードにリンクして、その国/地域コードを含むカードまたはドキュメントに基づく外部向けのドキュメントで、指定されたアドレス形式を使用するようにします。</span><span class="sxs-lookup"><span data-stu-id="88fd0-138">You link an address format to a country/region code so that external-facing documents based on cards or documents with that country/region code use the specified address format.</span></span>|
|<span data-ttu-id="88fd0-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88fd0-139">lastModifiedDateTime</span></span>|<span data-ttu-id="88fd0-140">datetime</span><span class="sxs-lookup"><span data-stu-id="88fd0-140">datetime</span></span>|<span data-ttu-id="88fd0-141">国/地域が変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="88fd0-141">The last datetime the country/region was modified.</span></span> <span data-ttu-id="88fd0-142">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="88fd0-142">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="88fd0-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="88fd0-143">Relationships</span></span>
<span data-ttu-id="88fd0-144">なし</span><span class="sxs-lookup"><span data-stu-id="88fd0-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88fd0-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88fd0-145">JSON representation</span></span>

<span data-ttu-id="88fd0-146">CountriesRegions の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="88fd0-146">Here is a JSON representation of the countriesRegions.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```


