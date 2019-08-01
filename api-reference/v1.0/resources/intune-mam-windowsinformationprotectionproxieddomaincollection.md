---
title: windowsInformationProtectionProxiedDomainCollection リソースの種類
description: Windows 情報保護のプロキシ化されたドメイン コレクション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0de9ee342cdb0fb42460d9118c87ed7e2a747b55
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037633"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="e9a2d-103">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9a2d-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="e9a2d-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e9a2d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9a2d-105">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="e9a2d-105">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="e9a2d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9a2d-106">Properties</span></span>
|<span data-ttu-id="e9a2d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9a2d-107">Property</span></span>|<span data-ttu-id="e9a2d-108">型</span><span class="sxs-lookup"><span data-stu-id="e9a2d-108">Type</span></span>|<span data-ttu-id="e9a2d-109">説明</span><span class="sxs-lookup"><span data-stu-id="e9a2d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9a2d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e9a2d-110">displayName</span></span>|<span data-ttu-id="e9a2d-111">String</span><span class="sxs-lookup"><span data-stu-id="e9a2d-111">String</span></span>|<span data-ttu-id="e9a2d-112">表示名</span><span class="sxs-lookup"><span data-stu-id="e9a2d-112">Display name</span></span>|
|<span data-ttu-id="e9a2d-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="e9a2d-113">proxiedDomains</span></span>|<span data-ttu-id="e9a2d-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e9a2d-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="e9a2d-115">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="e9a2d-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9a2d-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e9a2d-116">Relationships</span></span>
<span data-ttu-id="e9a2d-117">なし</span><span class="sxs-lookup"><span data-stu-id="e9a2d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9a2d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9a2d-118">JSON Representation</span></span>
<span data-ttu-id="e9a2d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e9a2d-119">Here is a JSON representation of the resource.</span></span>
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



