---
title: macOSFirewallApplication リソースの種類
description: MacOS ファイアウォール アプリケーションの一覧でアプリケーションを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe3bbd83c3101420ec011fda85304fabce06daf0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404212"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="6bdef-103">macOSFirewallApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6bdef-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="6bdef-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6bdef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6bdef-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6bdef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bdef-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6bdef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bdef-107">MacOS ファイアウォール アプリケーションの一覧でアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="6bdef-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="6bdef-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bdef-108">Properties</span></span>
|<span data-ttu-id="6bdef-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bdef-109">Property</span></span>|<span data-ttu-id="6bdef-110">型</span><span class="sxs-lookup"><span data-stu-id="6bdef-110">Type</span></span>|<span data-ttu-id="6bdef-111">説明</span><span class="sxs-lookup"><span data-stu-id="6bdef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bdef-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="6bdef-112">bundleId</span></span>|<span data-ttu-id="6bdef-113">String</span><span class="sxs-lookup"><span data-stu-id="6bdef-113">String</span></span>|<span data-ttu-id="6bdef-114">アプリケーションのメニューです。</span><span class="sxs-lookup"><span data-stu-id="6bdef-114">BundleId of the application.</span></span>|
|<span data-ttu-id="6bdef-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="6bdef-115">allowsIncomingConnections</span></span>|<span data-ttu-id="6bdef-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bdef-116">Boolean</span></span>|<span data-ttu-id="6bdef-117">着信接続ができるかどうか。</span><span class="sxs-lookup"><span data-stu-id="6bdef-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bdef-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6bdef-118">Relationships</span></span>
<span data-ttu-id="6bdef-119">なし</span><span class="sxs-lookup"><span data-stu-id="6bdef-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bdef-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6bdef-120">JSON Representation</span></span>
<span data-ttu-id="6bdef-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6bdef-121">Here is a JSON representation of the resource.</span></span>
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




