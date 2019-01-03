---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
ms.openlocfilehash: d00dc72d7a7156fb90cbeee914c157f446dda81a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341987"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="7a81f-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a81f-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="7a81f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a81f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a81f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a81f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a81f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a81f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a81f-107">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="7a81f-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="7a81f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a81f-108">Properties</span></span>
|<span data-ttu-id="7a81f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a81f-109">Property</span></span>|<span data-ttu-id="7a81f-110">種類</span><span class="sxs-lookup"><span data-stu-id="7a81f-110">Type</span></span>|<span data-ttu-id="7a81f-111">説明</span><span class="sxs-lookup"><span data-stu-id="7a81f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a81f-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="7a81f-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="7a81f-113">文字列</span><span class="sxs-lookup"><span data-stu-id="7a81f-113">String</span></span>|<span data-ttu-id="7a81f-114">IP アドレスまたは完全修飾ドメイン名 (FQDN) です。</span><span class="sxs-lookup"><span data-stu-id="7a81f-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="7a81f-115">プロキシ</span><span class="sxs-lookup"><span data-stu-id="7a81f-115">proxy</span></span>|<span data-ttu-id="7a81f-116">文字列</span><span class="sxs-lookup"><span data-stu-id="7a81f-116">String</span></span>|<span data-ttu-id="7a81f-117">プロキシの IP アドレスまたは FQDN です。</span><span class="sxs-lookup"><span data-stu-id="7a81f-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a81f-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a81f-118">Relationships</span></span>
<span data-ttu-id="7a81f-119">なし</span><span class="sxs-lookup"><span data-stu-id="7a81f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a81f-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a81f-120">JSON Representation</span></span>
<span data-ttu-id="7a81f-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a81f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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


