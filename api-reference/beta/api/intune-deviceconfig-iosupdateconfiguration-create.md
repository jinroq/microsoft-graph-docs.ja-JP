---
title: iosUpdateConfiguration の作成
description: 新しい iosUpdateConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b650c64e1c5c90462f4a513e77d43cdc0424a7ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923310"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="26828-103">iosUpdateConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="26828-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="26828-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26828-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26828-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="26828-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26828-106">新しい [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="26828-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26828-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="26828-107">Prerequisites</span></span>
<span data-ttu-id="26828-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26828-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26828-110">Permission type</span></span>|<span data-ttu-id="26828-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="26828-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26828-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26828-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26828-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26828-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26828-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26828-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26828-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26828-115">Not supported.</span></span>|
|<span data-ttu-id="26828-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26828-116">Application</span></span>|<span data-ttu-id="26828-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26828-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26828-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26828-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="26828-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26828-119">Request headers</span></span>
|<span data-ttu-id="26828-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26828-120">Header</span></span>|<span data-ttu-id="26828-121">値</span><span class="sxs-lookup"><span data-stu-id="26828-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26828-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26828-122">Authorization</span></span>|<span data-ttu-id="26828-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="26828-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26828-124">承諾</span><span class="sxs-lookup"><span data-stu-id="26828-124">Accept</span></span>|<span data-ttu-id="26828-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26828-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26828-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="26828-126">Request body</span></span>
<span data-ttu-id="26828-127">要求本文で、iosUpdateConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="26828-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="26828-128">次の表に、iosUpdateConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="26828-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="26828-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26828-129">Property</span></span>|<span data-ttu-id="26828-130">型</span><span class="sxs-lookup"><span data-stu-id="26828-130">Type</span></span>|<span data-ttu-id="26828-131">説明</span><span class="sxs-lookup"><span data-stu-id="26828-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26828-132">id</span><span class="sxs-lookup"><span data-stu-id="26828-132">id</span></span>|<span data-ttu-id="26828-133">文字列</span><span class="sxs-lookup"><span data-stu-id="26828-133">String</span></span>|<span data-ttu-id="26828-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="26828-134">Key of the entity.</span></span> <span data-ttu-id="26828-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26828-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26828-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26828-136">lastModifiedDateTime</span></span>|<span data-ttu-id="26828-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26828-137">DateTimeOffset</span></span>|<span data-ttu-id="26828-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="26828-138">DateTime the object was last modified.</span></span> <span data-ttu-id="26828-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26828-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26828-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26828-140">roleScopeTagIds</span></span>|<span data-ttu-id="26828-141">String collection</span><span class="sxs-lookup"><span data-stu-id="26828-141">String collection</span></span>|<span data-ttu-id="26828-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="26828-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="26828-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26828-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26828-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="26828-144">supportsScopeTags</span></span>|<span data-ttu-id="26828-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="26828-145">Boolean</span></span>|<span data-ttu-id="26828-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="26828-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="26828-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="26828-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="26828-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="26828-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="26828-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="26828-149">This property is read-only.</span></span> <span data-ttu-id="26828-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26828-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26828-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26828-151">createdDateTime</span></span>|<span data-ttu-id="26828-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26828-152">DateTimeOffset</span></span>|<span data-ttu-id="26828-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="26828-153">DateTime the object was created.</span></span> <span data-ttu-id="26828-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26828-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26828-155">description</span><span class="sxs-lookup"><span data-stu-id="26828-155">description</span></span>|<span data-ttu-id="26828-156">String</span><span class="sxs-lookup"><span data-stu-id="26828-156">String</span></span>|<span data-ttu-id="26828-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="26828-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26828-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26828-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26828-159">displayName</span><span class="sxs-lookup"><span data-stu-id="26828-159">displayName</span></span>|<span data-ttu-id="26828-160">String</span><span class="sxs-lookup"><span data-stu-id="26828-160">String</span></span>|<span data-ttu-id="26828-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="26828-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26828-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26828-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26828-163">version</span><span class="sxs-lookup"><span data-stu-id="26828-163">version</span></span>|<span data-ttu-id="26828-164">Int32</span><span class="sxs-lookup"><span data-stu-id="26828-164">Int32</span></span>|<span data-ttu-id="26828-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="26828-165">Version of the device configuration.</span></span> <span data-ttu-id="26828-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26828-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26828-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="26828-167">isEnabled</span></span>|<span data-ttu-id="26828-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="26828-168">Boolean</span></span>|<span data-ttu-id="26828-169">UI での設定の有効化</span><span class="sxs-lookup"><span data-stu-id="26828-169">Is setting enabled in UI</span></span>|
|<span data-ttu-id="26828-170">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="26828-170">activeHoursStart</span></span>|<span data-ttu-id="26828-171">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="26828-171">TimeOfDay</span></span>|<span data-ttu-id="26828-172">アクティブ時間の開始 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="26828-172">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="26828-173">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="26828-173">activeHoursEnd</span></span>|<span data-ttu-id="26828-174">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="26828-174">TimeOfDay</span></span>|<span data-ttu-id="26828-175">アクティブ時間の終了 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="26828-175">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="26828-176">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="26828-176">scheduledInstallDays</span></span>|<span data-ttu-id="26828-177">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="26828-177">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="26828-178">アクティブ時間が設定されている曜日。</span><span class="sxs-lookup"><span data-stu-id="26828-178">Days in week for which active hours are configured.</span></span> <span data-ttu-id="26828-179">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="26828-179">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="26828-180">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="26828-180">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="26828-181">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="26828-181">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="26828-182">Int32</span><span class="sxs-lookup"><span data-stu-id="26828-182">Int32</span></span>|<span data-ttu-id="26828-183">UTC タイム オフセット (分単位で示されます)</span><span class="sxs-lookup"><span data-stu-id="26828-183">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="26828-184">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="26828-184">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="26828-185">Int32</span><span class="sxs-lookup"><span data-stu-id="26828-185">Int32</span></span>|<span data-ttu-id="26828-186">ソフトウェア更新プログラムが iOS デバイスに表示されるまでの日数。 0 ~ 90 の範囲内にある。</span><span class="sxs-lookup"><span data-stu-id="26828-186">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="26828-187">応答</span><span class="sxs-lookup"><span data-stu-id="26828-187">Response</span></span>
<span data-ttu-id="26828-188">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="26828-188">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26828-189">例</span><span class="sxs-lookup"><span data-stu-id="26828-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="26828-190">要求</span><span class="sxs-lookup"><span data-stu-id="26828-190">Request</span></span>
<span data-ttu-id="26828-191">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26828-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 482

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
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

### <a name="response"></a><span data-ttu-id="26828-192">応答</span><span class="sxs-lookup"><span data-stu-id="26828-192">Response</span></span>
<span data-ttu-id="26828-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26828-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




