---
title: modifiedProperty リソースの種類
description: Azure の AD の古い値とすべてのリソースの新しい値を持つすべての変更されたプロパティを示します
ms.openlocfilehash: c504969ee12798969aa39490e79cb5b60bdb5435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069103"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="877ad-103">modifiedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="877ad-103">modifiedProperty resource type</span></span>
<span data-ttu-id="877ad-104">Azure の AD の古い値とすべてのリソースの新しい値を持つすべての変更されたプロパティを示します</span><span class="sxs-lookup"><span data-stu-id="877ad-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="877ad-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="877ad-105">Properties</span></span>
| <span data-ttu-id="877ad-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="877ad-106">Property</span></span>     | <span data-ttu-id="877ad-107">型</span><span class="sxs-lookup"><span data-stu-id="877ad-107">Type</span></span>   |<span data-ttu-id="877ad-108">説明</span><span class="sxs-lookup"><span data-stu-id="877ad-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="877ad-109">displayName</span><span class="sxs-lookup"><span data-stu-id="877ad-109">displayName</span></span>|<span data-ttu-id="877ad-110">String</span><span class="sxs-lookup"><span data-stu-id="877ad-110">String</span></span>|<span data-ttu-id="877ad-111">変更されたターゲットの属性のプロパティ名を示します。</span><span class="sxs-lookup"><span data-stu-id="877ad-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="877ad-112">newValue</span><span class="sxs-lookup"><span data-stu-id="877ad-112">newValue</span></span>|<span data-ttu-id="877ad-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="877ad-113">String</span></span>|<span data-ttu-id="877ad-114">これらの更新された値を示します。</span><span class="sxs-lookup"><span data-stu-id="877ad-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="877ad-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="877ad-115">oldValue</span></span>|<span data-ttu-id="877ad-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="877ad-116">String</span></span>|<span data-ttu-id="877ad-117">(更新) する前にプロパティの以前の値を示します。</span><span class="sxs-lookup"><span data-stu-id="877ad-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="877ad-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="877ad-118">JSON representation</span></span>

<span data-ttu-id="877ad-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="877ad-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->