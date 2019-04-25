---
title: rolePermission リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a90de4e78bbc831ebb9eb7bf5ee65c26434fc06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554115"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="c234e-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c234e-103">rolePermission resource type</span></span>

> <span data-ttu-id="c234e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c234e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c234e-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c234e-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c234e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c234e-106">Properties</span></span>
|<span data-ttu-id="c234e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c234e-107">Property</span></span>|<span data-ttu-id="c234e-108">型</span><span class="sxs-lookup"><span data-stu-id="c234e-108">Type</span></span>|<span data-ttu-id="c234e-109">説明</span><span class="sxs-lookup"><span data-stu-id="c234e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c234e-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="c234e-110">resourceActions</span></span>|<span data-ttu-id="c234e-111">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c234e-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="c234e-112">アクション</span><span class="sxs-lookup"><span data-stu-id="c234e-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="c234e-113">関係</span><span class="sxs-lookup"><span data-stu-id="c234e-113">Relationships</span></span>
<span data-ttu-id="c234e-114">なし</span><span class="sxs-lookup"><span data-stu-id="c234e-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c234e-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c234e-115">JSON Representation</span></span>
<span data-ttu-id="c234e-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c234e-116">Here is a JSON representation of the resource.</span></span>
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



