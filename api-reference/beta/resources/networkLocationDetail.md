---
title: networkLocationDetail リソースの種類
description: ネットワーク上の場所に関連付けられている詳細情報を示します。 .
ms.openlocfilehash: 5dd1410318d380a1b943de6a7dbb0d739172cc76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070961"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="4bf63-104">networkLocationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4bf63-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="4bf63-105">ネットワーク上の場所に関連付けられている詳細情報を示します。</span><span class="sxs-lookup"><span data-stu-id="4bf63-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="4bf63-106">.</span><span class="sxs-lookup"><span data-stu-id="4bf63-106"></span></span>



## <a name="properties"></a><span data-ttu-id="4bf63-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bf63-107">Properties</span></span>
| <span data-ttu-id="4bf63-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bf63-108">Property</span></span>     | <span data-ttu-id="4bf63-109">型</span><span class="sxs-lookup"><span data-stu-id="4bf63-109">Type</span></span>   |<span data-ttu-id="4bf63-110">説明</span><span class="sxs-lookup"><span data-stu-id="4bf63-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bf63-111">networkType</span><span class="sxs-lookup"><span data-stu-id="4bf63-111">networkType</span></span>|<span data-ttu-id="4bf63-112">String</span><span class="sxs-lookup"><span data-stu-id="4bf63-112">String</span></span>|<span data-ttu-id="4bf63-113">ネットワークの種類を提供します。</span><span class="sxs-lookup"><span data-stu-id="4bf63-113">Provides the type of the network.</span></span> <span data-ttu-id="4bf63-114">使用可能な値は、 `intranet`、 `extranet`、`namedNetwork`と`trusted`。</span><span class="sxs-lookup"><span data-stu-id="4bf63-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="4bf63-115">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="4bf63-115">networkName</span></span>|<span data-ttu-id="4bf63-116">String</span><span class="sxs-lookup"><span data-stu-id="4bf63-116">String</span></span>|<span data-ttu-id="4bf63-117">ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="4bf63-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4bf63-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4bf63-118">JSON representation</span></span>

<span data-ttu-id="4bf63-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4bf63-119">Here is a JSON representation of the resource.</span></span>

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