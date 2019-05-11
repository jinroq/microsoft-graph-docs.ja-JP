---
title: reportRoot リソースの種類
description: コンテキストに応じて、デバイスのインスタンスまたはトラブルシューティングレポートを表すリソース。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: c975abfa3cb580d107967c7adaf66627bad2ad2e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938731"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="6f25f-103">reportRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f25f-103">reportRoot resource type</span></span>

> <span data-ttu-id="6f25f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f25f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f25f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f25f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f25f-106">コンテキストに応じて、デバイスのインスタンスまたはトラブルシューティングレポートを表すリソース。</span><span class="sxs-lookup"><span data-stu-id="6f25f-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="6f25f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6f25f-107">Methods</span></span>
|<span data-ttu-id="6f25f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6f25f-108">Method</span></span>|<span data-ttu-id="6f25f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6f25f-109">Return Type</span></span>|<span data-ttu-id="6f25f-110">説明</span><span class="sxs-lookup"><span data-stu-id="6f25f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6f25f-111">ReportRoot の取得</span><span class="sxs-lookup"><span data-stu-id="6f25f-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="6f25f-112">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6f25f-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="6f25f-113">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="6f25f-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="6f25f-114">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6f25f-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="6f25f-115">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="6f25f-115">**Device configuration**</span></span>|
|[<span data-ttu-id="6f25f-116">deviceConfigurationUserActivity function</span><span class="sxs-lookup"><span data-stu-id="6f25f-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="6f25f-117">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="6f25f-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="6f25f-118">deviceConfigurationDeviceActivity function</span><span class="sxs-lookup"><span data-stu-id="6f25f-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="6f25f-119">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="6f25f-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="6f25f-120">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="6f25f-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="6f25f-121">managedDeviceEnrollmentAbandonmentDetails 関数</span><span class="sxs-lookup"><span data-stu-id="6f25f-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="6f25f-122">レポート</span><span class="sxs-lookup"><span data-stu-id="6f25f-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="6f25f-123">登録 abandonment 詳細レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="6f25f-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="6f25f-124">managedDeviceEnrollmentAbandonmentSummary 関数</span><span class="sxs-lookup"><span data-stu-id="6f25f-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="6f25f-125">レポート</span><span class="sxs-lookup"><span data-stu-id="6f25f-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="6f25f-126">登録 abandonment の概要レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="6f25f-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="6f25f-127">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="6f25f-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="6f25f-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6f25f-128">Not yet documented</span></span>|
|[<span data-ttu-id="6f25f-129">managedDeviceEnrollmentFailureTrends 関数</span><span class="sxs-lookup"><span data-stu-id="6f25f-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="6f25f-130">登録失敗傾向レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="6f25f-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="6f25f-131">managedDeviceEnrollmentTopFailures 関数</span><span class="sxs-lookup"><span data-stu-id="6f25f-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="6f25f-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6f25f-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6f25f-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f25f-133">Properties</span></span>
|<span data-ttu-id="6f25f-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f25f-134">Property</span></span>|<span data-ttu-id="6f25f-135">型</span><span class="sxs-lookup"><span data-stu-id="6f25f-135">Type</span></span>|<span data-ttu-id="6f25f-136">説明</span><span class="sxs-lookup"><span data-stu-id="6f25f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f25f-137">id</span><span class="sxs-lookup"><span data-stu-id="6f25f-137">id</span></span>|<span data-ttu-id="6f25f-138">String</span><span class="sxs-lookup"><span data-stu-id="6f25f-138">String</span></span>|<span data-ttu-id="6f25f-139">このエンティティの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="6f25f-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f25f-140">関係</span><span class="sxs-lookup"><span data-stu-id="6f25f-140">Relationships</span></span>
<span data-ttu-id="6f25f-141">なし</span><span class="sxs-lookup"><span data-stu-id="6f25f-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f25f-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f25f-142">JSON Representation</span></span>
<span data-ttu-id="6f25f-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6f25f-143">Here is a JSON representation of the resource.</span></span>
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



