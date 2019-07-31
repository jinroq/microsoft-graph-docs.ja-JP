---
title: networkInterface リソースの種類
description: このホストに関連付けられているネットワークインターフェイスカード (NIC) を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ef932729149ea21580ff5a8f1cc3f52e253bfc50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009616"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="02c17-103">networkInterface リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02c17-103">networkInterface resource type</span></span>

<span data-ttu-id="02c17-104">このホストに関連付けられているネットワークインターフェイスカード (NIC) を表します。</span><span class="sxs-lookup"><span data-stu-id="02c17-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="02c17-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02c17-105">Properties</span></span>

| <span data-ttu-id="02c17-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02c17-106">Property</span></span>   | <span data-ttu-id="02c17-107">型</span><span class="sxs-lookup"><span data-stu-id="02c17-107">Type</span></span> |<span data-ttu-id="02c17-108">説明</span><span class="sxs-lookup"><span data-stu-id="02c17-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02c17-109">description</span><span class="sxs-lookup"><span data-stu-id="02c17-109">description</span></span>|<span data-ttu-id="02c17-110">String</span><span class="sxs-lookup"><span data-stu-id="02c17-110">String</span></span>|<span data-ttu-id="02c17-111">NIC の説明 (イーサネットアダプター、ワイヤレス LAN アダプターのローカルエリア接続 \* < # > など)。</span><span class="sxs-lookup"><span data-stu-id="02c17-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="02c17-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="02c17-112">ipV4Address</span></span>|<span data-ttu-id="02c17-113">String</span><span class="sxs-lookup"><span data-stu-id="02c17-113">String</span></span>|<span data-ttu-id="02c17-114">この NIC に関連付けられている最後の IPv4 アドレス。</span><span class="sxs-lookup"><span data-stu-id="02c17-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="02c17-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="02c17-115">ipV6Address</span></span>|<span data-ttu-id="02c17-116">String</span><span class="sxs-lookup"><span data-stu-id="02c17-116">String</span></span>|<span data-ttu-id="02c17-117">この NIC に関連付けられている最後のパブリック (グローバル) IPv6 アドレス。</span><span class="sxs-lookup"><span data-stu-id="02c17-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="02c17-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="02c17-118">localIpV6Address</span></span>|<span data-ttu-id="02c17-119">String</span><span class="sxs-lookup"><span data-stu-id="02c17-119">String</span></span>|<span data-ttu-id="02c17-120">この NIC に関連付けられている最後のローカル (リンクローカルまたはサイトローカル) IPv6 アドレス。</span><span class="sxs-lookup"><span data-stu-id="02c17-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="02c17-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="02c17-121">macAddress</span></span>|<span data-ttu-id="02c17-122">String</span><span class="sxs-lookup"><span data-stu-id="02c17-122">String</span></span>|<span data-ttu-id="02c17-123">このホスト上の NIC の MAC アドレス。</span><span class="sxs-lookup"><span data-stu-id="02c17-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02c17-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02c17-124">JSON representation</span></span>

<span data-ttu-id="02c17-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02c17-125">The following is a JSON representation of the resource.</span></span>

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
