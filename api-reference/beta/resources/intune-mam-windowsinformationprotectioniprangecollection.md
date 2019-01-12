---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9981b585818bb6db712b0088b2fde275179917ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911827"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="caff8-103">windowsInformationProtectionIPRangeCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="caff8-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="caff8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="caff8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="caff8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="caff8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="caff8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="caff8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caff8-107">Windows 情報保護の IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="caff8-107">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="caff8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="caff8-108">Properties</span></span>
|<span data-ttu-id="caff8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="caff8-109">Property</span></span>|<span data-ttu-id="caff8-110">種類</span><span class="sxs-lookup"><span data-stu-id="caff8-110">Type</span></span>|<span data-ttu-id="caff8-111">説明</span><span class="sxs-lookup"><span data-stu-id="caff8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caff8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="caff8-112">displayName</span></span>|<span data-ttu-id="caff8-113">文字列</span><span class="sxs-lookup"><span data-stu-id="caff8-113">String</span></span>|<span data-ttu-id="caff8-114">表示名</span><span class="sxs-lookup"><span data-stu-id="caff8-114">Display name</span></span>|
|<span data-ttu-id="caff8-115">範囲</span><span class="sxs-lookup"><span data-stu-id="caff8-115">ranges</span></span>|<span data-ttu-id="caff8-116">[ipRange](../resources/intune-shared-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="caff8-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="caff8-117">IP 範囲のコレクション</span><span class="sxs-lookup"><span data-stu-id="caff8-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="caff8-118">関係</span><span class="sxs-lookup"><span data-stu-id="caff8-118">Relationships</span></span>
<span data-ttu-id="caff8-119">なし</span><span class="sxs-lookup"><span data-stu-id="caff8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="caff8-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="caff8-120">JSON Representation</span></span>
<span data-ttu-id="caff8-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="caff8-121">Here is a JSON representation of the resource.</span></span>
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





