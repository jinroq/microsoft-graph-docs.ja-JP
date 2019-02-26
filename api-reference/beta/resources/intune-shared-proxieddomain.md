---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5edabc31761a3abd79a94bb700392923d2d54513
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151206"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="06181-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06181-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="06181-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06181-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06181-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06181-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06181-106">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="06181-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="06181-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06181-107">Properties</span></span>
|<span data-ttu-id="06181-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06181-108">Property</span></span>|<span data-ttu-id="06181-109">型</span><span class="sxs-lookup"><span data-stu-id="06181-109">Type</span></span>|<span data-ttu-id="06181-110">説明</span><span class="sxs-lookup"><span data-stu-id="06181-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06181-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="06181-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="06181-112">文字列</span><span class="sxs-lookup"><span data-stu-id="06181-112">String</span></span>|<span data-ttu-id="06181-113">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="06181-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="06181-114">プロキシ</span><span class="sxs-lookup"><span data-stu-id="06181-114">proxy</span></span>|<span data-ttu-id="06181-115">文字列</span><span class="sxs-lookup"><span data-stu-id="06181-115">String</span></span>|<span data-ttu-id="06181-116">プロキシ IP または FQDN</span><span class="sxs-lookup"><span data-stu-id="06181-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="06181-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06181-117">Relationships</span></span>
<span data-ttu-id="06181-118">なし</span><span class="sxs-lookup"><span data-stu-id="06181-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06181-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06181-119">JSON Representation</span></span>
<span data-ttu-id="06181-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06181-120">Here is a JSON representation of the resource.</span></span>
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




