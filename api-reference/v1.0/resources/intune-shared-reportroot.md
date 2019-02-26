---
title: reportRoot リソースの種類
description: 履歴レポートのインスタンスを表すリソースです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 98f29935304c5eac2262049f76a9bcf006aa694b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264093"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="22fd9-103">reportRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22fd9-103">reportRoot resource type</span></span>

> <span data-ttu-id="22fd9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22fd9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22fd9-105">履歴レポートのインスタンスを表すリソースです。</span><span class="sxs-lookup"><span data-stu-id="22fd9-105">The resource that represents an instance of History Reports.</span></span>

## <a name="methods"></a><span data-ttu-id="22fd9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="22fd9-106">Methods</span></span>
|<span data-ttu-id="22fd9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="22fd9-107">Method</span></span>|<span data-ttu-id="22fd9-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="22fd9-108">Return Type</span></span>|<span data-ttu-id="22fd9-109">説明</span><span class="sxs-lookup"><span data-stu-id="22fd9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22fd9-110">ReportRoot の取得</span><span class="sxs-lookup"><span data-stu-id="22fd9-110">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="22fd9-111">reportRoot</span><span class="sxs-lookup"><span data-stu-id="22fd9-111">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="22fd9-112">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="22fd9-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="22fd9-113">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="22fd9-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="22fd9-114">reportRoot</span><span class="sxs-lookup"><span data-stu-id="22fd9-114">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="22fd9-115">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="22fd9-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="22fd9-116">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="22fd9-116">**Device configuration**</span></span>|
|[<span data-ttu-id="22fd9-117">deviceConfigurationDeviceActivity function</span><span class="sxs-lookup"><span data-stu-id="22fd9-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="22fd9-118">レポート</span><span class="sxs-lookup"><span data-stu-id="22fd9-118">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="22fd9-119">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="22fd9-119">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="22fd9-120">deviceConfigurationUserActivity function</span><span class="sxs-lookup"><span data-stu-id="22fd9-120">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="22fd9-121">レポート</span><span class="sxs-lookup"><span data-stu-id="22fd9-121">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="22fd9-122">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="22fd9-122">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="22fd9-123">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="22fd9-123">**Troubleshooting**</span></span>|
|[<span data-ttu-id="22fd9-124">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="22fd9-124">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="22fd9-125">レポート</span><span class="sxs-lookup"><span data-stu-id="22fd9-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="22fd9-126">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="22fd9-126">Not yet documented.</span></span>|
|[<span data-ttu-id="22fd9-127">managedDeviceEnrollmentTopFailures 関数</span><span class="sxs-lookup"><span data-stu-id="22fd9-127">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="22fd9-128">レポート</span><span class="sxs-lookup"><span data-stu-id="22fd9-128">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="22fd9-129">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="22fd9-129">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="22fd9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22fd9-130">Properties</span></span>
|<span data-ttu-id="22fd9-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22fd9-131">Property</span></span>|<span data-ttu-id="22fd9-132">型</span><span class="sxs-lookup"><span data-stu-id="22fd9-132">Type</span></span>|<span data-ttu-id="22fd9-133">説明</span><span class="sxs-lookup"><span data-stu-id="22fd9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22fd9-134">id</span><span class="sxs-lookup"><span data-stu-id="22fd9-134">id</span></span>|<span data-ttu-id="22fd9-135">String</span><span class="sxs-lookup"><span data-stu-id="22fd9-135">String</span></span>|<span data-ttu-id="22fd9-136">このエンティティの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="22fd9-136">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22fd9-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="22fd9-137">Relationships</span></span>
<span data-ttu-id="22fd9-138">なし</span><span class="sxs-lookup"><span data-stu-id="22fd9-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22fd9-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22fd9-139">JSON Representation</span></span>
<span data-ttu-id="22fd9-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22fd9-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a><span data-ttu-id="22fd9-141">例</span><span class="sxs-lookup"><span data-stu-id="22fd9-141">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
