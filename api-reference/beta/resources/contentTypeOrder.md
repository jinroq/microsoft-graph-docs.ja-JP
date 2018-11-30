---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: a6b83627d86bbb35357f03dbee3605c6fb1df7a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073450"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="39aba-102">ContentTypeOrder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39aba-102">ContentTypeOrder resource type</span></span>

> <span data-ttu-id="39aba-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="39aba-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39aba-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39aba-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="39aba-105">**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="39aba-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39aba-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39aba-106">JSON representation</span></span>

<span data-ttu-id="39aba-107">以下は、**contentTypeOrder** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39aba-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="39aba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39aba-108">Properties</span></span>

| <span data-ttu-id="39aba-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="39aba-109">Property name</span></span> | <span data-ttu-id="39aba-110">型</span><span class="sxs-lookup"><span data-stu-id="39aba-110">Type</span></span>    | <span data-ttu-id="39aba-111">説明</span><span class="sxs-lookup"><span data-stu-id="39aba-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="39aba-112">**default**</span><span class="sxs-lookup"><span data-stu-id="39aba-112">**default**</span></span>   | <span data-ttu-id="39aba-113">boolean</span><span class="sxs-lookup"><span data-stu-id="39aba-113">boolean</span></span> | <span data-ttu-id="39aba-114">既定のコンテンツ タイプかどうか。</span><span class="sxs-lookup"><span data-stu-id="39aba-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="39aba-115">**position**</span><span class="sxs-lookup"><span data-stu-id="39aba-115">**position**</span></span>  | <span data-ttu-id="39aba-116">Int32</span><span class="sxs-lookup"><span data-stu-id="39aba-116">Int32</span></span>   | <span data-ttu-id="39aba-117">コンテンツ タイプが選択 UI で表示される位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="39aba-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
