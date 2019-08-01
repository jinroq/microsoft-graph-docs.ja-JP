---
title: visualInfo リソースの種類
description: Activity オブジェクトの**Visualelements**プロパティを表すための複合型。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b26fba2e8ea29dab6f753de36e1c981f8e31c2f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035022"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="89f97-103">visualInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89f97-103">visualInfo resource type</span></span>

<span data-ttu-id="89f97-104">[Activity](../resources/projectrome-activity.md)オブジェクトの**visualelements**プロパティを表すための複合型。</span><span class="sxs-lookup"><span data-stu-id="89f97-104">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="89f97-105">各ユーザーアクティビティは、アダプティブカードとしてタイムラインに表示されます。</span><span class="sxs-lookup"><span data-stu-id="89f97-105">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="89f97-106">アプリ開発者は、アプリで行われたアクティビティの本質をキャプチャするカスタムカードを提供することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="89f97-106">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="89f97-107">これは、コンテンツプロパティにカスタム JSON カードを提供することによって可能になります。</span><span class="sxs-lookup"><span data-stu-id="89f97-107">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="89f97-108">アプリでは、アダプティブカードを使用したビジュアルメタデータに加えて、コンテンツメタデータを指定できます。これにより、ユーザーのアクティビティに対する推論を構築する際に使用されるデータが提供されます。</span><span class="sxs-lookup"><span data-stu-id="89f97-108">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="89f97-109">これは、アクティビティの contentInfo プロパティを使用して、コンテンツを説明するために schema.org プロパティを活用する JSON オブジェクトを提供することによって可能になります。</span><span class="sxs-lookup"><span data-stu-id="89f97-109">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="89f97-110">カスタムカードが提供されていない場合は、表示テキストと説明のプロパティを使用して、簡単なカードが生成されます。</span><span class="sxs-lookup"><span data-stu-id="89f97-110">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="89f97-111">カスタムカードは、アプリ内から最適なコンテンツを示すために推奨されています。</span><span class="sxs-lookup"><span data-stu-id="89f97-111">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="89f97-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89f97-112">Properties</span></span>

|<span data-ttu-id="89f97-113">名前</span><span class="sxs-lookup"><span data-stu-id="89f97-113">Name</span></span> | <span data-ttu-id="89f97-114">型</span><span class="sxs-lookup"><span data-stu-id="89f97-114">Type</span></span> | <span data-ttu-id="89f97-115">説明</span><span class="sxs-lookup"><span data-stu-id="89f97-115">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="89f97-116">テキスト</span><span class="sxs-lookup"><span data-stu-id="89f97-116">displayText</span></span> | <span data-ttu-id="89f97-117">String</span><span class="sxs-lookup"><span data-stu-id="89f97-117">String</span></span> | <span data-ttu-id="89f97-118">必須。</span><span class="sxs-lookup"><span data-stu-id="89f97-118">Required.</span></span> <span data-ttu-id="89f97-119">ユーザーの一意のアクティビティの短いテキスト説明 (たとえば、アクティビティがドキュメントの作成を参照する場合のドキュメント名)。</span><span class="sxs-lookup"><span data-stu-id="89f97-119">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="89f97-120">description</span><span class="sxs-lookup"><span data-stu-id="89f97-120">description</span></span> | <span data-ttu-id="89f97-121">String</span><span class="sxs-lookup"><span data-stu-id="89f97-121">String</span></span> | <span data-ttu-id="89f97-122">省略可能。</span><span class="sxs-lookup"><span data-stu-id="89f97-122">Optional.</span></span> <span data-ttu-id="89f97-123">ユーザー固有のアクティビティに関する長いテキストの説明 (例: ドキュメント名、最初の文、またはメタデータ)</span><span class="sxs-lookup"><span data-stu-id="89f97-123">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="89f97-124">背景</span><span class="sxs-lookup"><span data-stu-id="89f97-124">backgroundColor</span></span> | <span data-ttu-id="89f97-125">String</span><span class="sxs-lookup"><span data-stu-id="89f97-125">String</span></span> | <span data-ttu-id="89f97-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="89f97-126">Optional.</span></span> <span data-ttu-id="89f97-127">アクティビティのアプリケーションソースの UI ブランドカラーでアクティビティをレンダリングするために使用される背景色。</span><span class="sxs-lookup"><span data-stu-id="89f97-127">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="89f97-128">有効な16進カラーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="89f97-128">Must be a valid hex color</span></span>|
|<span data-ttu-id="89f97-129">content</span><span class="sxs-lookup"><span data-stu-id="89f97-129">content</span></span> | <span data-ttu-id="89f97-130">型指定のない JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="89f97-130">Untyped JSON object</span></span> | <span data-ttu-id="89f97-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="89f97-131">Optional.</span></span> <span data-ttu-id="89f97-132">Windows シェル UI でアクティビティをレンダリングするためにカスタムコンテンツを提供するために使用されるデータ JSON オブジェクトのカスタム部分</span><span class="sxs-lookup"><span data-stu-id="89f97-132">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="89f97-133">帰属</span><span class="sxs-lookup"><span data-stu-id="89f97-133">attribution</span></span> | [<span data-ttu-id="89f97-134">imageInfo</span><span class="sxs-lookup"><span data-stu-id="89f97-134">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="89f97-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="89f97-135">Optional.</span></span> <span data-ttu-id="89f97-136">アクティビティの生成に使用されたアプリケーションを表すアイコンを表すために使用される JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="89f97-136">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89f97-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89f97-137">JSON Representation</span></span>

<span data-ttu-id="89f97-138">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89f97-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
