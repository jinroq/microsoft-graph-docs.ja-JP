---
title: networklocationdetail リソースの種類
description: ネットワークの場所に関連付けられている詳細を示します。 .
localization_priority: Normal
ms.openlocfilehash: c4a5323099258d9670b970b1bb85bd0d01f3cf8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342178"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="7b4ba-104">networklocationdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b4ba-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="7b4ba-105">ネットワークの場所に関連付けられている詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="7b4ba-105">Indicates details associated with the network location.</span></span>



## <a name="properties"></a><span data-ttu-id="7b4ba-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b4ba-106">Properties</span></span>
| <span data-ttu-id="7b4ba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b4ba-107">Property</span></span>     | <span data-ttu-id="7b4ba-108">型</span><span class="sxs-lookup"><span data-stu-id="7b4ba-108">Type</span></span>   |<span data-ttu-id="7b4ba-109">説明</span><span class="sxs-lookup"><span data-stu-id="7b4ba-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b4ba-110">networkType</span><span class="sxs-lookup"><span data-stu-id="7b4ba-110">networkType</span></span>|<span data-ttu-id="7b4ba-111">networkType</span><span class="sxs-lookup"><span data-stu-id="7b4ba-111">networkType</span></span>|<span data-ttu-id="7b4ba-112">ネットワークの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="7b4ba-112">Provides the type of the network.</span></span> <span data-ttu-id="7b4ba-113">使用可能な値`intranet`は`extranet`、 `namedNetwork`、、 `trusted`、です。</span><span class="sxs-lookup"><span data-stu-id="7b4ba-113">The possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="7b4ba-114">networknames</span><span class="sxs-lookup"><span data-stu-id="7b4ba-114">networkNames</span></span>|<span data-ttu-id="7b4ba-115">String collection</span><span class="sxs-lookup"><span data-stu-id="7b4ba-115">String collection</span></span>|<span data-ttu-id="7b4ba-116">ネットワークの名前。</span><span class="sxs-lookup"><span data-stu-id="7b4ba-116">Names of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7b4ba-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b4ba-117">JSON representation</span></span>

<span data-ttu-id="7b4ba-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7b4ba-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail"
}-->

```json
{
  "networkType": "string",
  "networkNames": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
