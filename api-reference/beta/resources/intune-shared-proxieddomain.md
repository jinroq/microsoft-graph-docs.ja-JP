---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9260d0fc9b446e7f61bfebff577ac10f9f3e4aee
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986404"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="891eb-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="891eb-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="891eb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="891eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="891eb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="891eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="891eb-106">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="891eb-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="891eb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="891eb-107">Properties</span></span>
|<span data-ttu-id="891eb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="891eb-108">Property</span></span>|<span data-ttu-id="891eb-109">型</span><span class="sxs-lookup"><span data-stu-id="891eb-109">Type</span></span>|<span data-ttu-id="891eb-110">説明</span><span class="sxs-lookup"><span data-stu-id="891eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="891eb-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="891eb-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="891eb-112">文字列</span><span class="sxs-lookup"><span data-stu-id="891eb-112">String</span></span>|<span data-ttu-id="891eb-113">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="891eb-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="891eb-114">プロキシ</span><span class="sxs-lookup"><span data-stu-id="891eb-114">proxy</span></span>|<span data-ttu-id="891eb-115">文字列</span><span class="sxs-lookup"><span data-stu-id="891eb-115">String</span></span>|<span data-ttu-id="891eb-116">プロキシ IP または FQDN</span><span class="sxs-lookup"><span data-stu-id="891eb-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="891eb-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="891eb-117">Relationships</span></span>
<span data-ttu-id="891eb-118">なし</span><span class="sxs-lookup"><span data-stu-id="891eb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="891eb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="891eb-119">JSON Representation</span></span>
<span data-ttu-id="891eb-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="891eb-120">Here is a JSON representation of the resource.</span></span>
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





