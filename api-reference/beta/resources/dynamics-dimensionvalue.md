---
title: dimensionValues リソースの種類
description: Dynamics 365 Business Central の寸法値。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: af7ba3b49051a4e89fcdf2a4a408a1f72fc547ad
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973616"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="4322b-103">dimensionValues リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4322b-103">dimensionValues resource type</span></span>
<span data-ttu-id="4322b-104">Dynamics 365 Business Central のディメンション値を表します。</span><span class="sxs-lookup"><span data-stu-id="4322b-104">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="4322b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="4322b-105">Methods</span></span>

| <span data-ttu-id="4322b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4322b-106">Method</span></span>       | <span data-ttu-id="4322b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4322b-107">Return Type</span></span>  |<span data-ttu-id="4322b-108">説明</span><span class="sxs-lookup"><span data-stu-id="4322b-108">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="4322b-109">DimensionValues の値を取得する</span><span class="sxs-lookup"><span data-stu-id="4322b-109">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="4322b-110">dimensionValues</span><span class="sxs-lookup"><span data-stu-id="4322b-110">dimensionValues</span></span>|<span data-ttu-id="4322b-111">ディメンション値オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="4322b-111">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="4322b-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4322b-112">Properties</span></span>
| <span data-ttu-id="4322b-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4322b-113">Property</span></span>           | <span data-ttu-id="4322b-114">型</span><span class="sxs-lookup"><span data-stu-id="4322b-114">Type</span></span>                  |<span data-ttu-id="4322b-115">説明</span><span class="sxs-lookup"><span data-stu-id="4322b-115">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="4322b-116">id</span><span class="sxs-lookup"><span data-stu-id="4322b-116">id</span></span>                  |<span data-ttu-id="4322b-117">GUID</span><span class="sxs-lookup"><span data-stu-id="4322b-117">GUID</span></span>                   |<span data-ttu-id="4322b-118">アイテムの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="4322b-118">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="4322b-119">code</span><span class="sxs-lookup"><span data-stu-id="4322b-119">code</span></span>                |<span data-ttu-id="4322b-120">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="4322b-120">string, maximum size 20</span></span>|<span data-ttu-id="4322b-121">寸法値コード。</span><span class="sxs-lookup"><span data-stu-id="4322b-121">The dimension value code.</span></span>                          |
|<span data-ttu-id="4322b-122">displayName</span><span class="sxs-lookup"><span data-stu-id="4322b-122">displayName</span></span>         |<span data-ttu-id="4322b-123">string</span><span class="sxs-lookup"><span data-stu-id="4322b-123">string</span></span>                 |<span data-ttu-id="4322b-124">次元の値の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="4322b-124">Specifies the dimension value's name.</span></span> <span data-ttu-id="4322b-125">この名前は、ディメンション値が使用される場所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="4322b-125">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="4322b-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4322b-126">lastModifiedDateTime</span></span>|<span data-ttu-id="4322b-127">datetime</span><span class="sxs-lookup"><span data-stu-id="4322b-127">datetime</span></span>               |<span data-ttu-id="4322b-128">ディメンション値が変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="4322b-128">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="4322b-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4322b-129">JSON representation</span></span>

<span data-ttu-id="4322b-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4322b-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


