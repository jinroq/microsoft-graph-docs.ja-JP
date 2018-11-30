---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: 8cb47837d8df1c38ed25fc87d3b4d7da450fed1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020416"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="6e575-102">ContentTypeOrder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e575-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="6e575-103">**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="6e575-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e575-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e575-104">JSON representation</span></span>

<span data-ttu-id="6e575-105">以下は、**contentTypeOrder** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6e575-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="6e575-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e575-106">Properties</span></span>

| <span data-ttu-id="6e575-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6e575-107">Property name</span></span> | <span data-ttu-id="6e575-108">種類</span><span class="sxs-lookup"><span data-stu-id="6e575-108">Type</span></span>    | <span data-ttu-id="6e575-109">説明</span><span class="sxs-lookup"><span data-stu-id="6e575-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="6e575-110">**default**</span><span class="sxs-lookup"><span data-stu-id="6e575-110">**default**</span></span>   | <span data-ttu-id="6e575-111">boolean</span><span class="sxs-lookup"><span data-stu-id="6e575-111">boolean</span></span> | <span data-ttu-id="6e575-112">既定のコンテンツ タイプかどうか。</span><span class="sxs-lookup"><span data-stu-id="6e575-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="6e575-113">**position**</span><span class="sxs-lookup"><span data-stu-id="6e575-113">**position**</span></span>  | <span data-ttu-id="6e575-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6e575-114">Int32</span></span>   | <span data-ttu-id="6e575-115">コンテンツ タイプが選択 UI で表示される位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="6e575-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
