---
title: iosUpdateConfiguration の更新
description: iosUpdateConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 87b9e113c82adf31ee21e026a71268d65da84a25
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329856"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="fe6e1-103">iosUpdateConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="fe6e1-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="fe6e1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe6e1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe6e1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe6e1-107">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-107">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe6e1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fe6e1-108">Prerequisites</span></span>
<span data-ttu-id="fe6e1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe6e1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe6e1-111">Permission type</span></span>|<span data-ttu-id="fe6e1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe6e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe6e1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe6e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe6e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe6e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe6e1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe6e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe6e1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-116">Not supported.</span></span>|
|<span data-ttu-id="fe6e1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe6e1-117">Application</span></span>|<span data-ttu-id="fe6e1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe6e1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe6e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fe6e1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe6e1-120">Request headers</span></span>
|<span data-ttu-id="fe6e1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe6e1-121">Header</span></span>|<span data-ttu-id="fe6e1-122">値</span><span class="sxs-lookup"><span data-stu-id="fe6e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe6e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe6e1-123">Authorization</span></span>|<span data-ttu-id="fe6e1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe6e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe6e1-125">Accept</span></span>|<span data-ttu-id="fe6e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe6e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe6e1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe6e1-127">Request body</span></span>
<span data-ttu-id="fe6e1-128">要求本文で、[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-128">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="fe6e1-129">次の表に、[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-129">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="fe6e1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe6e1-130">Property</span></span>|<span data-ttu-id="fe6e1-131">種類</span><span class="sxs-lookup"><span data-stu-id="fe6e1-131">Type</span></span>|<span data-ttu-id="fe6e1-132">説明</span><span class="sxs-lookup"><span data-stu-id="fe6e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe6e1-133">ID</span><span class="sxs-lookup"><span data-stu-id="fe6e1-133">id</span></span>|<span data-ttu-id="fe6e1-134">String</span><span class="sxs-lookup"><span data-stu-id="fe6e1-134">String</span></span>|<span data-ttu-id="fe6e1-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-135">Key of the entity.</span></span> <span data-ttu-id="fe6e1-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe6e1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe6e1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe6e1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fe6e1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe6e1-138">DateTimeOffset</span></span>|<span data-ttu-id="fe6e1-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fe6e1-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe6e1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe6e1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe6e1-141">roleScopeTagIds</span></span>|<span data-ttu-id="fe6e1-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fe6e1-142">String collection</span></span>|<span data-ttu-id="fe6e1-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fe6e1-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe6e1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe6e1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fe6e1-145">supportsScopeTags</span></span>|<span data-ttu-id="fe6e1-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="fe6e1-146">Boolean</span></span>|<span data-ttu-id="fe6e1-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fe6e1-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fe6e1-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fe6e1-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-150">This property is read-only.</span></span> <span data-ttu-id="fe6e1-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe6e1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe6e1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe6e1-152">createdDateTime</span></span>|<span data-ttu-id="fe6e1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe6e1-153">DateTimeOffset</span></span>|<span data-ttu-id="fe6e1-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-154">DateTime the object was created.</span></span> <span data-ttu-id="fe6e1-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe6e1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe6e1-156">説明</span><span class="sxs-lookup"><span data-stu-id="fe6e1-156">description</span></span>|<span data-ttu-id="fe6e1-157">String</span><span class="sxs-lookup"><span data-stu-id="fe6e1-157">String</span></span>|<span data-ttu-id="fe6e1-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe6e1-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe6e1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe6e1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fe6e1-160">displayName</span></span>|<span data-ttu-id="fe6e1-161">String</span><span class="sxs-lookup"><span data-stu-id="fe6e1-161">String</span></span>|<span data-ttu-id="fe6e1-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe6e1-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe6e1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe6e1-164">version</span><span class="sxs-lookup"><span data-stu-id="fe6e1-164">version</span></span>|<span data-ttu-id="fe6e1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fe6e1-165">Int32</span></span>|<span data-ttu-id="fe6e1-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-166">Version of the device configuration.</span></span> <span data-ttu-id="fe6e1-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fe6e1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe6e1-168">isEnabled</span><span class="sxs-lookup"><span data-stu-id="fe6e1-168">isEnabled</span></span>|<span data-ttu-id="fe6e1-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe6e1-169">Boolean</span></span>|<span data-ttu-id="fe6e1-170">UI で有効に設定</span><span class="sxs-lookup"><span data-stu-id="fe6e1-170">Is setting enabled in UI</span></span>|
|<span data-ttu-id="fe6e1-171">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="fe6e1-171">activeHoursStart</span></span>|<span data-ttu-id="fe6e1-172">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fe6e1-172">TimeOfDay</span></span>|<span data-ttu-id="fe6e1-173">アクティブ時間の開始 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="fe6e1-173">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="fe6e1-174">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="fe6e1-174">activeHoursEnd</span></span>|<span data-ttu-id="fe6e1-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fe6e1-175">TimeOfDay</span></span>|<span data-ttu-id="fe6e1-176">アクティブ時間の終了 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="fe6e1-176">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="fe6e1-177">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="fe6e1-177">scheduledInstallDays</span></span>|<span data-ttu-id="fe6e1-178">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fe6e1-178">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="fe6e1-179">アクティブ時間が設定されている曜日。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-179">Days in week for which active hours are configured.</span></span> <span data-ttu-id="fe6e1-180">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-180">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="fe6e1-181">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-181">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="fe6e1-182">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="fe6e1-182">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="fe6e1-183">Int32</span><span class="sxs-lookup"><span data-stu-id="fe6e1-183">Int32</span></span>|<span data-ttu-id="fe6e1-184">UTC タイム オフセット (分単位で示されます)</span><span class="sxs-lookup"><span data-stu-id="fe6e1-184">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="fe6e1-185">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="fe6e1-185">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="fe6e1-186">Int32</span><span class="sxs-lookup"><span data-stu-id="fe6e1-186">Int32</span></span>|<span data-ttu-id="fe6e1-187">日がソフトウェアの更新の前に 0 から 90 までに至るまでの iOS デバイスに表示されます。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-187">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="fe6e1-188">応答</span><span class="sxs-lookup"><span data-stu-id="fe6e1-188">Response</span></span>
<span data-ttu-id="fe6e1-189">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-189">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe6e1-190">例</span><span class="sxs-lookup"><span data-stu-id="fe6e1-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe6e1-191">要求</span><span class="sxs-lookup"><span data-stu-id="fe6e1-191">Request</span></span>
<span data-ttu-id="fe6e1-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 485

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="fe6e1-193">応答</span><span class="sxs-lookup"><span data-stu-id="fe6e1-193">Response</span></span>
<span data-ttu-id="fe6e1-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe6e1-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 654

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```





