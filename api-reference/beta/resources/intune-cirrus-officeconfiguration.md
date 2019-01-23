---
title: officeConfiguration リソースの種類
description: すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc76295b21602328689ee48f8aed8be74bd82093
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406550"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="f9778-103">officeConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f9778-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="f9778-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9778-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9778-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9778-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9778-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9778-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9778-107">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="f9778-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="f9778-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f9778-108">Methods</span></span>
|<span data-ttu-id="f9778-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f9778-109">Method</span></span>|<span data-ttu-id="f9778-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f9778-110">Return Type</span></span>|<span data-ttu-id="f9778-111">説明</span><span class="sxs-lookup"><span data-stu-id="f9778-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9778-112">OfficeConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="f9778-112">Get officeConfiguration</span></span>|[<span data-ttu-id="f9778-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9778-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="f9778-114">[OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9778-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="f9778-115">OfficeConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="f9778-115">Update officeConfiguration</span></span>|[<span data-ttu-id="f9778-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9778-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="f9778-117">[OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f9778-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9778-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9778-118">Properties</span></span>
|<span data-ttu-id="f9778-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9778-119">Property</span></span>|<span data-ttu-id="f9778-120">型</span><span class="sxs-lookup"><span data-stu-id="f9778-120">Type</span></span>|<span data-ttu-id="f9778-121">説明</span><span class="sxs-lookup"><span data-stu-id="f9778-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9778-122">id</span><span class="sxs-lookup"><span data-stu-id="f9778-122">id</span></span>|<span data-ttu-id="f9778-123">String</span><span class="sxs-lookup"><span data-stu-id="f9778-123">String</span></span>|<span data-ttu-id="f9778-124">Office の構成の id です。</span><span class="sxs-lookup"><span data-stu-id="f9778-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="f9778-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="f9778-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="f9778-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f9778-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="f9778-127">Office クライアントでは、チェック状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f9778-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="f9778-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="f9778-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="f9778-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="f9778-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="f9778-130">テナント チェックインの彫像を記述するエンティティ</span><span class="sxs-lookup"><span data-stu-id="f9778-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9778-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f9778-131">Relationships</span></span>
|<span data-ttu-id="f9778-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f9778-132">Relationship</span></span>|<span data-ttu-id="f9778-133">型</span><span class="sxs-lookup"><span data-stu-id="f9778-133">Type</span></span>|<span data-ttu-id="f9778-134">説明</span><span class="sxs-lookup"><span data-stu-id="f9778-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9778-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="f9778-135">clientConfigurations</span></span>|<span data-ttu-id="f9778-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f9778-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="f9778-137">Office クライアントの構成の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f9778-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9778-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f9778-138">JSON Representation</span></span>
<span data-ttu-id="f9778-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f9778-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```



