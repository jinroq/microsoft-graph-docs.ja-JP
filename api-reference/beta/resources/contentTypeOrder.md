---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 32cca632933cf2b0fad1f8e9149973d95b4322d3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341233"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="56e78-102">ContentTypeOrder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56e78-102">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56e78-103">**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="56e78-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56e78-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56e78-104">JSON representation</span></span>

<span data-ttu-id="56e78-105">以下は、**contentTypeOrder** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="56e78-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="56e78-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56e78-106">Properties</span></span>

| <span data-ttu-id="56e78-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="56e78-107">Property name</span></span> | <span data-ttu-id="56e78-108">種類</span><span class="sxs-lookup"><span data-stu-id="56e78-108">Type</span></span>    | <span data-ttu-id="56e78-109">説明</span><span class="sxs-lookup"><span data-stu-id="56e78-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="56e78-110">**default**</span><span class="sxs-lookup"><span data-stu-id="56e78-110">**default**</span></span>   | <span data-ttu-id="56e78-111">boolean</span><span class="sxs-lookup"><span data-stu-id="56e78-111">boolean</span></span> | <span data-ttu-id="56e78-112">既定のコンテンツ タイプかどうか。</span><span class="sxs-lookup"><span data-stu-id="56e78-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="56e78-113">**position**</span><span class="sxs-lookup"><span data-stu-id="56e78-113">**position**</span></span>  | <span data-ttu-id="56e78-114">Int32</span><span class="sxs-lookup"><span data-stu-id="56e78-114">Int32</span></span>   | <span data-ttu-id="56e78-115">コンテンツ タイプが選択 UI で表示される位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="56e78-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
