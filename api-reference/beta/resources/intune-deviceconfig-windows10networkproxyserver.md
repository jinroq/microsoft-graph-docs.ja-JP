---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c193c5b5d1ba61626bb348f52caf39ded58a77c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951916"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="95bca-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95bca-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="95bca-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95bca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95bca-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95bca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95bca-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="95bca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95bca-107">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="95bca-107">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="95bca-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95bca-108">Properties</span></span>
|<span data-ttu-id="95bca-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95bca-109">Property</span></span>|<span data-ttu-id="95bca-110">種類</span><span class="sxs-lookup"><span data-stu-id="95bca-110">Type</span></span>|<span data-ttu-id="95bca-111">説明</span><span class="sxs-lookup"><span data-stu-id="95bca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95bca-112">address</span><span class="sxs-lookup"><span data-stu-id="95bca-112">address</span></span>|<span data-ttu-id="95bca-113">String</span><span class="sxs-lookup"><span data-stu-id="95bca-113">String</span></span>|<span data-ttu-id="95bca-114">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="95bca-114">Address to the proxy server.</span></span> <span data-ttu-id="95bca-115"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="95bca-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="95bca-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="95bca-116">exceptions</span></span>|<span data-ttu-id="95bca-117">String コレクション</span><span class="sxs-lookup"><span data-stu-id="95bca-117">String collection</span></span>|<span data-ttu-id="95bca-118">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="95bca-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="95bca-119">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="95bca-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="95bca-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="95bca-120">useForLocalAddresses</span></span>|<span data-ttu-id="95bca-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="95bca-121">Boolean</span></span>|<span data-ttu-id="95bca-122">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="95bca-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95bca-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95bca-123">Relationships</span></span>
<span data-ttu-id="95bca-124">なし</span><span class="sxs-lookup"><span data-stu-id="95bca-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="95bca-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95bca-125">JSON Representation</span></span>
<span data-ttu-id="95bca-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95bca-126">Here is a JSON representation of the resource.</span></span>
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





