---
title: officeClientConfiguration リソースの種類
description: Office クライアントの構成。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: c762158345e957c265d3784e46f2ef91421603be
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949403"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="06b59-103">officeClientConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06b59-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="06b59-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06b59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06b59-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06b59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06b59-106">Office クライアントの構成。</span><span class="sxs-lookup"><span data-stu-id="06b59-106">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="06b59-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="06b59-107">Methods</span></span>
|<span data-ttu-id="06b59-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="06b59-108">Method</span></span>|<span data-ttu-id="06b59-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="06b59-109">Return Type</span></span>|<span data-ttu-id="06b59-110">説明</span><span class="sxs-lookup"><span data-stu-id="06b59-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06b59-111">リスト officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="06b59-111">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="06b59-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="06b59-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="06b59-113">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="06b59-113">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="06b59-114">OfficeClientConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="06b59-114">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="06b59-115">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="06b59-115">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="06b59-116">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="06b59-116">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="06b59-117">assign アクション</span><span class="sxs-lookup"><span data-stu-id="06b59-117">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="06b59-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="06b59-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="06b59-119">ポリシーの対象グループをすべて置換します。</span><span class="sxs-lookup"><span data-stu-id="06b59-119">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="06b59-120">updatePriorities アクション</span><span class="sxs-lookup"><span data-stu-id="06b59-120">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="06b59-121">None</span><span class="sxs-lookup"><span data-stu-id="06b59-121">None</span></span>|<span data-ttu-id="06b59-122">ポリシーの優先度を更新します。</span><span class="sxs-lookup"><span data-stu-id="06b59-122">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="06b59-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06b59-123">Properties</span></span>
|<span data-ttu-id="06b59-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06b59-124">Property</span></span>|<span data-ttu-id="06b59-125">種類</span><span class="sxs-lookup"><span data-stu-id="06b59-125">Type</span></span>|<span data-ttu-id="06b59-126">説明</span><span class="sxs-lookup"><span data-stu-id="06b59-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06b59-127">id</span><span class="sxs-lookup"><span data-stu-id="06b59-127">id</span></span>|<span data-ttu-id="06b59-128">文字列</span><span class="sxs-lookup"><span data-stu-id="06b59-128">String</span></span>|<span data-ttu-id="06b59-129">Office クライアント構成ポリシーの Id。</span><span class="sxs-lookup"><span data-stu-id="06b59-129">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="06b59-130">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="06b59-130">userPreferencePayload</span></span>|<span data-ttu-id="06b59-131">Stream</span><span class="sxs-lookup"><span data-stu-id="06b59-131">Stream</span></span>|<span data-ttu-id="06b59-132">プリファレンス設定 JSON 文字列はバイナリ形式です。これらの値はユーザーが上書きできます。</span><span class="sxs-lookup"><span data-stu-id="06b59-132">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="06b59-133">policyPayload</span><span class="sxs-lookup"><span data-stu-id="06b59-133">policyPayload</span></span>|<span data-ttu-id="06b59-134">Stream</span><span class="sxs-lookup"><span data-stu-id="06b59-134">Stream</span></span>|<span data-ttu-id="06b59-135">ポリシー設定 JSON 文字列 (バイナリ形式) では、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="06b59-135">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="06b59-136">description</span><span class="sxs-lookup"><span data-stu-id="06b59-136">description</span></span>|<span data-ttu-id="06b59-137">String</span><span class="sxs-lookup"><span data-stu-id="06b59-137">String</span></span>|<span data-ttu-id="06b59-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="06b59-138">Not yet documented</span></span>|
|<span data-ttu-id="06b59-139">displayName</span><span class="sxs-lookup"><span data-stu-id="06b59-139">displayName</span></span>|<span data-ttu-id="06b59-140">String</span><span class="sxs-lookup"><span data-stu-id="06b59-140">String</span></span>|<span data-ttu-id="06b59-141">管理者が提供する office クライアント構成ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="06b59-141">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="06b59-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06b59-142">lastModifiedDateTime</span></span>|<span data-ttu-id="06b59-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="06b59-143">DateTime</span></span>|<span data-ttu-id="06b59-144">ポリシーの最終更新日時スタンプ。</span><span class="sxs-lookup"><span data-stu-id="06b59-144">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="06b59-145">priority</span><span class="sxs-lookup"><span data-stu-id="06b59-145">priority</span></span>|<span data-ttu-id="06b59-146">Int32</span><span class="sxs-lookup"><span data-stu-id="06b59-146">Int32</span></span>|<span data-ttu-id="06b59-147">優先度の値は、テナントの各ポリシーの一意の値である必要があり、競合の解決に使用されます。低い値は、優先度が高くなります。</span><span class="sxs-lookup"><span data-stu-id="06b59-147">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="06b59-148">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="06b59-148">userCheckinSummary</span></span>|[<span data-ttu-id="06b59-149">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="06b59-149">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="06b59-150">ポリシーのユーザーチェックインの概要。</span><span class="sxs-lookup"><span data-stu-id="06b59-150">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="06b59-151">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="06b59-151">checkinStatuses</span></span>|<span data-ttu-id="06b59-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="06b59-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="06b59-153">Office クライアントのチェックイン状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="06b59-153">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06b59-154">関係</span><span class="sxs-lookup"><span data-stu-id="06b59-154">Relationships</span></span>
|<span data-ttu-id="06b59-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06b59-155">Relationship</span></span>|<span data-ttu-id="06b59-156">型</span><span class="sxs-lookup"><span data-stu-id="06b59-156">Type</span></span>|<span data-ttu-id="06b59-157">説明</span><span class="sxs-lookup"><span data-stu-id="06b59-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06b59-158">assignments</span><span class="sxs-lookup"><span data-stu-id="06b59-158">assignments</span></span>|<span data-ttu-id="06b59-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="06b59-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="06b59-160">ポリシーのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="06b59-160">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06b59-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06b59-161">JSON Representation</span></span>
<span data-ttu-id="06b59-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06b59-162">Here is a JSON representation of the resource.</span></span>
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



