---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f29c69789f6b2a4d41bbb5179ff71f721c64c88f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162105"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="b4df6-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4df6-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="b4df6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4df6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4df6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4df6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4df6-106">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="b4df6-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="b4df6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4df6-107">Properties</span></span>
|<span data-ttu-id="b4df6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4df6-108">Property</span></span>|<span data-ttu-id="b4df6-109">型</span><span class="sxs-lookup"><span data-stu-id="b4df6-109">Type</span></span>|<span data-ttu-id="b4df6-110">説明</span><span class="sxs-lookup"><span data-stu-id="b4df6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4df6-111">address</span><span class="sxs-lookup"><span data-stu-id="b4df6-111">address</span></span>|<span data-ttu-id="b4df6-112">String</span><span class="sxs-lookup"><span data-stu-id="b4df6-112">String</span></span>|<span data-ttu-id="b4df6-113">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="b4df6-113">Address to the proxy server.</span></span> <span data-ttu-id="b4df6-114"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="b4df6-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="b4df6-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="b4df6-115">exceptions</span></span>|<span data-ttu-id="b4df6-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b4df6-116">String collection</span></span>|<span data-ttu-id="b4df6-117">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="b4df6-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="b4df6-118">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="b4df6-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="b4df6-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="b4df6-119">useForLocalAddresses</span></span>|<span data-ttu-id="b4df6-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4df6-120">Boolean</span></span>|<span data-ttu-id="b4df6-121">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b4df6-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4df6-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b4df6-122">Relationships</span></span>
<span data-ttu-id="b4df6-123">なし</span><span class="sxs-lookup"><span data-stu-id="b4df6-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4df6-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4df6-124">JSON Representation</span></span>
<span data-ttu-id="b4df6-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b4df6-125">Here is a JSON representation of the resource.</span></span>
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




