---
title: modifiedProperty リソースの種類
description: ターゲットシステムで実行された変更について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dcf55dfc83414b5a516bac6cbeefa3358323b5fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966704"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="b0477-103">modifiedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0477-103">modifiedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0477-104">ターゲットシステムで実行された変更について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0477-104">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="b0477-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0477-105">Properties</span></span>

| <span data-ttu-id="b0477-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0477-106">Property</span></span>     | <span data-ttu-id="b0477-107">型</span><span class="sxs-lookup"><span data-stu-id="b0477-107">Type</span></span>        | <span data-ttu-id="b0477-108">説明</span><span class="sxs-lookup"><span data-stu-id="b0477-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0477-109">displayName</span><span class="sxs-lookup"><span data-stu-id="b0477-109">displayName</span></span>|<span data-ttu-id="b0477-110">String</span><span class="sxs-lookup"><span data-stu-id="b0477-110">String</span></span>|<span data-ttu-id="b0477-111">変更されたプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="b0477-111">Name of property that was modified.</span></span>|
|<span data-ttu-id="b0477-112">newValue</span><span class="sxs-lookup"><span data-stu-id="b0477-112">newValue</span></span>|<span data-ttu-id="b0477-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0477-113">String</span></span>|<span data-ttu-id="b0477-114">新しいプロパティ値。</span><span class="sxs-lookup"><span data-stu-id="b0477-114">New property value.</span></span>|
|<span data-ttu-id="b0477-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="b0477-115">oldValue</span></span>|<span data-ttu-id="b0477-116">String</span><span class="sxs-lookup"><span data-stu-id="b0477-116">String</span></span>|<span data-ttu-id="b0477-117">Old プロパティの値。</span><span class="sxs-lookup"><span data-stu-id="b0477-117">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0477-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0477-118">JSON representation</span></span>

<span data-ttu-id="b0477-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b0477-119">The following is a JSON representation of the resource.</span></span>

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
