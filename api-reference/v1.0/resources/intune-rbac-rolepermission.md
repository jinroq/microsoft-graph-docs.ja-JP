---
title: rolePermission リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2573b2319d06d6d10d952d94c8fc0a17ab8a36dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037101"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="8855a-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8855a-103">rolePermission resource type</span></span>

> <span data-ttu-id="8855a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8855a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8855a-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8855a-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8855a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8855a-106">Properties</span></span>
|<span data-ttu-id="8855a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8855a-107">Property</span></span>|<span data-ttu-id="8855a-108">型</span><span class="sxs-lookup"><span data-stu-id="8855a-108">Type</span></span>|<span data-ttu-id="8855a-109">説明</span><span class="sxs-lookup"><span data-stu-id="8855a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8855a-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="8855a-110">resourceActions</span></span>|<span data-ttu-id="8855a-111">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8855a-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="8855a-112">アクション</span><span class="sxs-lookup"><span data-stu-id="8855a-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8855a-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8855a-113">Relationships</span></span>
<span data-ttu-id="8855a-114">なし</span><span class="sxs-lookup"><span data-stu-id="8855a-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8855a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8855a-115">JSON Representation</span></span>
<span data-ttu-id="8855a-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8855a-116">Here is a JSON representation of the resource.</span></span>
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



