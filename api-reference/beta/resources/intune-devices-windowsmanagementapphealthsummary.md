---
title: windowsManagementAppHealthSummary リソースの種類
description: Windows 管理アプリケーションの健康状態の概要のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 40ba93025059a85a11b061464d04bca4118b88bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843821"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="80e7e-103">windowsManagementAppHealthSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80e7e-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="80e7e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="80e7e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80e7e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80e7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80e7e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80e7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80e7e-107">Windows 管理アプリケーションの健康状態の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="80e7e-107">Contains properties for the health summary of the Windows management app.</span></span>
## <a name="methods"></a><span data-ttu-id="80e7e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="80e7e-108">Methods</span></span>
|<span data-ttu-id="80e7e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="80e7e-109">Method</span></span>|<span data-ttu-id="80e7e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="80e7e-110">Return Type</span></span>|<span data-ttu-id="80e7e-111">説明</span><span class="sxs-lookup"><span data-stu-id="80e7e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="80e7e-112">WindowsManagementAppHealthSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="80e7e-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="80e7e-113">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="80e7e-113">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="80e7e-114">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80e7e-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="80e7e-115">WindowsManagementAppHealthSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="80e7e-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="80e7e-116">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="80e7e-116">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="80e7e-117">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="80e7e-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="80e7e-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80e7e-118">Properties</span></span>
|<span data-ttu-id="80e7e-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80e7e-119">Property</span></span>|<span data-ttu-id="80e7e-120">種類</span><span class="sxs-lookup"><span data-stu-id="80e7e-120">Type</span></span>|<span data-ttu-id="80e7e-121">説明</span><span class="sxs-lookup"><span data-stu-id="80e7e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80e7e-122">ID</span><span class="sxs-lookup"><span data-stu-id="80e7e-122">id</span></span>|<span data-ttu-id="80e7e-123">String</span><span class="sxs-lookup"><span data-stu-id="80e7e-123">String</span></span>|<span data-ttu-id="80e7e-124">Windows 管理アプリケーションの稼働状態の概要エンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="80e7e-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="80e7e-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80e7e-125">healthyDeviceCount</span></span>|<span data-ttu-id="80e7e-126">Int32</span><span class="sxs-lookup"><span data-stu-id="80e7e-126">Int32</span></span>|<span data-ttu-id="80e7e-127">正常なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="80e7e-127">Healthy device count.</span></span>|
|<span data-ttu-id="80e7e-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80e7e-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="80e7e-129">Int32</span><span class="sxs-lookup"><span data-stu-id="80e7e-129">Int32</span></span>|<span data-ttu-id="80e7e-130">問題のあるデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="80e7e-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="80e7e-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80e7e-131">unknownDeviceCount</span></span>|<span data-ttu-id="80e7e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="80e7e-132">Int32</span></span>|<span data-ttu-id="80e7e-133">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="80e7e-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80e7e-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="80e7e-134">Relationships</span></span>
<span data-ttu-id="80e7e-135">なし</span><span class="sxs-lookup"><span data-stu-id="80e7e-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80e7e-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80e7e-136">JSON Representation</span></span>
<span data-ttu-id="80e7e-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80e7e-137">Here is a JSON representation of the resource.</span></span>
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





