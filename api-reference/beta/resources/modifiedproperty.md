---
title: modifiedProperty リソースの種類
description: Azure の AD の古い値とすべてのリソースの新しい値を持つすべての変更されたプロパティを示します
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844456"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="88229-103">modifiedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88229-103">modifiedProperty resource type</span></span>
<span data-ttu-id="88229-104">Azure の AD の古い値とすべてのリソースの新しい値を持つすべての変更されたプロパティを示します</span><span class="sxs-lookup"><span data-stu-id="88229-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="88229-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88229-105">Properties</span></span>
| <span data-ttu-id="88229-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88229-106">Property</span></span>     | <span data-ttu-id="88229-107">種類</span><span class="sxs-lookup"><span data-stu-id="88229-107">Type</span></span>   |<span data-ttu-id="88229-108">説明</span><span class="sxs-lookup"><span data-stu-id="88229-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88229-109">displayName</span><span class="sxs-lookup"><span data-stu-id="88229-109">displayName</span></span>|<span data-ttu-id="88229-110">String</span><span class="sxs-lookup"><span data-stu-id="88229-110">String</span></span>|<span data-ttu-id="88229-111">変更されたターゲットの属性のプロパティ名を示します。</span><span class="sxs-lookup"><span data-stu-id="88229-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="88229-112">newValue</span><span class="sxs-lookup"><span data-stu-id="88229-112">newValue</span></span>|<span data-ttu-id="88229-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="88229-113">String</span></span>|<span data-ttu-id="88229-114">これらの更新された値を示します。</span><span class="sxs-lookup"><span data-stu-id="88229-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="88229-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="88229-115">oldValue</span></span>|<span data-ttu-id="88229-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="88229-116">String</span></span>|<span data-ttu-id="88229-117">(更新) する前にプロパティの以前の値を示します。</span><span class="sxs-lookup"><span data-stu-id="88229-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88229-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88229-118">JSON representation</span></span>

<span data-ttu-id="88229-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="88229-119">Here is a JSON representation of the resource.</span></span>

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
