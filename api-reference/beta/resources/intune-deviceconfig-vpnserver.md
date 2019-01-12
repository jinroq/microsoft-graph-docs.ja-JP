---
title: vpnServer のリソースの種類
description: VPN サーバーの定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 61eaedb7ecca3f4a7074d079f2b10164dfe2ad76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969549"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="0b04a-103">vpnServer のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b04a-103">vpnServer resource type</span></span>

> <span data-ttu-id="0b04a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0b04a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b04a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b04a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b04a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b04a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b04a-107">VPN サーバーの定義です。</span><span class="sxs-lookup"><span data-stu-id="0b04a-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="0b04a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b04a-108">Properties</span></span>
|<span data-ttu-id="0b04a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b04a-109">Property</span></span>|<span data-ttu-id="0b04a-110">種類</span><span class="sxs-lookup"><span data-stu-id="0b04a-110">Type</span></span>|<span data-ttu-id="0b04a-111">説明</span><span class="sxs-lookup"><span data-stu-id="0b04a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b04a-112">説明</span><span class="sxs-lookup"><span data-stu-id="0b04a-112">description</span></span>|<span data-ttu-id="0b04a-113">String</span><span class="sxs-lookup"><span data-stu-id="0b04a-113">String</span></span>|<span data-ttu-id="0b04a-114">説明。</span><span class="sxs-lookup"><span data-stu-id="0b04a-114">Description.</span></span>|
|<span data-ttu-id="0b04a-115">address</span><span class="sxs-lookup"><span data-stu-id="0b04a-115">address</span></span>|<span data-ttu-id="0b04a-116">String</span><span class="sxs-lookup"><span data-stu-id="0b04a-116">String</span></span>|<span data-ttu-id="0b04a-117">アドレス (IP アドレス、FQDN、または URL)</span><span class="sxs-lookup"><span data-stu-id="0b04a-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="0b04a-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="0b04a-118">isDefaultServer</span></span>|<span data-ttu-id="0b04a-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="0b04a-119">Boolean</span></span>|<span data-ttu-id="0b04a-120">既定のサーバーです。</span><span class="sxs-lookup"><span data-stu-id="0b04a-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b04a-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0b04a-121">Relationships</span></span>
<span data-ttu-id="0b04a-122">なし</span><span class="sxs-lookup"><span data-stu-id="0b04a-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b04a-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b04a-123">JSON Representation</span></span>
<span data-ttu-id="0b04a-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0b04a-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```





