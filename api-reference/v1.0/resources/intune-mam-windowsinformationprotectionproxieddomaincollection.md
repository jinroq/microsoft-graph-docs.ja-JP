---
title: windowsInformationProtectionProxiedDomainCollection リソースの種類
description: Windows 情報保護のプロキシ化されたドメイン コレクション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 026a69dc7697a0b779d72dfcab1695cf8c219d83
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550561"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="2aeb7-103">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2aeb7-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="2aeb7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2aeb7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2aeb7-105">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="2aeb7-105">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="2aeb7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2aeb7-106">Properties</span></span>
|<span data-ttu-id="2aeb7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2aeb7-107">Property</span></span>|<span data-ttu-id="2aeb7-108">型</span><span class="sxs-lookup"><span data-stu-id="2aeb7-108">Type</span></span>|<span data-ttu-id="2aeb7-109">説明</span><span class="sxs-lookup"><span data-stu-id="2aeb7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aeb7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="2aeb7-110">displayName</span></span>|<span data-ttu-id="2aeb7-111">String</span><span class="sxs-lookup"><span data-stu-id="2aeb7-111">String</span></span>|<span data-ttu-id="2aeb7-112">表示名</span><span class="sxs-lookup"><span data-stu-id="2aeb7-112">Display name</span></span>|
|<span data-ttu-id="2aeb7-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="2aeb7-113">proxiedDomains</span></span>|<span data-ttu-id="2aeb7-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2aeb7-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="2aeb7-115">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="2aeb7-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="2aeb7-116">関係</span><span class="sxs-lookup"><span data-stu-id="2aeb7-116">Relationships</span></span>
<span data-ttu-id="2aeb7-117">なし</span><span class="sxs-lookup"><span data-stu-id="2aeb7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2aeb7-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2aeb7-118">JSON Representation</span></span>
<span data-ttu-id="2aeb7-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2aeb7-119">Here is a JSON representation of the resource.</span></span>
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



