---
title: macOSFirewallApplication リソースの種類
description: MacOS ファイアウォール アプリケーションの一覧でアプリケーションを表します。
author: tfitzmac
ms.openlocfilehash: 0d248194eed1b6e1841d2e4533aa1f79b772ccc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302724"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="cc669-103">macOSFirewallApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc669-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="cc669-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc669-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc669-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc669-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc669-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc669-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc669-107">MacOS ファイアウォール アプリケーションの一覧でアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="cc669-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="cc669-108">Properties</span><span class="sxs-lookup"><span data-stu-id="cc669-108">Properties</span></span>
|<span data-ttu-id="cc669-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc669-109">Property</span></span>|<span data-ttu-id="cc669-110">種類</span><span class="sxs-lookup"><span data-stu-id="cc669-110">Type</span></span>|<span data-ttu-id="cc669-111">説明</span><span class="sxs-lookup"><span data-stu-id="cc669-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc669-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="cc669-112">bundleId</span></span>|<span data-ttu-id="cc669-113">String</span><span class="sxs-lookup"><span data-stu-id="cc669-113">String</span></span>|<span data-ttu-id="cc669-114">アプリケーションのメニューです。</span><span class="sxs-lookup"><span data-stu-id="cc669-114">BundleId of the application.</span></span>|
|<span data-ttu-id="cc669-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="cc669-115">allowsIncomingConnections</span></span>|<span data-ttu-id="cc669-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="cc669-116">Boolean</span></span>|<span data-ttu-id="cc669-117">着信接続ができるかどうか。</span><span class="sxs-lookup"><span data-stu-id="cc669-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc669-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc669-118">Relationships</span></span>
<span data-ttu-id="cc669-119">なし</span><span class="sxs-lookup"><span data-stu-id="cc669-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc669-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc669-120">JSON Representation</span></span>
<span data-ttu-id="cc669-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc669-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```





