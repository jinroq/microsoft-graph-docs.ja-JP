---
title: 組織リソースの種類
description: organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e1afa1ded131844f687fa2dbad1a8e07639b264
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250055"
---
# <a name="organization-resource-type"></a><span data-ttu-id="03677-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03677-103">organization resource type</span></span>

> <span data-ttu-id="03677-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="03677-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03677-105">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="03677-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="03677-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="03677-106">Methods</span></span>
|<span data-ttu-id="03677-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="03677-107">Method</span></span>|<span data-ttu-id="03677-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="03677-108">Return Type</span></span>|<span data-ttu-id="03677-109">説明</span><span class="sxs-lookup"><span data-stu-id="03677-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03677-110">List organizations</span><span class="sxs-lookup"><span data-stu-id="03677-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="03677-111">[organization](../resources/intune-onboarding-organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="03677-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="03677-112">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="03677-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="03677-113">Get organization</span><span class="sxs-lookup"><span data-stu-id="03677-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="03677-114">organization</span><span class="sxs-lookup"><span data-stu-id="03677-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="03677-115">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="03677-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="03677-116">Update organization</span><span class="sxs-lookup"><span data-stu-id="03677-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="03677-117">organization</span><span class="sxs-lookup"><span data-stu-id="03677-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="03677-118">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="03677-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="03677-119">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="03677-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="03677-120">Int32</span><span class="sxs-lookup"><span data-stu-id="03677-120">Int32</span></span>|<span data-ttu-id="03677-121">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="03677-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="03677-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03677-122">Properties</span></span>
|<span data-ttu-id="03677-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03677-123">Property</span></span>|<span data-ttu-id="03677-124">型</span><span class="sxs-lookup"><span data-stu-id="03677-124">Type</span></span>|<span data-ttu-id="03677-125">説明</span><span class="sxs-lookup"><span data-stu-id="03677-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03677-126">id</span><span class="sxs-lookup"><span data-stu-id="03677-126">id</span></span>|<span data-ttu-id="03677-127">String</span><span class="sxs-lookup"><span data-stu-id="03677-127">String</span></span>|<span data-ttu-id="03677-128">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="03677-128">The GUID for the object.</span></span>|
|<span data-ttu-id="03677-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="03677-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="03677-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="03677-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="03677-131">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="03677-131">Mobile device management authority.</span></span> <span data-ttu-id="03677-132">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="03677-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03677-133">関係</span><span class="sxs-lookup"><span data-stu-id="03677-133">Relationships</span></span>
<span data-ttu-id="03677-134">なし</span><span class="sxs-lookup"><span data-stu-id="03677-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03677-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03677-135">JSON Representation</span></span>
<span data-ttu-id="03677-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="03677-136">Here is a JSON representation of the resource.</span></span>
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
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->



