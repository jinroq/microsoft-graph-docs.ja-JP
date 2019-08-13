---
title: macOSFirewallApplication リソースの種類
description: MacOS ファイアウォールアプリケーションの一覧にあるアプリを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 305e313dcc4dc86f71b2c4e20f29bd54d3b82e5e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366533"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="97fc2-103">macOSFirewallApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97fc2-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="97fc2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97fc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97fc2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97fc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97fc2-106">MacOS ファイアウォールアプリケーションの一覧にあるアプリを表します。</span><span class="sxs-lookup"><span data-stu-id="97fc2-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="97fc2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97fc2-107">Properties</span></span>
|<span data-ttu-id="97fc2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97fc2-108">Property</span></span>|<span data-ttu-id="97fc2-109">型</span><span class="sxs-lookup"><span data-stu-id="97fc2-109">Type</span></span>|<span data-ttu-id="97fc2-110">説明</span><span class="sxs-lookup"><span data-stu-id="97fc2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97fc2-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="97fc2-111">bundleId</span></span>|<span data-ttu-id="97fc2-112">String</span><span class="sxs-lookup"><span data-stu-id="97fc2-112">String</span></span>|<span data-ttu-id="97fc2-113">アプリケーションの BundleId。</span><span class="sxs-lookup"><span data-stu-id="97fc2-113">BundleId of the application.</span></span>|
|<span data-ttu-id="97fc2-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="97fc2-114">allowsIncomingConnections</span></span>|<span data-ttu-id="97fc2-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="97fc2-115">Boolean</span></span>|<span data-ttu-id="97fc2-116">受信接続を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="97fc2-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97fc2-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97fc2-117">Relationships</span></span>
<span data-ttu-id="97fc2-118">なし</span><span class="sxs-lookup"><span data-stu-id="97fc2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97fc2-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97fc2-119">JSON Representation</span></span>
<span data-ttu-id="97fc2-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97fc2-120">Here is a JSON representation of the resource.</span></span>
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



