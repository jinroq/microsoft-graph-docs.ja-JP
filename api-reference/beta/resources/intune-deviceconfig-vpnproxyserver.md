---
title: vpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9aa15cd1ccf7e299be97d52073924258efd069d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969451"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="7e5e4-103">vpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e5e4-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="7e5e4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e5e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e5e4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e5e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e5e4-106">VPN プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="7e5e4-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="7e5e4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e5e4-107">Properties</span></span>
|<span data-ttu-id="7e5e4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e5e4-108">Property</span></span>|<span data-ttu-id="7e5e4-109">型</span><span class="sxs-lookup"><span data-stu-id="7e5e4-109">Type</span></span>|<span data-ttu-id="7e5e4-110">説明</span><span class="sxs-lookup"><span data-stu-id="7e5e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e5e4-111">自動構成 Scripturl</span><span class="sxs-lookup"><span data-stu-id="7e5e4-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="7e5e4-112">String</span><span class="sxs-lookup"><span data-stu-id="7e5e4-112">String</span></span>|<span data-ttu-id="7e5e4-113">プロキシの自動構成スクリプトの url。</span><span class="sxs-lookup"><span data-stu-id="7e5e4-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="7e5e4-114">address</span><span class="sxs-lookup"><span data-stu-id="7e5e4-114">address</span></span>|<span data-ttu-id="7e5e4-115">String</span><span class="sxs-lookup"><span data-stu-id="7e5e4-115">String</span></span>|<span data-ttu-id="7e5e4-116">連絡先.</span><span class="sxs-lookup"><span data-stu-id="7e5e4-116">Address.</span></span>|
|<span data-ttu-id="7e5e4-117">ポート</span><span class="sxs-lookup"><span data-stu-id="7e5e4-117">port</span></span>|<span data-ttu-id="7e5e4-118">Int32</span><span class="sxs-lookup"><span data-stu-id="7e5e4-118">Int32</span></span>|<span data-ttu-id="7e5e4-119">ポート.</span><span class="sxs-lookup"><span data-stu-id="7e5e4-119">Port.</span></span> <span data-ttu-id="7e5e4-120">有効な値は 0 ~ 65535</span><span class="sxs-lookup"><span data-stu-id="7e5e4-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e5e4-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e5e4-121">Relationships</span></span>
<span data-ttu-id="7e5e4-122">なし</span><span class="sxs-lookup"><span data-stu-id="7e5e4-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e5e4-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e5e4-123">JSON Representation</span></span>
<span data-ttu-id="7e5e4-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e5e4-124">Here is a JSON representation of the resource.</span></span>
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





