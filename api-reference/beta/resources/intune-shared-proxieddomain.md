---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d0b5f347081c0e2bb19ced382ed24faad1f7837
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938605"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="2ba76-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ba76-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="2ba76-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ba76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ba76-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ba76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ba76-106">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="2ba76-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="2ba76-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ba76-107">Properties</span></span>
|<span data-ttu-id="2ba76-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ba76-108">Property</span></span>|<span data-ttu-id="2ba76-109">型</span><span class="sxs-lookup"><span data-stu-id="2ba76-109">Type</span></span>|<span data-ttu-id="2ba76-110">説明</span><span class="sxs-lookup"><span data-stu-id="2ba76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba76-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="2ba76-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="2ba76-112">文字列</span><span class="sxs-lookup"><span data-stu-id="2ba76-112">String</span></span>|<span data-ttu-id="2ba76-113">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="2ba76-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="2ba76-114">プロキシ</span><span class="sxs-lookup"><span data-stu-id="2ba76-114">proxy</span></span>|<span data-ttu-id="2ba76-115">文字列</span><span class="sxs-lookup"><span data-stu-id="2ba76-115">String</span></span>|<span data-ttu-id="2ba76-116">プロキシ IP または FQDN</span><span class="sxs-lookup"><span data-stu-id="2ba76-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ba76-117">関係</span><span class="sxs-lookup"><span data-stu-id="2ba76-117">Relationships</span></span>
<span data-ttu-id="2ba76-118">なし</span><span class="sxs-lookup"><span data-stu-id="2ba76-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ba76-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ba76-119">JSON Representation</span></span>
<span data-ttu-id="2ba76-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ba76-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```




