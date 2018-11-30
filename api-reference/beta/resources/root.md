---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Root
ms.openlocfilehash: 771eb39baf2a7ce7a85fb43120d6e9e7358f6f6c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070213"
---
# <a name="root-resource-type"></a><span data-ttu-id="09614-102">Root リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09614-102">Root resource type</span></span>

> <span data-ttu-id="09614-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09614-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09614-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09614-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09614-105">**Root** ファセットは、オブジェクトが階層内の最上位であることを示します。</span><span class="sxs-lookup"><span data-stu-id="09614-105">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="09614-106">このファセットに値が存在する (null ではない) ことで、オブジェクトがルートであることを示します。</span><span class="sxs-lookup"><span data-stu-id="09614-106">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="09614-107">null (または存在しない) 値は、オブジェクトがルートでないことを示します。</span><span class="sxs-lookup"><span data-stu-id="09614-107">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="09614-108">**注**:現在、このファセットは空ですが、将来のリビジョンでは、このファセットに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="09614-108">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09614-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09614-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="09614-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09614-110">Properties</span></span>

<span data-ttu-id="09614-111">**ルート** リソースにはプロパティがありません。</span><span class="sxs-lookup"><span data-stu-id="09614-111">The **Root** resource has no properties.</span></span>


<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root"
} -->
