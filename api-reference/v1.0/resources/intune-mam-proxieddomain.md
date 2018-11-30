---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
ms.openlocfilehash: d73ed20341a7de025f6f2d39536a1e791b978f55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022751"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="d31ec-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d31ec-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="d31ec-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d31ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d31ec-105">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="d31ec-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="d31ec-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d31ec-106">Properties</span></span>
|<span data-ttu-id="d31ec-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d31ec-107">Property</span></span>|<span data-ttu-id="d31ec-108">型</span><span class="sxs-lookup"><span data-stu-id="d31ec-108">Type</span></span>|<span data-ttu-id="d31ec-109">説明</span><span class="sxs-lookup"><span data-stu-id="d31ec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d31ec-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="d31ec-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="d31ec-111">文字列</span><span class="sxs-lookup"><span data-stu-id="d31ec-111">String</span></span>|<span data-ttu-id="d31ec-112">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="d31ec-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="d31ec-113">プロキシ</span><span class="sxs-lookup"><span data-stu-id="d31ec-113">proxy</span></span>|<span data-ttu-id="d31ec-114">文字列</span><span class="sxs-lookup"><span data-stu-id="d31ec-114">String</span></span>|<span data-ttu-id="d31ec-115">プロキシ IP</span><span class="sxs-lookup"><span data-stu-id="d31ec-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="d31ec-116">関係</span><span class="sxs-lookup"><span data-stu-id="d31ec-116">Relationships</span></span>
<span data-ttu-id="d31ec-117">なし</span><span class="sxs-lookup"><span data-stu-id="d31ec-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d31ec-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d31ec-118">JSON Representation</span></span>
<span data-ttu-id="d31ec-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d31ec-119">Here is a JSON representation of the resource.</span></span>
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



