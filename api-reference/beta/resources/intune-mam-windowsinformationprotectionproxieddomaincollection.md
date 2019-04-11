---
title: windowsInformationProtectionProxiedDomainCollection リソースの種類
description: Windows 情報保護のプロキシ化されたドメイン コレクション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cf20d0a0afb33732278b9c8f988b3008854b770
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799273"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="4973f-103">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4973f-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="4973f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4973f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4973f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4973f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4973f-106">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="4973f-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="4973f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4973f-107">Properties</span></span>
|<span data-ttu-id="4973f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4973f-108">Property</span></span>|<span data-ttu-id="4973f-109">型</span><span class="sxs-lookup"><span data-stu-id="4973f-109">Type</span></span>|<span data-ttu-id="4973f-110">説明</span><span class="sxs-lookup"><span data-stu-id="4973f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4973f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4973f-111">displayName</span></span>|<span data-ttu-id="4973f-112">String</span><span class="sxs-lookup"><span data-stu-id="4973f-112">String</span></span>|<span data-ttu-id="4973f-113">表示名</span><span class="sxs-lookup"><span data-stu-id="4973f-113">Display name</span></span>|
|<span data-ttu-id="4973f-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="4973f-114">proxiedDomains</span></span>|<span data-ttu-id="4973f-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4973f-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="4973f-116">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="4973f-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="4973f-117">関係</span><span class="sxs-lookup"><span data-stu-id="4973f-117">Relationships</span></span>
<span data-ttu-id="4973f-118">なし</span><span class="sxs-lookup"><span data-stu-id="4973f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4973f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4973f-119">JSON Representation</span></span>
<span data-ttu-id="4973f-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4973f-120">Here is a JSON representation of the resource.</span></span>
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





