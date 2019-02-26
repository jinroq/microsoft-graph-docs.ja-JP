---
title: windowsManagementAppHealthSummary リソースの種類
description: Windows 管理アプリの正常性の概要のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f62f5967702143149176cecd2513478256ead6d3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172059"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="bc020-103">windowsManagementAppHealthSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc020-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="bc020-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc020-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc020-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc020-106">Windows 管理アプリの正常性の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bc020-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="bc020-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc020-107">Methods</span></span>
|<span data-ttu-id="bc020-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc020-108">Method</span></span>|<span data-ttu-id="bc020-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bc020-109">Return Type</span></span>|<span data-ttu-id="bc020-110">説明</span><span class="sxs-lookup"><span data-stu-id="bc020-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc020-111">windowsManagementAppHealthSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="bc020-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="bc020-112">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="bc020-112">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="bc020-113">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bc020-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="bc020-114">windowsManagementAppHealthSummary の更新</span><span class="sxs-lookup"><span data-stu-id="bc020-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="bc020-115">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="bc020-115">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="bc020-116">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc020-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc020-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc020-117">Properties</span></span>
|<span data-ttu-id="bc020-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc020-118">Property</span></span>|<span data-ttu-id="bc020-119">型</span><span class="sxs-lookup"><span data-stu-id="bc020-119">Type</span></span>|<span data-ttu-id="bc020-120">説明</span><span class="sxs-lookup"><span data-stu-id="bc020-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc020-121">id</span><span class="sxs-lookup"><span data-stu-id="bc020-121">id</span></span>|<span data-ttu-id="bc020-122">String</span><span class="sxs-lookup"><span data-stu-id="bc020-122">String</span></span>|<span data-ttu-id="bc020-123">Windows management app health summary エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bc020-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="bc020-124">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc020-124">healthyDeviceCount</span></span>|<span data-ttu-id="bc020-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bc020-125">Int32</span></span>|<span data-ttu-id="bc020-126">正常なデバイス数。</span><span class="sxs-lookup"><span data-stu-id="bc020-126">Healthy device count.</span></span>|
|<span data-ttu-id="bc020-127">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc020-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="bc020-128">Int32</span><span class="sxs-lookup"><span data-stu-id="bc020-128">Int32</span></span>|<span data-ttu-id="bc020-129">異常なデバイス数。</span><span class="sxs-lookup"><span data-stu-id="bc020-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="bc020-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc020-130">unknownDeviceCount</span></span>|<span data-ttu-id="bc020-131">Int32</span><span class="sxs-lookup"><span data-stu-id="bc020-131">Int32</span></span>|<span data-ttu-id="bc020-132">デバイス数が不明です。</span><span class="sxs-lookup"><span data-stu-id="bc020-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc020-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc020-133">Relationships</span></span>
<span data-ttu-id="bc020-134">なし</span><span class="sxs-lookup"><span data-stu-id="bc020-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc020-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc020-135">JSON Representation</span></span>
<span data-ttu-id="bc020-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bc020-136">Here is a JSON representation of the resource.</span></span>
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




