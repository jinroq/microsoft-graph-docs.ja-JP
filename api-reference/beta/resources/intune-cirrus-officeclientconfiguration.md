---
title: officeClientConfiguration リソースの種類
description: Office クライアントの構成。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a8371da85ee4bbc54943a8fbb29ec99dcb49a49
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150562"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="13b14-103">officeClientConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13b14-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="13b14-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13b14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13b14-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13b14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13b14-106">Office クライアントの構成。</span><span class="sxs-lookup"><span data-stu-id="13b14-106">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="13b14-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="13b14-107">Methods</span></span>
|<span data-ttu-id="13b14-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="13b14-108">Method</span></span>|<span data-ttu-id="13b14-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="13b14-109">Return Type</span></span>|<span data-ttu-id="13b14-110">説明</span><span class="sxs-lookup"><span data-stu-id="13b14-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13b14-111">リスト officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="13b14-111">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="13b14-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="13b14-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="13b14-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="13b14-113">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="13b14-114">officeClientConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="13b14-114">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="13b14-115">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="13b14-115">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="13b14-116">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="13b14-116">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="13b14-117">assign action</span><span class="sxs-lookup"><span data-stu-id="13b14-117">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="13b14-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="13b14-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="13b14-119">ポリシーの対象グループをすべて置換します。</span><span class="sxs-lookup"><span data-stu-id="13b14-119">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="13b14-120">updatePriorities アクション</span><span class="sxs-lookup"><span data-stu-id="13b14-120">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="13b14-121">なし</span><span class="sxs-lookup"><span data-stu-id="13b14-121">None</span></span>|<span data-ttu-id="13b14-122">ポリシーの優先度を更新します。</span><span class="sxs-lookup"><span data-stu-id="13b14-122">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="13b14-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13b14-123">Properties</span></span>
|<span data-ttu-id="13b14-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13b14-124">Property</span></span>|<span data-ttu-id="13b14-125">型</span><span class="sxs-lookup"><span data-stu-id="13b14-125">Type</span></span>|<span data-ttu-id="13b14-126">説明</span><span class="sxs-lookup"><span data-stu-id="13b14-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b14-127">id</span><span class="sxs-lookup"><span data-stu-id="13b14-127">id</span></span>|<span data-ttu-id="13b14-128">文字列</span><span class="sxs-lookup"><span data-stu-id="13b14-128">String</span></span>|<span data-ttu-id="13b14-129">office クライアント構成ポリシーの Id。</span><span class="sxs-lookup"><span data-stu-id="13b14-129">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="13b14-130">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="13b14-130">userPreferencePayload</span></span>|<span data-ttu-id="13b14-131">Stream</span><span class="sxs-lookup"><span data-stu-id="13b14-131">Stream</span></span>|<span data-ttu-id="13b14-132">プリファレンス設定 JSON 文字列はバイナリ形式です。これらの値はユーザーが上書きできます。</span><span class="sxs-lookup"><span data-stu-id="13b14-132">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="13b14-133">policypayload</span><span class="sxs-lookup"><span data-stu-id="13b14-133">policyPayload</span></span>|<span data-ttu-id="13b14-134">Stream</span><span class="sxs-lookup"><span data-stu-id="13b14-134">Stream</span></span>|<span data-ttu-id="13b14-135">ポリシー設定 JSON 文字列 (バイナリ形式) では、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="13b14-135">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="13b14-136">説明</span><span class="sxs-lookup"><span data-stu-id="13b14-136">description</span></span>|<span data-ttu-id="13b14-137">String</span><span class="sxs-lookup"><span data-stu-id="13b14-137">String</span></span>|<span data-ttu-id="13b14-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13b14-138">Not yet documented</span></span>|
|<span data-ttu-id="13b14-139">displayName</span><span class="sxs-lookup"><span data-stu-id="13b14-139">displayName</span></span>|<span data-ttu-id="13b14-140">String</span><span class="sxs-lookup"><span data-stu-id="13b14-140">String</span></span>|<span data-ttu-id="13b14-141">管理者が提供する office クライアント構成ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="13b14-141">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="13b14-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13b14-142">lastModifiedDateTime</span></span>|<span data-ttu-id="13b14-143">DateTime
</span><span class="sxs-lookup"><span data-stu-id="13b14-143">DateTime</span></span>|<span data-ttu-id="13b14-144">ポリシーの最終更新日時スタンプ。</span><span class="sxs-lookup"><span data-stu-id="13b14-144">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="13b14-145">priority</span><span class="sxs-lookup"><span data-stu-id="13b14-145">priority</span></span>|<span data-ttu-id="13b14-146">Int32</span><span class="sxs-lookup"><span data-stu-id="13b14-146">Int32</span></span>|<span data-ttu-id="13b14-147">優先度の値は、テナントの各ポリシーの一意の値である必要があり、競合の解決に使用されます。低い値は、優先度が高くなります。</span><span class="sxs-lookup"><span data-stu-id="13b14-147">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="13b14-148">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="13b14-148">userCheckinSummary</span></span>|[<span data-ttu-id="13b14-149">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="13b14-149">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="13b14-150">ポリシーのユーザーチェックインの概要。</span><span class="sxs-lookup"><span data-stu-id="13b14-150">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="13b14-151">checkinstatuses</span><span class="sxs-lookup"><span data-stu-id="13b14-151">checkinStatuses</span></span>|<span data-ttu-id="13b14-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="13b14-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="13b14-153">office クライアントのチェックイン状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="13b14-153">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13b14-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13b14-154">Relationships</span></span>
|<span data-ttu-id="13b14-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13b14-155">Relationship</span></span>|<span data-ttu-id="13b14-156">型</span><span class="sxs-lookup"><span data-stu-id="13b14-156">Type</span></span>|<span data-ttu-id="13b14-157">説明</span><span class="sxs-lookup"><span data-stu-id="13b14-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b14-158">assignments</span><span class="sxs-lookup"><span data-stu-id="13b14-158">assignments</span></span>|<span data-ttu-id="13b14-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="13b14-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="13b14-160">ポリシーのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="13b14-160">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13b14-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13b14-161">JSON Representation</span></span>
<span data-ttu-id="13b14-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13b14-162">Here is a JSON representation of the resource.</span></span>
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



