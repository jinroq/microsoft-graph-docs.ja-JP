---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Root
localization_priority: Normal
ms.openlocfilehash: 017a4571288839d8d92f182a3a1a44023c4737e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866137"
---
# <a name="root-resource-type"></a><span data-ttu-id="1f329-102">Root リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f329-102">Root resource type</span></span>

> <span data-ttu-id="1f329-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f329-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f329-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f329-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f329-105">**Root** ファセットは、オブジェクトが階層内の最上位であることを示します。</span><span class="sxs-lookup"><span data-stu-id="1f329-105">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="1f329-106">このファセットに値が存在する (null ではない) ことで、オブジェクトがルートであることを示します。</span><span class="sxs-lookup"><span data-stu-id="1f329-106">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="1f329-107">null (または存在しない) 値は、オブジェクトがルートでないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1f329-107">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="1f329-108">**注**:現在、このファセットは空ですが、将来のリビジョンでは、このファセットに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1f329-108">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f329-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f329-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="1f329-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f329-110">Properties</span></span>

<span data-ttu-id="1f329-111">**ルート** リソースにはプロパティがありません。</span><span class="sxs-lookup"><span data-stu-id="1f329-111">The **Root** resource has no properties.</span></span>


<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root"
} -->
