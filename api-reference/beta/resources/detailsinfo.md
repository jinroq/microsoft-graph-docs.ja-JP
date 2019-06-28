---
title: 詳細情報リソースの種類
description: 関連付けられている id またはシステムに関する任意の情報を含むことができるプロパティバッグ。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d3a6726c2151376d858f7962527e4dc6f9b53e7
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349412"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="ac150-103">詳細情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac150-103">detailsInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac150-104">関連付けられている id またはシステムに関する任意の情報を含むことができるプロパティバッグ。</span><span class="sxs-lookup"><span data-stu-id="ac150-104">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="ac150-105">これには、プロビジョニングされているプロパティの詳細、またはソース/ターゲットシステムを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ac150-105">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="ac150-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac150-106">Properties</span></span>
<span data-ttu-id="ac150-107">[詳細**情報**] リソースは、 **ApplicationId**、 **ObjectId**、 **UPN**などの追加のプロパティを含む JSON 文字列です。</span><span class="sxs-lookup"><span data-stu-id="ac150-107">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="ac150-108">プロパティのセットは、プロビジョニングされているリソースの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="ac150-108">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="ac150-109">この例については、「リストの内容の[概要](../api/provisioningobjectsummary-list.md)」をお示します。</span><span class="sxs-lookup"><span data-stu-id="ac150-109">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="ac150-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac150-110">Relationships</span></span>
<span data-ttu-id="ac150-111">なし</span><span class="sxs-lookup"><span data-stu-id="ac150-111">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ac150-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac150-112">JSON Representation</span></span>
<span data-ttu-id="ac150-113">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac150-113">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detailsInfo",
  "openType": true,
 "optionalProperties": [
 
 ],
}-->
``` json
{
  "@odata.type": "microsoft.graph.detailsInfo"
}
```
