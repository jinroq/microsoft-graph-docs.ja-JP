---
title: modifiedProperty リソースの種類
description: ターゲットシステムで実行された変更について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03ae8cb2c36cb811325839341c0fa8b3f395c954
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35348706"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="3d93e-103">modifiedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d93e-103">modifiedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d93e-104">ターゲットシステムで実行された変更について説明します。</span><span class="sxs-lookup"><span data-stu-id="3d93e-104">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="3d93e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d93e-105">Properties</span></span>

| <span data-ttu-id="3d93e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d93e-106">Property</span></span>     | <span data-ttu-id="3d93e-107">型</span><span class="sxs-lookup"><span data-stu-id="3d93e-107">Type</span></span>        | <span data-ttu-id="3d93e-108">説明</span><span class="sxs-lookup"><span data-stu-id="3d93e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3d93e-109">displayName</span><span class="sxs-lookup"><span data-stu-id="3d93e-109">displayName</span></span>|<span data-ttu-id="3d93e-110">String</span><span class="sxs-lookup"><span data-stu-id="3d93e-110">String</span></span>|<span data-ttu-id="3d93e-111">変更されたプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="3d93e-111">Name of property that was modified.</span></span>|
|<span data-ttu-id="3d93e-112">newValue</span><span class="sxs-lookup"><span data-stu-id="3d93e-112">newValue</span></span>|<span data-ttu-id="3d93e-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3d93e-113">String</span></span>|<span data-ttu-id="3d93e-114">新しいプロパティ値。</span><span class="sxs-lookup"><span data-stu-id="3d93e-114">New property value.</span></span>|
|<span data-ttu-id="3d93e-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="3d93e-115">oldValue</span></span>|<span data-ttu-id="3d93e-116">String</span><span class="sxs-lookup"><span data-stu-id="3d93e-116">String</span></span>|<span data-ttu-id="3d93e-117">Old プロパティの値。</span><span class="sxs-lookup"><span data-stu-id="3d93e-117">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d93e-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d93e-118">JSON representation</span></span>

<span data-ttu-id="3d93e-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3d93e-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
