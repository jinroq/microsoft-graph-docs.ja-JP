---
title: ActiveDirectoryWindowsAutopilotDeploymentProfile を作成する
description: 新しい activeDirectoryWindowsAutopilotDeploymentProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 054d4ae2db44e69f9c9718bd488fa4a186e98b8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981123"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="8d66d-103">ActiveDirectoryWindowsAutopilotDeploymentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="8d66d-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="8d66d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d66d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d66d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d66d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d66d-106">新しい[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d66d-106">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d66d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8d66d-107">Prerequisites</span></span>
<span data-ttu-id="8d66d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d66d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d66d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d66d-110">Permission type</span></span>|<span data-ttu-id="8d66d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d66d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d66d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d66d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d66d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d66d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d66d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d66d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d66d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d66d-115">Not supported.</span></span>|
|<span data-ttu-id="8d66d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d66d-116">Application</span></span>|<span data-ttu-id="8d66d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d66d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d66d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d66d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="8d66d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d66d-119">Request headers</span></span>
|<span data-ttu-id="8d66d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d66d-120">Header</span></span>|<span data-ttu-id="8d66d-121">値</span><span class="sxs-lookup"><span data-stu-id="8d66d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d66d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d66d-122">Authorization</span></span>|<span data-ttu-id="8d66d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d66d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d66d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8d66d-124">Accept</span></span>|<span data-ttu-id="8d66d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d66d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d66d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d66d-126">Request body</span></span>
<span data-ttu-id="8d66d-127">要求本文で、activeDirectoryWindowsAutopilotDeploymentProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d66d-127">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="8d66d-128">次の表に、activeDirectoryWindowsAutopilotDeploymentProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8d66d-128">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="8d66d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d66d-129">Property</span></span>|<span data-ttu-id="8d66d-130">型</span><span class="sxs-lookup"><span data-stu-id="8d66d-130">Type</span></span>|<span data-ttu-id="8d66d-131">説明</span><span class="sxs-lookup"><span data-stu-id="8d66d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d66d-132">id</span><span class="sxs-lookup"><span data-stu-id="8d66d-132">id</span></span>|<span data-ttu-id="8d66d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8d66d-133">String</span></span>|<span data-ttu-id="8d66d-134">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルキー</span><span class="sxs-lookup"><span data-stu-id="8d66d-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8d66d-135">displayName</span></span>|<span data-ttu-id="8d66d-136">String</span><span class="sxs-lookup"><span data-stu-id="8d66d-136">String</span></span>|<span data-ttu-id="8d66d-137">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="8d66d-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-138">description</span><span class="sxs-lookup"><span data-stu-id="8d66d-138">description</span></span>|<span data-ttu-id="8d66d-139">String</span><span class="sxs-lookup"><span data-stu-id="8d66d-139">String</span></span>|<span data-ttu-id="8d66d-140">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="8d66d-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-141">language</span><span class="sxs-lookup"><span data-stu-id="8d66d-141">language</span></span>|<span data-ttu-id="8d66d-142">String</span><span class="sxs-lookup"><span data-stu-id="8d66d-142">String</span></span>|<span data-ttu-id="8d66d-143">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承したデバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="8d66d-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d66d-144">createdDateTime</span></span>|<span data-ttu-id="8d66d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d66d-145">DateTimeOffset</span></span>|<span data-ttu-id="8d66d-146">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの作成時刻</span><span class="sxs-lookup"><span data-stu-id="8d66d-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d66d-147">lastModifiedDateTime</span></span>|<span data-ttu-id="8d66d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d66d-148">DateTimeOffset</span></span>|<span data-ttu-id="8d66d-149">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="8d66d-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="8d66d-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="8d66d-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="8d66d-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="8d66d-152">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された、すぐに使える状態設定</span><span class="sxs-lookup"><span data-stu-id="8d66d-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="8d66d-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="8d66d-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="8d66d-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="8d66d-155">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="8d66d-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="8d66d-156">extractHardwareHash</span></span>|<span data-ttu-id="8d66d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d66d-157">Boolean</span></span>|<span data-ttu-id="8d66d-158">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルのハードウェアハッシュ抽出</span><span class="sxs-lookup"><span data-stu-id="8d66d-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="8d66d-159">deviceNameTemplate</span></span>|<span data-ttu-id="8d66d-160">String</span><span class="sxs-lookup"><span data-stu-id="8d66d-160">String</span></span>|<span data-ttu-id="8d66d-161">自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。</span><span class="sxs-lookup"><span data-stu-id="8d66d-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="8d66d-162">これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="8d66d-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="8d66d-163">テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="8d66d-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="8d66d-164">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8d66d-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="8d66d-165">deviceType</span></span>|[<span data-ttu-id="8d66d-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="8d66d-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="8d66d-167">このプロファイルを適用できる自動操縦デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="8d66d-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="8d66d-168">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8d66d-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="8d66d-169">可能な値は、`windowsPc`、`surfaceHub2` です。</span><span class="sxs-lookup"><span data-stu-id="8d66d-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="8d66d-170">Enableホワイトグローブ</span><span class="sxs-lookup"><span data-stu-id="8d66d-170">enableWhiteGlove</span></span>|<span data-ttu-id="8d66d-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d66d-171">Boolean</span></span>|<span data-ttu-id="8d66d-172">プロファイルの自動操縦白の手袋を有効にします。</span><span class="sxs-lookup"><span data-stu-id="8d66d-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="8d66d-173">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8d66d-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8d66d-174">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d66d-174">roleScopeTagIds</span></span>|<span data-ttu-id="8d66d-175">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8d66d-175">String collection</span></span>|<span data-ttu-id="8d66d-176">プロファイルのスコープタグ。</span><span class="sxs-lookup"><span data-stu-id="8d66d-176">Scope tags for the profile.</span></span> <span data-ttu-id="8d66d-177">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8d66d-177">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8d66d-178">応答</span><span class="sxs-lookup"><span data-stu-id="8d66d-178">Response</span></span>
<span data-ttu-id="8d66d-179">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8d66d-179">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d66d-180">例</span><span class="sxs-lookup"><span data-stu-id="8d66d-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d66d-181">要求</span><span class="sxs-lookup"><span data-stu-id="8d66d-181">Request</span></span>
<span data-ttu-id="8d66d-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d66d-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1167

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value",
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8d66d-183">応答</span><span class="sxs-lookup"><span data-stu-id="8d66d-183">Response</span></span>
<span data-ttu-id="8d66d-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d66d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1339

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
  "id": "49fe234a-234a-49fe-4a23-fe494a23fe49",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value",
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





