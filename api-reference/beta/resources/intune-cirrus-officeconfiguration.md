---
title: officeConfiguration リソースの種類
description: すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 767782e26dd203e2ab5488b30520d8cbcf44d1e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921361"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="b79ea-103">officeConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b79ea-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="b79ea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b79ea-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b79ea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b79ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b79ea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b79ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b79ea-107">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="b79ea-107">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="b79ea-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b79ea-108">Methods</span></span>
|<span data-ttu-id="b79ea-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b79ea-109">Method</span></span>|<span data-ttu-id="b79ea-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b79ea-110">Return Type</span></span>|<span data-ttu-id="b79ea-111">説明</span><span class="sxs-lookup"><span data-stu-id="b79ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b79ea-112">OfficeConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="b79ea-112">Get officeConfiguration</span></span>|[<span data-ttu-id="b79ea-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b79ea-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="b79ea-114">[OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b79ea-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="b79ea-115">OfficeConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="b79ea-115">Update officeConfiguration</span></span>|[<span data-ttu-id="b79ea-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b79ea-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="b79ea-117">[OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b79ea-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b79ea-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b79ea-118">Properties</span></span>
|<span data-ttu-id="b79ea-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b79ea-119">Property</span></span>|<span data-ttu-id="b79ea-120">型</span><span class="sxs-lookup"><span data-stu-id="b79ea-120">Type</span></span>|<span data-ttu-id="b79ea-121">説明</span><span class="sxs-lookup"><span data-stu-id="b79ea-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b79ea-122">ID</span><span class="sxs-lookup"><span data-stu-id="b79ea-122">id</span></span>|<span data-ttu-id="b79ea-123">String</span><span class="sxs-lookup"><span data-stu-id="b79ea-123">String</span></span>|<span data-ttu-id="b79ea-124">Office の構成の id です。</span><span class="sxs-lookup"><span data-stu-id="b79ea-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="b79ea-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="b79ea-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="b79ea-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b79ea-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="b79ea-127">Office クライアントでは、チェック状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="b79ea-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="b79ea-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b79ea-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="b79ea-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b79ea-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="b79ea-130">テナント チェックインの彫像を記述するエンティティ</span><span class="sxs-lookup"><span data-stu-id="b79ea-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="b79ea-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b79ea-131">Relationships</span></span>
|<span data-ttu-id="b79ea-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b79ea-132">Relationship</span></span>|<span data-ttu-id="b79ea-133">型</span><span class="sxs-lookup"><span data-stu-id="b79ea-133">Type</span></span>|<span data-ttu-id="b79ea-134">説明</span><span class="sxs-lookup"><span data-stu-id="b79ea-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b79ea-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="b79ea-135">clientConfigurations</span></span>|<span data-ttu-id="b79ea-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b79ea-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="b79ea-137">Office クライアントの構成の一覧です。</span><span class="sxs-lookup"><span data-stu-id="b79ea-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b79ea-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b79ea-138">JSON Representation</span></span>
<span data-ttu-id="b79ea-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b79ea-139">Here is a JSON representation of the resource.</span></span>
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



