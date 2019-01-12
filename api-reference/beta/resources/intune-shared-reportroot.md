---
title: reportRoot リソースの種類
description: デバイスまたはコンテキストに応じて、トラブルシューティング レポートのインスタンスを表すリソースです。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: efb8950b9956901161c822df8b467b0182a4cc75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959588"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="ff17c-103">reportRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff17c-103">reportRoot resource type</span></span>

> <span data-ttu-id="ff17c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff17c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff17c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff17c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff17c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff17c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff17c-107">デバイスまたはコンテキストに応じて、トラブルシューティング レポートのインスタンスを表すリソースです。</span><span class="sxs-lookup"><span data-stu-id="ff17c-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="ff17c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff17c-108">Methods</span></span>
|<span data-ttu-id="ff17c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff17c-109">Method</span></span>|<span data-ttu-id="ff17c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ff17c-110">Return Type</span></span>|<span data-ttu-id="ff17c-111">説明</span><span class="sxs-lookup"><span data-stu-id="ff17c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff17c-112">ReportRoot の取得</span><span class="sxs-lookup"><span data-stu-id="ff17c-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="ff17c-113">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ff17c-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="ff17c-114">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="ff17c-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="ff17c-115">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ff17c-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="ff17c-116">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="ff17c-116">**Device configuration**</span></span>|
|[<span data-ttu-id="ff17c-117">deviceConfigurationUserActivity function</span><span class="sxs-lookup"><span data-stu-id="ff17c-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="ff17c-118">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="ff17c-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="ff17c-119">deviceConfigurationDeviceActivity function</span><span class="sxs-lookup"><span data-stu-id="ff17c-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="ff17c-120">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="ff17c-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="ff17c-121">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="ff17c-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="ff17c-122">managedDeviceEnrollmentAbandonmentDetails 関数</span><span class="sxs-lookup"><span data-stu-id="ff17c-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="ff17c-123">レポート</span><span class="sxs-lookup"><span data-stu-id="ff17c-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="ff17c-124">登録放棄の詳細レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="ff17c-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="ff17c-125">managedDeviceEnrollmentAbandonmentSummary 関数</span><span class="sxs-lookup"><span data-stu-id="ff17c-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="ff17c-126">レポート</span><span class="sxs-lookup"><span data-stu-id="ff17c-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="ff17c-127">登録放棄の概要レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="ff17c-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="ff17c-128">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="ff17c-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="ff17c-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ff17c-129">Not yet documented</span></span>|
|[<span data-ttu-id="ff17c-130">managedDeviceEnrollmentFailureTrends 関数</span><span class="sxs-lookup"><span data-stu-id="ff17c-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="ff17c-131">登録の失敗の傾向レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="ff17c-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="ff17c-132">managedDeviceEnrollmentTopFailures 関数</span><span class="sxs-lookup"><span data-stu-id="ff17c-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="ff17c-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ff17c-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ff17c-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff17c-134">Properties</span></span>
|<span data-ttu-id="ff17c-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff17c-135">Property</span></span>|<span data-ttu-id="ff17c-136">種類</span><span class="sxs-lookup"><span data-stu-id="ff17c-136">Type</span></span>|<span data-ttu-id="ff17c-137">説明</span><span class="sxs-lookup"><span data-stu-id="ff17c-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff17c-138">ID</span><span class="sxs-lookup"><span data-stu-id="ff17c-138">id</span></span>|<span data-ttu-id="ff17c-139">String</span><span class="sxs-lookup"><span data-stu-id="ff17c-139">String</span></span>|<span data-ttu-id="ff17c-140">このエンティティの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="ff17c-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff17c-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff17c-141">Relationships</span></span>
<span data-ttu-id="ff17c-142">なし</span><span class="sxs-lookup"><span data-stu-id="ff17c-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff17c-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff17c-143">JSON Representation</span></span>
<span data-ttu-id="ff17c-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff17c-144">Here is a JSON representation of the resource.</span></span>
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



