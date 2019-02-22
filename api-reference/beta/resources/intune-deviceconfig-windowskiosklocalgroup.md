---
title: windowsKioskLocalGroup リソースの種類
description: キオスク構成のローカルグループを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3479226d770c7030fefed1a7f2f65a02808479d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169525"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="4c7dc-103">windowsKioskLocalGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c7dc-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="4c7dc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c7dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c7dc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c7dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c7dc-106">キオスク構成のローカルグループを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="4c7dc-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="4c7dc-107">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="4c7dc-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c7dc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c7dc-108">Properties</span></span>
|<span data-ttu-id="4c7dc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c7dc-109">Property</span></span>|<span data-ttu-id="4c7dc-110">型</span><span class="sxs-lookup"><span data-stu-id="4c7dc-110">Type</span></span>|<span data-ttu-id="4c7dc-111">説明</span><span class="sxs-lookup"><span data-stu-id="4c7dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c7dc-112">groupName</span><span class="sxs-lookup"><span data-stu-id="4c7dc-112">groupName</span></span>|<span data-ttu-id="4c7dc-113">String</span><span class="sxs-lookup"><span data-stu-id="4c7dc-113">String</span></span>|<span data-ttu-id="4c7dc-114">このキオスク構成にロックされるローカルグループの名前</span><span class="sxs-lookup"><span data-stu-id="4c7dc-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c7dc-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4c7dc-115">Relationships</span></span>
<span data-ttu-id="4c7dc-116">なし</span><span class="sxs-lookup"><span data-stu-id="4c7dc-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c7dc-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c7dc-117">JSON Representation</span></span>
<span data-ttu-id="4c7dc-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4c7dc-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```




