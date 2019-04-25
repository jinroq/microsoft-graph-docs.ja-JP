---
title: dimensions リソースの種類
description: Dynamics 365 Business Central のディメンション。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 92ba48a7ad55b6a7dff28ccc1547769c149e378b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543089"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="91e87-103">Dimensions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91e87-103">Dimensions resource type</span></span>
<span data-ttu-id="91e87-104">Dynamics 365 Business Central のディメンションを表します。</span><span class="sxs-lookup"><span data-stu-id="91e87-104">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="91e87-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="91e87-105">Methods</span></span>
| <span data-ttu-id="91e87-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="91e87-106">Method</span></span>       | <span data-ttu-id="91e87-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="91e87-107">Return Type</span></span>  |<span data-ttu-id="91e87-108">説明</span><span class="sxs-lookup"><span data-stu-id="91e87-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="91e87-109">ディメンションを取得する</span><span class="sxs-lookup"><span data-stu-id="91e87-109">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="91e87-110">大きさ</span><span class="sxs-lookup"><span data-stu-id="91e87-110">dimension</span></span>|<span data-ttu-id="91e87-111">次元を取得します。</span><span class="sxs-lookup"><span data-stu-id="91e87-111">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="91e87-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91e87-112">Properties</span></span>
| <span data-ttu-id="91e87-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91e87-113">Property</span></span>           | <span data-ttu-id="91e87-114">型</span><span class="sxs-lookup"><span data-stu-id="91e87-114">Type</span></span>                  |<span data-ttu-id="91e87-115">説明</span><span class="sxs-lookup"><span data-stu-id="91e87-115">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="91e87-116">id</span><span class="sxs-lookup"><span data-stu-id="91e87-116">id</span></span>                  |<span data-ttu-id="91e87-117">GUID</span><span class="sxs-lookup"><span data-stu-id="91e87-117">GUID</span></span>                   |<span data-ttu-id="91e87-118">アイテムの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="91e87-118">The unique ID of the item.</span></span>|
|<span data-ttu-id="91e87-119">code</span><span class="sxs-lookup"><span data-stu-id="91e87-119">code</span></span>                |<span data-ttu-id="91e87-120">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="91e87-120">string, maximum size 20</span></span>|<span data-ttu-id="91e87-121">次元コード。</span><span class="sxs-lookup"><span data-stu-id="91e87-121">The dimension code.</span></span>       |
|<span data-ttu-id="91e87-122">displayName</span><span class="sxs-lookup"><span data-stu-id="91e87-122">displayName</span></span>         |<span data-ttu-id="91e87-123">string</span><span class="sxs-lookup"><span data-stu-id="91e87-123">string</span></span>                 |<span data-ttu-id="91e87-124">ディメンションの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="91e87-124">Specifies the dimension's name.</span></span> <span data-ttu-id="91e87-125">この名前は、ディメンションが使用される場所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="91e87-125">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="91e87-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91e87-126">lastModifiedDateTime</span></span>|<span data-ttu-id="91e87-127">datetime</span><span class="sxs-lookup"><span data-stu-id="91e87-127">datetime</span></span>               |<span data-ttu-id="91e87-128">ディメンションが変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="91e87-128">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="91e87-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91e87-129">JSON representation</span></span>

<span data-ttu-id="91e87-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91e87-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

