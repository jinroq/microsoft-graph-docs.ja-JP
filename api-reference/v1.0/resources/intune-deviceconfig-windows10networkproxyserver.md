---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
ms.openlocfilehash: c2eaeaa4d89f981e5fa992e7a79a7863f0848a9f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344038"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="73cb6-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73cb6-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="73cb6-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="73cb6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73cb6-105">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="73cb6-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="73cb6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73cb6-106">Properties</span></span>
|<span data-ttu-id="73cb6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73cb6-107">Property</span></span>|<span data-ttu-id="73cb6-108">種類</span><span class="sxs-lookup"><span data-stu-id="73cb6-108">Type</span></span>|<span data-ttu-id="73cb6-109">説明</span><span class="sxs-lookup"><span data-stu-id="73cb6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73cb6-110">address</span><span class="sxs-lookup"><span data-stu-id="73cb6-110">address</span></span>|<span data-ttu-id="73cb6-111">String</span><span class="sxs-lookup"><span data-stu-id="73cb6-111">String</span></span>|<span data-ttu-id="73cb6-112">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="73cb6-112">Address to the proxy server.</span></span> <span data-ttu-id="73cb6-113"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="73cb6-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="73cb6-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="73cb6-114">exceptions</span></span>|<span data-ttu-id="73cb6-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="73cb6-115">String collection</span></span>|<span data-ttu-id="73cb6-116">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="73cb6-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="73cb6-117">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="73cb6-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="73cb6-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="73cb6-118">useForLocalAddresses</span></span>|<span data-ttu-id="73cb6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="73cb6-119">Boolean</span></span>|<span data-ttu-id="73cb6-120">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="73cb6-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73cb6-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="73cb6-121">Relationships</span></span>
<span data-ttu-id="73cb6-122">なし</span><span class="sxs-lookup"><span data-stu-id="73cb6-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73cb6-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73cb6-123">JSON Representation</span></span>
<span data-ttu-id="73cb6-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="73cb6-124">Here is a JSON representation of the resource.</span></span>
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



