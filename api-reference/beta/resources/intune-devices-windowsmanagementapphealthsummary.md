---
title: windowsManagementAppHealthSummary リソースの種類
description: Windows 管理アプリケーションの健康状態の概要のプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ca46f61259b8b956439c541bf8d5703a35aa93b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393852"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="90752-103">windowsManagementAppHealthSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90752-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="90752-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="90752-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90752-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90752-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90752-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90752-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90752-107">Windows 管理アプリケーションの健康状態の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="90752-107">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="90752-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="90752-108">Methods</span></span>
|<span data-ttu-id="90752-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="90752-109">Method</span></span>|<span data-ttu-id="90752-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="90752-110">Return Type</span></span>|<span data-ttu-id="90752-111">説明</span><span class="sxs-lookup"><span data-stu-id="90752-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90752-112">WindowsManagementAppHealthSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="90752-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="90752-113">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="90752-113">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="90752-114">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90752-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="90752-115">WindowsManagementAppHealthSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="90752-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="90752-116">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="90752-116">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="90752-117">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="90752-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="90752-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90752-118">Properties</span></span>
|<span data-ttu-id="90752-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90752-119">Property</span></span>|<span data-ttu-id="90752-120">型</span><span class="sxs-lookup"><span data-stu-id="90752-120">Type</span></span>|<span data-ttu-id="90752-121">説明</span><span class="sxs-lookup"><span data-stu-id="90752-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90752-122">id</span><span class="sxs-lookup"><span data-stu-id="90752-122">id</span></span>|<span data-ttu-id="90752-123">String</span><span class="sxs-lookup"><span data-stu-id="90752-123">String</span></span>|<span data-ttu-id="90752-124">Windows 管理アプリケーションの稼働状態の概要エンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="90752-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="90752-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90752-125">healthyDeviceCount</span></span>|<span data-ttu-id="90752-126">Int32</span><span class="sxs-lookup"><span data-stu-id="90752-126">Int32</span></span>|<span data-ttu-id="90752-127">正常なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="90752-127">Healthy device count.</span></span>|
|<span data-ttu-id="90752-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90752-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="90752-129">Int32</span><span class="sxs-lookup"><span data-stu-id="90752-129">Int32</span></span>|<span data-ttu-id="90752-130">問題のあるデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="90752-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="90752-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90752-131">unknownDeviceCount</span></span>|<span data-ttu-id="90752-132">Int32</span><span class="sxs-lookup"><span data-stu-id="90752-132">Int32</span></span>|<span data-ttu-id="90752-133">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="90752-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90752-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="90752-134">Relationships</span></span>
<span data-ttu-id="90752-135">なし</span><span class="sxs-lookup"><span data-stu-id="90752-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90752-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90752-136">JSON Representation</span></span>
<span data-ttu-id="90752-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="90752-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```




