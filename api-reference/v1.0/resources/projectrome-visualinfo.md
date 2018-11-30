---
title: visualInfo リソースの種類
description: アクティビティ オブジェクトの**visualElements**プロパティを表すための複合型です。
ms.openlocfilehash: f77e25a7aad7d4357f6444fbdbd0f06a5cffd023
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022095"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="735cd-103">visualInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="735cd-103">visualInfo resource type</span></span>

<span data-ttu-id="735cd-104">[アクティビティ](../resources/projectrome-activity.md)オブジェクトの**visualElements**プロパティを表すための複合型です。</span><span class="sxs-lookup"><span data-stu-id="735cd-104">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="735cd-105">各ユーザーの利用状況は、アダプティブ ・ カードとしてタイムラインに表示されます。</span><span class="sxs-lookup"><span data-stu-id="735cd-105">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="735cd-106">アプリの開発者は、アプリケーションで行われた活動の本質をキャプチャするカスタム カードを提供することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="735cd-106">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="735cd-107">コンテンツのプロパティで、カスタム JSON カードを提供することで可能です。</span><span class="sxs-lookup"><span data-stu-id="735cd-107">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="735cd-108">アプリケーションだけでなく、適応型のカードを使用して visual メタデータは、コンテンツ メタデータ: データを含むを指定できます将来の再契約に新しい活動を提供するためにユーザーのアクティビティの推論を構築するために使用します。</span><span class="sxs-lookup"><span data-stu-id="735cd-108">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="735cd-109">Schema.org のコンテンツを記述するプロパティを利用している JSON オブジェクトを提供するアクティビティの contentInfo プロパティを使用して可能です。</span><span class="sxs-lookup"><span data-stu-id="735cd-109">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="735cd-110">カスタム カードが指定されていない場合、表示テキストと説明のプロパティを使用して単純なカードが生成されます。</span><span class="sxs-lookup"><span data-stu-id="735cd-110">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="735cd-111">カスタム カードはアプリ内での最適なコンテンツの紹介をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="735cd-111">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="735cd-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="735cd-112">Properties</span></span>

|<span data-ttu-id="735cd-113">名前</span><span class="sxs-lookup"><span data-stu-id="735cd-113">Name</span></span> | <span data-ttu-id="735cd-114">型</span><span class="sxs-lookup"><span data-stu-id="735cd-114">Type</span></span> | <span data-ttu-id="735cd-115">説明</span><span class="sxs-lookup"><span data-stu-id="735cd-115">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="735cd-116">表示テキスト</span><span class="sxs-lookup"><span data-stu-id="735cd-116">displayText</span></span> | <span data-ttu-id="735cd-117">String</span><span class="sxs-lookup"><span data-stu-id="735cd-117">String</span></span> | <span data-ttu-id="735cd-118">必須。</span><span class="sxs-lookup"><span data-stu-id="735cd-118">Required.</span></span> <span data-ttu-id="735cd-119">ユーザーの一意のアクティビティ (たとえば、アクティビティがドキュメントの作成を参照する場所の場合の文書名) の説明文を短く</span><span class="sxs-lookup"><span data-stu-id="735cd-119">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="735cd-120">説明</span><span class="sxs-lookup"><span data-stu-id="735cd-120">description</span></span> | <span data-ttu-id="735cd-121">String</span><span class="sxs-lookup"><span data-stu-id="735cd-121">String</span></span> | <span data-ttu-id="735cd-122">省略可能。</span><span class="sxs-lookup"><span data-stu-id="735cd-122">Optional.</span></span> <span data-ttu-id="735cd-123">ユーザーの固有の活動の長いテキストの説明 (例: ドキュメントの名前、最初の文、またはメタデータ)</span><span class="sxs-lookup"><span data-stu-id="735cd-123">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="735cd-124">背景色</span><span class="sxs-lookup"><span data-stu-id="735cd-124">backgroundColor</span></span> | <span data-ttu-id="735cd-125">String</span><span class="sxs-lookup"><span data-stu-id="735cd-125">String</span></span> | <span data-ttu-id="735cd-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="735cd-126">Optional.</span></span> <span data-ttu-id="735cd-127">UI のアクティビティのアプリケーションのソースのブランド カラーでアクティビティを表示するために使用する背景色です。</span><span class="sxs-lookup"><span data-stu-id="735cd-127">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="735cd-128">有効な 16 進数の色をする必要があります。</span><span class="sxs-lookup"><span data-stu-id="735cd-128">Must be a valid hex color</span></span>|
|<span data-ttu-id="735cd-129">content</span><span class="sxs-lookup"><span data-stu-id="735cd-129">content</span></span> | <span data-ttu-id="735cd-130">JSON オブジェクトの型指定されていません。</span><span class="sxs-lookup"><span data-stu-id="735cd-130">Untyped JSON object</span></span> | <span data-ttu-id="735cd-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="735cd-131">Optional.</span></span> <span data-ttu-id="735cd-132">Windows シェル UI のアクティビティを表示するカスタムのコンテンツを提供するカスタムのデータを JSON オブジェクトの使用</span><span class="sxs-lookup"><span data-stu-id="735cd-132">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="735cd-133">属性</span><span class="sxs-lookup"><span data-stu-id="735cd-133">attribution</span></span> | [<span data-ttu-id="735cd-134">imageInfo</span><span class="sxs-lookup"><span data-stu-id="735cd-134">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="735cd-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="735cd-135">Optional.</span></span> <span data-ttu-id="735cd-136">JSON オブジェクトを使用してアクティビティを生成するアプリケーションを表すアイコンを表すために使用</span><span class="sxs-lookup"><span data-stu-id="735cd-136">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="735cd-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="735cd-137">JSON Representation</span></span>

<span data-ttu-id="735cd-138">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="735cd-138">The following is a JSON representation of the resource.</span></span>

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
