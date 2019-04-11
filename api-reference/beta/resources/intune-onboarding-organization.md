---
title: 組織リソースの種類
description: organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9806c1d263710ecaef2c04af89926e7568ad94da
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778104"
---
# <a name="organization-resource-type"></a><span data-ttu-id="dd49d-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dd49d-103">organization resource type</span></span>

> <span data-ttu-id="dd49d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd49d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd49d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dd49d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd49d-106">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="dd49d-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="dd49d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="dd49d-107">Methods</span></span>
|<span data-ttu-id="dd49d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dd49d-108">Method</span></span>|<span data-ttu-id="dd49d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dd49d-109">Return Type</span></span>|<span data-ttu-id="dd49d-110">説明</span><span class="sxs-lookup"><span data-stu-id="dd49d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dd49d-111">organizations のリスト</span><span class="sxs-lookup"><span data-stu-id="dd49d-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="dd49d-112">[organization](../resources/intune-onboarding-organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dd49d-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="dd49d-113">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dd49d-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="dd49d-114">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="dd49d-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="dd49d-115">組織</span><span class="sxs-lookup"><span data-stu-id="dd49d-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="dd49d-116">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dd49d-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="dd49d-117">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="dd49d-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="dd49d-118">組織</span><span class="sxs-lookup"><span data-stu-id="dd49d-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="dd49d-119">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dd49d-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="dd49d-120">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="dd49d-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="dd49d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="dd49d-121">Int32</span></span>|<span data-ttu-id="dd49d-122">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="dd49d-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="dd49d-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd49d-123">Properties</span></span>
|<span data-ttu-id="dd49d-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd49d-124">Property</span></span>|<span data-ttu-id="dd49d-125">型</span><span class="sxs-lookup"><span data-stu-id="dd49d-125">Type</span></span>|<span data-ttu-id="dd49d-126">説明</span><span class="sxs-lookup"><span data-stu-id="dd49d-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd49d-127">id</span><span class="sxs-lookup"><span data-stu-id="dd49d-127">id</span></span>|<span data-ttu-id="dd49d-128">String</span><span class="sxs-lookup"><span data-stu-id="dd49d-128">String</span></span>|<span data-ttu-id="dd49d-129">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="dd49d-129">The GUID for the object.</span></span>|
|<span data-ttu-id="dd49d-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="dd49d-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="dd49d-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="dd49d-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="dd49d-132">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="dd49d-132">Mobile device management authority.</span></span> <span data-ttu-id="dd49d-133">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="dd49d-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="dd49d-134">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="dd49d-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="dd49d-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="dd49d-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="dd49d-136">証明書コネクタの設定。</span><span class="sxs-lookup"><span data-stu-id="dd49d-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd49d-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dd49d-137">Relationships</span></span>
<span data-ttu-id="dd49d-138">なし</span><span class="sxs-lookup"><span data-stu-id="dd49d-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd49d-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dd49d-139">JSON Representation</span></span>
<span data-ttu-id="dd49d-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dd49d-140">Here is a JSON representation of the resource.</span></span>
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





