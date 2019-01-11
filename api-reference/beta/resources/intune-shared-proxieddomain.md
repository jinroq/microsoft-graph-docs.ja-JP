---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b25d40058f4f79add5875698777e23f658992e05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846775"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="5cb13-103">proxiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5cb13-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="5cb13-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5cb13-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cb13-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cb13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cb13-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cb13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cb13-107">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="5cb13-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="5cb13-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cb13-108">Properties</span></span>
|<span data-ttu-id="5cb13-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cb13-109">Property</span></span>|<span data-ttu-id="5cb13-110">種類</span><span class="sxs-lookup"><span data-stu-id="5cb13-110">Type</span></span>|<span data-ttu-id="5cb13-111">説明</span><span class="sxs-lookup"><span data-stu-id="5cb13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cb13-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="5cb13-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="5cb13-113">文字列</span><span class="sxs-lookup"><span data-stu-id="5cb13-113">String</span></span>|<span data-ttu-id="5cb13-114">IP アドレスまたは完全修飾ドメイン名 (FQDN) です。</span><span class="sxs-lookup"><span data-stu-id="5cb13-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="5cb13-115">プロキシ</span><span class="sxs-lookup"><span data-stu-id="5cb13-115">proxy</span></span>|<span data-ttu-id="5cb13-116">文字列</span><span class="sxs-lookup"><span data-stu-id="5cb13-116">String</span></span>|<span data-ttu-id="5cb13-117">プロキシの IP アドレスまたは FQDN です。</span><span class="sxs-lookup"><span data-stu-id="5cb13-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cb13-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5cb13-118">Relationships</span></span>
<span data-ttu-id="5cb13-119">なし</span><span class="sxs-lookup"><span data-stu-id="5cb13-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cb13-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5cb13-120">JSON Representation</span></span>
<span data-ttu-id="5cb13-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5cb13-121">Here is a JSON representation of the resource.</span></span>
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



