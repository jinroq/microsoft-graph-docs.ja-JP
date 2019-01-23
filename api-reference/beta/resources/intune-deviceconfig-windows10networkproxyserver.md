---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 673cfe99e9cafe1b57fde5c70b7059286a6cc554
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418583"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="5ace9-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ace9-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="5ace9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ace9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5ace9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ace9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ace9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ace9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ace9-107">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="5ace9-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="5ace9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ace9-108">Properties</span></span>
|<span data-ttu-id="5ace9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ace9-109">Property</span></span>|<span data-ttu-id="5ace9-110">型</span><span class="sxs-lookup"><span data-stu-id="5ace9-110">Type</span></span>|<span data-ttu-id="5ace9-111">説明</span><span class="sxs-lookup"><span data-stu-id="5ace9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ace9-112">address</span><span class="sxs-lookup"><span data-stu-id="5ace9-112">address</span></span>|<span data-ttu-id="5ace9-113">String</span><span class="sxs-lookup"><span data-stu-id="5ace9-113">String</span></span>|<span data-ttu-id="5ace9-114">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="5ace9-114">Address to the proxy server.</span></span> <span data-ttu-id="5ace9-115"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="5ace9-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="5ace9-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="5ace9-116">exceptions</span></span>|<span data-ttu-id="5ace9-117">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5ace9-117">String collection</span></span>|<span data-ttu-id="5ace9-118">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="5ace9-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="5ace9-119">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="5ace9-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="5ace9-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="5ace9-120">useForLocalAddresses</span></span>|<span data-ttu-id="5ace9-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ace9-121">Boolean</span></span>|<span data-ttu-id="5ace9-122">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ace9-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ace9-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5ace9-123">Relationships</span></span>
<span data-ttu-id="5ace9-124">なし</span><span class="sxs-lookup"><span data-stu-id="5ace9-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ace9-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ace9-125">JSON Representation</span></span>
<span data-ttu-id="5ace9-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5ace9-126">Here is a JSON representation of the resource.</span></span>
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




