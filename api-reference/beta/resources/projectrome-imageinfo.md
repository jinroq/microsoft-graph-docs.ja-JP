---
title: imageInfo リソースの種類
description: Activity オブジェクトの visualInfo パーツの**属性**プロパティを表すための複合型。
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 53496734f79121edd010a429ec0a8da28b16e836
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008888"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="5a216-103">imageInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a216-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a216-104">[Activity](../resources/projectrome-activity.md)オブジェクトの[visualinfo](../resources/projectrome-visualinfo.md)パーツの**属性**プロパティを表すための複合型。</span><span class="sxs-lookup"><span data-stu-id="5a216-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="5a216-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a216-105">Properties</span></span>

|<span data-ttu-id="5a216-106">名前</span><span class="sxs-lookup"><span data-stu-id="5a216-106">Name</span></span> | <span data-ttu-id="5a216-107">型</span><span class="sxs-lookup"><span data-stu-id="5a216-107">Type</span></span> | <span data-ttu-id="5a216-108">説明</span><span class="sxs-lookup"><span data-stu-id="5a216-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="5a216-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="5a216-109">iconUrl</span></span> | <span data-ttu-id="5a216-110">String</span><span class="sxs-lookup"><span data-stu-id="5a216-110">String</span></span> | <span data-ttu-id="5a216-111">オプションアクティビティを生成するために使用されるアプリケーションを表すアイコンを指す URI。</span><span class="sxs-lookup"><span data-stu-id="5a216-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="5a216-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="5a216-112">alternateText</span></span> | <span data-ttu-id="5a216-113">String</span><span class="sxs-lookup"><span data-stu-id="5a216-113">String</span></span> | <span data-ttu-id="5a216-114">オプションalt キーを押しながら、画像にアクセスできるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="5a216-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="5a216-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="5a216-115">addImageQuery</span></span> | <span data-ttu-id="5a216-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a216-116">Boolean</span></span> | <span data-ttu-id="5a216-117">オプションパラメータパラメーターへの応答として、サーバーが画像を動的に表示できることを示すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="5a216-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="5a216-118">例-コントラストの高い画像</span><span class="sxs-lookup"><span data-stu-id="5a216-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a216-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a216-119">JSON Representation</span></span>

<span data-ttu-id="5a216-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="5a216-120">Here is a JSON representation of the resource</span></span>

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
