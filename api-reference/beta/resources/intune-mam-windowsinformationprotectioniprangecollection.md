---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e844c2da60babdcad5fad4a522a750bb2f013721
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418786"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="48977-103">windowsInformationProtectionIPRangeCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48977-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="48977-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="48977-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48977-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48977-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48977-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="48977-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48977-107">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="48977-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="48977-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48977-108">Properties</span></span>
|<span data-ttu-id="48977-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48977-109">Property</span></span>|<span data-ttu-id="48977-110">型</span><span class="sxs-lookup"><span data-stu-id="48977-110">Type</span></span>|<span data-ttu-id="48977-111">説明</span><span class="sxs-lookup"><span data-stu-id="48977-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48977-112">displayName</span><span class="sxs-lookup"><span data-stu-id="48977-112">displayName</span></span>|<span data-ttu-id="48977-113">文字列</span><span class="sxs-lookup"><span data-stu-id="48977-113">String</span></span>|<span data-ttu-id="48977-114">表示名</span><span class="sxs-lookup"><span data-stu-id="48977-114">Display name</span></span>|
|<span data-ttu-id="48977-115">範囲</span><span class="sxs-lookup"><span data-stu-id="48977-115">ranges</span></span>|<span data-ttu-id="48977-116">[ipRange](../resources/intune-shared-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="48977-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="48977-117">IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="48977-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="48977-118">関係</span><span class="sxs-lookup"><span data-stu-id="48977-118">Relationships</span></span>
<span data-ttu-id="48977-119">なし</span><span class="sxs-lookup"><span data-stu-id="48977-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48977-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48977-120">JSON Representation</span></span>
<span data-ttu-id="48977-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="48977-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```




