---
title: resourceAction リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a48d09d8aeadc9a5d60559d25a4bdcc322d10f21
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553891"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="8f900-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f900-103">resourceAction resource type</span></span>

> <span data-ttu-id="8f900-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f900-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f900-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8f900-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8f900-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f900-106">Properties</span></span>
|<span data-ttu-id="8f900-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f900-107">Property</span></span>|<span data-ttu-id="8f900-108">型</span><span class="sxs-lookup"><span data-stu-id="8f900-108">Type</span></span>|<span data-ttu-id="8f900-109">説明</span><span class="sxs-lookup"><span data-stu-id="8f900-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f900-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="8f900-110">allowedResourceActions</span></span>|<span data-ttu-id="8f900-111">String collection</span><span class="sxs-lookup"><span data-stu-id="8f900-111">String collection</span></span>|<span data-ttu-id="8f900-112">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="8f900-112">Allowed Actions</span></span>|
|<span data-ttu-id="8f900-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="8f900-113">notAllowedResourceActions</span></span>|<span data-ttu-id="8f900-114">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8f900-114">String collection</span></span>|<span data-ttu-id="8f900-115">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="8f900-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f900-116">関係</span><span class="sxs-lookup"><span data-stu-id="8f900-116">Relationships</span></span>
<span data-ttu-id="8f900-117">なし</span><span class="sxs-lookup"><span data-stu-id="8f900-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f900-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f900-118">JSON Representation</span></span>
<span data-ttu-id="8f900-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8f900-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



