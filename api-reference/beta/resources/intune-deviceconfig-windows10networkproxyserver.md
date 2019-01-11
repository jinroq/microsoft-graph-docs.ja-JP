---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7efe08c565aaeab109339c43e80225b6946299c3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876259"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="229a9-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="229a9-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="229a9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="229a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="229a9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="229a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="229a9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="229a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="229a9-107">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="229a9-107">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="229a9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="229a9-108">Properties</span></span>
|<span data-ttu-id="229a9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="229a9-109">Property</span></span>|<span data-ttu-id="229a9-110">種類</span><span class="sxs-lookup"><span data-stu-id="229a9-110">Type</span></span>|<span data-ttu-id="229a9-111">説明</span><span class="sxs-lookup"><span data-stu-id="229a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="229a9-112">address</span><span class="sxs-lookup"><span data-stu-id="229a9-112">address</span></span>|<span data-ttu-id="229a9-113">String</span><span class="sxs-lookup"><span data-stu-id="229a9-113">String</span></span>|<span data-ttu-id="229a9-114">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="229a9-114">Address to the proxy server.</span></span> <span data-ttu-id="229a9-115"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="229a9-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="229a9-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="229a9-116">exceptions</span></span>|<span data-ttu-id="229a9-117">String コレクション</span><span class="sxs-lookup"><span data-stu-id="229a9-117">String collection</span></span>|<span data-ttu-id="229a9-118">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="229a9-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="229a9-119">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="229a9-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="229a9-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="229a9-120">useForLocalAddresses</span></span>|<span data-ttu-id="229a9-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="229a9-121">Boolean</span></span>|<span data-ttu-id="229a9-122">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="229a9-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="229a9-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="229a9-123">Relationships</span></span>
<span data-ttu-id="229a9-124">なし</span><span class="sxs-lookup"><span data-stu-id="229a9-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="229a9-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="229a9-125">JSON Representation</span></span>
<span data-ttu-id="229a9-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="229a9-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```





