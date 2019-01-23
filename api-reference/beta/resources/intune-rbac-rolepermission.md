---
title: rolePermission リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 932fff06ac979d6ec18ac4c79d50777552e8bfc7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395000"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="29120-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29120-103">rolePermission resource type</span></span>

> <span data-ttu-id="29120-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29120-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29120-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29120-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29120-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29120-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29120-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29120-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="29120-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29120-108">Properties</span></span>
|<span data-ttu-id="29120-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29120-109">Property</span></span>|<span data-ttu-id="29120-110">型</span><span class="sxs-lookup"><span data-stu-id="29120-110">Type</span></span>|<span data-ttu-id="29120-111">説明</span><span class="sxs-lookup"><span data-stu-id="29120-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29120-112">actions</span><span class="sxs-lookup"><span data-stu-id="29120-112">actions</span></span>|<span data-ttu-id="29120-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="29120-113">String collection</span></span>|<span data-ttu-id="29120-114">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="29120-114">Allowed Actions</span></span>|
|<span data-ttu-id="29120-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="29120-115">resourceActions</span></span>|<span data-ttu-id="29120-116">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="29120-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="29120-117">アクション</span><span class="sxs-lookup"><span data-stu-id="29120-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="29120-118">関係</span><span class="sxs-lookup"><span data-stu-id="29120-118">Relationships</span></span>
<span data-ttu-id="29120-119">なし</span><span class="sxs-lookup"><span data-stu-id="29120-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29120-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29120-120">JSON Representation</span></span>
<span data-ttu-id="29120-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29120-121">Here is a JSON representation of the resource.</span></span>
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




