---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4e9f727916f055fe197f98b07625b00406e16e83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921102"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="270c3-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="270c3-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="270c3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="270c3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="270c3-105">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="270c3-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="270c3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="270c3-106">Properties</span></span>
|<span data-ttu-id="270c3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="270c3-107">Property</span></span>|<span data-ttu-id="270c3-108">種類</span><span class="sxs-lookup"><span data-stu-id="270c3-108">Type</span></span>|<span data-ttu-id="270c3-109">説明</span><span class="sxs-lookup"><span data-stu-id="270c3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270c3-110">address</span><span class="sxs-lookup"><span data-stu-id="270c3-110">address</span></span>|<span data-ttu-id="270c3-111">String</span><span class="sxs-lookup"><span data-stu-id="270c3-111">String</span></span>|<span data-ttu-id="270c3-112">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="270c3-112">Address to the proxy server.</span></span> <span data-ttu-id="270c3-113"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="270c3-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="270c3-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="270c3-114">exceptions</span></span>|<span data-ttu-id="270c3-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="270c3-115">String collection</span></span>|<span data-ttu-id="270c3-116">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="270c3-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="270c3-117">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="270c3-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="270c3-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="270c3-118">useForLocalAddresses</span></span>|<span data-ttu-id="270c3-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="270c3-119">Boolean</span></span>|<span data-ttu-id="270c3-120">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="270c3-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="270c3-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="270c3-121">Relationships</span></span>
<span data-ttu-id="270c3-122">なし</span><span class="sxs-lookup"><span data-stu-id="270c3-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="270c3-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="270c3-123">JSON Representation</span></span>
<span data-ttu-id="270c3-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="270c3-124">Here is a JSON representation of the resource.</span></span>
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



