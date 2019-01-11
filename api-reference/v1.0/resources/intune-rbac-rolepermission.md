---
title: rolePermission リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3e284198b7b2e6ad3fe120bd1c17c96a1872b793
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816605"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="fe96a-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe96a-103">rolePermission resource type</span></span>

> <span data-ttu-id="fe96a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe96a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe96a-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fe96a-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="fe96a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe96a-106">Properties</span></span>
|<span data-ttu-id="fe96a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe96a-107">Property</span></span>|<span data-ttu-id="fe96a-108">種類</span><span class="sxs-lookup"><span data-stu-id="fe96a-108">Type</span></span>|<span data-ttu-id="fe96a-109">説明</span><span class="sxs-lookup"><span data-stu-id="fe96a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe96a-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="fe96a-110">resourceActions</span></span>|<span data-ttu-id="fe96a-111">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe96a-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="fe96a-112">アクション</span><span class="sxs-lookup"><span data-stu-id="fe96a-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe96a-113">関係</span><span class="sxs-lookup"><span data-stu-id="fe96a-113">Relationships</span></span>
<span data-ttu-id="fe96a-114">なし</span><span class="sxs-lookup"><span data-stu-id="fe96a-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fe96a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe96a-115">JSON Representation</span></span>
<span data-ttu-id="fe96a-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fe96a-116">Here is a JSON representation of the resource.</span></span>
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



