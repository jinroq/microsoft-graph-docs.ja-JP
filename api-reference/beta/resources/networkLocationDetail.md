---
title: networklocationdetail リソースの種類
description: ネットワークの場所に関連付けられている詳細を示します。 .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581444"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="2f53f-104">networklocationdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f53f-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="2f53f-105">ネットワークの場所に関連付けられている詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="2f53f-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="2f53f-106">.</span><span class="sxs-lookup"><span data-stu-id="2f53f-106"></span></span>



## <a name="properties"></a><span data-ttu-id="2f53f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f53f-107">Properties</span></span>
| <span data-ttu-id="2f53f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f53f-108">Property</span></span>     | <span data-ttu-id="2f53f-109">型</span><span class="sxs-lookup"><span data-stu-id="2f53f-109">Type</span></span>   |<span data-ttu-id="2f53f-110">説明</span><span class="sxs-lookup"><span data-stu-id="2f53f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f53f-111">networkType</span><span class="sxs-lookup"><span data-stu-id="2f53f-111">networkType</span></span>|<span data-ttu-id="2f53f-112">String</span><span class="sxs-lookup"><span data-stu-id="2f53f-112">String</span></span>|<span data-ttu-id="2f53f-113">ネットワークの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="2f53f-113">Provides the type of the network.</span></span> <span data-ttu-id="2f53f-114">可能な値`intranet`は`extranet` `namedNetwork`、、、 `trusted`およびです。</span><span class="sxs-lookup"><span data-stu-id="2f53f-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="2f53f-115">networkname</span><span class="sxs-lookup"><span data-stu-id="2f53f-115">networkName</span></span>|<span data-ttu-id="2f53f-116">String</span><span class="sxs-lookup"><span data-stu-id="2f53f-116">String</span></span>|<span data-ttu-id="2f53f-117">ネットワークの名前。</span><span class="sxs-lookup"><span data-stu-id="2f53f-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2f53f-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f53f-118">JSON representation</span></span>

<span data-ttu-id="2f53f-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2f53f-119">Here is a JSON representation of the resource.</span></span>

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
