---
title: networkInterface リソースの種類
description: このホストに関連付けられているネットワーク インターフェイス カード (NIC) を表します。
ms.openlocfilehash: 7044b4f469e74424b0dc27ffa38c5feb081faa45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067179"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="9d5c5-103">networkInterface リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9d5c5-103">networkInterface resource type</span></span>

<span data-ttu-id="9d5c5-104">このホストに関連付けられているネットワーク インターフェイス カード (NIC) を表します。</span><span class="sxs-lookup"><span data-stu-id="9d5c5-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="9d5c5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d5c5-105">Properties</span></span>

| <span data-ttu-id="9d5c5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d5c5-106">Property</span></span>   | <span data-ttu-id="9d5c5-107">型</span><span class="sxs-lookup"><span data-stu-id="9d5c5-107">Type</span></span> |<span data-ttu-id="9d5c5-108">説明</span><span class="sxs-lookup"><span data-stu-id="9d5c5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d5c5-109">説明</span><span class="sxs-lookup"><span data-stu-id="9d5c5-109">description</span></span>|<span data-ttu-id="9d5c5-110">String</span><span class="sxs-lookup"><span data-stu-id="9d5c5-110">String</span></span>|<span data-ttu-id="9d5c5-111">NIC の説明 (イーサネット アダプターなどで、ワイヤレス LAN アダプターのローカル エリア接続 \* <> # など。)。</span><span class="sxs-lookup"><span data-stu-id="9d5c5-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="9d5c5-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="9d5c5-112">ipV4Address</span></span>|<span data-ttu-id="9d5c5-113">String</span><span class="sxs-lookup"><span data-stu-id="9d5c5-113">String</span></span>|<span data-ttu-id="9d5c5-114">この NIC に関連付けられている最後の IPv4 アドレス</span><span class="sxs-lookup"><span data-stu-id="9d5c5-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="9d5c5-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="9d5c5-115">ipV6Address</span></span>|<span data-ttu-id="9d5c5-116">String</span><span class="sxs-lookup"><span data-stu-id="9d5c5-116">String</span></span>|<span data-ttu-id="9d5c5-117">最終公開 (別名) IPv6 グローバル アドレスこの NIC に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="9d5c5-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="9d5c5-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="9d5c5-118">localIpV6Address</span></span>|<span data-ttu-id="9d5c5-119">String</span><span class="sxs-lookup"><span data-stu-id="9d5c5-119">String</span></span>|<span data-ttu-id="9d5c5-120">この NIC に関連付けられているローカルの (リンク ローカル アドレスまたはサイト ローカル) IPv6 アドレスを最後します。</span><span class="sxs-lookup"><span data-stu-id="9d5c5-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="9d5c5-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="9d5c5-121">macAddress</span></span>|<span data-ttu-id="9d5c5-122">String</span><span class="sxs-lookup"><span data-stu-id="9d5c5-122">String</span></span>|<span data-ttu-id="9d5c5-123">このホスト上の NIC の MAC アドレスです。</span><span class="sxs-lookup"><span data-stu-id="9d5c5-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d5c5-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9d5c5-124">JSON representation</span></span>

<span data-ttu-id="9d5c5-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d5c5-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->