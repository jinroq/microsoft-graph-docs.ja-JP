---
title: changeTrackedEntity リソースの種類
description: ''
localization_priority: Normal
ms.openlocfilehash: 838aeca84b6928c709a3c4775c95ab3ef8fd7692
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33347944"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="88c42-102">changeTrackedEntity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88c42-102">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="88c42-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88c42-103">Properties</span></span>
|<span data-ttu-id="88c42-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88c42-104">Property</span></span>|<span data-ttu-id="88c42-105">型</span><span class="sxs-lookup"><span data-stu-id="88c42-105">Type</span></span>|<span data-ttu-id="88c42-106">説明</span><span class="sxs-lookup"><span data-stu-id="88c42-106">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88c42-107">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88c42-107">createdDateTime</span></span>| <span data-ttu-id="88c42-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c42-108">DateTimeOffset</span></span>| |
|<span data-ttu-id="88c42-109">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88c42-109">lastModifiedDateTime</span></span>| <span data-ttu-id="88c42-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c42-110">DateTimeOffset</span></span>| |
|<span data-ttu-id="88c42-111">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="88c42-111">lastModifiedBy</span></span>| [<span data-ttu-id="88c42-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="88c42-112">identitySet</span></span>](identityset.md) | |

## <a name="relationships"></a><span data-ttu-id="88c42-113">関係</span><span class="sxs-lookup"><span data-stu-id="88c42-113">Relationships</span></span>
<span data-ttu-id="88c42-114">なし</span><span class="sxs-lookup"><span data-stu-id="88c42-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="88c42-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88c42-115">JSON Representation</span></span>
<span data-ttu-id="88c42-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="88c42-116">Here is a JSON representation of the resource.</span></span>
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



