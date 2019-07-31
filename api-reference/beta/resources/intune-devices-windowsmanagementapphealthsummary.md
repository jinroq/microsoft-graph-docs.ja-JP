---
title: windowsManagementAppHealthSummary リソースの種類
description: Windows 管理アプリの正常性の概要のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d54eb789b33a27f7e7c7a62e3a3e37aafff990ce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999361"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="06182-103">windowsManagementAppHealthSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06182-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="06182-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06182-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06182-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06182-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06182-106">Windows 管理アプリの正常性の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="06182-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="06182-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="06182-107">Methods</span></span>
|<span data-ttu-id="06182-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="06182-108">Method</span></span>|<span data-ttu-id="06182-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="06182-109">Return Type</span></span>|<span data-ttu-id="06182-110">説明</span><span class="sxs-lookup"><span data-stu-id="06182-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06182-111">WindowsManagementAppHealthSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="06182-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="06182-112">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="06182-112">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="06182-113">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="06182-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="06182-114">WindowsManagementAppHealthSummary の更新</span><span class="sxs-lookup"><span data-stu-id="06182-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="06182-115">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="06182-115">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="06182-116">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="06182-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06182-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06182-117">Properties</span></span>
|<span data-ttu-id="06182-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06182-118">Property</span></span>|<span data-ttu-id="06182-119">型</span><span class="sxs-lookup"><span data-stu-id="06182-119">Type</span></span>|<span data-ttu-id="06182-120">説明</span><span class="sxs-lookup"><span data-stu-id="06182-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06182-121">id</span><span class="sxs-lookup"><span data-stu-id="06182-121">id</span></span>|<span data-ttu-id="06182-122">String</span><span class="sxs-lookup"><span data-stu-id="06182-122">String</span></span>|<span data-ttu-id="06182-123">Windows management app health summary エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="06182-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="06182-124">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06182-124">healthyDeviceCount</span></span>|<span data-ttu-id="06182-125">Int32</span><span class="sxs-lookup"><span data-stu-id="06182-125">Int32</span></span>|<span data-ttu-id="06182-126">正常なデバイス数。</span><span class="sxs-lookup"><span data-stu-id="06182-126">Healthy device count.</span></span>|
|<span data-ttu-id="06182-127">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06182-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="06182-128">Int32</span><span class="sxs-lookup"><span data-stu-id="06182-128">Int32</span></span>|<span data-ttu-id="06182-129">異常なデバイス数。</span><span class="sxs-lookup"><span data-stu-id="06182-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="06182-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06182-130">unknownDeviceCount</span></span>|<span data-ttu-id="06182-131">Int32</span><span class="sxs-lookup"><span data-stu-id="06182-131">Int32</span></span>|<span data-ttu-id="06182-132">デバイス数が不明です。</span><span class="sxs-lookup"><span data-stu-id="06182-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06182-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06182-133">Relationships</span></span>
<span data-ttu-id="06182-134">なし</span><span class="sxs-lookup"><span data-stu-id="06182-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06182-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06182-135">JSON Representation</span></span>
<span data-ttu-id="06182-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06182-136">Here is a JSON representation of the resource.</span></span>
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





