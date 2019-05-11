---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de20421b16eae22130508584b8483085d49ac9d9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940520"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="ba1bb-103">windowsInformationProtectionIPRangeCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba1bb-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="ba1bb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba1bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba1bb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba1bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba1bb-106">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="ba1bb-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="ba1bb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba1bb-107">Properties</span></span>
|<span data-ttu-id="ba1bb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba1bb-108">Property</span></span>|<span data-ttu-id="ba1bb-109">型</span><span class="sxs-lookup"><span data-stu-id="ba1bb-109">Type</span></span>|<span data-ttu-id="ba1bb-110">説明</span><span class="sxs-lookup"><span data-stu-id="ba1bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba1bb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ba1bb-111">displayName</span></span>|<span data-ttu-id="ba1bb-112">String</span><span class="sxs-lookup"><span data-stu-id="ba1bb-112">String</span></span>|<span data-ttu-id="ba1bb-113">表示名</span><span class="sxs-lookup"><span data-stu-id="ba1bb-113">Display name</span></span>|
|<span data-ttu-id="ba1bb-114">範囲</span><span class="sxs-lookup"><span data-stu-id="ba1bb-114">ranges</span></span>|<span data-ttu-id="ba1bb-115">[ipRange](../resources/intune-shared-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ba1bb-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="ba1bb-116">IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="ba1bb-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba1bb-117">関係</span><span class="sxs-lookup"><span data-stu-id="ba1bb-117">Relationships</span></span>
<span data-ttu-id="ba1bb-118">なし</span><span class="sxs-lookup"><span data-stu-id="ba1bb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba1bb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba1bb-119">JSON Representation</span></span>
<span data-ttu-id="ba1bb-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba1bb-120">Here is a JSON representation of the resource.</span></span>
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




