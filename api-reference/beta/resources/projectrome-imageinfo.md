---
title: imageInfo リソースの種類
description: activity オブジェクトの visualinfo パーツの**属性**プロパティを表すための複合型。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 6ffdacefb11f583f8c9529a36472a01537643c3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344010"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="95c73-103">imageInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95c73-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95c73-104">[activity](../resources/projectrome-activity.md)オブジェクトの[visualinfo](../resources/projectrome-visualinfo.md)パーツの**属性**プロパティを表すための複合型。</span><span class="sxs-lookup"><span data-stu-id="95c73-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="95c73-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95c73-105">Properties</span></span>

|<span data-ttu-id="95c73-106">名前</span><span class="sxs-lookup"><span data-stu-id="95c73-106">Name</span></span> | <span data-ttu-id="95c73-107">型</span><span class="sxs-lookup"><span data-stu-id="95c73-107">Type</span></span> | <span data-ttu-id="95c73-108">説明</span><span class="sxs-lookup"><span data-stu-id="95c73-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="95c73-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="95c73-109">iconUrl</span></span> | <span data-ttu-id="95c73-110">String</span><span class="sxs-lookup"><span data-stu-id="95c73-110">String</span></span> | <span data-ttu-id="95c73-111">オプションアクティビティを生成するために使用されるアプリケーションを表すアイコンを指す URI。</span><span class="sxs-lookup"><span data-stu-id="95c73-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="95c73-112">alternatetext</span><span class="sxs-lookup"><span data-stu-id="95c73-112">alternateText</span></span> | <span data-ttu-id="95c73-113">String</span><span class="sxs-lookup"><span data-stu-id="95c73-113">String</span></span> | <span data-ttu-id="95c73-114">オプションalt キーを押しながら、画像にアクセスできるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="95c73-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="95c73-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="95c73-115">addImageQuery</span></span> | <span data-ttu-id="95c73-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="95c73-116">Boolean</span></span> | <span data-ttu-id="95c73-117">オプションパラメータパラメーターへの応答として、サーバーが画像を動的に表示できることを示すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="95c73-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="95c73-118">例-コントラストの高い画像</span><span class="sxs-lookup"><span data-stu-id="95c73-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95c73-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95c73-119">JSON Representation</span></span>

<span data-ttu-id="95c73-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="95c73-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
