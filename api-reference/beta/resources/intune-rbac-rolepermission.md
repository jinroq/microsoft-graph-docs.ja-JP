---
title: rolePermission リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b56df927cda3cbf98e7d736311aba2db5e53906
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145382"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="9dd94-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9dd94-103">rolePermission resource type</span></span>

> <span data-ttu-id="9dd94-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9dd94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9dd94-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9dd94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dd94-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9dd94-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9dd94-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dd94-107">Properties</span></span>
|<span data-ttu-id="9dd94-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dd94-108">Property</span></span>|<span data-ttu-id="9dd94-109">型</span><span class="sxs-lookup"><span data-stu-id="9dd94-109">Type</span></span>|<span data-ttu-id="9dd94-110">説明</span><span class="sxs-lookup"><span data-stu-id="9dd94-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dd94-111">actions</span><span class="sxs-lookup"><span data-stu-id="9dd94-111">actions</span></span>|<span data-ttu-id="9dd94-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9dd94-112">String collection</span></span>|<span data-ttu-id="9dd94-113">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="9dd94-113">Allowed Actions</span></span>|
|<span data-ttu-id="9dd94-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="9dd94-114">resourceActions</span></span>|<span data-ttu-id="9dd94-115">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9dd94-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="9dd94-116">アクション</span><span class="sxs-lookup"><span data-stu-id="9dd94-116">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dd94-117">関係</span><span class="sxs-lookup"><span data-stu-id="9dd94-117">Relationships</span></span>
<span data-ttu-id="9dd94-118">なし</span><span class="sxs-lookup"><span data-stu-id="9dd94-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dd94-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9dd94-119">JSON Representation</span></span>
<span data-ttu-id="9dd94-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9dd94-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
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




