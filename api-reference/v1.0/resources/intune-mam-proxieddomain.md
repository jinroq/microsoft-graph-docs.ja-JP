---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e7530bf3bc08deded241257a9c787698682cd9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037829"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="52a6d-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52a6d-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="52a6d-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="52a6d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52a6d-105">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="52a6d-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="52a6d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52a6d-106">Properties</span></span>
|<span data-ttu-id="52a6d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52a6d-107">Property</span></span>|<span data-ttu-id="52a6d-108">型</span><span class="sxs-lookup"><span data-stu-id="52a6d-108">Type</span></span>|<span data-ttu-id="52a6d-109">説明</span><span class="sxs-lookup"><span data-stu-id="52a6d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52a6d-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="52a6d-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="52a6d-111">文字列</span><span class="sxs-lookup"><span data-stu-id="52a6d-111">String</span></span>|<span data-ttu-id="52a6d-112">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="52a6d-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="52a6d-113">プロキシ</span><span class="sxs-lookup"><span data-stu-id="52a6d-113">proxy</span></span>|<span data-ttu-id="52a6d-114">文字列</span><span class="sxs-lookup"><span data-stu-id="52a6d-114">String</span></span>|<span data-ttu-id="52a6d-115">プロキシ IP または FQDN</span><span class="sxs-lookup"><span data-stu-id="52a6d-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="52a6d-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52a6d-116">Relationships</span></span>
<span data-ttu-id="52a6d-117">なし</span><span class="sxs-lookup"><span data-stu-id="52a6d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52a6d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52a6d-118">JSON Representation</span></span>
<span data-ttu-id="52a6d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52a6d-119">Here is a JSON representation of the resource.</span></span>
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



