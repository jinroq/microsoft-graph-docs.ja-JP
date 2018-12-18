---
title: plannerPlanContextDetailsCollection リソースの種類
description: " 値は、plannerPlanContextDetails オブジェクトです。"
author: TarkanSevilmis
ms.openlocfilehash: 725239a83f1c059aeef39f68b0d4d58ce8c91013
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346768"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="a0204-103">plannerPlanContextDetailsCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0204-103">plannerPlanContextDetailsCollection resource type</span></span>

> <span data-ttu-id="a0204-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a0204-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0204-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0204-105">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="a0204-106">**PlannerPlanContextDetailsCollection**リソースでは、プランがリンクされている外部のコンテキストのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a0204-106">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="a0204-107">このリソースは、オープン型であり、 [plannerPlanDetails](plannerplandetails.md)オブジェクトの一部であります。</span><span class="sxs-lookup"><span data-stu-id="a0204-107">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="a0204-108">プロパティ名、プロパティ値のペアでは、アプリケーション固有のコンテキストの識別子値は、 [plannerPlanContextDetails](plannerplancontextdetails.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a0204-108">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="a0204-109">Properties</span><span class="sxs-lookup"><span data-stu-id="a0204-109">Properties</span></span>
<span data-ttu-id="a0204-110">クライアントでは、オープン型のプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="a0204-110">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="a0204-111">この場合、クライアントは、プロパティ名と外部のコンテキストを表す特徴的な識別子を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a0204-111">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="a0204-112">プロパティの値は、 [plannerPlanContextDetails](plannerplancontextdetails.md)オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="a0204-112">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="a0204-113">OData を基に、オープン型のプロパティ名は次の文字を含めることはできません: `.`、 `:`、 `@`、 `%`。</span><span class="sxs-lookup"><span data-stu-id="a0204-113">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="a0204-114">これらの文字は、URL エンコード形式にエンコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a0204-114">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="a0204-115">お気に入りの一覧で項目を削除するに値が必要な[plannerPlanContextCollection](plannerplancontextcollection.md)コレクションから削除する代わりに、このオブジェクトのエントリを自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="a0204-115">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
