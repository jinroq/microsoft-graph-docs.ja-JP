---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dcdb371ddcf7887fee8169eb29bbd856e5b8ab2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806168"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="26c24-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26c24-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="26c24-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="26c24-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26c24-105">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="26c24-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="26c24-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26c24-106">Properties</span></span>
|<span data-ttu-id="26c24-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26c24-107">Property</span></span>|<span data-ttu-id="26c24-108">種類</span><span class="sxs-lookup"><span data-stu-id="26c24-108">Type</span></span>|<span data-ttu-id="26c24-109">説明</span><span class="sxs-lookup"><span data-stu-id="26c24-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26c24-110">address</span><span class="sxs-lookup"><span data-stu-id="26c24-110">address</span></span>|<span data-ttu-id="26c24-111">String</span><span class="sxs-lookup"><span data-stu-id="26c24-111">String</span></span>|<span data-ttu-id="26c24-112">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="26c24-112">Address to the proxy server.</span></span> <span data-ttu-id="26c24-113"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="26c24-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="26c24-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="26c24-114">exceptions</span></span>|<span data-ttu-id="26c24-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="26c24-115">String collection</span></span>|<span data-ttu-id="26c24-116">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="26c24-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="26c24-117">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="26c24-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="26c24-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="26c24-118">useForLocalAddresses</span></span>|<span data-ttu-id="26c24-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="26c24-119">Boolean</span></span>|<span data-ttu-id="26c24-120">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="26c24-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26c24-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26c24-121">Relationships</span></span>
<span data-ttu-id="26c24-122">なし</span><span class="sxs-lookup"><span data-stu-id="26c24-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26c24-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26c24-123">JSON Representation</span></span>
<span data-ttu-id="26c24-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="26c24-124">Here is a JSON representation of the resource.</span></span>
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



