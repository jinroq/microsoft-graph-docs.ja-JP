---
title: officeConfiguration リソースの種類
description: すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
author: tfitzmac
ms.openlocfilehash: bf74789d4debda00b21173ff2974db8224cd15f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305545"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="d8401-103">officeConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d8401-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="d8401-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d8401-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8401-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8401-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8401-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8401-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8401-107">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="d8401-107">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="d8401-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8401-108">Methods</span></span>
|<span data-ttu-id="d8401-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8401-109">Method</span></span>|<span data-ttu-id="d8401-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d8401-110">Return Type</span></span>|<span data-ttu-id="d8401-111">説明</span><span class="sxs-lookup"><span data-stu-id="d8401-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8401-112">OfficeConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="d8401-112">Get officeConfiguration</span></span>|[<span data-ttu-id="d8401-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8401-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="d8401-114">[OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8401-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="d8401-115">OfficeConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="d8401-115">Update officeConfiguration</span></span>|[<span data-ttu-id="d8401-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8401-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="d8401-117">[OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d8401-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8401-118">Properties</span><span class="sxs-lookup"><span data-stu-id="d8401-118">Properties</span></span>
|<span data-ttu-id="d8401-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8401-119">Property</span></span>|<span data-ttu-id="d8401-120">種類</span><span class="sxs-lookup"><span data-stu-id="d8401-120">Type</span></span>|<span data-ttu-id="d8401-121">説明</span><span class="sxs-lookup"><span data-stu-id="d8401-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8401-122">ID</span><span class="sxs-lookup"><span data-stu-id="d8401-122">id</span></span>|<span data-ttu-id="d8401-123">String</span><span class="sxs-lookup"><span data-stu-id="d8401-123">String</span></span>|<span data-ttu-id="d8401-124">Office の構成の id です。</span><span class="sxs-lookup"><span data-stu-id="d8401-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="d8401-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="d8401-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="d8401-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d8401-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="d8401-127">Office クライアントでは、チェック状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="d8401-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="d8401-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d8401-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="d8401-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d8401-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="d8401-130">テナント チェックインの彫像を記述するエンティティ</span><span class="sxs-lookup"><span data-stu-id="d8401-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8401-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8401-131">Relationships</span></span>
|<span data-ttu-id="d8401-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8401-132">Relationship</span></span>|<span data-ttu-id="d8401-133">型</span><span class="sxs-lookup"><span data-stu-id="d8401-133">Type</span></span>|<span data-ttu-id="d8401-134">説明</span><span class="sxs-lookup"><span data-stu-id="d8401-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8401-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="d8401-135">clientConfigurations</span></span>|<span data-ttu-id="d8401-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d8401-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="d8401-137">Office クライアントの構成の一覧です。</span><span class="sxs-lookup"><span data-stu-id="d8401-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8401-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8401-138">JSON Representation</span></span>
<span data-ttu-id="d8401-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d8401-139">Here is a JSON representation of the resource.</span></span>
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



