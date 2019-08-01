---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9354704c5326e9f92814e06aee9ef12635c0faa5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037689"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="58237-103">windowsInformationProtectionIPRangeCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58237-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="58237-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="58237-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58237-105">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="58237-105">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="58237-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58237-106">Properties</span></span>
|<span data-ttu-id="58237-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58237-107">Property</span></span>|<span data-ttu-id="58237-108">型</span><span class="sxs-lookup"><span data-stu-id="58237-108">Type</span></span>|<span data-ttu-id="58237-109">説明</span><span class="sxs-lookup"><span data-stu-id="58237-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58237-110">displayName</span><span class="sxs-lookup"><span data-stu-id="58237-110">displayName</span></span>|<span data-ttu-id="58237-111">String</span><span class="sxs-lookup"><span data-stu-id="58237-111">String</span></span>|<span data-ttu-id="58237-112">表示名</span><span class="sxs-lookup"><span data-stu-id="58237-112">Display name</span></span>|
|<span data-ttu-id="58237-113">範囲</span><span class="sxs-lookup"><span data-stu-id="58237-113">ranges</span></span>|<span data-ttu-id="58237-114">[ipRange](../resources/intune-mam-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="58237-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="58237-115">インターネットプロトコルアドレス範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="58237-115">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="58237-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58237-116">Relationships</span></span>
<span data-ttu-id="58237-117">なし</span><span class="sxs-lookup"><span data-stu-id="58237-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58237-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58237-118">JSON Representation</span></span>
<span data-ttu-id="58237-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58237-119">Here is a JSON representation of the resource.</span></span>
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



