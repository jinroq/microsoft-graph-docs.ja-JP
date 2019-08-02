---
title: 組織リソースの種類
description: organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: baf50eb876d33c3fdb08f5f4162ce2f0267fa499
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037283"
---
# <a name="organization-resource-type"></a><span data-ttu-id="17bb9-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17bb9-103">organization resource type</span></span>

> <span data-ttu-id="17bb9-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="17bb9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17bb9-105">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="17bb9-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="17bb9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="17bb9-106">Methods</span></span>
|<span data-ttu-id="17bb9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="17bb9-107">Method</span></span>|<span data-ttu-id="17bb9-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="17bb9-108">Return Type</span></span>|<span data-ttu-id="17bb9-109">説明</span><span class="sxs-lookup"><span data-stu-id="17bb9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="17bb9-110">List organizations</span><span class="sxs-lookup"><span data-stu-id="17bb9-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="17bb9-111">[organization](../resources/intune-onboarding-organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17bb9-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="17bb9-112">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="17bb9-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="17bb9-113">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="17bb9-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="17bb9-114">organization</span><span class="sxs-lookup"><span data-stu-id="17bb9-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="17bb9-115">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="17bb9-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="17bb9-116">Update organization</span><span class="sxs-lookup"><span data-stu-id="17bb9-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="17bb9-117">organization</span><span class="sxs-lookup"><span data-stu-id="17bb9-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="17bb9-118">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="17bb9-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="17bb9-119">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="17bb9-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="17bb9-120">Int32</span><span class="sxs-lookup"><span data-stu-id="17bb9-120">Int32</span></span>|<span data-ttu-id="17bb9-121">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="17bb9-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="17bb9-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17bb9-122">Properties</span></span>
|<span data-ttu-id="17bb9-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17bb9-123">Property</span></span>|<span data-ttu-id="17bb9-124">型</span><span class="sxs-lookup"><span data-stu-id="17bb9-124">Type</span></span>|<span data-ttu-id="17bb9-125">説明</span><span class="sxs-lookup"><span data-stu-id="17bb9-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17bb9-126">id</span><span class="sxs-lookup"><span data-stu-id="17bb9-126">id</span></span>|<span data-ttu-id="17bb9-127">String</span><span class="sxs-lookup"><span data-stu-id="17bb9-127">String</span></span>|<span data-ttu-id="17bb9-128">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="17bb9-128">The GUID for the object.</span></span>|
|<span data-ttu-id="17bb9-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="17bb9-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="17bb9-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="17bb9-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="17bb9-131">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="17bb9-131">Mobile device management authority.</span></span> <span data-ttu-id="17bb9-132">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="17bb9-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17bb9-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="17bb9-133">Relationships</span></span>
<span data-ttu-id="17bb9-134">なし</span><span class="sxs-lookup"><span data-stu-id="17bb9-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17bb9-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17bb9-135">JSON Representation</span></span>
<span data-ttu-id="17bb9-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17bb9-136">Here is a JSON representation of the resource.</span></span>
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



