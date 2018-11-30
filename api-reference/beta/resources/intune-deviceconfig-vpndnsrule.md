---
title: vpnDnsRule リソースの種類
description: VPN の DNS ルール定義します。
ms.openlocfilehash: dcb6a0d3a0cd709e8a88835c553f9f29cb094e57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068242"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="c7fc6-103">vpnDnsRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7fc6-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="c7fc6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c7fc6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7fc6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7fc6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7fc6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7fc6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7fc6-107">VPN の DNS ルール定義します。</span><span class="sxs-lookup"><span data-stu-id="c7fc6-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="c7fc6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7fc6-108">Properties</span></span>
|<span data-ttu-id="c7fc6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7fc6-109">Property</span></span>|<span data-ttu-id="c7fc6-110">型</span><span class="sxs-lookup"><span data-stu-id="c7fc6-110">Type</span></span>|<span data-ttu-id="c7fc6-111">説明</span><span class="sxs-lookup"><span data-stu-id="c7fc6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7fc6-112">名前</span><span class="sxs-lookup"><span data-stu-id="c7fc6-112">name</span></span>|<span data-ttu-id="c7fc6-113">String</span><span class="sxs-lookup"><span data-stu-id="c7fc6-113">String</span></span>|<span data-ttu-id="c7fc6-114">名前です。</span><span class="sxs-lookup"><span data-stu-id="c7fc6-114">Name.</span></span>|
|<span data-ttu-id="c7fc6-115">サーバー</span><span class="sxs-lookup"><span data-stu-id="c7fc6-115">servers</span></span>|<span data-ttu-id="c7fc6-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c7fc6-116">String collection</span></span>|<span data-ttu-id="c7fc6-117">サーバーです。</span><span class="sxs-lookup"><span data-stu-id="c7fc6-117">Servers.</span></span>|
|<span data-ttu-id="c7fc6-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="c7fc6-118">proxyServerUri</span></span>|<span data-ttu-id="c7fc6-119">String</span><span class="sxs-lookup"><span data-stu-id="c7fc6-119">String</span></span>|<span data-ttu-id="c7fc6-120">プロキシ サーバーの Uri。</span><span class="sxs-lookup"><span data-stu-id="c7fc6-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7fc6-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7fc6-121">Relationships</span></span>
<span data-ttu-id="c7fc6-122">なし</span><span class="sxs-lookup"><span data-stu-id="c7fc6-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7fc6-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7fc6-123">JSON Representation</span></span>
<span data-ttu-id="c7fc6-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7fc6-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String"
}
```





