---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dfe20e52ad63cf1d0d6a958f2ef5f4f89a53ad6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260698"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="05af8-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="05af8-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="05af8-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="05af8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05af8-105">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="05af8-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="05af8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05af8-106">Properties</span></span>
|<span data-ttu-id="05af8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05af8-107">Property</span></span>|<span data-ttu-id="05af8-108">型</span><span class="sxs-lookup"><span data-stu-id="05af8-108">Type</span></span>|<span data-ttu-id="05af8-109">説明</span><span class="sxs-lookup"><span data-stu-id="05af8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05af8-110">address</span><span class="sxs-lookup"><span data-stu-id="05af8-110">address</span></span>|<span data-ttu-id="05af8-111">String</span><span class="sxs-lookup"><span data-stu-id="05af8-111">String</span></span>|<span data-ttu-id="05af8-112">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="05af8-112">Address to the proxy server.</span></span> <span data-ttu-id="05af8-113"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="05af8-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="05af8-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="05af8-114">exceptions</span></span>|<span data-ttu-id="05af8-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="05af8-115">String collection</span></span>|<span data-ttu-id="05af8-116">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="05af8-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="05af8-117">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="05af8-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="05af8-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="05af8-118">useForLocalAddresses</span></span>|<span data-ttu-id="05af8-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="05af8-119">Boolean</span></span>|<span data-ttu-id="05af8-120">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="05af8-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05af8-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="05af8-121">Relationships</span></span>
<span data-ttu-id="05af8-122">なし</span><span class="sxs-lookup"><span data-stu-id="05af8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05af8-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05af8-123">JSON Representation</span></span>
<span data-ttu-id="05af8-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="05af8-124">Here is a JSON representation of the resource.</span></span>
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



