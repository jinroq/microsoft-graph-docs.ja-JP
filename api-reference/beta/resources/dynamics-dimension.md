---
title: dimensions リソースの種類
description: Dynamics 365 Business Central のディメンション。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 5bd5382ae020baaf726db53f9252c4d3498833ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973626"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="36b66-103">Dimensions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="36b66-103">Dimensions resource type</span></span>
<span data-ttu-id="36b66-104">Dynamics 365 Business Central のディメンションを表します。</span><span class="sxs-lookup"><span data-stu-id="36b66-104">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="36b66-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="36b66-105">Methods</span></span>
| <span data-ttu-id="36b66-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="36b66-106">Method</span></span>       | <span data-ttu-id="36b66-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="36b66-107">Return Type</span></span>  |<span data-ttu-id="36b66-108">説明</span><span class="sxs-lookup"><span data-stu-id="36b66-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="36b66-109">ディメンションを取得する</span><span class="sxs-lookup"><span data-stu-id="36b66-109">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="36b66-110">大きさ</span><span class="sxs-lookup"><span data-stu-id="36b66-110">dimension</span></span>|<span data-ttu-id="36b66-111">次元を取得します。</span><span class="sxs-lookup"><span data-stu-id="36b66-111">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="36b66-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36b66-112">Properties</span></span>
| <span data-ttu-id="36b66-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36b66-113">Property</span></span>           | <span data-ttu-id="36b66-114">型</span><span class="sxs-lookup"><span data-stu-id="36b66-114">Type</span></span>                  |<span data-ttu-id="36b66-115">説明</span><span class="sxs-lookup"><span data-stu-id="36b66-115">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="36b66-116">id</span><span class="sxs-lookup"><span data-stu-id="36b66-116">id</span></span>                  |<span data-ttu-id="36b66-117">GUID</span><span class="sxs-lookup"><span data-stu-id="36b66-117">GUID</span></span>                   |<span data-ttu-id="36b66-118">アイテムの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="36b66-118">The unique ID of the item.</span></span>|
|<span data-ttu-id="36b66-119">code</span><span class="sxs-lookup"><span data-stu-id="36b66-119">code</span></span>                |<span data-ttu-id="36b66-120">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="36b66-120">string, maximum size 20</span></span>|<span data-ttu-id="36b66-121">次元コード。</span><span class="sxs-lookup"><span data-stu-id="36b66-121">The dimension code.</span></span>       |
|<span data-ttu-id="36b66-122">displayName</span><span class="sxs-lookup"><span data-stu-id="36b66-122">displayName</span></span>         |<span data-ttu-id="36b66-123">string</span><span class="sxs-lookup"><span data-stu-id="36b66-123">string</span></span>                 |<span data-ttu-id="36b66-124">ディメンションの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="36b66-124">Specifies the dimension's name.</span></span> <span data-ttu-id="36b66-125">この名前は、ディメンションが使用される場所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="36b66-125">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="36b66-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36b66-126">lastModifiedDateTime</span></span>|<span data-ttu-id="36b66-127">datetime</span><span class="sxs-lookup"><span data-stu-id="36b66-127">datetime</span></span>               |<span data-ttu-id="36b66-128">ディメンションが変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="36b66-128">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="36b66-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="36b66-129">JSON representation</span></span>

<span data-ttu-id="36b66-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="36b66-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

