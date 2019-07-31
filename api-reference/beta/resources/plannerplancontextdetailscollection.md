---
title: プラン/プラン Contextのコレクションリソースの種類
description: " 値は、\"Plan/コンテキスト詳細\" オブジェクトです。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b8adf130dc925a4d9eb17819acf7b2a670a6c7b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965902"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="c8bcd-103">プラン/プラン Contextのコレクションリソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8bcd-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="c8bcd-104">Plan**グループ**は、プランがリンクされている外部コンテキストのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="c8bcd-105">このリソースは、オープンタイプであり、" [plan" プランの詳細](plannerplandetails.md)オブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="c8bcd-106">プロパティと値のペアのプロパティ名は、コンテキストのアプリケーション固有の識別子です。値は、" [plan/コンテキスト詳細](plannerplancontextdetails.md)" オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="c8bcd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8bcd-107">Properties</span></span>
<span data-ttu-id="c8bcd-108">オープン型のプロパティは、クライアントで定義できます。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="c8bcd-109">この場合、クライアントは、プロパティ名として、外部コンテキストを表すディスティンクティブ識別子を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="c8bcd-110">プロパティの値は、" [plan/コンテキスト詳細](plannerplancontextdetails.md)" オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="c8bcd-111">OData に基づいて、オープン型のプロパティ名に次の文字を`.`含める`:`こと`@`は`%`できません:、、、。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="c8bcd-112">これらの文字は、URL エンコード形式でエンコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="c8bcd-113">[お気に入り] の一覧から項目を削除するには、その値を[プラン](plannerplancontextcollection.md)から削除する必要があります。このコレクションは、このオブジェクトのエントリを自動的に削除します。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8bcd-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8bcd-114">JSON representation</span></span>
<span data-ttu-id="c8bcd-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8bcd-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
}-->

```json
{
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
