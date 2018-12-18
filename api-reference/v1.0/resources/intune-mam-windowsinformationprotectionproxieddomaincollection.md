---
title: windowsInformationProtectionProxiedDomainCollection リソースの種類
description: Windows 情報保護のプロキシ化されたドメイン コレクション
author: tfitzmac
ms.openlocfilehash: c95c54c5bbfcc1b5202a0c56a6e3932b35ffac88
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309472"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="de236-103">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de236-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="de236-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="de236-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de236-105">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="de236-105">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="de236-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de236-106">Properties</span></span>
|<span data-ttu-id="de236-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de236-107">Property</span></span>|<span data-ttu-id="de236-108">種類</span><span class="sxs-lookup"><span data-stu-id="de236-108">Type</span></span>|<span data-ttu-id="de236-109">説明</span><span class="sxs-lookup"><span data-stu-id="de236-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de236-110">displayName</span><span class="sxs-lookup"><span data-stu-id="de236-110">displayName</span></span>|<span data-ttu-id="de236-111">文字列</span><span class="sxs-lookup"><span data-stu-id="de236-111">String</span></span>|<span data-ttu-id="de236-112">表示名</span><span class="sxs-lookup"><span data-stu-id="de236-112">Display name</span></span>|
|<span data-ttu-id="de236-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="de236-113">proxiedDomains</span></span>|<span data-ttu-id="de236-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="de236-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="de236-115">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="de236-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="de236-116">関係</span><span class="sxs-lookup"><span data-stu-id="de236-116">Relationships</span></span>
<span data-ttu-id="de236-117">なし</span><span class="sxs-lookup"><span data-stu-id="de236-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de236-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de236-118">JSON Representation</span></span>
<span data-ttu-id="de236-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de236-119">Here is a JSON representation of the resource.</span></span>
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



