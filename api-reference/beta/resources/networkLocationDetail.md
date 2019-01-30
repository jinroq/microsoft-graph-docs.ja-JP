---
title: networkLocationDetail リソースの種類
description: ネットワーク上の場所に関連付けられている詳細情報を示します。 .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643763"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="a15ad-104">networkLocationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a15ad-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="a15ad-105">ネットワーク上の場所に関連付けられている詳細情報を示します。</span><span class="sxs-lookup"><span data-stu-id="a15ad-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="a15ad-106">.</span><span class="sxs-lookup"><span data-stu-id="a15ad-106"></span></span>



## <a name="properties"></a><span data-ttu-id="a15ad-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a15ad-107">Properties</span></span>
| <span data-ttu-id="a15ad-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a15ad-108">Property</span></span>     | <span data-ttu-id="a15ad-109">型</span><span class="sxs-lookup"><span data-stu-id="a15ad-109">Type</span></span>   |<span data-ttu-id="a15ad-110">説明</span><span class="sxs-lookup"><span data-stu-id="a15ad-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a15ad-111">networkType</span><span class="sxs-lookup"><span data-stu-id="a15ad-111">networkType</span></span>|<span data-ttu-id="a15ad-112">String</span><span class="sxs-lookup"><span data-stu-id="a15ad-112">String</span></span>|<span data-ttu-id="a15ad-113">ネットワークの種類を提供します。</span><span class="sxs-lookup"><span data-stu-id="a15ad-113">Provides the type of the network.</span></span> <span data-ttu-id="a15ad-114">使用可能な値は、 `intranet`、 `extranet`、`namedNetwork`と`trusted`。</span><span class="sxs-lookup"><span data-stu-id="a15ad-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="a15ad-115">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="a15ad-115">networkName</span></span>|<span data-ttu-id="a15ad-116">String</span><span class="sxs-lookup"><span data-stu-id="a15ad-116">String</span></span>|<span data-ttu-id="a15ad-117">ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="a15ad-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a15ad-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a15ad-118">JSON representation</span></span>

<span data-ttu-id="a15ad-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a15ad-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
