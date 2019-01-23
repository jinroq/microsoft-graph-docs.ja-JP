---
title: reportRoot リソースの種類
description: デバイスまたはコンテキストに応じて、トラブルシューティング レポートのインスタンスを表すリソースです。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 378f1758773bfcffda5d9039d3b60d4ac4bd5cc5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421334"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="303b0-103">reportRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="303b0-103">reportRoot resource type</span></span>

> <span data-ttu-id="303b0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="303b0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="303b0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="303b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="303b0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="303b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="303b0-107">デバイスまたはコンテキストに応じて、トラブルシューティング レポートのインスタンスを表すリソースです。</span><span class="sxs-lookup"><span data-stu-id="303b0-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="303b0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="303b0-108">Methods</span></span>
|<span data-ttu-id="303b0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="303b0-109">Method</span></span>|<span data-ttu-id="303b0-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="303b0-110">Return Type</span></span>|<span data-ttu-id="303b0-111">説明</span><span class="sxs-lookup"><span data-stu-id="303b0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="303b0-112">ReportRoot の取得</span><span class="sxs-lookup"><span data-stu-id="303b0-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="303b0-113">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="303b0-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="303b0-114">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="303b0-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="303b0-115">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="303b0-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="303b0-116">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="303b0-116">**Device configuration**</span></span>|
|[<span data-ttu-id="303b0-117">deviceConfigurationUserActivity function</span><span class="sxs-lookup"><span data-stu-id="303b0-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="303b0-118">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="303b0-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="303b0-119">deviceConfigurationDeviceActivity function</span><span class="sxs-lookup"><span data-stu-id="303b0-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="303b0-120">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="303b0-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="303b0-121">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="303b0-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="303b0-122">managedDeviceEnrollmentAbandonmentDetails 関数</span><span class="sxs-lookup"><span data-stu-id="303b0-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="303b0-123">レポート</span><span class="sxs-lookup"><span data-stu-id="303b0-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="303b0-124">登録放棄の詳細レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="303b0-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="303b0-125">managedDeviceEnrollmentAbandonmentSummary 関数</span><span class="sxs-lookup"><span data-stu-id="303b0-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="303b0-126">レポート</span><span class="sxs-lookup"><span data-stu-id="303b0-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="303b0-127">登録放棄の概要レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="303b0-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="303b0-128">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="303b0-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="303b0-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="303b0-129">Not yet documented</span></span>|
|[<span data-ttu-id="303b0-130">managedDeviceEnrollmentFailureTrends 関数</span><span class="sxs-lookup"><span data-stu-id="303b0-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="303b0-131">登録の失敗の傾向レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="303b0-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="303b0-132">managedDeviceEnrollmentTopFailures 関数</span><span class="sxs-lookup"><span data-stu-id="303b0-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="303b0-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="303b0-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="303b0-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="303b0-134">Properties</span></span>
|<span data-ttu-id="303b0-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="303b0-135">Property</span></span>|<span data-ttu-id="303b0-136">型</span><span class="sxs-lookup"><span data-stu-id="303b0-136">Type</span></span>|<span data-ttu-id="303b0-137">説明</span><span class="sxs-lookup"><span data-stu-id="303b0-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="303b0-138">id</span><span class="sxs-lookup"><span data-stu-id="303b0-138">id</span></span>|<span data-ttu-id="303b0-139">String</span><span class="sxs-lookup"><span data-stu-id="303b0-139">String</span></span>|<span data-ttu-id="303b0-140">このエンティティの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="303b0-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="303b0-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="303b0-141">Relationships</span></span>
<span data-ttu-id="303b0-142">なし</span><span class="sxs-lookup"><span data-stu-id="303b0-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="303b0-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="303b0-143">JSON Representation</span></span>
<span data-ttu-id="303b0-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="303b0-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



