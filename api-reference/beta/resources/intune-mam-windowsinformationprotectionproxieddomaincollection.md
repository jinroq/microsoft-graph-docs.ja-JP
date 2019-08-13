---
title: windowsInformationProtectionProxiedDomainCollection リソースの種類
description: Windows 情報保護のプロキシ化されたドメイン コレクション
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cccaf79205dfd0114a3d26dae1fd547d07811d42
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342104"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="da5c0-103">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="da5c0-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="da5c0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da5c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da5c0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da5c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da5c0-106">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="da5c0-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="da5c0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da5c0-107">Properties</span></span>
|<span data-ttu-id="da5c0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da5c0-108">Property</span></span>|<span data-ttu-id="da5c0-109">型</span><span class="sxs-lookup"><span data-stu-id="da5c0-109">Type</span></span>|<span data-ttu-id="da5c0-110">説明</span><span class="sxs-lookup"><span data-stu-id="da5c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da5c0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="da5c0-111">displayName</span></span>|<span data-ttu-id="da5c0-112">String</span><span class="sxs-lookup"><span data-stu-id="da5c0-112">String</span></span>|<span data-ttu-id="da5c0-113">表示名</span><span class="sxs-lookup"><span data-stu-id="da5c0-113">Display name</span></span>|
|<span data-ttu-id="da5c0-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="da5c0-114">proxiedDomains</span></span>|<span data-ttu-id="da5c0-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="da5c0-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="da5c0-116">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="da5c0-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="da5c0-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da5c0-117">Relationships</span></span>
<span data-ttu-id="da5c0-118">なし</span><span class="sxs-lookup"><span data-stu-id="da5c0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da5c0-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da5c0-119">JSON Representation</span></span>
<span data-ttu-id="da5c0-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="da5c0-120">Here is a JSON representation of the resource.</span></span>
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



