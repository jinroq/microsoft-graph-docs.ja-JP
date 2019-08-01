---
title: modifiedProperty リソースの種類
description: 変更された Azure AD リソースのすべてのプロパティ (古い値と新しい値を含む) を示します。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 0c5375ea3e188d6023e3588531e07877f6de38ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036100"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="8ce23-103">modifiedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ce23-103">modifiedProperty resource type</span></span>

<span data-ttu-id="8ce23-104">変更された Azure AD リソースのすべてのプロパティ (古い値と新しい値を含む) を示します。</span><span class="sxs-lookup"><span data-stu-id="8ce23-104">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="8ce23-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ce23-105">Properties</span></span>

| <span data-ttu-id="8ce23-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ce23-106">Property</span></span>     | <span data-ttu-id="8ce23-107">型</span><span class="sxs-lookup"><span data-stu-id="8ce23-107">Type</span></span>   |<span data-ttu-id="8ce23-108">説明</span><span class="sxs-lookup"><span data-stu-id="8ce23-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ce23-109">displayName</span><span class="sxs-lookup"><span data-stu-id="8ce23-109">displayName</span></span>|<span data-ttu-id="8ce23-110">String</span><span class="sxs-lookup"><span data-stu-id="8ce23-110">String</span></span>|<span data-ttu-id="8ce23-111">変更されたターゲット属性のプロパティ名を示します。</span><span class="sxs-lookup"><span data-stu-id="8ce23-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="8ce23-112">newValue</span><span class="sxs-lookup"><span data-stu-id="8ce23-112">newValue</span></span>|<span data-ttu-id="8ce23-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8ce23-113">String</span></span>|<span data-ttu-id="8ce23-114">これらの更新された値を示します。</span><span class="sxs-lookup"><span data-stu-id="8ce23-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="8ce23-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="8ce23-115">oldValue</span></span>|<span data-ttu-id="8ce23-116">String</span><span class="sxs-lookup"><span data-stu-id="8ce23-116">String</span></span>|<span data-ttu-id="8ce23-117">プロパティの以前の値 (更新前) を示します。</span><span class="sxs-lookup"><span data-stu-id="8ce23-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ce23-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ce23-118">JSON representation</span></span>

<span data-ttu-id="8ce23-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8ce23-119">Here is a JSON representation of the resource.</span></span>

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
