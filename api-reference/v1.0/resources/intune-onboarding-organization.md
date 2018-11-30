---
title: 組織リソースの種類
description: organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。
ms.openlocfilehash: ddc3b47777ea586a0f31c0d1d18aaa5727c828e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022277"
---
# <a name="organization-resource-type"></a><span data-ttu-id="ec786-103">organization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ec786-103">organization resource type</span></span>

> <span data-ttu-id="ec786-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec786-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec786-105">organization リソースは、グローバル設定インスタンスと、テナント レベルで操作およびプロビジョニングされるリソースを表わします。</span><span class="sxs-lookup"><span data-stu-id="ec786-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="ec786-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ec786-106">Methods</span></span>
|<span data-ttu-id="ec786-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ec786-107">Method</span></span>|<span data-ttu-id="ec786-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ec786-108">Return Type</span></span>|<span data-ttu-id="ec786-109">説明</span><span class="sxs-lookup"><span data-stu-id="ec786-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ec786-110">List organizations</span><span class="sxs-lookup"><span data-stu-id="ec786-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="ec786-111">[organization](../resources/intune-onboarding-organization.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ec786-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="ec786-112">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ec786-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="ec786-113">Get organization</span><span class="sxs-lookup"><span data-stu-id="ec786-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="ec786-114">organization</span><span class="sxs-lookup"><span data-stu-id="ec786-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ec786-115">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ec786-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ec786-116">Update organization</span><span class="sxs-lookup"><span data-stu-id="ec786-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="ec786-117">organization</span><span class="sxs-lookup"><span data-stu-id="ec786-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ec786-118">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ec786-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ec786-119">setMobileDeviceManagementAuthority アクション</span><span class="sxs-lookup"><span data-stu-id="ec786-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="ec786-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ec786-120">Int32</span></span>|<span data-ttu-id="ec786-121">モバイル デバイス管理権限の設定</span><span class="sxs-lookup"><span data-stu-id="ec786-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="ec786-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec786-122">Properties</span></span>
|<span data-ttu-id="ec786-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec786-123">Property</span></span>|<span data-ttu-id="ec786-124">型</span><span class="sxs-lookup"><span data-stu-id="ec786-124">Type</span></span>|<span data-ttu-id="ec786-125">説明</span><span class="sxs-lookup"><span data-stu-id="ec786-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec786-126">id</span><span class="sxs-lookup"><span data-stu-id="ec786-126">id</span></span>|<span data-ttu-id="ec786-127">String</span><span class="sxs-lookup"><span data-stu-id="ec786-127">String</span></span>|<span data-ttu-id="ec786-128">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="ec786-128">The GUID for the object.</span></span>|
|<span data-ttu-id="ec786-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ec786-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="ec786-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="ec786-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="ec786-131">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="ec786-131">Mobile device management authority.</span></span> <span data-ttu-id="ec786-132">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="ec786-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec786-133">関係</span><span class="sxs-lookup"><span data-stu-id="ec786-133">Relationships</span></span>
<span data-ttu-id="ec786-134">なし</span><span class="sxs-lookup"><span data-stu-id="ec786-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ec786-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ec786-135">JSON Representation</span></span>
<span data-ttu-id="ec786-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ec786-136">Here is a JSON representation of the resource.</span></span>
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

