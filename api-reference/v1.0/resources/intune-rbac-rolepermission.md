---
title: rolePermission リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 16c78e2ee4475a717879d501aabeb5fe2ae0d481
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021813"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="2df9f-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2df9f-103">rolePermission resource type</span></span>

> <span data-ttu-id="2df9f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2df9f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2df9f-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2df9f-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2df9f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2df9f-106">Properties</span></span>
|<span data-ttu-id="2df9f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2df9f-107">Property</span></span>|<span data-ttu-id="2df9f-108">型</span><span class="sxs-lookup"><span data-stu-id="2df9f-108">Type</span></span>|<span data-ttu-id="2df9f-109">説明</span><span class="sxs-lookup"><span data-stu-id="2df9f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2df9f-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="2df9f-110">resourceActions</span></span>|<span data-ttu-id="2df9f-111">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2df9f-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="2df9f-112">アクション</span><span class="sxs-lookup"><span data-stu-id="2df9f-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="2df9f-113">関係</span><span class="sxs-lookup"><span data-stu-id="2df9f-113">Relationships</span></span>
<span data-ttu-id="2df9f-114">なし</span><span class="sxs-lookup"><span data-stu-id="2df9f-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2df9f-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2df9f-115">JSON Representation</span></span>
<span data-ttu-id="2df9f-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2df9f-116">Here is a JSON representation of the resource.</span></span>
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



