---
title: macOSFirewallApplication リソースの種類
description: MacOS ファイアウォールアプリケーションの一覧にあるアプリを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eb1f77bdadf62ddf6ac5362653ddb7d535f8c85
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946211"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="ca3e5-103">macOSFirewallApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ca3e5-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="ca3e5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca3e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca3e5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca3e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca3e5-106">MacOS ファイアウォールアプリケーションの一覧にあるアプリを表します。</span><span class="sxs-lookup"><span data-stu-id="ca3e5-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="ca3e5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca3e5-107">Properties</span></span>
|<span data-ttu-id="ca3e5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca3e5-108">Property</span></span>|<span data-ttu-id="ca3e5-109">型</span><span class="sxs-lookup"><span data-stu-id="ca3e5-109">Type</span></span>|<span data-ttu-id="ca3e5-110">説明</span><span class="sxs-lookup"><span data-stu-id="ca3e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca3e5-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="ca3e5-111">bundleId</span></span>|<span data-ttu-id="ca3e5-112">String</span><span class="sxs-lookup"><span data-stu-id="ca3e5-112">String</span></span>|<span data-ttu-id="ca3e5-113">アプリケーションの BundleId。</span><span class="sxs-lookup"><span data-stu-id="ca3e5-113">BundleId of the application.</span></span>|
|<span data-ttu-id="ca3e5-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="ca3e5-114">allowsIncomingConnections</span></span>|<span data-ttu-id="ca3e5-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca3e5-115">Boolean</span></span>|<span data-ttu-id="ca3e5-116">受信接続を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ca3e5-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca3e5-117">関係</span><span class="sxs-lookup"><span data-stu-id="ca3e5-117">Relationships</span></span>
<span data-ttu-id="ca3e5-118">なし</span><span class="sxs-lookup"><span data-stu-id="ca3e5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca3e5-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca3e5-119">JSON Representation</span></span>
<span data-ttu-id="ca3e5-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ca3e5-120">Here is a JSON representation of the resource.</span></span>
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




