---
title: modifiedProperty リソースの種類
description: 変更された Azure AD のリソースについて、古い値と新しい値を持つすべての変更されたプロパティを示します。
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506237"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="09df1-103">modifiedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09df1-103">modifiedProperty resource type</span></span>
<span data-ttu-id="09df1-104">変更された Azure AD のリソースについて、古い値と新しい値を持つすべての変更されたプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="09df1-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="09df1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09df1-105">Properties</span></span>
| <span data-ttu-id="09df1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09df1-106">Property</span></span>     | <span data-ttu-id="09df1-107">型</span><span class="sxs-lookup"><span data-stu-id="09df1-107">Type</span></span>   |<span data-ttu-id="09df1-108">説明</span><span class="sxs-lookup"><span data-stu-id="09df1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09df1-109">displayName</span><span class="sxs-lookup"><span data-stu-id="09df1-109">displayName</span></span>|<span data-ttu-id="09df1-110">String</span><span class="sxs-lookup"><span data-stu-id="09df1-110">String</span></span>|<span data-ttu-id="09df1-111">変更されたターゲット属性のプロパティ名を示します。</span><span class="sxs-lookup"><span data-stu-id="09df1-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="09df1-112">newValue</span><span class="sxs-lookup"><span data-stu-id="09df1-112">newValue</span></span>|<span data-ttu-id="09df1-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="09df1-113">String</span></span>|<span data-ttu-id="09df1-114">これらの更新された値を示します。</span><span class="sxs-lookup"><span data-stu-id="09df1-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="09df1-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="09df1-115">oldValue</span></span>|<span data-ttu-id="09df1-116">String</span><span class="sxs-lookup"><span data-stu-id="09df1-116">String</span></span>|<span data-ttu-id="09df1-117">プロパティの以前の値 (更新前) を示します。</span><span class="sxs-lookup"><span data-stu-id="09df1-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09df1-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09df1-118">JSON representation</span></span>

<span data-ttu-id="09df1-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09df1-119">Here is a JSON representation of the resource.</span></span>

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
