---
title: macOSFirewallApplication リソースの種類
description: MacOS ファイアウォールアプリケーションの一覧にあるアプリを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ecd256445a54049149943d14f081f55877be240d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000985"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="9a141-103">macOSFirewallApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a141-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="9a141-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a141-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a141-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9a141-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a141-106">MacOS ファイアウォールアプリケーションの一覧にあるアプリを表します。</span><span class="sxs-lookup"><span data-stu-id="9a141-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="9a141-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a141-107">Properties</span></span>
|<span data-ttu-id="9a141-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a141-108">Property</span></span>|<span data-ttu-id="9a141-109">型</span><span class="sxs-lookup"><span data-stu-id="9a141-109">Type</span></span>|<span data-ttu-id="9a141-110">説明</span><span class="sxs-lookup"><span data-stu-id="9a141-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a141-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="9a141-111">bundleId</span></span>|<span data-ttu-id="9a141-112">String</span><span class="sxs-lookup"><span data-stu-id="9a141-112">String</span></span>|<span data-ttu-id="9a141-113">アプリケーションの BundleId。</span><span class="sxs-lookup"><span data-stu-id="9a141-113">BundleId of the application.</span></span>|
|<span data-ttu-id="9a141-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="9a141-114">allowsIncomingConnections</span></span>|<span data-ttu-id="9a141-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a141-115">Boolean</span></span>|<span data-ttu-id="9a141-116">受信接続を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9a141-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a141-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9a141-117">Relationships</span></span>
<span data-ttu-id="9a141-118">なし</span><span class="sxs-lookup"><span data-stu-id="9a141-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a141-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a141-119">JSON Representation</span></span>
<span data-ttu-id="9a141-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9a141-120">Here is a JSON representation of the resource.</span></span>
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





