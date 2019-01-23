---
title: windowsKioskAzureADGroup リソースの種類
description: キオスクの構成の AzureAD グループを識別するに使用するクラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d4c8e0867346253c6501ebe8be490ba56800ab3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392571"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="345c4-103">windowsKioskAzureADGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="345c4-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="345c4-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="345c4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="345c4-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="345c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="345c4-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="345c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="345c4-107">キオスクの構成の AzureAD グループを識別するに使用するクラス</span><span class="sxs-lookup"><span data-stu-id="345c4-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="345c4-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="345c4-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="345c4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="345c4-109">Properties</span></span>
|<span data-ttu-id="345c4-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="345c4-110">Property</span></span>|<span data-ttu-id="345c4-111">型</span><span class="sxs-lookup"><span data-stu-id="345c4-111">Type</span></span>|<span data-ttu-id="345c4-112">説明</span><span class="sxs-lookup"><span data-stu-id="345c4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="345c4-113">displayName</span><span class="sxs-lookup"><span data-stu-id="345c4-113">displayName</span></span>|<span data-ttu-id="345c4-114">String</span><span class="sxs-lookup"><span data-stu-id="345c4-114">String</span></span>|<span data-ttu-id="345c4-115">この構成にキオスクがロックアウトされている AzureAD グループの表示名</span><span class="sxs-lookup"><span data-stu-id="345c4-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="345c4-116">groupId</span><span class="sxs-lookup"><span data-stu-id="345c4-116">groupId</span></span>|<span data-ttu-id="345c4-117">String</span><span class="sxs-lookup"><span data-stu-id="345c4-117">String</span></span>|<span data-ttu-id="345c4-118">この構成にキオスクがロックアウトされている AzureAD グループの ID</span><span class="sxs-lookup"><span data-stu-id="345c4-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="345c4-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="345c4-119">Relationships</span></span>
<span data-ttu-id="345c4-120">なし</span><span class="sxs-lookup"><span data-stu-id="345c4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="345c4-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="345c4-121">JSON Representation</span></span>
<span data-ttu-id="345c4-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="345c4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```




