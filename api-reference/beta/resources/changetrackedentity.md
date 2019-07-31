---
title: changeTrackedEntity リソースの種類
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3815b22c7bd76a894df0e98415e0c30bb77decd1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974057"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="0e345-102">changeTrackedEntity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e345-102">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="0e345-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e345-103">Properties</span></span>
|<span data-ttu-id="0e345-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e345-104">Property</span></span>|<span data-ttu-id="0e345-105">型</span><span class="sxs-lookup"><span data-stu-id="0e345-105">Type</span></span>|<span data-ttu-id="0e345-106">説明</span><span class="sxs-lookup"><span data-stu-id="0e345-106">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e345-107">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e345-107">createdDateTime</span></span>| <span data-ttu-id="0e345-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e345-108">DateTimeOffset</span></span>| |
|<span data-ttu-id="0e345-109">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e345-109">lastModifiedDateTime</span></span>| <span data-ttu-id="0e345-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e345-110">DateTimeOffset</span></span>| |
|<span data-ttu-id="0e345-111">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0e345-111">lastModifiedBy</span></span>| [<span data-ttu-id="0e345-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="0e345-112">identitySet</span></span>](identityset.md) | |

## <a name="relationships"></a><span data-ttu-id="0e345-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e345-113">Relationships</span></span>
<span data-ttu-id="0e345-114">なし</span><span class="sxs-lookup"><span data-stu-id="0e345-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e345-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e345-115">JSON Representation</span></span>
<span data-ttu-id="0e345-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e345-116">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType":"microsoft.graph.entity",
  "abstract":true
}-->

``` json
{
    "createdDateTime":"String (timestamp)",
    "lastModifiedDateTime" :"String (timestamp)",
    "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```



