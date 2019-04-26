---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 120eff89a01434803c1e2f4f5ba84d3f088e1022
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571962"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="db12c-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="db12c-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="db12c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db12c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db12c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="db12c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db12c-106">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="db12c-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="db12c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db12c-107">Properties</span></span>
|<span data-ttu-id="db12c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db12c-108">Property</span></span>|<span data-ttu-id="db12c-109">型</span><span class="sxs-lookup"><span data-stu-id="db12c-109">Type</span></span>|<span data-ttu-id="db12c-110">説明</span><span class="sxs-lookup"><span data-stu-id="db12c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db12c-111">address</span><span class="sxs-lookup"><span data-stu-id="db12c-111">address</span></span>|<span data-ttu-id="db12c-112">String</span><span class="sxs-lookup"><span data-stu-id="db12c-112">String</span></span>|<span data-ttu-id="db12c-113">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="db12c-113">Address to the proxy server.</span></span> <span data-ttu-id="db12c-114"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="db12c-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="db12c-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="db12c-115">exceptions</span></span>|<span data-ttu-id="db12c-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="db12c-116">String collection</span></span>|<span data-ttu-id="db12c-117">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="db12c-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="db12c-118">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="db12c-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="db12c-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="db12c-119">useForLocalAddresses</span></span>|<span data-ttu-id="db12c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="db12c-120">Boolean</span></span>|<span data-ttu-id="db12c-121">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="db12c-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db12c-122">関係</span><span class="sxs-lookup"><span data-stu-id="db12c-122">Relationships</span></span>
<span data-ttu-id="db12c-123">なし</span><span class="sxs-lookup"><span data-stu-id="db12c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db12c-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db12c-124">JSON Representation</span></span>
<span data-ttu-id="db12c-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="db12c-125">Here is a JSON representation of the resource.</span></span>
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





