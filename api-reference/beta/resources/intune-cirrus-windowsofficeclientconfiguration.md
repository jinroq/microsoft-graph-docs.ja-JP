---
title: windowsOfficeClientConfiguration リソースの種類
description: Windows 用の office ポリシーの設定について説明するエンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 23307b9342b3a33ce4a405691a1755527a366705
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944857"
---
# <a name="windowsofficeclientconfiguration-resource-type"></a><span data-ttu-id="415ef-103">windowsOfficeClientConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="415ef-103">windowsOfficeClientConfiguration resource type</span></span>

> <span data-ttu-id="415ef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="415ef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="415ef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="415ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="415ef-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="415ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="415ef-107">Windows 用の office ポリシーの設定について説明するエンティティです。</span><span class="sxs-lookup"><span data-stu-id="415ef-107">Entity that describes office policy settings for Windows.</span></span>

<span data-ttu-id="415ef-108">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="415ef-108">Inherits from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="415ef-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="415ef-109">Methods</span></span>
|<span data-ttu-id="415ef-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="415ef-110">Method</span></span>|<span data-ttu-id="415ef-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="415ef-111">Return Type</span></span>|<span data-ttu-id="415ef-112">説明</span><span class="sxs-lookup"><span data-stu-id="415ef-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="415ef-113">リスト windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="415ef-113">List windowsOfficeClientConfigurations</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-list.md)|<span data-ttu-id="415ef-114">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="415ef-114">[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) collection</span></span>|<span data-ttu-id="415ef-115">[WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="415ef-115">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="415ef-116">WindowsOfficeClientConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="415ef-116">Get windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-get.md)|[<span data-ttu-id="415ef-117">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="415ef-117">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="415ef-118">[WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="415ef-118">Read properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="415ef-119">WindowsOfficeClientConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="415ef-119">Create windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-create.md)|[<span data-ttu-id="415ef-120">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="415ef-120">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="415ef-121">新しい[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="415ef-121">Create a new [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="415ef-122">WindowsOfficeClientConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="415ef-122">Delete windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-delete.md)|<span data-ttu-id="415ef-123">なし</span><span class="sxs-lookup"><span data-stu-id="415ef-123">None</span></span>|<span data-ttu-id="415ef-124">の[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="415ef-124">Deletes a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>|
|[<span data-ttu-id="415ef-125">WindowsOfficeClientConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="415ef-125">Update windowsOfficeClientConfiguration</span></span>](../api/intune-cirrus-windowsofficeclientconfiguration-update.md)|[<span data-ttu-id="415ef-126">windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="415ef-126">windowsOfficeClientConfiguration</span></span>](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|<span data-ttu-id="415ef-127">[WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="415ef-127">Update the properties of a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="415ef-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="415ef-128">Properties</span></span>
|<span data-ttu-id="415ef-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="415ef-129">Property</span></span>|<span data-ttu-id="415ef-130">種類</span><span class="sxs-lookup"><span data-stu-id="415ef-130">Type</span></span>|<span data-ttu-id="415ef-131">説明</span><span class="sxs-lookup"><span data-stu-id="415ef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="415ef-132">ID</span><span class="sxs-lookup"><span data-stu-id="415ef-132">id</span></span>|<span data-ttu-id="415ef-133">String</span><span class="sxs-lookup"><span data-stu-id="415ef-133">String</span></span>|<span data-ttu-id="415ef-134">Office クライアントの構成のポリシーの id。</span><span class="sxs-lookup"><span data-stu-id="415ef-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="415ef-135">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="415ef-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="415ef-136">userPreferencePayload</span></span>|<span data-ttu-id="415ef-137">Stream</span><span class="sxs-lookup"><span data-stu-id="415ef-137">Stream</span></span>|<span data-ttu-id="415ef-138">JSON の環境設定は、バイナリ形式の文字列は、ユーザーがこれらの値をオーバーライドすることができます。</span><span class="sxs-lookup"><span data-stu-id="415ef-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="415ef-139">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="415ef-140">policyPayload</span><span class="sxs-lookup"><span data-stu-id="415ef-140">policyPayload</span></span>|<span data-ttu-id="415ef-141">Stream</span><span class="sxs-lookup"><span data-stu-id="415ef-141">Stream</span></span>|<span data-ttu-id="415ef-142">JSON のポリシー設定はバイナリ形式の文字列は、ユーザーがこれらの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="415ef-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="415ef-143">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="415ef-144">説明</span><span class="sxs-lookup"><span data-stu-id="415ef-144">description</span></span>|<span data-ttu-id="415ef-145">String</span><span class="sxs-lookup"><span data-stu-id="415ef-145">String</span></span>|<span data-ttu-id="415ef-146">管理者には、office クライアントの説明の構成のポリシーが用意されています。</span><span class="sxs-lookup"><span data-stu-id="415ef-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="415ef-147">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="415ef-148">displayName</span><span class="sxs-lookup"><span data-stu-id="415ef-148">displayName</span></span>|<span data-ttu-id="415ef-149">String</span><span class="sxs-lookup"><span data-stu-id="415ef-149">String</span></span>|<span data-ttu-id="415ef-150">管理者は、office クライアントの構成のポリシーの名前を提供します。</span><span class="sxs-lookup"><span data-stu-id="415ef-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="415ef-151">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="415ef-152">priority</span><span class="sxs-lookup"><span data-stu-id="415ef-152">priority</span></span>|<span data-ttu-id="415ef-153">Int32</span><span class="sxs-lookup"><span data-stu-id="415ef-153">Int32</span></span>|<span data-ttu-id="415ef-154">優先度の値がテナントの下にある各ポリシーの一意の値にする必要があり、競合の解決に使用する、値が低い優先順位が高いことを意味します。</span><span class="sxs-lookup"><span data-stu-id="415ef-154">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="415ef-155">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="415ef-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="415ef-156">lastModifiedDateTime</span></span>|<span data-ttu-id="415ef-157">DateTime</span><span class="sxs-lookup"><span data-stu-id="415ef-157">DateTime</span></span>|<span data-ttu-id="415ef-158">ポリシーの最終変更された日付時刻スタンプ。</span><span class="sxs-lookup"><span data-stu-id="415ef-158">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="415ef-159">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="415ef-160">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="415ef-160">userCheckinSummary</span></span>|[<span data-ttu-id="415ef-161">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="415ef-161">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="415ef-162">ポリシーの概要チェックのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="415ef-162">User check-in summary for the policy.</span></span> <span data-ttu-id="415ef-163">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="415ef-164">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="415ef-164">checkinStatuses</span></span>|<span data-ttu-id="415ef-165">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="415ef-165">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="415ef-166">Office クライアントでは、チェック状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="415ef-166">List of office Client check-in status.</span></span> <span data-ttu-id="415ef-167">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="415ef-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="415ef-168">Relationships</span></span>
|<span data-ttu-id="415ef-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="415ef-169">Relationship</span></span>|<span data-ttu-id="415ef-170">型</span><span class="sxs-lookup"><span data-stu-id="415ef-170">Type</span></span>|<span data-ttu-id="415ef-171">説明</span><span class="sxs-lookup"><span data-stu-id="415ef-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="415ef-172">assignments</span><span class="sxs-lookup"><span data-stu-id="415ef-172">assignments</span></span>|<span data-ttu-id="415ef-173">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="415ef-173">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="415ef-174">一連のポリシーの割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="415ef-174">The list of group assignments for the policy.</span></span> <span data-ttu-id="415ef-175">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="415ef-175">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="415ef-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="415ef-176">JSON Representation</span></span>
<span data-ttu-id="415ef-177">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="415ef-177">Here is a JSON representation of the resource.</span></span>
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



