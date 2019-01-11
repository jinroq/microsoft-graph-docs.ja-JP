---
title: 組織リソースの種類
description: organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7c6f99c378bc7fd53f473419a5ca4f4350f7c57b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812048"
---
# <a name="organization-resource-type"></a><span data-ttu-id="4fef4-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fef4-103">organization resource type</span></span>

> <span data-ttu-id="4fef4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4fef4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fef4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fef4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fef4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4fef4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fef4-107">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="4fef4-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="4fef4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fef4-108">Methods</span></span>
|<span data-ttu-id="4fef4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fef4-109">Method</span></span>|<span data-ttu-id="4fef4-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4fef4-110">Return Type</span></span>|<span data-ttu-id="4fef4-111">説明</span><span class="sxs-lookup"><span data-stu-id="4fef4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4fef4-112">List organizations</span><span class="sxs-lookup"><span data-stu-id="4fef4-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="4fef4-113">[organization](../resources/intune-onboarding-organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fef4-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="4fef4-114">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4fef4-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="4fef4-115">Get organization</span><span class="sxs-lookup"><span data-stu-id="4fef4-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="4fef4-116">organization</span><span class="sxs-lookup"><span data-stu-id="4fef4-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="4fef4-117">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4fef4-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="4fef4-118">Update organization</span><span class="sxs-lookup"><span data-stu-id="4fef4-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="4fef4-119">organization</span><span class="sxs-lookup"><span data-stu-id="4fef4-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="4fef4-120">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4fef4-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="4fef4-121">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="4fef4-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="4fef4-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4fef4-122">Int32</span></span>|<span data-ttu-id="4fef4-123">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="4fef4-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="4fef4-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fef4-124">Properties</span></span>
|<span data-ttu-id="4fef4-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fef4-125">Property</span></span>|<span data-ttu-id="4fef4-126">種類</span><span class="sxs-lookup"><span data-stu-id="4fef4-126">Type</span></span>|<span data-ttu-id="4fef4-127">説明</span><span class="sxs-lookup"><span data-stu-id="4fef4-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fef4-128">ID</span><span class="sxs-lookup"><span data-stu-id="4fef4-128">id</span></span>|<span data-ttu-id="4fef4-129">String</span><span class="sxs-lookup"><span data-stu-id="4fef4-129">String</span></span>|<span data-ttu-id="4fef4-130">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="4fef4-130">The GUID for the object.</span></span>|
|<span data-ttu-id="4fef4-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="4fef4-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="4fef4-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="4fef4-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="4fef4-133">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="4fef4-133">Mobile device management authority.</span></span> <span data-ttu-id="4fef4-134">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="4fef4-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="4fef4-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="4fef4-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="4fef4-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="4fef4-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="4fef4-137">コネクタ証明書の設定です。</span><span class="sxs-lookup"><span data-stu-id="4fef4-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fef4-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fef4-138">Relationships</span></span>
<span data-ttu-id="4fef4-139">なし</span><span class="sxs-lookup"><span data-stu-id="4fef4-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4fef4-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fef4-140">JSON Representation</span></span>
<span data-ttu-id="4fef4-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4fef4-141">Here is a JSON representation of the resource.</span></span>
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





