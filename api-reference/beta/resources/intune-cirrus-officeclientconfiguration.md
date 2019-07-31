---
title: officeClientConfiguration リソースの種類
description: Office クライアントの構成。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3688503cf19d8cebe51b4afe7abd1563257f9192
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004763"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="e42ee-103">officeClientConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e42ee-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="e42ee-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e42ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e42ee-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e42ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e42ee-106">Office クライアントの構成。</span><span class="sxs-lookup"><span data-stu-id="e42ee-106">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="e42ee-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e42ee-107">Methods</span></span>
|<span data-ttu-id="e42ee-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e42ee-108">Method</span></span>|<span data-ttu-id="e42ee-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e42ee-109">Return Type</span></span>|<span data-ttu-id="e42ee-110">説明</span><span class="sxs-lookup"><span data-stu-id="e42ee-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e42ee-111">リスト officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="e42ee-111">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="e42ee-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e42ee-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="e42ee-113">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e42ee-113">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="e42ee-114">OfficeClientConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="e42ee-114">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="e42ee-115">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="e42ee-115">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="e42ee-116">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e42ee-116">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e42ee-117">assign アクション</span><span class="sxs-lookup"><span data-stu-id="e42ee-117">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="e42ee-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e42ee-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e42ee-119">ポリシーの対象グループをすべて置換します。</span><span class="sxs-lookup"><span data-stu-id="e42ee-119">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="e42ee-120">updatePriorities アクション</span><span class="sxs-lookup"><span data-stu-id="e42ee-120">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="e42ee-121">None</span><span class="sxs-lookup"><span data-stu-id="e42ee-121">None</span></span>|<span data-ttu-id="e42ee-122">ポリシーの優先度を更新します。</span><span class="sxs-lookup"><span data-stu-id="e42ee-122">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="e42ee-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e42ee-123">Properties</span></span>
|<span data-ttu-id="e42ee-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e42ee-124">Property</span></span>|<span data-ttu-id="e42ee-125">型</span><span class="sxs-lookup"><span data-stu-id="e42ee-125">Type</span></span>|<span data-ttu-id="e42ee-126">説明</span><span class="sxs-lookup"><span data-stu-id="e42ee-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e42ee-127">id</span><span class="sxs-lookup"><span data-stu-id="e42ee-127">id</span></span>|<span data-ttu-id="e42ee-128">文字列</span><span class="sxs-lookup"><span data-stu-id="e42ee-128">String</span></span>|<span data-ttu-id="e42ee-129">Office クライアント構成ポリシーの Id。</span><span class="sxs-lookup"><span data-stu-id="e42ee-129">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="e42ee-130">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="e42ee-130">userPreferencePayload</span></span>|<span data-ttu-id="e42ee-131">Stream</span><span class="sxs-lookup"><span data-stu-id="e42ee-131">Stream</span></span>|<span data-ttu-id="e42ee-132">プリファレンス設定 JSON 文字列はバイナリ形式です。これらの値はユーザーが上書きできます。</span><span class="sxs-lookup"><span data-stu-id="e42ee-132">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="e42ee-133">policyPayload</span><span class="sxs-lookup"><span data-stu-id="e42ee-133">policyPayload</span></span>|<span data-ttu-id="e42ee-134">Stream</span><span class="sxs-lookup"><span data-stu-id="e42ee-134">Stream</span></span>|<span data-ttu-id="e42ee-135">ポリシー設定 JSON 文字列 (バイナリ形式) では、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="e42ee-135">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="e42ee-136">description</span><span class="sxs-lookup"><span data-stu-id="e42ee-136">description</span></span>|<span data-ttu-id="e42ee-137">String</span><span class="sxs-lookup"><span data-stu-id="e42ee-137">String</span></span>|<span data-ttu-id="e42ee-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e42ee-138">Not yet documented</span></span>|
|<span data-ttu-id="e42ee-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e42ee-139">displayName</span></span>|<span data-ttu-id="e42ee-140">String</span><span class="sxs-lookup"><span data-stu-id="e42ee-140">String</span></span>|<span data-ttu-id="e42ee-141">管理者が提供する office クライアント構成ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="e42ee-141">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="e42ee-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e42ee-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e42ee-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="e42ee-143">DateTime</span></span>|<span data-ttu-id="e42ee-144">ポリシーの最終更新日時スタンプ。</span><span class="sxs-lookup"><span data-stu-id="e42ee-144">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="e42ee-145">priority</span><span class="sxs-lookup"><span data-stu-id="e42ee-145">priority</span></span>|<span data-ttu-id="e42ee-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e42ee-146">Int32</span></span>|<span data-ttu-id="e42ee-147">優先度の値は、テナントの各ポリシーの一意の値である必要があり、競合の解決に使用されます。低い値は、優先度が高くなります。</span><span class="sxs-lookup"><span data-stu-id="e42ee-147">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="e42ee-148">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="e42ee-148">userCheckinSummary</span></span>|[<span data-ttu-id="e42ee-149">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="e42ee-149">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="e42ee-150">ポリシーのユーザーチェックインの概要。</span><span class="sxs-lookup"><span data-stu-id="e42ee-150">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="e42ee-151">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="e42ee-151">checkinStatuses</span></span>|<span data-ttu-id="e42ee-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e42ee-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="e42ee-153">Office クライアントのチェックイン状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="e42ee-153">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e42ee-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e42ee-154">Relationships</span></span>
|<span data-ttu-id="e42ee-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e42ee-155">Relationship</span></span>|<span data-ttu-id="e42ee-156">型</span><span class="sxs-lookup"><span data-stu-id="e42ee-156">Type</span></span>|<span data-ttu-id="e42ee-157">説明</span><span class="sxs-lookup"><span data-stu-id="e42ee-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e42ee-158">assignments</span><span class="sxs-lookup"><span data-stu-id="e42ee-158">assignments</span></span>|<span data-ttu-id="e42ee-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e42ee-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e42ee-160">ポリシーのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="e42ee-160">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e42ee-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e42ee-161">JSON Representation</span></span>
<span data-ttu-id="e42ee-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e42ee-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
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
  ]
}
```



