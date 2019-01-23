---
title: windowsInformationProtectionProxiedDomainCollection リソースの種類
description: Windows 情報保護のプロキシ化されたドメイン コレクション
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c65a4b6a94f317c5d75b440aeef7fe387496be32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421677"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="3e31b-103">windowsInformationProtectionProxiedDomainCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3e31b-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="3e31b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3e31b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e31b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e31b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e31b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3e31b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e31b-107">Windows 情報保護のプロキシ化されたドメイン コレクション</span><span class="sxs-lookup"><span data-stu-id="3e31b-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="3e31b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e31b-108">Properties</span></span>
|<span data-ttu-id="3e31b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e31b-109">Property</span></span>|<span data-ttu-id="3e31b-110">型</span><span class="sxs-lookup"><span data-stu-id="3e31b-110">Type</span></span>|<span data-ttu-id="3e31b-111">説明</span><span class="sxs-lookup"><span data-stu-id="3e31b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e31b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3e31b-112">displayName</span></span>|<span data-ttu-id="3e31b-113">文字列</span><span class="sxs-lookup"><span data-stu-id="3e31b-113">String</span></span>|<span data-ttu-id="3e31b-114">表示名</span><span class="sxs-lookup"><span data-stu-id="3e31b-114">Display name</span></span>|
|<span data-ttu-id="3e31b-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="3e31b-115">proxiedDomains</span></span>|<span data-ttu-id="3e31b-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3e31b-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="3e31b-117">プロキシ化されたドメインのコレクション</span><span class="sxs-lookup"><span data-stu-id="3e31b-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e31b-118">関係</span><span class="sxs-lookup"><span data-stu-id="3e31b-118">Relationships</span></span>
<span data-ttu-id="3e31b-119">なし</span><span class="sxs-lookup"><span data-stu-id="3e31b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e31b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e31b-120">JSON Representation</span></span>
<span data-ttu-id="3e31b-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3e31b-121">Here is a JSON representation of the resource.</span></span>
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




