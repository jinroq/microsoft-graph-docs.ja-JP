---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ccea5804c3f4eddb02b5d4163302362f29b5fbc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890497"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="b9397-102">ContentTypeOrder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9397-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="b9397-103">**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="b9397-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9397-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9397-104">JSON representation</span></span>

<span data-ttu-id="b9397-105">以下は、**contentTypeOrder** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b9397-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="b9397-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9397-106">Properties</span></span>

| <span data-ttu-id="b9397-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b9397-107">Property name</span></span> | <span data-ttu-id="b9397-108">種類</span><span class="sxs-lookup"><span data-stu-id="b9397-108">Type</span></span>    | <span data-ttu-id="b9397-109">説明</span><span class="sxs-lookup"><span data-stu-id="b9397-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="b9397-110">**default**</span><span class="sxs-lookup"><span data-stu-id="b9397-110">**default**</span></span>   | <span data-ttu-id="b9397-111">boolean</span><span class="sxs-lookup"><span data-stu-id="b9397-111">boolean</span></span> | <span data-ttu-id="b9397-112">既定のコンテンツ タイプかどうか。</span><span class="sxs-lookup"><span data-stu-id="b9397-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="b9397-113">**position**</span><span class="sxs-lookup"><span data-stu-id="b9397-113">**position**</span></span>  | <span data-ttu-id="b9397-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b9397-114">Int32</span></span>   | <span data-ttu-id="b9397-115">コンテンツ タイプが選択 UI で表示される位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="b9397-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
