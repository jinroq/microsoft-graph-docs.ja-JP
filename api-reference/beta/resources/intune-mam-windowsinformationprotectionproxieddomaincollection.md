---
title: windowsInformationProtectionProxiedDomainCollection リソースの種類
description: Windows 情報保護のプロキシ化されたドメイン コレクション
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a2f4b1e29afd113c2e06b611fabd525f9f5a6ba1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916903"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="718c8-103">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="718c8-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="718c8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="718c8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="718c8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="718c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="718c8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="718c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="718c8-107">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="718c8-107">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="718c8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="718c8-108">Properties</span></span>
|<span data-ttu-id="718c8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="718c8-109">Property</span></span>|<span data-ttu-id="718c8-110">種類</span><span class="sxs-lookup"><span data-stu-id="718c8-110">Type</span></span>|<span data-ttu-id="718c8-111">説明</span><span class="sxs-lookup"><span data-stu-id="718c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="718c8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="718c8-112">displayName</span></span>|<span data-ttu-id="718c8-113">文字列</span><span class="sxs-lookup"><span data-stu-id="718c8-113">String</span></span>|<span data-ttu-id="718c8-114">表示名</span><span class="sxs-lookup"><span data-stu-id="718c8-114">Display name</span></span>|
|<span data-ttu-id="718c8-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="718c8-115">proxiedDomains</span></span>|<span data-ttu-id="718c8-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="718c8-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="718c8-117">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="718c8-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="718c8-118">関係</span><span class="sxs-lookup"><span data-stu-id="718c8-118">Relationships</span></span>
<span data-ttu-id="718c8-119">なし</span><span class="sxs-lookup"><span data-stu-id="718c8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="718c8-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="718c8-120">JSON Representation</span></span>
<span data-ttu-id="718c8-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="718c8-121">Here is a JSON representation of the resource.</span></span>
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





