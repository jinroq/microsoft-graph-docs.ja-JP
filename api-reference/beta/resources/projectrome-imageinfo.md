---
title: imageInfo リソースの種類
description: アクティビティ オブジェクトの visualInfo の一部の**属性**のプロパティを表すための複合型です。
localization_priority: Normal
ms.openlocfilehash: 9df93e24c2019f246fc9da269b40ab690ae81aa4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828568"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="f03a4-103">imageInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f03a4-103">imageInfo resource type</span></span>

> <span data-ttu-id="f03a4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f03a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f03a4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f03a4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f03a4-106">[アクティビティ](../resources/projectrome-activity.md)オブジェクトの[visualInfo](../resources/projectrome-visualinfo.md)の一部の**属性**のプロパティを表すための複合型です。</span><span class="sxs-lookup"><span data-stu-id="f03a4-106">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="f03a4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f03a4-107">Properties</span></span>

|<span data-ttu-id="f03a4-108">名前</span><span class="sxs-lookup"><span data-stu-id="f03a4-108">Name</span></span> | <span data-ttu-id="f03a4-109">種類</span><span class="sxs-lookup"><span data-stu-id="f03a4-109">Type</span></span> | <span data-ttu-id="f03a4-110">説明</span><span class="sxs-lookup"><span data-stu-id="f03a4-110">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="f03a4-111">iconUrl</span><span class="sxs-lookup"><span data-stu-id="f03a4-111">iconUrl</span></span> | <span data-ttu-id="f03a4-112">String</span><span class="sxs-lookup"><span data-stu-id="f03a4-112">String</span></span> | <span data-ttu-id="f03a4-113">省略可能です。活動を生成するために使用するアプリケーションを表すアイコンをポイントする URI</span><span class="sxs-lookup"><span data-stu-id="f03a4-113">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="f03a4-114">alternateText</span><span class="sxs-lookup"><span data-stu-id="f03a4-114">alternateText</span></span> | <span data-ttu-id="f03a4-115">String</span><span class="sxs-lookup"><span data-stu-id="f03a4-115">String</span></span> | <span data-ttu-id="f03a4-116">省略可能です。イメージの alt テキストのアクセス可能なコンテンツ</span><span class="sxs-lookup"><span data-stu-id="f03a4-116">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="f03a4-117">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="f03a4-117">addImageQuery</span></span> | <span data-ttu-id="f03a4-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="f03a4-118">Boolean</span></span> | <span data-ttu-id="f03a4-119">省略可能です。サーバーを指定するためのパラメーターは、パラメーターへの応答に動的にイメージをレンダリングすることです。</span><span class="sxs-lookup"><span data-stu-id="f03a4-119">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="f03a4-120">例: ハイコントラスト イメージ</span><span class="sxs-lookup"><span data-stu-id="f03a4-120">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f03a4-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f03a4-121">JSON Representation</span></span>

<span data-ttu-id="f03a4-122">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f03a4-122">Here is a JSON representation of the resource</span></span>

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
