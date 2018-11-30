---
title: imageInfo リソースの種類
description: アクティビティ オブジェクトの visualInfo の一部の**属性**のプロパティを表すための複合型です。
ms.openlocfilehash: 051338230850da7e754c5e8ad4f7d9c52fe17b32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023140"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="0c397-103">imageInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c397-103">imageInfo resource type</span></span>

<span data-ttu-id="0c397-104">[アクティビティ](../resources/projectrome-activity.md)オブジェクトの[visualInfo](../resources/projectrome-visualinfo.md)の一部の**属性**のプロパティを表すための複合型です。</span><span class="sxs-lookup"><span data-stu-id="0c397-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="0c397-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c397-105">Properties</span></span>

|<span data-ttu-id="0c397-106">名前</span><span class="sxs-lookup"><span data-stu-id="0c397-106">Name</span></span> | <span data-ttu-id="0c397-107">型</span><span class="sxs-lookup"><span data-stu-id="0c397-107">Type</span></span> | <span data-ttu-id="0c397-108">説明</span><span class="sxs-lookup"><span data-stu-id="0c397-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="0c397-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="0c397-109">iconUrl</span></span> | <span data-ttu-id="0c397-110">String</span><span class="sxs-lookup"><span data-stu-id="0c397-110">String</span></span> | <span data-ttu-id="0c397-111">省略可能です。活動を生成するために使用するアプリケーションを表すアイコンをポイントする URI</span><span class="sxs-lookup"><span data-stu-id="0c397-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="0c397-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="0c397-112">alternateText</span></span> | <span data-ttu-id="0c397-113">String</span><span class="sxs-lookup"><span data-stu-id="0c397-113">String</span></span> | <span data-ttu-id="0c397-114">省略可能です。イメージの alt テキストのアクセス可能なコンテンツ</span><span class="sxs-lookup"><span data-stu-id="0c397-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="0c397-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="0c397-115">addImageQuery</span></span> | <span data-ttu-id="0c397-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="0c397-116">Boolean</span></span> | <span data-ttu-id="0c397-117">省略可能です。サーバーを指定するためのパラメーターは、パラメーターへの応答に動的にイメージをレンダリングすることです。</span><span class="sxs-lookup"><span data-stu-id="0c397-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="0c397-118">例: ハイコントラスト イメージ</span><span class="sxs-lookup"><span data-stu-id="0c397-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c397-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c397-119">JSON Representation</span></span>

<span data-ttu-id="0c397-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0c397-120">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->