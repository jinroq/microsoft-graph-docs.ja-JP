---
title: resourceAction リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88ea0c947a87135f874755f49d0847a3c2a08fae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037157"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="725c3-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="725c3-103">resourceAction resource type</span></span>

> <span data-ttu-id="725c3-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="725c3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="725c3-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="725c3-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="725c3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="725c3-106">Properties</span></span>
|<span data-ttu-id="725c3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="725c3-107">Property</span></span>|<span data-ttu-id="725c3-108">型</span><span class="sxs-lookup"><span data-stu-id="725c3-108">Type</span></span>|<span data-ttu-id="725c3-109">説明</span><span class="sxs-lookup"><span data-stu-id="725c3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="725c3-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="725c3-110">allowedResourceActions</span></span>|<span data-ttu-id="725c3-111">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="725c3-111">String collection</span></span>|<span data-ttu-id="725c3-112">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="725c3-112">Allowed Actions</span></span>|
|<span data-ttu-id="725c3-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="725c3-113">notAllowedResourceActions</span></span>|<span data-ttu-id="725c3-114">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="725c3-114">String collection</span></span>|<span data-ttu-id="725c3-115">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="725c3-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="725c3-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="725c3-116">Relationships</span></span>
<span data-ttu-id="725c3-117">なし</span><span class="sxs-lookup"><span data-stu-id="725c3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="725c3-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="725c3-118">JSON Representation</span></span>
<span data-ttu-id="725c3-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="725c3-119">Here is a JSON representation of the resource.</span></span>
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



