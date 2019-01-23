---
title: resourceAction リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5442ed8ee55005b1261da09d999e9c27053276d2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415265"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="276a7-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="276a7-103">resourceAction resource type</span></span>

> <span data-ttu-id="276a7-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="276a7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="276a7-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="276a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="276a7-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="276a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="276a7-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="276a7-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="276a7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="276a7-108">Properties</span></span>
|<span data-ttu-id="276a7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="276a7-109">Property</span></span>|<span data-ttu-id="276a7-110">型</span><span class="sxs-lookup"><span data-stu-id="276a7-110">Type</span></span>|<span data-ttu-id="276a7-111">説明</span><span class="sxs-lookup"><span data-stu-id="276a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="276a7-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="276a7-112">allowedResourceActions</span></span>|<span data-ttu-id="276a7-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="276a7-113">String collection</span></span>|<span data-ttu-id="276a7-114">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="276a7-114">Allowed Actions</span></span>|
|<span data-ttu-id="276a7-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="276a7-115">notAllowedResourceActions</span></span>|<span data-ttu-id="276a7-116">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="276a7-116">String collection</span></span>|<span data-ttu-id="276a7-117">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="276a7-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="276a7-118">関係</span><span class="sxs-lookup"><span data-stu-id="276a7-118">Relationships</span></span>
<span data-ttu-id="276a7-119">なし</span><span class="sxs-lookup"><span data-stu-id="276a7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="276a7-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="276a7-120">JSON Representation</span></span>
<span data-ttu-id="276a7-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="276a7-121">Here is a JSON representation of the resource.</span></span>
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




