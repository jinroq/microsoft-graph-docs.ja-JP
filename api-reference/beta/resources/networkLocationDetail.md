---
title: networkLocationDetail リソースの種類
description: ネットワーク上の場所に関連付けられている詳細情報を示します。 .
localization_priority: Normal
ms.openlocfilehash: 62bdb23c63beb89b85386e6bea67face097cf1ae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570940"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="90c53-104">networkLocationDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90c53-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="90c53-105">ネットワーク上の場所に関連付けられている詳細情報を示します。</span><span class="sxs-lookup"><span data-stu-id="90c53-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="90c53-106">.</span><span class="sxs-lookup"><span data-stu-id="90c53-106"></span></span>



## <a name="properties"></a><span data-ttu-id="90c53-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90c53-107">Properties</span></span>
| <span data-ttu-id="90c53-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90c53-108">Property</span></span>     | <span data-ttu-id="90c53-109">型</span><span class="sxs-lookup"><span data-stu-id="90c53-109">Type</span></span>   |<span data-ttu-id="90c53-110">説明</span><span class="sxs-lookup"><span data-stu-id="90c53-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90c53-111">networkType</span><span class="sxs-lookup"><span data-stu-id="90c53-111">networkType</span></span>| <span data-ttu-id="90c53-112">列挙型文字列</span><span class="sxs-lookup"><span data-stu-id="90c53-112">enum-string</span></span> |<span data-ttu-id="90c53-113">ネットワークの種類を提供します。</span><span class="sxs-lookup"><span data-stu-id="90c53-113">Provides the type of the network.</span></span> <span data-ttu-id="90c53-114">使用可能な値は、 `intranet`、 `extranet`、`namedNetwork`と`trusted`。</span><span class="sxs-lookup"><span data-stu-id="90c53-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="90c53-115">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="90c53-115">networkName</span></span>|<span data-ttu-id="90c53-116">String</span><span class="sxs-lookup"><span data-stu-id="90c53-116">String</span></span>|<span data-ttu-id="90c53-117">ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="90c53-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="90c53-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90c53-118">JSON representation</span></span>

<span data-ttu-id="90c53-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="90c53-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": " intranet | extranet | namedNetwork | trusted ",
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
