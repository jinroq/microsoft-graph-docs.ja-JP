---
title: office/リソースの種類
description: すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47ee6458d8c045ff99ce244a43e3058d040093fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011975"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="c40a4-103">office/リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c40a4-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="c40a4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c40a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c40a4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c40a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c40a4-106">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="c40a4-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="c40a4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c40a4-107">Methods</span></span>
|<span data-ttu-id="c40a4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c40a4-108">Method</span></span>|<span data-ttu-id="c40a4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c40a4-109">Return Type</span></span>|<span data-ttu-id="c40a4-110">説明</span><span class="sxs-lookup"><span data-stu-id="c40a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c40a4-111">オフィス/全情報の収集</span><span class="sxs-lookup"><span data-stu-id="c40a4-111">Get officeConfiguration</span></span>|[<span data-ttu-id="c40a4-112">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c40a4-112">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="c40a4-113">このオブジェクトのプロパティとリレーションシップ[](../resources/intune-cirrus-officeconfiguration.md)を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c40a4-113">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="c40a4-114">Officeの変更の更新</span><span class="sxs-lookup"><span data-stu-id="c40a4-114">Update officeConfiguration</span></span>|[<span data-ttu-id="c40a4-115">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="c40a4-115">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="c40a4-116">[オフィス](../resources/intune-cirrus-officeconfiguration.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c40a4-116">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c40a4-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c40a4-117">Properties</span></span>
|<span data-ttu-id="c40a4-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c40a4-118">Property</span></span>|<span data-ttu-id="c40a4-119">型</span><span class="sxs-lookup"><span data-stu-id="c40a4-119">Type</span></span>|<span data-ttu-id="c40a4-120">説明</span><span class="sxs-lookup"><span data-stu-id="c40a4-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c40a4-121">id</span><span class="sxs-lookup"><span data-stu-id="c40a4-121">id</span></span>|<span data-ttu-id="c40a4-122">String</span><span class="sxs-lookup"><span data-stu-id="c40a4-122">String</span></span>|<span data-ttu-id="c40a4-123">Office 構成の Id。</span><span class="sxs-lookup"><span data-stu-id="c40a4-123">Id of the office configuration.</span></span>|
|<span data-ttu-id="c40a4-124">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="c40a4-124">tenantCheckinStatuses</span></span>|<span data-ttu-id="c40a4-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c40a4-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="c40a4-126">Office クライアントのチェックイン状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="c40a4-126">List of office Client check-in status.</span></span>|
|<span data-ttu-id="c40a4-127">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c40a4-127">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="c40a4-128">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c40a4-128">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="c40a4-129">テナントのチェックイン statues を記述するエンティティ</span><span class="sxs-lookup"><span data-stu-id="c40a4-129">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="c40a4-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c40a4-130">Relationships</span></span>
|<span data-ttu-id="c40a4-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c40a4-131">Relationship</span></span>|<span data-ttu-id="c40a4-132">型</span><span class="sxs-lookup"><span data-stu-id="c40a4-132">Type</span></span>|<span data-ttu-id="c40a4-133">説明</span><span class="sxs-lookup"><span data-stu-id="c40a4-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c40a4-134">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="c40a4-134">clientConfigurations</span></span>|<span data-ttu-id="c40a4-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c40a4-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="c40a4-136">Office クライアント構成のリスト。</span><span class="sxs-lookup"><span data-stu-id="c40a4-136">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c40a4-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c40a4-137">JSON Representation</span></span>
<span data-ttu-id="c40a4-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c40a4-138">Here is a JSON representation of the resource.</span></span>
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



