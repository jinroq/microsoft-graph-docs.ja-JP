---
title: macOSFirewallApplication リソースの種類
description: macOS ファイアウォールアプリケーションの一覧にあるアプリを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 477911dba492bdda09eb815aba968bb7f63955bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145403"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="f5b12-103">macOSFirewallApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5b12-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="f5b12-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5b12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5b12-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5b12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5b12-106">macOS ファイアウォールアプリケーションの一覧にあるアプリを表します。</span><span class="sxs-lookup"><span data-stu-id="f5b12-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="f5b12-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5b12-107">Properties</span></span>
|<span data-ttu-id="f5b12-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5b12-108">Property</span></span>|<span data-ttu-id="f5b12-109">型</span><span class="sxs-lookup"><span data-stu-id="f5b12-109">Type</span></span>|<span data-ttu-id="f5b12-110">説明</span><span class="sxs-lookup"><span data-stu-id="f5b12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5b12-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="f5b12-111">bundleId</span></span>|<span data-ttu-id="f5b12-112">String</span><span class="sxs-lookup"><span data-stu-id="f5b12-112">String</span></span>|<span data-ttu-id="f5b12-113">アプリケーションの BundleId。</span><span class="sxs-lookup"><span data-stu-id="f5b12-113">BundleId of the application.</span></span>|
|<span data-ttu-id="f5b12-114">allowsincomingconnections</span><span class="sxs-lookup"><span data-stu-id="f5b12-114">allowsIncomingConnections</span></span>|<span data-ttu-id="f5b12-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="f5b12-115">Boolean</span></span>|<span data-ttu-id="f5b12-116">受信接続を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f5b12-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5b12-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5b12-117">Relationships</span></span>
<span data-ttu-id="f5b12-118">なし</span><span class="sxs-lookup"><span data-stu-id="f5b12-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5b12-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5b12-119">JSON Representation</span></span>
<span data-ttu-id="f5b12-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5b12-120">Here is a JSON representation of the resource.</span></span>
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




