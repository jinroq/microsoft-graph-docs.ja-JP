---
title: reportRoot リソースの種類
description: 履歴レポートのインスタンスを表すリソースです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a8fa8011ad4550ec80acd0b4d6d2159f10647de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036863"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="0bc66-103">reportRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0bc66-103">reportRoot resource type</span></span>

> <span data-ttu-id="0bc66-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0bc66-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bc66-105">履歴レポートのインスタンスを表すリソースです。</span><span class="sxs-lookup"><span data-stu-id="0bc66-105">The resource that represents an instance of History Reports.</span></span>

## <a name="methods"></a><span data-ttu-id="0bc66-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0bc66-106">Methods</span></span>
|<span data-ttu-id="0bc66-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0bc66-107">Method</span></span>|<span data-ttu-id="0bc66-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0bc66-108">Return Type</span></span>|<span data-ttu-id="0bc66-109">説明</span><span class="sxs-lookup"><span data-stu-id="0bc66-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0bc66-110">ReportRoot の取得</span><span class="sxs-lookup"><span data-stu-id="0bc66-110">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="0bc66-111">reportRoot</span><span class="sxs-lookup"><span data-stu-id="0bc66-111">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="0bc66-112">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0bc66-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="0bc66-113">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="0bc66-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="0bc66-114">reportRoot</span><span class="sxs-lookup"><span data-stu-id="0bc66-114">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="0bc66-115">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0bc66-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="0bc66-116">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="0bc66-116">**Device configuration**</span></span>|
|[<span data-ttu-id="0bc66-117">deviceConfigurationDeviceActivity function</span><span class="sxs-lookup"><span data-stu-id="0bc66-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="0bc66-118">レポート</span><span class="sxs-lookup"><span data-stu-id="0bc66-118">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="0bc66-119">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="0bc66-119">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="0bc66-120">deviceConfigurationUserActivity function</span><span class="sxs-lookup"><span data-stu-id="0bc66-120">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="0bc66-121">レポート</span><span class="sxs-lookup"><span data-stu-id="0bc66-121">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="0bc66-122">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="0bc66-122">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="0bc66-123">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="0bc66-123">**Troubleshooting**</span></span>|
|[<span data-ttu-id="0bc66-124">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="0bc66-124">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="0bc66-125">レポート</span><span class="sxs-lookup"><span data-stu-id="0bc66-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="0bc66-126">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="0bc66-126">Not yet documented.</span></span>|
|[<span data-ttu-id="0bc66-127">managedDeviceEnrollmentTopFailures 関数</span><span class="sxs-lookup"><span data-stu-id="0bc66-127">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="0bc66-128">レポート</span><span class="sxs-lookup"><span data-stu-id="0bc66-128">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="0bc66-129">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="0bc66-129">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="0bc66-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bc66-130">Properties</span></span>
|<span data-ttu-id="0bc66-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bc66-131">Property</span></span>|<span data-ttu-id="0bc66-132">型</span><span class="sxs-lookup"><span data-stu-id="0bc66-132">Type</span></span>|<span data-ttu-id="0bc66-133">説明</span><span class="sxs-lookup"><span data-stu-id="0bc66-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bc66-134">id</span><span class="sxs-lookup"><span data-stu-id="0bc66-134">id</span></span>|<span data-ttu-id="0bc66-135">String</span><span class="sxs-lookup"><span data-stu-id="0bc66-135">String</span></span>|<span data-ttu-id="0bc66-136">このエンティティの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="0bc66-136">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bc66-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0bc66-137">Relationships</span></span>
<span data-ttu-id="0bc66-138">なし</span><span class="sxs-lookup"><span data-stu-id="0bc66-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bc66-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0bc66-139">JSON Representation</span></span>
<span data-ttu-id="0bc66-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0bc66-140">Here is a JSON representation of the resource.</span></span>
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

## <a name="example"></a><span data-ttu-id="0bc66-141">例</span><span class="sxs-lookup"><span data-stu-id="0bc66-141">Example</span></span>

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
