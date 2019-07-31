---
title: vpnServer リソースの種類
description: VPN サーバーの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ead65c0657ebf999562899da5012d02fe7847a16
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969423"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="bcc1c-103">vpnServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bcc1c-103">vpnServer resource type</span></span>

> <span data-ttu-id="bcc1c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcc1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcc1c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bcc1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcc1c-106">VPN サーバーの定義。</span><span class="sxs-lookup"><span data-stu-id="bcc1c-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="bcc1c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcc1c-107">Properties</span></span>
|<span data-ttu-id="bcc1c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcc1c-108">Property</span></span>|<span data-ttu-id="bcc1c-109">型</span><span class="sxs-lookup"><span data-stu-id="bcc1c-109">Type</span></span>|<span data-ttu-id="bcc1c-110">説明</span><span class="sxs-lookup"><span data-stu-id="bcc1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcc1c-111">description</span><span class="sxs-lookup"><span data-stu-id="bcc1c-111">description</span></span>|<span data-ttu-id="bcc1c-112">String</span><span class="sxs-lookup"><span data-stu-id="bcc1c-112">String</span></span>|<span data-ttu-id="bcc1c-113">説明。</span><span class="sxs-lookup"><span data-stu-id="bcc1c-113">Description.</span></span>|
|<span data-ttu-id="bcc1c-114">address</span><span class="sxs-lookup"><span data-stu-id="bcc1c-114">address</span></span>|<span data-ttu-id="bcc1c-115">String</span><span class="sxs-lookup"><span data-stu-id="bcc1c-115">String</span></span>|<span data-ttu-id="bcc1c-116">Address (IP アドレス、FQDN または URL)</span><span class="sxs-lookup"><span data-stu-id="bcc1c-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="bcc1c-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="bcc1c-117">isDefaultServer</span></span>|<span data-ttu-id="bcc1c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcc1c-118">Boolean</span></span>|<span data-ttu-id="bcc1c-119">既定のサーバー。</span><span class="sxs-lookup"><span data-stu-id="bcc1c-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcc1c-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcc1c-120">Relationships</span></span>
<span data-ttu-id="bcc1c-121">なし</span><span class="sxs-lookup"><span data-stu-id="bcc1c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bcc1c-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bcc1c-122">JSON Representation</span></span>
<span data-ttu-id="bcc1c-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bcc1c-123">Here is a JSON representation of the resource.</span></span>
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





