---
title: windowsKioskLocalGroup リソースの種類
description: キオスクの構成にローカル グループを識別するために使用するクラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1134b6a842b54dc49fcd15a92d21aef227b35182
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424631"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="82dc6-103">windowsKioskLocalGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82dc6-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="82dc6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="82dc6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82dc6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82dc6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82dc6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82dc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82dc6-107">キオスクの構成にローカル グループを識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="82dc6-107">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="82dc6-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="82dc6-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82dc6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82dc6-109">Properties</span></span>
|<span data-ttu-id="82dc6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82dc6-110">Property</span></span>|<span data-ttu-id="82dc6-111">型</span><span class="sxs-lookup"><span data-stu-id="82dc6-111">Type</span></span>|<span data-ttu-id="82dc6-112">説明</span><span class="sxs-lookup"><span data-stu-id="82dc6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82dc6-113">グループ名</span><span class="sxs-lookup"><span data-stu-id="82dc6-113">groupName</span></span>|<span data-ttu-id="82dc6-114">String</span><span class="sxs-lookup"><span data-stu-id="82dc6-114">String</span></span>|<span data-ttu-id="82dc6-115">この構成にキオスクがロックアウトされているローカル グループの名前</span><span class="sxs-lookup"><span data-stu-id="82dc6-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="82dc6-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82dc6-116">Relationships</span></span>
<span data-ttu-id="82dc6-117">なし</span><span class="sxs-lookup"><span data-stu-id="82dc6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82dc6-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82dc6-118">JSON Representation</span></span>
<span data-ttu-id="82dc6-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82dc6-119">Here is a JSON representation of the resource.</span></span>
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




