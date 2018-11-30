---
title: vpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
ms.openlocfilehash: 31e711475bf0f797eead80ca3fe2f3c9af8ba27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067838"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="df557-103">vpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df557-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="df557-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df557-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df557-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df557-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df557-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="df557-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df557-107">VPN プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="df557-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="df557-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df557-108">Properties</span></span>
|<span data-ttu-id="df557-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df557-109">Property</span></span>|<span data-ttu-id="df557-110">型</span><span class="sxs-lookup"><span data-stu-id="df557-110">Type</span></span>|<span data-ttu-id="df557-111">説明</span><span class="sxs-lookup"><span data-stu-id="df557-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df557-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="df557-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="df557-113">String</span><span class="sxs-lookup"><span data-stu-id="df557-113">String</span></span>|<span data-ttu-id="df557-114">プロキシの自動構成スクリプトの url です。</span><span class="sxs-lookup"><span data-stu-id="df557-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="df557-115">address</span><span class="sxs-lookup"><span data-stu-id="df557-115">address</span></span>|<span data-ttu-id="df557-116">String</span><span class="sxs-lookup"><span data-stu-id="df557-116">String</span></span>|<span data-ttu-id="df557-117">アドレスです。</span><span class="sxs-lookup"><span data-stu-id="df557-117">Address.</span></span>|
|<span data-ttu-id="df557-118">port</span><span class="sxs-lookup"><span data-stu-id="df557-118">port</span></span>|<span data-ttu-id="df557-119">Int32</span><span class="sxs-lookup"><span data-stu-id="df557-119">Int32</span></span>|<span data-ttu-id="df557-120">ポートです。</span><span class="sxs-lookup"><span data-stu-id="df557-120">Port.</span></span> <span data-ttu-id="df557-121">0 から 65535 までの有効な値</span><span class="sxs-lookup"><span data-stu-id="df557-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="df557-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="df557-122">Relationships</span></span>
<span data-ttu-id="df557-123">なし</span><span class="sxs-lookup"><span data-stu-id="df557-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df557-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df557-124">JSON Representation</span></span>
<span data-ttu-id="df557-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="df557-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```





