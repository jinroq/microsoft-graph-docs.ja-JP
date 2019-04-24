---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6a2f52613eae9d8e06751672c95230dfc3b00c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584825"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="18abe-103">windowsInformationProtectionIPRangeCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18abe-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="18abe-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18abe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18abe-105">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="18abe-105">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="18abe-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18abe-106">Properties</span></span>
|<span data-ttu-id="18abe-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18abe-107">Property</span></span>|<span data-ttu-id="18abe-108">型</span><span class="sxs-lookup"><span data-stu-id="18abe-108">Type</span></span>|<span data-ttu-id="18abe-109">説明</span><span class="sxs-lookup"><span data-stu-id="18abe-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18abe-110">displayName</span><span class="sxs-lookup"><span data-stu-id="18abe-110">displayName</span></span>|<span data-ttu-id="18abe-111">String</span><span class="sxs-lookup"><span data-stu-id="18abe-111">String</span></span>|<span data-ttu-id="18abe-112">表示名</span><span class="sxs-lookup"><span data-stu-id="18abe-112">Display name</span></span>|
|<span data-ttu-id="18abe-113">範囲</span><span class="sxs-lookup"><span data-stu-id="18abe-113">ranges</span></span>|<span data-ttu-id="18abe-114">[ipRange](../resources/intune-mam-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="18abe-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="18abe-115">インターネットプロトコルアドレス範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="18abe-115">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="18abe-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18abe-116">Relationships</span></span>
<span data-ttu-id="18abe-117">なし</span><span class="sxs-lookup"><span data-stu-id="18abe-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18abe-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18abe-118">JSON Representation</span></span>
<span data-ttu-id="18abe-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18abe-119">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



