---
title: reportRoot リソースの種類
description: 履歴レポートのインスタンスを表すリソースです。
author: tfitzmac
ms.openlocfilehash: 46b4844487a1cb714dde791e6867c277c1693f66
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303970"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="353fe-103">reportRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="353fe-103">reportRoot resource type</span></span>

> <span data-ttu-id="353fe-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="353fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="353fe-105">履歴レポートのインスタンスを表すリソースです。</span><span class="sxs-lookup"><span data-stu-id="353fe-105">The resource that represents an instance of History Reports.</span></span>
## <a name="methods"></a><span data-ttu-id="353fe-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="353fe-106">Methods</span></span>
|<span data-ttu-id="353fe-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="353fe-107">Method</span></span>|<span data-ttu-id="353fe-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="353fe-108">Return Type</span></span>|<span data-ttu-id="353fe-109">説明</span><span class="sxs-lookup"><span data-stu-id="353fe-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="353fe-110">ReportRoot の取得</span><span class="sxs-lookup"><span data-stu-id="353fe-110">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="353fe-111">reportRoot</span><span class="sxs-lookup"><span data-stu-id="353fe-111">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="353fe-112">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="353fe-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="353fe-113">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="353fe-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="353fe-114">reportRoot</span><span class="sxs-lookup"><span data-stu-id="353fe-114">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="353fe-115">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="353fe-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="353fe-116">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="353fe-116">**Device configuration**</span></span>|
|[<span data-ttu-id="353fe-117">deviceConfigurationDeviceActivity function</span><span class="sxs-lookup"><span data-stu-id="353fe-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="353fe-118">レポート</span><span class="sxs-lookup"><span data-stu-id="353fe-118">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="353fe-119">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="353fe-119">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="353fe-120">deviceConfigurationUserActivity function</span><span class="sxs-lookup"><span data-stu-id="353fe-120">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="353fe-121">レポート</span><span class="sxs-lookup"><span data-stu-id="353fe-121">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="353fe-122">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="353fe-122">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="353fe-123">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="353fe-123">**Troubleshooting**</span></span>|
|[<span data-ttu-id="353fe-124">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="353fe-124">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="353fe-125">レポート</span><span class="sxs-lookup"><span data-stu-id="353fe-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="353fe-126">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="353fe-126">Not yet documented.</span></span>|
|[<span data-ttu-id="353fe-127">managedDeviceEnrollmentTopFailures 関数</span><span class="sxs-lookup"><span data-stu-id="353fe-127">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="353fe-128">レポート</span><span class="sxs-lookup"><span data-stu-id="353fe-128">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="353fe-129">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="353fe-129">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="353fe-130">Properties</span><span class="sxs-lookup"><span data-stu-id="353fe-130">Properties</span></span>
|<span data-ttu-id="353fe-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="353fe-131">Property</span></span>|<span data-ttu-id="353fe-132">種類</span><span class="sxs-lookup"><span data-stu-id="353fe-132">Type</span></span>|<span data-ttu-id="353fe-133">説明</span><span class="sxs-lookup"><span data-stu-id="353fe-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="353fe-134">ID</span><span class="sxs-lookup"><span data-stu-id="353fe-134">id</span></span>|<span data-ttu-id="353fe-135">String</span><span class="sxs-lookup"><span data-stu-id="353fe-135">String</span></span>|<span data-ttu-id="353fe-136">このエンティティの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="353fe-136">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="353fe-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="353fe-137">Relationships</span></span>
<span data-ttu-id="353fe-138">なし</span><span class="sxs-lookup"><span data-stu-id="353fe-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="353fe-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="353fe-139">JSON Representation</span></span>
<span data-ttu-id="353fe-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="353fe-140">Here is a JSON representation of the resource.</span></span>
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

## <a name="example"></a><span data-ttu-id="353fe-141">例</span><span class="sxs-lookup"><span data-stu-id="353fe-141">Example</span></span>

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