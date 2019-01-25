---
title: imageInfo リソースの種類
description: アクティビティ オブジェクトの visualInfo の一部の**属性**のプロパティを表すための複合型です。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 112b1dc3d1db45f3fe470c1c21d483b09c00202c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514916"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="5d4da-103">imageInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5d4da-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d4da-104">[アクティビティ](../resources/projectrome-activity.md)オブジェクトの[visualInfo](../resources/projectrome-visualinfo.md)の一部の**属性**のプロパティを表すための複合型です。</span><span class="sxs-lookup"><span data-stu-id="5d4da-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="5d4da-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d4da-105">Properties</span></span>

|<span data-ttu-id="5d4da-106">名前</span><span class="sxs-lookup"><span data-stu-id="5d4da-106">Name</span></span> | <span data-ttu-id="5d4da-107">型</span><span class="sxs-lookup"><span data-stu-id="5d4da-107">Type</span></span> | <span data-ttu-id="5d4da-108">説明</span><span class="sxs-lookup"><span data-stu-id="5d4da-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="5d4da-109">IconUrl</span><span class="sxs-lookup"><span data-stu-id="5d4da-109">iconUrl</span></span> | <span data-ttu-id="5d4da-110">String</span><span class="sxs-lookup"><span data-stu-id="5d4da-110">String</span></span> | <span data-ttu-id="5d4da-111">省略可能です。活動を生成するために使用するアプリケーションを表すアイコンをポイントする URI</span><span class="sxs-lookup"><span data-stu-id="5d4da-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="5d4da-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="5d4da-112">alternateText</span></span> | <span data-ttu-id="5d4da-113">String</span><span class="sxs-lookup"><span data-stu-id="5d4da-113">String</span></span> | <span data-ttu-id="5d4da-114">省略可能です。イメージの alt テキストのアクセス可能なコンテンツ</span><span class="sxs-lookup"><span data-stu-id="5d4da-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="5d4da-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="5d4da-115">addImageQuery</span></span> | <span data-ttu-id="5d4da-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="5d4da-116">Boolean</span></span> | <span data-ttu-id="5d4da-117">省略可能です。サーバーを指定するためのパラメーターは、パラメーターへの応答に動的にイメージをレンダリングすることです。</span><span class="sxs-lookup"><span data-stu-id="5d4da-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="5d4da-118">例: ハイコントラスト イメージ</span><span class="sxs-lookup"><span data-stu-id="5d4da-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d4da-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5d4da-119">JSON Representation</span></span>

<span data-ttu-id="5d4da-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="5d4da-120">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-imageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
