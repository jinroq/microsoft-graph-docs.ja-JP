---
title: 組織リソースの種類
description: organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd38274fea11f4312b60719fe04464d9b283fe9c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961377"
---
# <a name="organization-resource-type"></a><span data-ttu-id="6b28e-103">organization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b28e-103">organization resource type</span></span>

> <span data-ttu-id="6b28e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b28e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b28e-105">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="6b28e-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="6b28e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6b28e-106">Methods</span></span>
|<span data-ttu-id="6b28e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6b28e-107">Method</span></span>|<span data-ttu-id="6b28e-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6b28e-108">Return Type</span></span>|<span data-ttu-id="6b28e-109">説明</span><span class="sxs-lookup"><span data-stu-id="6b28e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b28e-110">List organizations</span><span class="sxs-lookup"><span data-stu-id="6b28e-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="6b28e-111">[organization](../resources/intune-onboarding-organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b28e-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="6b28e-112">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6b28e-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="6b28e-113">Get organization</span><span class="sxs-lookup"><span data-stu-id="6b28e-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="6b28e-114">organization</span><span class="sxs-lookup"><span data-stu-id="6b28e-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="6b28e-115">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6b28e-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="6b28e-116">Update organization</span><span class="sxs-lookup"><span data-stu-id="6b28e-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="6b28e-117">organization</span><span class="sxs-lookup"><span data-stu-id="6b28e-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="6b28e-118">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6b28e-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="6b28e-119">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="6b28e-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="6b28e-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6b28e-120">Int32</span></span>|<span data-ttu-id="6b28e-121">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="6b28e-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="6b28e-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b28e-122">Properties</span></span>
|<span data-ttu-id="6b28e-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b28e-123">Property</span></span>|<span data-ttu-id="6b28e-124">型</span><span class="sxs-lookup"><span data-stu-id="6b28e-124">Type</span></span>|<span data-ttu-id="6b28e-125">説明</span><span class="sxs-lookup"><span data-stu-id="6b28e-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b28e-126">ID</span><span class="sxs-lookup"><span data-stu-id="6b28e-126">id</span></span>|<span data-ttu-id="6b28e-127">String</span><span class="sxs-lookup"><span data-stu-id="6b28e-127">String</span></span>|<span data-ttu-id="6b28e-128">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="6b28e-128">The GUID for the object.</span></span>|
|<span data-ttu-id="6b28e-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="6b28e-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="6b28e-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="6b28e-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="6b28e-131">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="6b28e-131">Mobile device management authority.</span></span> <span data-ttu-id="6b28e-132">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="6b28e-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b28e-133">関係</span><span class="sxs-lookup"><span data-stu-id="6b28e-133">Relationships</span></span>
<span data-ttu-id="6b28e-134">なし</span><span class="sxs-lookup"><span data-stu-id="6b28e-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b28e-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b28e-135">JSON Representation</span></span>
<span data-ttu-id="6b28e-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6b28e-136">Here is a JSON representation of the resource.</span></span>
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

