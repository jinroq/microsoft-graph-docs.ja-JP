---
title: networkLocationDetail リソースの種類
description: ネットワーク上の場所に関連付けられている詳細情報を示します。 .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834322"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="b43b5-104">networkLocationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b43b5-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="b43b5-105">ネットワーク上の場所に関連付けられている詳細情報を示します。</span><span class="sxs-lookup"><span data-stu-id="b43b5-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="b43b5-106">.</span><span class="sxs-lookup"><span data-stu-id="b43b5-106"></span></span>



## <a name="properties"></a><span data-ttu-id="b43b5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b43b5-107">Properties</span></span>
| <span data-ttu-id="b43b5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b43b5-108">Property</span></span>     | <span data-ttu-id="b43b5-109">種類</span><span class="sxs-lookup"><span data-stu-id="b43b5-109">Type</span></span>   |<span data-ttu-id="b43b5-110">説明</span><span class="sxs-lookup"><span data-stu-id="b43b5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b43b5-111">networkType</span><span class="sxs-lookup"><span data-stu-id="b43b5-111">networkType</span></span>|<span data-ttu-id="b43b5-112">String</span><span class="sxs-lookup"><span data-stu-id="b43b5-112">String</span></span>|<span data-ttu-id="b43b5-113">ネットワークの種類を提供します。</span><span class="sxs-lookup"><span data-stu-id="b43b5-113">Provides the type of the network.</span></span> <span data-ttu-id="b43b5-114">使用可能な値は、 `intranet`、 `extranet`、`namedNetwork`と`trusted`。</span><span class="sxs-lookup"><span data-stu-id="b43b5-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="b43b5-115">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="b43b5-115">networkName</span></span>|<span data-ttu-id="b43b5-116">String</span><span class="sxs-lookup"><span data-stu-id="b43b5-116">String</span></span>|<span data-ttu-id="b43b5-117">ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="b43b5-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b43b5-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b43b5-118">JSON representation</span></span>

<span data-ttu-id="b43b5-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b43b5-119">Here is a JSON representation of the resource.</span></span>

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
