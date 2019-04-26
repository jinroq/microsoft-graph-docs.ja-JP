---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ccea5804c3f4eddb02b5d4163302362f29b5fbc8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561328"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="ea966-102">ContentTypeOrder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ea966-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="ea966-103">**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea966-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea966-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ea966-104">JSON representation</span></span>

<span data-ttu-id="ea966-105">以下は、**contentTypeOrder** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ea966-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="ea966-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea966-106">Properties</span></span>

| <span data-ttu-id="ea966-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ea966-107">Property name</span></span> | <span data-ttu-id="ea966-108">種類</span><span class="sxs-lookup"><span data-stu-id="ea966-108">Type</span></span>    | <span data-ttu-id="ea966-109">説明</span><span class="sxs-lookup"><span data-stu-id="ea966-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="ea966-110">**default**</span><span class="sxs-lookup"><span data-stu-id="ea966-110">**default**</span></span>   | <span data-ttu-id="ea966-111">boolean</span><span class="sxs-lookup"><span data-stu-id="ea966-111">boolean</span></span> | <span data-ttu-id="ea966-112">既定のコンテンツ タイプかどうか。</span><span class="sxs-lookup"><span data-stu-id="ea966-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="ea966-113">**position**</span><span class="sxs-lookup"><span data-stu-id="ea966-113">**position**</span></span>  | <span data-ttu-id="ea966-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ea966-114">Int32</span></span>   | <span data-ttu-id="ea966-115">コンテンツ タイプが選択 UI で表示される位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea966-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
