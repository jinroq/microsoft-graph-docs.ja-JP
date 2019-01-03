---
title: visualInfo リソースの種類
description: アクティビティ オブジェクトの**visualElements**プロパティを表すための複合型です。
ms.openlocfilehash: ac895e854051cb487fa9afd0ff9ada972b97aa19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070577"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="91aa6-103">visualInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91aa6-103">visualInfo resource type</span></span>

> <span data-ttu-id="91aa6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91aa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91aa6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91aa6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91aa6-106">[アクティビティ](../resources/projectrome-activity.md)オブジェクトの**visualElements**プロパティを表すための複合型です。</span><span class="sxs-lookup"><span data-stu-id="91aa6-106">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="91aa6-107">各ユーザーの利用状況は、アダプティブ ・ カードとしてタイムラインに表示されます。</span><span class="sxs-lookup"><span data-stu-id="91aa6-107">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="91aa6-108">アプリの開発者は、アプリケーションで行われた活動の本質をキャプチャするカスタム カードを提供することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="91aa6-108">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="91aa6-109">コンテンツのプロパティで、カスタム JSON カードを提供することで可能です。</span><span class="sxs-lookup"><span data-stu-id="91aa6-109">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="91aa6-110">アプリケーションだけでなく、適応型のカードを使用して visual メタデータは、コンテンツ メタデータ: データを含むを指定できます将来の再契約に新しい活動を提供するためにユーザーのアクティビティの推論を構築するために使用します。</span><span class="sxs-lookup"><span data-stu-id="91aa6-110">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="91aa6-111">Schema.org のコンテンツを記述するプロパティを利用している JSON オブジェクトを提供するアクティビティの contentInfo プロパティを使用して可能です。</span><span class="sxs-lookup"><span data-stu-id="91aa6-111">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="91aa6-112">カスタム カードが指定されていない場合、表示テキストと説明のプロパティを使用して単純なカードが生成されます。</span><span class="sxs-lookup"><span data-stu-id="91aa6-112">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="91aa6-113">カスタム カードはアプリ内での最適なコンテンツの紹介をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="91aa6-113">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="91aa6-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91aa6-114">Properties</span></span>

|<span data-ttu-id="91aa6-115">名前</span><span class="sxs-lookup"><span data-stu-id="91aa6-115">Name</span></span> | <span data-ttu-id="91aa6-116">型</span><span class="sxs-lookup"><span data-stu-id="91aa6-116">Type</span></span> | <span data-ttu-id="91aa6-117">説明</span><span class="sxs-lookup"><span data-stu-id="91aa6-117">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="91aa6-118">表示テキスト</span><span class="sxs-lookup"><span data-stu-id="91aa6-118">displayText</span></span> | <span data-ttu-id="91aa6-119">String</span><span class="sxs-lookup"><span data-stu-id="91aa6-119">String</span></span> | <span data-ttu-id="91aa6-120">必須。</span><span class="sxs-lookup"><span data-stu-id="91aa6-120">Required.</span></span> <span data-ttu-id="91aa6-121">ユーザーの一意のアクティビティ (たとえば、アクティビティがドキュメントの作成を参照する場所の場合の文書名) の説明文を短く</span><span class="sxs-lookup"><span data-stu-id="91aa6-121">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="91aa6-122">説明</span><span class="sxs-lookup"><span data-stu-id="91aa6-122">description</span></span> | <span data-ttu-id="91aa6-123">String</span><span class="sxs-lookup"><span data-stu-id="91aa6-123">String</span></span> | <span data-ttu-id="91aa6-124">省略可能。</span><span class="sxs-lookup"><span data-stu-id="91aa6-124">Optional.</span></span> <span data-ttu-id="91aa6-125">ユーザーの固有の活動の長いテキストの説明 (例: ドキュメントの名前、最初の文、またはメタデータ)</span><span class="sxs-lookup"><span data-stu-id="91aa6-125">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="91aa6-126">背景色</span><span class="sxs-lookup"><span data-stu-id="91aa6-126">backgroundColor</span></span> | <span data-ttu-id="91aa6-127">String</span><span class="sxs-lookup"><span data-stu-id="91aa6-127">String</span></span> | <span data-ttu-id="91aa6-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="91aa6-128">Optional.</span></span> <span data-ttu-id="91aa6-129">UI のアクティビティのアプリケーションのソースのブランド カラーでアクティビティを表示するために使用する背景色です。</span><span class="sxs-lookup"><span data-stu-id="91aa6-129">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="91aa6-130">有効な 16 進数の色をする必要があります。</span><span class="sxs-lookup"><span data-stu-id="91aa6-130">Must be a valid hex color</span></span>|
|<span data-ttu-id="91aa6-131">content</span><span class="sxs-lookup"><span data-stu-id="91aa6-131">content</span></span> | <span data-ttu-id="91aa6-132">JSON オブジェクトの型指定されていません。</span><span class="sxs-lookup"><span data-stu-id="91aa6-132">Untyped JSON object</span></span> | <span data-ttu-id="91aa6-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="91aa6-133">Optional.</span></span> <span data-ttu-id="91aa6-134">Windows シェル UI のアクティビティを表示するカスタムのコンテンツを提供するカスタムのデータを JSON オブジェクトの使用</span><span class="sxs-lookup"><span data-stu-id="91aa6-134">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="91aa6-135">属性</span><span class="sxs-lookup"><span data-stu-id="91aa6-135">attribution</span></span> | [<span data-ttu-id="91aa6-136">imageInfo</span><span class="sxs-lookup"><span data-stu-id="91aa6-136">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="91aa6-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="91aa6-137">Optional.</span></span> <span data-ttu-id="91aa6-138">JSON オブジェクトを使用してアクティビティを生成するアプリケーションを表すアイコンを表すために使用</span><span class="sxs-lookup"><span data-stu-id="91aa6-138">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91aa6-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91aa6-139">JSON Representation</span></span>

<span data-ttu-id="91aa6-140">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91aa6-140">The following is a JSON representation of the resource.</span></span>

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
    "@data.type": "microsoft.graph.visualInfo",
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
        "@data.type": "microsoft.graph.Json"
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