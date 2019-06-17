---
title: windowsInformationProtectionProxiedDomainCollection リソースの種類
description: Windows 情報保護のプロキシ化されたドメイン コレクション
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f33614af89cc6bc7c5e69f56b9ebcface738362
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994413"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="dbbae-103">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dbbae-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="dbbae-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dbbae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbbae-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dbbae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbbae-106">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="dbbae-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="dbbae-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dbbae-107">Properties</span></span>
|<span data-ttu-id="dbbae-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dbbae-108">Property</span></span>|<span data-ttu-id="dbbae-109">型</span><span class="sxs-lookup"><span data-stu-id="dbbae-109">Type</span></span>|<span data-ttu-id="dbbae-110">説明</span><span class="sxs-lookup"><span data-stu-id="dbbae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbbae-111">displayName</span><span class="sxs-lookup"><span data-stu-id="dbbae-111">displayName</span></span>|<span data-ttu-id="dbbae-112">String</span><span class="sxs-lookup"><span data-stu-id="dbbae-112">String</span></span>|<span data-ttu-id="dbbae-113">表示名</span><span class="sxs-lookup"><span data-stu-id="dbbae-113">Display name</span></span>|
|<span data-ttu-id="dbbae-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="dbbae-114">proxiedDomains</span></span>|<span data-ttu-id="dbbae-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dbbae-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="dbbae-116">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="dbbae-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbbae-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dbbae-117">Relationships</span></span>
<span data-ttu-id="dbbae-118">なし</span><span class="sxs-lookup"><span data-stu-id="dbbae-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbbae-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dbbae-119">JSON Representation</span></span>
<span data-ttu-id="dbbae-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dbbae-120">Here is a JSON representation of the resource.</span></span>
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





