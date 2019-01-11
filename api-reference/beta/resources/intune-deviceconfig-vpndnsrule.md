---
title: vpnDnsRule リソースの種類
description: VPN の DNS ルール定義します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d09e26b105a139f04db34ba69184fcf60e9ef238
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868202"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="10938-103">vpnDnsRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="10938-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="10938-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="10938-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10938-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10938-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10938-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="10938-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10938-107">VPN の DNS ルール定義します。</span><span class="sxs-lookup"><span data-stu-id="10938-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="10938-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10938-108">Properties</span></span>
|<span data-ttu-id="10938-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10938-109">Property</span></span>|<span data-ttu-id="10938-110">種類</span><span class="sxs-lookup"><span data-stu-id="10938-110">Type</span></span>|<span data-ttu-id="10938-111">説明</span><span class="sxs-lookup"><span data-stu-id="10938-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10938-112">名前</span><span class="sxs-lookup"><span data-stu-id="10938-112">name</span></span>|<span data-ttu-id="10938-113">String</span><span class="sxs-lookup"><span data-stu-id="10938-113">String</span></span>|<span data-ttu-id="10938-114">名前です。</span><span class="sxs-lookup"><span data-stu-id="10938-114">Name.</span></span>|
|<span data-ttu-id="10938-115">サーバー</span><span class="sxs-lookup"><span data-stu-id="10938-115">servers</span></span>|<span data-ttu-id="10938-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="10938-116">String collection</span></span>|<span data-ttu-id="10938-117">サーバーです。</span><span class="sxs-lookup"><span data-stu-id="10938-117">Servers.</span></span>|
|<span data-ttu-id="10938-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="10938-118">proxyServerUri</span></span>|<span data-ttu-id="10938-119">String</span><span class="sxs-lookup"><span data-stu-id="10938-119">String</span></span>|<span data-ttu-id="10938-120">プロキシ サーバーの Uri。</span><span class="sxs-lookup"><span data-stu-id="10938-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10938-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="10938-121">Relationships</span></span>
<span data-ttu-id="10938-122">なし</span><span class="sxs-lookup"><span data-stu-id="10938-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10938-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10938-123">JSON Representation</span></span>
<span data-ttu-id="10938-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="10938-124">Here is a JSON representation of the resource.</span></span>
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





