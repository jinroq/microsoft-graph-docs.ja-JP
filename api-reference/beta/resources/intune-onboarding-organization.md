---
title: 組織リソースの種類
description: organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c587d5a15fa0161e10058eec4a2f8c6183a28a1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940156"
---
# <a name="organization-resource-type"></a><span data-ttu-id="887fb-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="887fb-103">organization resource type</span></span>

> <span data-ttu-id="887fb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="887fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="887fb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="887fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="887fb-106">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="887fb-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="887fb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="887fb-107">Methods</span></span>
|<span data-ttu-id="887fb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="887fb-108">Method</span></span>|<span data-ttu-id="887fb-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="887fb-109">Return Type</span></span>|<span data-ttu-id="887fb-110">説明</span><span class="sxs-lookup"><span data-stu-id="887fb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="887fb-111">List organizations</span><span class="sxs-lookup"><span data-stu-id="887fb-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="887fb-112">[organization](../resources/intune-onboarding-organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="887fb-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="887fb-113">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="887fb-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="887fb-114">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="887fb-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="887fb-115">organization</span><span class="sxs-lookup"><span data-stu-id="887fb-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="887fb-116">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="887fb-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="887fb-117">Update organization</span><span class="sxs-lookup"><span data-stu-id="887fb-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="887fb-118">organization</span><span class="sxs-lookup"><span data-stu-id="887fb-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="887fb-119">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="887fb-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="887fb-120">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="887fb-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="887fb-121">Int32</span><span class="sxs-lookup"><span data-stu-id="887fb-121">Int32</span></span>|<span data-ttu-id="887fb-122">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="887fb-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="887fb-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="887fb-123">Properties</span></span>
|<span data-ttu-id="887fb-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="887fb-124">Property</span></span>|<span data-ttu-id="887fb-125">型</span><span class="sxs-lookup"><span data-stu-id="887fb-125">Type</span></span>|<span data-ttu-id="887fb-126">説明</span><span class="sxs-lookup"><span data-stu-id="887fb-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="887fb-127">id</span><span class="sxs-lookup"><span data-stu-id="887fb-127">id</span></span>|<span data-ttu-id="887fb-128">String</span><span class="sxs-lookup"><span data-stu-id="887fb-128">String</span></span>|<span data-ttu-id="887fb-129">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="887fb-129">The GUID for the object.</span></span>|
|<span data-ttu-id="887fb-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="887fb-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="887fb-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="887fb-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="887fb-132">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="887fb-132">Mobile device management authority.</span></span> <span data-ttu-id="887fb-133">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="887fb-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="887fb-134">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="887fb-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="887fb-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="887fb-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="887fb-136">証明書コネクタの設定。</span><span class="sxs-lookup"><span data-stu-id="887fb-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="887fb-137">関係</span><span class="sxs-lookup"><span data-stu-id="887fb-137">Relationships</span></span>
<span data-ttu-id="887fb-138">なし</span><span class="sxs-lookup"><span data-stu-id="887fb-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="887fb-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="887fb-139">JSON Representation</span></span>
<span data-ttu-id="887fb-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="887fb-140">Here is a JSON representation of the resource.</span></span>
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




