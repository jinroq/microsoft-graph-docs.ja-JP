---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e9d23f8a6d771b116b35058c249866c70c7460d8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952658"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="c3a62-103">windowsInformationProtectionIPRangeCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3a62-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="c3a62-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3a62-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3a62-105">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="c3a62-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="c3a62-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3a62-106">Properties</span></span>
|<span data-ttu-id="c3a62-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3a62-107">Property</span></span>|<span data-ttu-id="c3a62-108">種類</span><span class="sxs-lookup"><span data-stu-id="c3a62-108">Type</span></span>|<span data-ttu-id="c3a62-109">説明</span><span class="sxs-lookup"><span data-stu-id="c3a62-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a62-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c3a62-110">displayName</span></span>|<span data-ttu-id="c3a62-111">文字列</span><span class="sxs-lookup"><span data-stu-id="c3a62-111">String</span></span>|<span data-ttu-id="c3a62-112">表示名</span><span class="sxs-lookup"><span data-stu-id="c3a62-112">Display name</span></span>|
|<span data-ttu-id="c3a62-113">範囲</span><span class="sxs-lookup"><span data-stu-id="c3a62-113">ranges</span></span>|<span data-ttu-id="c3a62-114">[ipRange](../resources/intune-mam-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c3a62-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="c3a62-115">IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="c3a62-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3a62-116">関係</span><span class="sxs-lookup"><span data-stu-id="c3a62-116">Relationships</span></span>
<span data-ttu-id="c3a62-117">なし</span><span class="sxs-lookup"><span data-stu-id="c3a62-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c3a62-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3a62-118">JSON Representation</span></span>
<span data-ttu-id="c3a62-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3a62-119">Here is a JSON representation of the resource.</span></span>
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



