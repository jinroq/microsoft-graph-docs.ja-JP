---
title: dimensionvalues リソースの種類
description: Dynamics 365 Business Central の寸法値。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365319"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="0fcbe-103">dimensionvalues リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0fcbe-103">dimensionValues resource type</span></span>
<span data-ttu-id="0fcbe-104">Dynamics 365 Business Central のディメンション値を表します。</span><span class="sxs-lookup"><span data-stu-id="0fcbe-104">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="0fcbe-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0fcbe-105">Methods</span></span>

| <span data-ttu-id="0fcbe-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0fcbe-106">Method</span></span>       | <span data-ttu-id="0fcbe-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0fcbe-107">Return Type</span></span>  |<span data-ttu-id="0fcbe-108">説明</span><span class="sxs-lookup"><span data-stu-id="0fcbe-108">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="0fcbe-109">dimensionvalues の値を取得する</span><span class="sxs-lookup"><span data-stu-id="0fcbe-109">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="0fcbe-110">dimensionvalues</span><span class="sxs-lookup"><span data-stu-id="0fcbe-110">dimensionValues</span></span>|<span data-ttu-id="0fcbe-111">ディメンション値オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="0fcbe-111">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="0fcbe-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fcbe-112">Properties</span></span>
| <span data-ttu-id="0fcbe-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fcbe-113">Property</span></span>           | <span data-ttu-id="0fcbe-114">型</span><span class="sxs-lookup"><span data-stu-id="0fcbe-114">Type</span></span>                  |<span data-ttu-id="0fcbe-115">説明</span><span class="sxs-lookup"><span data-stu-id="0fcbe-115">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="0fcbe-116">ID</span><span class="sxs-lookup"><span data-stu-id="0fcbe-116">id</span></span>                  |<span data-ttu-id="0fcbe-117">GUID</span><span class="sxs-lookup"><span data-stu-id="0fcbe-117">GUID</span></span>                   |<span data-ttu-id="0fcbe-118">アイテムの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="0fcbe-118">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="0fcbe-119">code</span><span class="sxs-lookup"><span data-stu-id="0fcbe-119">code</span></span>                |<span data-ttu-id="0fcbe-120">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="0fcbe-120">string, maximum size 20</span></span>|<span data-ttu-id="0fcbe-121">寸法値コード。</span><span class="sxs-lookup"><span data-stu-id="0fcbe-121">The dimension value code.</span></span>                          |
|<span data-ttu-id="0fcbe-122">displayName</span><span class="sxs-lookup"><span data-stu-id="0fcbe-122">displayName</span></span>         |<span data-ttu-id="0fcbe-123">string</span><span class="sxs-lookup"><span data-stu-id="0fcbe-123">string</span></span>                 |<span data-ttu-id="0fcbe-124">次元の値の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="0fcbe-124">Specifies the dimension value's name.</span></span> <span data-ttu-id="0fcbe-125">この名前は、ディメンション値が使用される場所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="0fcbe-125">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="0fcbe-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fcbe-126">lastModifiedDateTime</span></span>|<span data-ttu-id="0fcbe-127">datetime</span><span class="sxs-lookup"><span data-stu-id="0fcbe-127">datetime</span></span>               |<span data-ttu-id="0fcbe-128">ディメンション値が変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="0fcbe-128">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="0fcbe-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0fcbe-129">JSON representation</span></span>

<span data-ttu-id="0fcbe-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0fcbe-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


