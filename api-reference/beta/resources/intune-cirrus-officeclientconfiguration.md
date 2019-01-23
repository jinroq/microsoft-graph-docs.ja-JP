---
title: officeClientConfiguration リソースの種類
description: Office クライアントの構成。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c171f5f9f3dcedcab0d14b98a6fea0ba8fbe41eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393236"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="bcb5a-103">officeClientConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bcb5a-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="bcb5a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bcb5a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bcb5a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcb5a-107">Office クライアントの構成。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-107">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="bcb5a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcb5a-108">Methods</span></span>
|<span data-ttu-id="bcb5a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcb5a-109">Method</span></span>|<span data-ttu-id="bcb5a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bcb5a-110">Return Type</span></span>|<span data-ttu-id="bcb5a-111">説明</span><span class="sxs-lookup"><span data-stu-id="bcb5a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bcb5a-112">リスト officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="bcb5a-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="bcb5a-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bcb5a-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="bcb5a-114">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="bcb5a-115">OfficeClientConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="bcb5a-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="bcb5a-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="bcb5a-117">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bcb5a-118">assign action</span><span class="sxs-lookup"><span data-stu-id="bcb5a-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="bcb5a-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bcb5a-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bcb5a-120">ポリシーのすべての対象とするグループを交換してください。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="bcb5a-121">updatePriorities アクション</span><span class="sxs-lookup"><span data-stu-id="bcb5a-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="bcb5a-122">なし</span><span class="sxs-lookup"><span data-stu-id="bcb5a-122">None</span></span>|<span data-ttu-id="bcb5a-123">ポリシーの優先順位を更新します。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="bcb5a-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcb5a-124">Properties</span></span>
|<span data-ttu-id="bcb5a-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcb5a-125">Property</span></span>|<span data-ttu-id="bcb5a-126">型</span><span class="sxs-lookup"><span data-stu-id="bcb5a-126">Type</span></span>|<span data-ttu-id="bcb5a-127">説明</span><span class="sxs-lookup"><span data-stu-id="bcb5a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcb5a-128">id</span><span class="sxs-lookup"><span data-stu-id="bcb5a-128">id</span></span>|<span data-ttu-id="bcb5a-129">String</span><span class="sxs-lookup"><span data-stu-id="bcb5a-129">String</span></span>|<span data-ttu-id="bcb5a-130">Office クライアントの構成のポリシーの id。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="bcb5a-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="bcb5a-131">userPreferencePayload</span></span>|<span data-ttu-id="bcb5a-132">Stream</span><span class="sxs-lookup"><span data-stu-id="bcb5a-132">Stream</span></span>|<span data-ttu-id="bcb5a-133">JSON の環境設定は、バイナリ形式の文字列は、ユーザーがこれらの値をオーバーライドすることができます。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="bcb5a-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="bcb5a-134">policyPayload</span></span>|<span data-ttu-id="bcb5a-135">Stream</span><span class="sxs-lookup"><span data-stu-id="bcb5a-135">Stream</span></span>|<span data-ttu-id="bcb5a-136">JSON のポリシー設定はバイナリ形式の文字列は、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="bcb5a-137">説明</span><span class="sxs-lookup"><span data-stu-id="bcb5a-137">description</span></span>|<span data-ttu-id="bcb5a-138">String</span><span class="sxs-lookup"><span data-stu-id="bcb5a-138">String</span></span>|<span data-ttu-id="bcb5a-139">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bcb5a-139">Not yet documented</span></span>|
|<span data-ttu-id="bcb5a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="bcb5a-140">displayName</span></span>|<span data-ttu-id="bcb5a-141">String</span><span class="sxs-lookup"><span data-stu-id="bcb5a-141">String</span></span>|<span data-ttu-id="bcb5a-142">管理者には、office クライアントの説明の構成のポリシーが用意されています。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="bcb5a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcb5a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="bcb5a-144">DateTime
</span><span class="sxs-lookup"><span data-stu-id="bcb5a-144">DateTime</span></span>|<span data-ttu-id="bcb5a-145">ポリシーの最終変更された日付時刻スタンプ。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="bcb5a-146">priority</span><span class="sxs-lookup"><span data-stu-id="bcb5a-146">priority</span></span>|<span data-ttu-id="bcb5a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bcb5a-147">Int32</span></span>|<span data-ttu-id="bcb5a-148">優先度の値がテナントの下にある各ポリシーの一意の値にする必要があり、競合の解決に使用する、値が低い優先順位が高いことを意味します。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="bcb5a-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bcb5a-149">userCheckinSummary</span></span>|[<span data-ttu-id="bcb5a-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bcb5a-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="bcb5a-151">ポリシーの概要チェックのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="bcb5a-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="bcb5a-152">checkinStatuses</span></span>|<span data-ttu-id="bcb5a-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bcb5a-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="bcb5a-154">Office クライアントでは、チェック状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcb5a-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcb5a-155">Relationships</span></span>
|<span data-ttu-id="bcb5a-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcb5a-156">Relationship</span></span>|<span data-ttu-id="bcb5a-157">型</span><span class="sxs-lookup"><span data-stu-id="bcb5a-157">Type</span></span>|<span data-ttu-id="bcb5a-158">説明</span><span class="sxs-lookup"><span data-stu-id="bcb5a-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcb5a-159">assignments</span><span class="sxs-lookup"><span data-stu-id="bcb5a-159">assignments</span></span>|<span data-ttu-id="bcb5a-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bcb5a-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bcb5a-161">一連のポリシーの割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcb5a-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bcb5a-162">JSON Representation</span></span>
<span data-ttu-id="bcb5a-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bcb5a-163">Here is a JSON representation of the resource.</span></span>
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



