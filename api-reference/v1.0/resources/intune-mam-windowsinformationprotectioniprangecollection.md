---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
author: tfitzmac
ms.openlocfilehash: 12030ab0b71448c644e4e664f9095dea3e48a26c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319755"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="35b5c-103">windowsInformationProtectionIPRangeCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35b5c-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="35b5c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="35b5c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35b5c-105">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="35b5c-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="35b5c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35b5c-106">Properties</span></span>
|<span data-ttu-id="35b5c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35b5c-107">Property</span></span>|<span data-ttu-id="35b5c-108">種類</span><span class="sxs-lookup"><span data-stu-id="35b5c-108">Type</span></span>|<span data-ttu-id="35b5c-109">説明</span><span class="sxs-lookup"><span data-stu-id="35b5c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35b5c-110">displayName</span><span class="sxs-lookup"><span data-stu-id="35b5c-110">displayName</span></span>|<span data-ttu-id="35b5c-111">文字列</span><span class="sxs-lookup"><span data-stu-id="35b5c-111">String</span></span>|<span data-ttu-id="35b5c-112">表示名</span><span class="sxs-lookup"><span data-stu-id="35b5c-112">Display name</span></span>|
|<span data-ttu-id="35b5c-113">範囲</span><span class="sxs-lookup"><span data-stu-id="35b5c-113">ranges</span></span>|<span data-ttu-id="35b5c-114">[ipRange](../resources/intune-mam-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35b5c-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="35b5c-115">IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="35b5c-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="35b5c-116">関係</span><span class="sxs-lookup"><span data-stu-id="35b5c-116">Relationships</span></span>
<span data-ttu-id="35b5c-117">なし</span><span class="sxs-lookup"><span data-stu-id="35b5c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="35b5c-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35b5c-118">JSON Representation</span></span>
<span data-ttu-id="35b5c-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35b5c-119">Here is a JSON representation of the resource.</span></span>
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



