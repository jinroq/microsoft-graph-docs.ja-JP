---
title: vpnServer リソースの種類
description: VPN サーバーの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c3123f6ae290cf2116433400e54a9819b2c1cad
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367590"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="88a32-103">vpnServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88a32-103">vpnServer resource type</span></span>

> <span data-ttu-id="88a32-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88a32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88a32-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88a32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88a32-106">VPN サーバーの定義。</span><span class="sxs-lookup"><span data-stu-id="88a32-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="88a32-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88a32-107">Properties</span></span>
|<span data-ttu-id="88a32-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88a32-108">Property</span></span>|<span data-ttu-id="88a32-109">型</span><span class="sxs-lookup"><span data-stu-id="88a32-109">Type</span></span>|<span data-ttu-id="88a32-110">説明</span><span class="sxs-lookup"><span data-stu-id="88a32-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88a32-111">description</span><span class="sxs-lookup"><span data-stu-id="88a32-111">description</span></span>|<span data-ttu-id="88a32-112">String</span><span class="sxs-lookup"><span data-stu-id="88a32-112">String</span></span>|<span data-ttu-id="88a32-113">説明。</span><span class="sxs-lookup"><span data-stu-id="88a32-113">Description.</span></span>|
|<span data-ttu-id="88a32-114">address</span><span class="sxs-lookup"><span data-stu-id="88a32-114">address</span></span>|<span data-ttu-id="88a32-115">String</span><span class="sxs-lookup"><span data-stu-id="88a32-115">String</span></span>|<span data-ttu-id="88a32-116">Address (IP アドレス、FQDN または URL)</span><span class="sxs-lookup"><span data-stu-id="88a32-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="88a32-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="88a32-117">isDefaultServer</span></span>|<span data-ttu-id="88a32-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a32-118">Boolean</span></span>|<span data-ttu-id="88a32-119">既定のサーバー。</span><span class="sxs-lookup"><span data-stu-id="88a32-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88a32-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="88a32-120">Relationships</span></span>
<span data-ttu-id="88a32-121">なし</span><span class="sxs-lookup"><span data-stu-id="88a32-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88a32-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88a32-122">JSON Representation</span></span>
<span data-ttu-id="88a32-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="88a32-123">Here is a JSON representation of the resource.</span></span>
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



