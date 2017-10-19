---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: fe7309373ded16fe2660e0c5a69773c18ffb581a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="6ec99-102">ContentTypeOrder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ec99-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="6ec99-103">**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ec99-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ec99-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ec99-104">JSON representation</span></span>

<span data-ttu-id="6ec99-105">以下は、**contentTypeOrder** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ec99-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="6ec99-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ec99-106">Properties</span></span>

| <span data-ttu-id="6ec99-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6ec99-107">Property name</span></span> | <span data-ttu-id="6ec99-108">種類</span><span class="sxs-lookup"><span data-stu-id="6ec99-108">Type</span></span>    | <span data-ttu-id="6ec99-109">説明</span><span class="sxs-lookup"><span data-stu-id="6ec99-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="6ec99-110">**default**</span><span class="sxs-lookup"><span data-stu-id="6ec99-110">**default**</span></span>   | <span data-ttu-id="6ec99-111">boolean</span><span class="sxs-lookup"><span data-stu-id="6ec99-111">boolean</span></span> | <span data-ttu-id="6ec99-112">既定のコンテンツ タイプかどうか</span><span class="sxs-lookup"><span data-stu-id="6ec99-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="6ec99-113">**position**</span><span class="sxs-lookup"><span data-stu-id="6ec99-113">**position**</span></span>  | <span data-ttu-id="6ec99-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6ec99-114">Int32</span></span>   | <span data-ttu-id="6ec99-115">コンテンツ タイプが選択 UI で表示される位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ec99-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
