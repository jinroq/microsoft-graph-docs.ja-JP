---
title: rolePermission リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8b9ba237052fef2b4caa8123d147ea1782fa9b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932806"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="cbd68-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbd68-103">rolePermission resource type</span></span>

> <span data-ttu-id="cbd68-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbd68-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbd68-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cbd68-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="cbd68-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbd68-106">Properties</span></span>
|<span data-ttu-id="cbd68-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbd68-107">Property</span></span>|<span data-ttu-id="cbd68-108">種類</span><span class="sxs-lookup"><span data-stu-id="cbd68-108">Type</span></span>|<span data-ttu-id="cbd68-109">説明</span><span class="sxs-lookup"><span data-stu-id="cbd68-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbd68-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="cbd68-110">resourceActions</span></span>|<span data-ttu-id="cbd68-111">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cbd68-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="cbd68-112">アクション</span><span class="sxs-lookup"><span data-stu-id="cbd68-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbd68-113">関係</span><span class="sxs-lookup"><span data-stu-id="cbd68-113">Relationships</span></span>
<span data-ttu-id="cbd68-114">なし</span><span class="sxs-lookup"><span data-stu-id="cbd68-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cbd68-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cbd68-115">JSON Representation</span></span>
<span data-ttu-id="cbd68-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cbd68-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```



