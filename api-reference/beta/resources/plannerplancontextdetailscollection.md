---
title: プラン/プラン contextのコレクションリソースの種類
description: " 値は、\"plan/コンテキスト詳細\" オブジェクトです。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: ca1625a4bf137fc14cc780df4d4d1e5ec3bb226e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571858"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="07c47-103">プラン/プラン contextのコレクションリソースの種類</span><span class="sxs-lookup"><span data-stu-id="07c47-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="07c47-104">plan**グループ**は、プランがリンクされている外部コンテキストのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="07c47-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="07c47-105">このリソースは、オープンタイプであり、" [plan" プランの詳細](plannerplandetails.md)オブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="07c47-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="07c47-106">プロパティと値のペアのプロパティ名は、コンテキストのアプリケーション固有の識別子です。値は、" [plan/コンテキスト詳細](plannerplancontextdetails.md)" オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="07c47-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="07c47-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07c47-107">Properties</span></span>
<span data-ttu-id="07c47-108">オープン型のプロパティは、クライアントで定義できます。</span><span class="sxs-lookup"><span data-stu-id="07c47-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="07c47-109">この場合、クライアントは、プロパティ名として、外部コンテキストを表すディスティンクティブ識別子を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="07c47-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="07c47-110">プロパティの値は、" [plan/コンテキスト詳細](plannerplancontextdetails.md)" オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="07c47-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="07c47-111">OData に基づいて、オープン型のプロパティ名に次の文字を`.`含める`:`こと`@`は`%`できません:、、、。</span><span class="sxs-lookup"><span data-stu-id="07c47-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="07c47-112">これらの文字は、URL エンコード形式でエンコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="07c47-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="07c47-113">[お気に入り] の一覧から項目を削除するには、その値を[プラン](plannerplancontextcollection.md)から削除する必要があります。このコレクションは、このオブジェクトのエントリを自動的に削除します。</span><span class="sxs-lookup"><span data-stu-id="07c47-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetailscollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
