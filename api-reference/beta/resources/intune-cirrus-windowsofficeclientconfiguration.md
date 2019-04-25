---
title: windowsOfficeClientConfiguration リソースの種類
description: Windows 用の office ポリシー設定を説明するエンティティ。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61b64b53fb5a4000b0e8c5366c5a821c6941ce61
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526343"
---
# <a name="windowsofficeclientconfiguration-resource-type"></a><span data-ttu-id="33167-103">windowsOfficeClientConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="33167-103">windowsOfficeClientConfiguration resource type</span></span>

> <span data-ttu-id="33167-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33167-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33167-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="33167-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33167-106">Windows 用の office ポリシー設定を説明するエンティティ。</span><span class="sxs-lookup"><span data-stu-id="33167-106">Entity that describes office policy settings for Windows.</span></span>

<span data-ttu-id="33167-107">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-107">Inherits from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="33167-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="33167-108">Methods</span></span>
|<span data-ttu-id="33167-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="33167-109">Method</span></span>|<span data-ttu-id="33167-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="33167-110">Return Type</span></span>|<span data-ttu-id="33167-111">説明</span><span class="sxs-lookup"><span data-stu-id="33167-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="33167-112">リスト windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="33167-112">List windowsOfficeClientConfigurations</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-list.md)|<span data-ttu-id="33167-113">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="33167-113">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) collection</span></span>|<span data-ttu-id="33167-114">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="33167-114">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="33167-115">windowsOfficeClientConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="33167-115">Get windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-get.md)|[<span data-ttu-id="33167-116">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="33167-116">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="33167-117">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="33167-117">Read properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="33167-118">windowsOfficeClientConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="33167-118">Create windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-create.md)|[<span data-ttu-id="33167-119">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="33167-119">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="33167-120">新しい[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="33167-120">Create a new [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="33167-121">windowsOfficeClientConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="33167-121">Delete windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-delete.md)|<span data-ttu-id="33167-122">なし</span><span class="sxs-lookup"><span data-stu-id="33167-122">None</span></span>|<span data-ttu-id="33167-123">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="33167-123">Deletes a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>|
|[<span data-ttu-id="33167-124">windowsOfficeClientConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="33167-124">Update windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-update.md)|[<span data-ttu-id="33167-125">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="33167-125">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="33167-126">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="33167-126">Update the properties of a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="33167-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33167-127">Properties</span></span>
|<span data-ttu-id="33167-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33167-128">Property</span></span>|<span data-ttu-id="33167-129">種類</span><span class="sxs-lookup"><span data-stu-id="33167-129">Type</span></span>|<span data-ttu-id="33167-130">説明</span><span class="sxs-lookup"><span data-stu-id="33167-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33167-131">id</span><span class="sxs-lookup"><span data-stu-id="33167-131">id</span></span>|<span data-ttu-id="33167-132">String</span><span class="sxs-lookup"><span data-stu-id="33167-132">String</span></span>|<span data-ttu-id="33167-133">office クライアント構成ポリシーの Id。</span><span class="sxs-lookup"><span data-stu-id="33167-133">Id of the office client configuration policy.</span></span> <span data-ttu-id="33167-134">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-134">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="33167-135">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="33167-135">userPreferencePayload</span></span>|<span data-ttu-id="33167-136">Stream</span><span class="sxs-lookup"><span data-stu-id="33167-136">Stream</span></span>|<span data-ttu-id="33167-137">プリファレンス設定 JSON 文字列はバイナリ形式です。これらの値はユーザーが上書きできます。</span><span class="sxs-lookup"><span data-stu-id="33167-137">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="33167-138">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-138">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="33167-139">policypayload</span><span class="sxs-lookup"><span data-stu-id="33167-139">policyPayload</span></span>|<span data-ttu-id="33167-140">Stream</span><span class="sxs-lookup"><span data-stu-id="33167-140">Stream</span></span>|<span data-ttu-id="33167-141">ポリシー設定 JSON 文字列 (バイナリ形式) では、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="33167-141">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="33167-142">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-142">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="33167-143">description</span><span class="sxs-lookup"><span data-stu-id="33167-143">description</span></span>|<span data-ttu-id="33167-144">String</span><span class="sxs-lookup"><span data-stu-id="33167-144">String</span></span>|<span data-ttu-id="33167-145">管理者が提供する office クライアント構成ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="33167-145">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="33167-146">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-146">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="33167-147">displayName</span><span class="sxs-lookup"><span data-stu-id="33167-147">displayName</span></span>|<span data-ttu-id="33167-148">String</span><span class="sxs-lookup"><span data-stu-id="33167-148">String</span></span>|<span data-ttu-id="33167-149">管理者が指定した office クライアント構成ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="33167-149">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="33167-150">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-150">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="33167-151">priority</span><span class="sxs-lookup"><span data-stu-id="33167-151">priority</span></span>|<span data-ttu-id="33167-152">Int32</span><span class="sxs-lookup"><span data-stu-id="33167-152">Int32</span></span>|<span data-ttu-id="33167-153">優先度の値は、テナントの各ポリシーの一意の値である必要があり、競合の解決に使用されます。低い値は、優先度が高くなります。</span><span class="sxs-lookup"><span data-stu-id="33167-153">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="33167-154">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-154">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="33167-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33167-155">lastModifiedDateTime</span></span>|<span data-ttu-id="33167-156">DateTime
</span><span class="sxs-lookup"><span data-stu-id="33167-156">DateTime</span></span>|<span data-ttu-id="33167-157">ポリシーの最終更新日時スタンプ。</span><span class="sxs-lookup"><span data-stu-id="33167-157">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="33167-158">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-158">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="33167-159">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="33167-159">userCheckinSummary</span></span>|[<span data-ttu-id="33167-160">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="33167-160">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="33167-161">ポリシーのユーザーチェックインの概要。</span><span class="sxs-lookup"><span data-stu-id="33167-161">User check-in summary for the policy.</span></span> <span data-ttu-id="33167-162">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-162">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="33167-163">checkinstatuses</span><span class="sxs-lookup"><span data-stu-id="33167-163">checkinStatuses</span></span>|<span data-ttu-id="33167-164">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="33167-164">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="33167-165">office クライアントのチェックイン状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="33167-165">List of office Client check-in status.</span></span> <span data-ttu-id="33167-166">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-166">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="33167-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="33167-167">Relationships</span></span>
|<span data-ttu-id="33167-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="33167-168">Relationship</span></span>|<span data-ttu-id="33167-169">型</span><span class="sxs-lookup"><span data-stu-id="33167-169">Type</span></span>|<span data-ttu-id="33167-170">説明</span><span class="sxs-lookup"><span data-stu-id="33167-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33167-171">assignments</span><span class="sxs-lookup"><span data-stu-id="33167-171">assignments</span></span>|<span data-ttu-id="33167-172">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="33167-172">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="33167-173">ポリシーのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="33167-173">The list of group assignments for the policy.</span></span> <span data-ttu-id="33167-174">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="33167-174">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33167-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="33167-175">JSON Representation</span></span>
<span data-ttu-id="33167-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="33167-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsOfficeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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



