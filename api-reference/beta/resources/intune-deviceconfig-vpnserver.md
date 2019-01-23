---
title: vpnServer のリソースの種類
description: VPN サーバーの定義です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0febdae5745f1295e9c690213d4a51b79d7d3bdb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406809"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="ee38d-103">vpnServer のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee38d-103">vpnServer resource type</span></span>

> <span data-ttu-id="ee38d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ee38d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee38d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee38d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee38d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee38d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee38d-107">VPN サーバーの定義です。</span><span class="sxs-lookup"><span data-stu-id="ee38d-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="ee38d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee38d-108">Properties</span></span>
|<span data-ttu-id="ee38d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee38d-109">Property</span></span>|<span data-ttu-id="ee38d-110">型</span><span class="sxs-lookup"><span data-stu-id="ee38d-110">Type</span></span>|<span data-ttu-id="ee38d-111">説明</span><span class="sxs-lookup"><span data-stu-id="ee38d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee38d-112">説明</span><span class="sxs-lookup"><span data-stu-id="ee38d-112">description</span></span>|<span data-ttu-id="ee38d-113">String</span><span class="sxs-lookup"><span data-stu-id="ee38d-113">String</span></span>|<span data-ttu-id="ee38d-114">説明。</span><span class="sxs-lookup"><span data-stu-id="ee38d-114">Description.</span></span>|
|<span data-ttu-id="ee38d-115">address</span><span class="sxs-lookup"><span data-stu-id="ee38d-115">address</span></span>|<span data-ttu-id="ee38d-116">String</span><span class="sxs-lookup"><span data-stu-id="ee38d-116">String</span></span>|<span data-ttu-id="ee38d-117">アドレス (IP アドレス、FQDN、または URL)</span><span class="sxs-lookup"><span data-stu-id="ee38d-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="ee38d-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="ee38d-118">isDefaultServer</span></span>|<span data-ttu-id="ee38d-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee38d-119">Boolean</span></span>|<span data-ttu-id="ee38d-120">既定のサーバーです。</span><span class="sxs-lookup"><span data-stu-id="ee38d-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee38d-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ee38d-121">Relationships</span></span>
<span data-ttu-id="ee38d-122">なし</span><span class="sxs-lookup"><span data-stu-id="ee38d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee38d-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee38d-123">JSON Representation</span></span>
<span data-ttu-id="ee38d-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ee38d-124">Here is a JSON representation of the resource.</span></span>
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




