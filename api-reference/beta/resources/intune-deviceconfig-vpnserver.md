---
title: vpnServer リソースの種類
description: VPN サーバーの定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9dd09e7ab0280120dd207424a862696ba087e20c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170463"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="e8502-103">vpnServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8502-103">vpnServer resource type</span></span>

> <span data-ttu-id="e8502-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8502-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8502-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8502-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8502-106">VPN サーバーの定義。</span><span class="sxs-lookup"><span data-stu-id="e8502-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="e8502-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8502-107">Properties</span></span>
|<span data-ttu-id="e8502-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8502-108">Property</span></span>|<span data-ttu-id="e8502-109">型</span><span class="sxs-lookup"><span data-stu-id="e8502-109">Type</span></span>|<span data-ttu-id="e8502-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8502-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8502-111">説明</span><span class="sxs-lookup"><span data-stu-id="e8502-111">description</span></span>|<span data-ttu-id="e8502-112">String</span><span class="sxs-lookup"><span data-stu-id="e8502-112">String</span></span>|<span data-ttu-id="e8502-113">説明。</span><span class="sxs-lookup"><span data-stu-id="e8502-113">Description.</span></span>|
|<span data-ttu-id="e8502-114">address</span><span class="sxs-lookup"><span data-stu-id="e8502-114">address</span></span>|<span data-ttu-id="e8502-115">String</span><span class="sxs-lookup"><span data-stu-id="e8502-115">String</span></span>|<span data-ttu-id="e8502-116">Address (IP アドレス、FQDN または URL)</span><span class="sxs-lookup"><span data-stu-id="e8502-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="e8502-117">isdefaultserver</span><span class="sxs-lookup"><span data-stu-id="e8502-117">isDefaultServer</span></span>|<span data-ttu-id="e8502-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="e8502-118">Boolean</span></span>|<span data-ttu-id="e8502-119">既定のサーバー。</span><span class="sxs-lookup"><span data-stu-id="e8502-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8502-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8502-120">Relationships</span></span>
<span data-ttu-id="e8502-121">なし</span><span class="sxs-lookup"><span data-stu-id="e8502-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8502-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8502-122">JSON Representation</span></span>
<span data-ttu-id="e8502-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8502-123">Here is a JSON representation of the resource.</span></span>
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




