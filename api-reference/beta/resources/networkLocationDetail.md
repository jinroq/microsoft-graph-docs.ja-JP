---
title: networkLocationDetail リソースの種類
description: ネットワークの場所に関連付けられている詳細を示します。 .
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3b7e12a87889909737cac9a52fadf64231f7f2a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009609"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="88def-104">networkLocationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88def-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="88def-105">ネットワークの場所に関連付けられている詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="88def-105">Indicates details associated with the network location.</span></span>



## <a name="properties"></a><span data-ttu-id="88def-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88def-106">Properties</span></span>
| <span data-ttu-id="88def-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88def-107">Property</span></span>     | <span data-ttu-id="88def-108">型</span><span class="sxs-lookup"><span data-stu-id="88def-108">Type</span></span>   |<span data-ttu-id="88def-109">説明</span><span class="sxs-lookup"><span data-stu-id="88def-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88def-110">networkType</span><span class="sxs-lookup"><span data-stu-id="88def-110">networkType</span></span>|<span data-ttu-id="88def-111">networkType</span><span class="sxs-lookup"><span data-stu-id="88def-111">networkType</span></span>|<span data-ttu-id="88def-112">ネットワークの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="88def-112">Provides the type of the network.</span></span> <span data-ttu-id="88def-113">使用可能な値`intranet`は`extranet`、 `namedNetwork`、、 `trusted`、です。</span><span class="sxs-lookup"><span data-stu-id="88def-113">The possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="88def-114">networkNames</span><span class="sxs-lookup"><span data-stu-id="88def-114">networkNames</span></span>|<span data-ttu-id="88def-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="88def-115">String collection</span></span>|<span data-ttu-id="88def-116">ネットワークの名前。</span><span class="sxs-lookup"><span data-stu-id="88def-116">Names of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="88def-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88def-117">JSON representation</span></span>

<span data-ttu-id="88def-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="88def-118">Here is a JSON representation of the resource.</span></span>

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
