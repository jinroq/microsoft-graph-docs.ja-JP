---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b68f13ab80544d591b22fc77ab35110302dc48ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031011"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="eedd5-103">windows10NetworkProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eedd5-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="eedd5-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eedd5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eedd5-105">ネットワーク プロキシ サーバーのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="eedd5-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="eedd5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eedd5-106">Properties</span></span>
|<span data-ttu-id="eedd5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eedd5-107">Property</span></span>|<span data-ttu-id="eedd5-108">型</span><span class="sxs-lookup"><span data-stu-id="eedd5-108">Type</span></span>|<span data-ttu-id="eedd5-109">説明</span><span class="sxs-lookup"><span data-stu-id="eedd5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eedd5-110">address</span><span class="sxs-lookup"><span data-stu-id="eedd5-110">address</span></span>|<span data-ttu-id="eedd5-111">String</span><span class="sxs-lookup"><span data-stu-id="eedd5-111">String</span></span>|<span data-ttu-id="eedd5-112">プロキシ サーバーへのアドレス。</span><span class="sxs-lookup"><span data-stu-id="eedd5-112">Address to the proxy server.</span></span> <span data-ttu-id="eedd5-113"><server>\[“:”<port>\] 形式でアドレスを指定します</span><span class="sxs-lookup"><span data-stu-id="eedd5-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="eedd5-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="eedd5-114">exceptions</span></span>|<span data-ttu-id="eedd5-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="eedd5-115">String collection</span></span>|<span data-ttu-id="eedd5-116">プロキシ サーバーを使用できないアドレス。</span><span class="sxs-lookup"><span data-stu-id="eedd5-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="eedd5-117">システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。</span><span class="sxs-lookup"><span data-stu-id="eedd5-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="eedd5-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="eedd5-118">useForLocalAddresses</span></span>|<span data-ttu-id="eedd5-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="eedd5-119">Boolean</span></span>|<span data-ttu-id="eedd5-120">ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="eedd5-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eedd5-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eedd5-121">Relationships</span></span>
<span data-ttu-id="eedd5-122">なし</span><span class="sxs-lookup"><span data-stu-id="eedd5-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eedd5-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eedd5-123">JSON Representation</span></span>
<span data-ttu-id="eedd5-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eedd5-124">Here is a JSON representation of the resource.</span></span>
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



