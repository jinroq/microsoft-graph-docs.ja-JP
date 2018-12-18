---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
ms.openlocfilehash: dc924d75bc2cf1310cb715033281f59b70abb32a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320294"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="ace68-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ace68-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="ace68-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ace68-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ace68-105">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="ace68-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="ace68-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ace68-106">Properties</span></span>
|<span data-ttu-id="ace68-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ace68-107">Property</span></span>|<span data-ttu-id="ace68-108">種類</span><span class="sxs-lookup"><span data-stu-id="ace68-108">Type</span></span>|<span data-ttu-id="ace68-109">説明</span><span class="sxs-lookup"><span data-stu-id="ace68-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ace68-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="ace68-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="ace68-111">文字列</span><span class="sxs-lookup"><span data-stu-id="ace68-111">String</span></span>|<span data-ttu-id="ace68-112">IP アドレスまたは FQDN</span><span class="sxs-lookup"><span data-stu-id="ace68-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="ace68-113">プロキシ</span><span class="sxs-lookup"><span data-stu-id="ace68-113">proxy</span></span>|<span data-ttu-id="ace68-114">文字列</span><span class="sxs-lookup"><span data-stu-id="ace68-114">String</span></span>|<span data-ttu-id="ace68-115">プロキシ IP</span><span class="sxs-lookup"><span data-stu-id="ace68-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="ace68-116">関係</span><span class="sxs-lookup"><span data-stu-id="ace68-116">Relationships</span></span>
<span data-ttu-id="ace68-117">なし</span><span class="sxs-lookup"><span data-stu-id="ace68-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ace68-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ace68-118">JSON Representation</span></span>
<span data-ttu-id="ace68-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ace68-119">Here is a JSON representation of the resource.</span></span>
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



