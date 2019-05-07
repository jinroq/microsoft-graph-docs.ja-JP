---
title: modifiedProperty リソースの種類
description: 変更された Azure AD リソースのすべてのプロパティ (古い値と新しい値を含む) を示します。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: d87d0170dc811db074026e60efc63df928c65ada
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629279"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="f1df1-103">modifiedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1df1-103">modifiedProperty resource type</span></span>

<span data-ttu-id="f1df1-104">変更された Azure AD リソースのすべてのプロパティ (古い値と新しい値を含む) を示します。</span><span class="sxs-lookup"><span data-stu-id="f1df1-104">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="f1df1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1df1-105">Properties</span></span>

| <span data-ttu-id="f1df1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1df1-106">Property</span></span>     | <span data-ttu-id="f1df1-107">型</span><span class="sxs-lookup"><span data-stu-id="f1df1-107">Type</span></span>   |<span data-ttu-id="f1df1-108">説明</span><span class="sxs-lookup"><span data-stu-id="f1df1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1df1-109">displayName</span><span class="sxs-lookup"><span data-stu-id="f1df1-109">displayName</span></span>|<span data-ttu-id="f1df1-110">String</span><span class="sxs-lookup"><span data-stu-id="f1df1-110">String</span></span>|<span data-ttu-id="f1df1-111">変更されたターゲット属性のプロパティ名を示します。</span><span class="sxs-lookup"><span data-stu-id="f1df1-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="f1df1-112">newValue</span><span class="sxs-lookup"><span data-stu-id="f1df1-112">newValue</span></span>|<span data-ttu-id="f1df1-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f1df1-113">String</span></span>|<span data-ttu-id="f1df1-114">これらの更新された値を示します。</span><span class="sxs-lookup"><span data-stu-id="f1df1-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="f1df1-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="f1df1-115">oldValue</span></span>|<span data-ttu-id="f1df1-116">String</span><span class="sxs-lookup"><span data-stu-id="f1df1-116">String</span></span>|<span data-ttu-id="f1df1-117">プロパティの以前の値 (更新前) を示します。</span><span class="sxs-lookup"><span data-stu-id="f1df1-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1df1-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1df1-118">JSON representation</span></span>

<span data-ttu-id="f1df1-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1df1-119">Here is a JSON representation of the resource.</span></span>

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
