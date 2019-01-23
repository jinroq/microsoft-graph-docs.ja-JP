---
title: 組織リソースの種類
description: organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b47ec69063998a935640f05d04a17bfc5714c8d8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398234"
---
# <a name="organization-resource-type"></a><span data-ttu-id="6fb08-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6fb08-103">organization resource type</span></span>

> <span data-ttu-id="6fb08-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6fb08-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6fb08-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fb08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fb08-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6fb08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fb08-107">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="6fb08-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="6fb08-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6fb08-108">Methods</span></span>
|<span data-ttu-id="6fb08-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6fb08-109">Method</span></span>|<span data-ttu-id="6fb08-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6fb08-110">Return Type</span></span>|<span data-ttu-id="6fb08-111">説明</span><span class="sxs-lookup"><span data-stu-id="6fb08-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fb08-112">List organizations</span><span class="sxs-lookup"><span data-stu-id="6fb08-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="6fb08-113">[organization](../resources/intune-onboarding-organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6fb08-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="6fb08-114">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6fb08-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="6fb08-115">Get organization</span><span class="sxs-lookup"><span data-stu-id="6fb08-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="6fb08-116">organization</span><span class="sxs-lookup"><span data-stu-id="6fb08-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="6fb08-117">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6fb08-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="6fb08-118">Update organization</span><span class="sxs-lookup"><span data-stu-id="6fb08-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="6fb08-119">organization</span><span class="sxs-lookup"><span data-stu-id="6fb08-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="6fb08-120">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6fb08-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="6fb08-121">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="6fb08-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="6fb08-122">Int32</span><span class="sxs-lookup"><span data-stu-id="6fb08-122">Int32</span></span>|<span data-ttu-id="6fb08-123">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="6fb08-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="6fb08-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fb08-124">Properties</span></span>
|<span data-ttu-id="6fb08-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fb08-125">Property</span></span>|<span data-ttu-id="6fb08-126">型</span><span class="sxs-lookup"><span data-stu-id="6fb08-126">Type</span></span>|<span data-ttu-id="6fb08-127">説明</span><span class="sxs-lookup"><span data-stu-id="6fb08-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fb08-128">id</span><span class="sxs-lookup"><span data-stu-id="6fb08-128">id</span></span>|<span data-ttu-id="6fb08-129">String</span><span class="sxs-lookup"><span data-stu-id="6fb08-129">String</span></span>|<span data-ttu-id="6fb08-130">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="6fb08-130">The GUID for the object.</span></span>|
|<span data-ttu-id="6fb08-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="6fb08-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="6fb08-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="6fb08-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="6fb08-133">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="6fb08-133">Mobile device management authority.</span></span> <span data-ttu-id="6fb08-134">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="6fb08-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="6fb08-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="6fb08-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="6fb08-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="6fb08-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="6fb08-137">コネクタ証明書の設定です。</span><span class="sxs-lookup"><span data-stu-id="6fb08-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fb08-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6fb08-138">Relationships</span></span>
<span data-ttu-id="6fb08-139">なし</span><span class="sxs-lookup"><span data-stu-id="6fb08-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fb08-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6fb08-140">JSON Representation</span></span>
<span data-ttu-id="6fb08-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6fb08-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```




