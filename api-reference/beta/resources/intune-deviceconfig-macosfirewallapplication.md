---
title: macOSFirewallApplication リソースの種類
description: macOS ファイアウォールアプリケーションの一覧にあるアプリを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45d8742a888eb492b71bf9829b9621bde9608ef5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460479"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="d452a-103">macOSFirewallApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d452a-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="d452a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d452a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d452a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d452a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d452a-106">macOS ファイアウォールアプリケーションの一覧にあるアプリを表します。</span><span class="sxs-lookup"><span data-stu-id="d452a-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="d452a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d452a-107">Properties</span></span>
|<span data-ttu-id="d452a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d452a-108">Property</span></span>|<span data-ttu-id="d452a-109">型</span><span class="sxs-lookup"><span data-stu-id="d452a-109">Type</span></span>|<span data-ttu-id="d452a-110">説明</span><span class="sxs-lookup"><span data-stu-id="d452a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d452a-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="d452a-111">bundleId</span></span>|<span data-ttu-id="d452a-112">String</span><span class="sxs-lookup"><span data-stu-id="d452a-112">String</span></span>|<span data-ttu-id="d452a-113">アプリケーションの BundleId。</span><span class="sxs-lookup"><span data-stu-id="d452a-113">BundleId of the application.</span></span>|
|<span data-ttu-id="d452a-114">allowsincomingconnections</span><span class="sxs-lookup"><span data-stu-id="d452a-114">allowsIncomingConnections</span></span>|<span data-ttu-id="d452a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d452a-115">Boolean</span></span>|<span data-ttu-id="d452a-116">受信接続を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d452a-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d452a-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d452a-117">Relationships</span></span>
<span data-ttu-id="d452a-118">なし</span><span class="sxs-lookup"><span data-stu-id="d452a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d452a-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d452a-119">JSON Representation</span></span>
<span data-ttu-id="d452a-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d452a-120">Here is a JSON representation of the resource.</span></span>
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





