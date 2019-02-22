---
title: office/リソースの種類
description: すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e5c36a23be0ab32a14a08eaff297b832ba5274c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156050"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="bee12-103">office/リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bee12-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="bee12-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bee12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bee12-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bee12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bee12-106">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="bee12-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="bee12-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bee12-107">Methods</span></span>
|<span data-ttu-id="bee12-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bee12-108">Method</span></span>|<span data-ttu-id="bee12-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bee12-109">Return Type</span></span>|<span data-ttu-id="bee12-110">説明</span><span class="sxs-lookup"><span data-stu-id="bee12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bee12-111">オフィス/全情報の収集</span><span class="sxs-lookup"><span data-stu-id="bee12-111">Get officeConfiguration</span></span>|[<span data-ttu-id="bee12-112">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="bee12-112">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="bee12-113">このオブジェクトのプロパティとリレーションシップ[](../resources/intune-cirrus-officeconfiguration.md)を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bee12-113">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="bee12-114">officeの変更の更新</span><span class="sxs-lookup"><span data-stu-id="bee12-114">Update officeConfiguration</span></span>|[<span data-ttu-id="bee12-115">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="bee12-115">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="bee12-116">[オフィス](../resources/intune-cirrus-officeconfiguration.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bee12-116">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bee12-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bee12-117">Properties</span></span>
|<span data-ttu-id="bee12-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bee12-118">Property</span></span>|<span data-ttu-id="bee12-119">型</span><span class="sxs-lookup"><span data-stu-id="bee12-119">Type</span></span>|<span data-ttu-id="bee12-120">説明</span><span class="sxs-lookup"><span data-stu-id="bee12-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bee12-121">id</span><span class="sxs-lookup"><span data-stu-id="bee12-121">id</span></span>|<span data-ttu-id="bee12-122">String</span><span class="sxs-lookup"><span data-stu-id="bee12-122">String</span></span>|<span data-ttu-id="bee12-123">office 構成の Id。</span><span class="sxs-lookup"><span data-stu-id="bee12-123">Id of the office configuration.</span></span>|
|<span data-ttu-id="bee12-124">tenantcheckinstatuses</span><span class="sxs-lookup"><span data-stu-id="bee12-124">tenantCheckinStatuses</span></span>|<span data-ttu-id="bee12-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bee12-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="bee12-126">office クライアントのチェックイン状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="bee12-126">List of office Client check-in status.</span></span>|
|<span data-ttu-id="bee12-127">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bee12-127">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="bee12-128">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bee12-128">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="bee12-129">テナントのチェックイン statues を記述するエンティティ</span><span class="sxs-lookup"><span data-stu-id="bee12-129">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="bee12-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bee12-130">Relationships</span></span>
|<span data-ttu-id="bee12-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bee12-131">Relationship</span></span>|<span data-ttu-id="bee12-132">型</span><span class="sxs-lookup"><span data-stu-id="bee12-132">Type</span></span>|<span data-ttu-id="bee12-133">説明</span><span class="sxs-lookup"><span data-stu-id="bee12-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bee12-134">clientconfigurations</span><span class="sxs-lookup"><span data-stu-id="bee12-134">clientConfigurations</span></span>|<span data-ttu-id="bee12-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bee12-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="bee12-136">office クライアント構成のリスト。</span><span class="sxs-lookup"><span data-stu-id="bee12-136">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bee12-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bee12-137">JSON Representation</span></span>
<span data-ttu-id="bee12-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bee12-138">Here is a JSON representation of the resource.</span></span>
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



