---
title: windowsManagementAppHealthSummary リソースの種類
description: Windows 管理アプリケーションの健康状態の概要のプロパティが含まれています。
ms.openlocfilehash: dddcb40a0a66446ab6e87a2e684c1dbf0df547fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070112"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="e035f-103">windowsManagementAppHealthSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e035f-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="e035f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e035f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e035f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e035f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e035f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e035f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e035f-107">Windows 管理アプリケーションの健康状態の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e035f-107">Contains properties for the health summary of the Windows management app.</span></span>
## <a name="methods"></a><span data-ttu-id="e035f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e035f-108">Methods</span></span>
|<span data-ttu-id="e035f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e035f-109">Method</span></span>|<span data-ttu-id="e035f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e035f-110">Return Type</span></span>|<span data-ttu-id="e035f-111">説明</span><span class="sxs-lookup"><span data-stu-id="e035f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e035f-112">WindowsManagementAppHealthSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="e035f-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="e035f-113">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="e035f-113">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="e035f-114">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e035f-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="e035f-115">WindowsManagementAppHealthSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="e035f-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="e035f-116">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="e035f-116">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="e035f-117">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e035f-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e035f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e035f-118">Properties</span></span>
|<span data-ttu-id="e035f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e035f-119">Property</span></span>|<span data-ttu-id="e035f-120">型</span><span class="sxs-lookup"><span data-stu-id="e035f-120">Type</span></span>|<span data-ttu-id="e035f-121">説明</span><span class="sxs-lookup"><span data-stu-id="e035f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e035f-122">id</span><span class="sxs-lookup"><span data-stu-id="e035f-122">id</span></span>|<span data-ttu-id="e035f-123">String</span><span class="sxs-lookup"><span data-stu-id="e035f-123">String</span></span>|<span data-ttu-id="e035f-124">Windows 管理アプリケーションの稼働状態の概要エンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="e035f-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="e035f-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e035f-125">healthyDeviceCount</span></span>|<span data-ttu-id="e035f-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e035f-126">Int32</span></span>|<span data-ttu-id="e035f-127">正常なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e035f-127">Healthy device count.</span></span>|
|<span data-ttu-id="e035f-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e035f-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="e035f-129">Int32</span><span class="sxs-lookup"><span data-stu-id="e035f-129">Int32</span></span>|<span data-ttu-id="e035f-130">問題のあるデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e035f-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="e035f-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e035f-131">unknownDeviceCount</span></span>|<span data-ttu-id="e035f-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e035f-132">Int32</span></span>|<span data-ttu-id="e035f-133">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e035f-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e035f-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e035f-134">Relationships</span></span>
<span data-ttu-id="e035f-135">なし</span><span class="sxs-lookup"><span data-stu-id="e035f-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e035f-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e035f-136">JSON Representation</span></span>
<span data-ttu-id="e035f-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e035f-137">Here is a JSON representation of the resource.</span></span>
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





