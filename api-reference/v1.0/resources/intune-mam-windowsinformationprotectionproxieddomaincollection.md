---
title: windowsInformationProtectionProxiedDomainCollection リソースの種類
description: Windows 情報保護のプロキシ化されたドメイン コレクション
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dfc07b47115e4e5ce4be959ac7867a2963021abf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822100"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="18b0a-103">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18b0a-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="18b0a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="18b0a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18b0a-105">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="18b0a-105">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="18b0a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18b0a-106">Properties</span></span>
|<span data-ttu-id="18b0a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18b0a-107">Property</span></span>|<span data-ttu-id="18b0a-108">種類</span><span class="sxs-lookup"><span data-stu-id="18b0a-108">Type</span></span>|<span data-ttu-id="18b0a-109">説明</span><span class="sxs-lookup"><span data-stu-id="18b0a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b0a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="18b0a-110">displayName</span></span>|<span data-ttu-id="18b0a-111">文字列</span><span class="sxs-lookup"><span data-stu-id="18b0a-111">String</span></span>|<span data-ttu-id="18b0a-112">表示名</span><span class="sxs-lookup"><span data-stu-id="18b0a-112">Display name</span></span>|
|<span data-ttu-id="18b0a-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="18b0a-113">proxiedDomains</span></span>|<span data-ttu-id="18b0a-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="18b0a-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="18b0a-115">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="18b0a-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="18b0a-116">関係</span><span class="sxs-lookup"><span data-stu-id="18b0a-116">Relationships</span></span>
<span data-ttu-id="18b0a-117">なし</span><span class="sxs-lookup"><span data-stu-id="18b0a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="18b0a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18b0a-118">JSON Representation</span></span>
<span data-ttu-id="18b0a-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18b0a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```



