---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 634131c39d493bf429d9d23f795dee52123edc15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998249"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="c1669-103">windowsInformationProtectionIPRangeCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1669-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="c1669-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1669-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1669-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1669-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1669-106">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="c1669-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="c1669-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1669-107">Properties</span></span>
|<span data-ttu-id="c1669-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1669-108">Property</span></span>|<span data-ttu-id="c1669-109">型</span><span class="sxs-lookup"><span data-stu-id="c1669-109">Type</span></span>|<span data-ttu-id="c1669-110">説明</span><span class="sxs-lookup"><span data-stu-id="c1669-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1669-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c1669-111">displayName</span></span>|<span data-ttu-id="c1669-112">String</span><span class="sxs-lookup"><span data-stu-id="c1669-112">String</span></span>|<span data-ttu-id="c1669-113">表示名</span><span class="sxs-lookup"><span data-stu-id="c1669-113">Display name</span></span>|
|<span data-ttu-id="c1669-114">範囲</span><span class="sxs-lookup"><span data-stu-id="c1669-114">ranges</span></span>|<span data-ttu-id="c1669-115">[ipRange](../resources/intune-shared-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1669-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="c1669-116">IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="c1669-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1669-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1669-117">Relationships</span></span>
<span data-ttu-id="c1669-118">なし</span><span class="sxs-lookup"><span data-stu-id="c1669-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1669-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1669-119">JSON Representation</span></span>
<span data-ttu-id="c1669-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1669-120">Here is a JSON representation of the resource.</span></span>
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





