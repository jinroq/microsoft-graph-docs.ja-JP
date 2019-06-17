---
title: AzureADWindowsAutopilotDeploymentProfile の更新
description: AzureADWindowsAutopilotDeploymentProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37e5ffea7e59c6c622b122b590138066b153b7d6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978571"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="4bb12-103">AzureADWindowsAutopilotDeploymentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="4bb12-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="4bb12-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bb12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bb12-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4bb12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bb12-106">[AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4bb12-106">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bb12-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4bb12-107">Prerequisites</span></span>
<span data-ttu-id="4bb12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bb12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bb12-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4bb12-110">Permission type</span></span>|<span data-ttu-id="4bb12-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4bb12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bb12-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4bb12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4bb12-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bb12-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4bb12-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4bb12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bb12-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bb12-115">Not supported.</span></span>|
|<span data-ttu-id="4bb12-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4bb12-116">Application</span></span>|<span data-ttu-id="4bb12-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bb12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bb12-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4bb12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="4bb12-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4bb12-119">Request headers</span></span>
|<span data-ttu-id="4bb12-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4bb12-120">Header</span></span>|<span data-ttu-id="4bb12-121">値</span><span class="sxs-lookup"><span data-stu-id="4bb12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bb12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bb12-122">Authorization</span></span>|<span data-ttu-id="4bb12-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4bb12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bb12-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4bb12-124">Accept</span></span>|<span data-ttu-id="4bb12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4bb12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bb12-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4bb12-126">Request body</span></span>
<span data-ttu-id="4bb12-127">要求本文で、 [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4bb12-127">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="4bb12-128">次の表に、 [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4bb12-128">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="4bb12-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bb12-129">Property</span></span>|<span data-ttu-id="4bb12-130">型</span><span class="sxs-lookup"><span data-stu-id="4bb12-130">Type</span></span>|<span data-ttu-id="4bb12-131">説明</span><span class="sxs-lookup"><span data-stu-id="4bb12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bb12-132">id</span><span class="sxs-lookup"><span data-stu-id="4bb12-132">id</span></span>|<span data-ttu-id="4bb12-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4bb12-133">String</span></span>|<span data-ttu-id="4bb12-134">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルキー</span><span class="sxs-lookup"><span data-stu-id="4bb12-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4bb12-135">displayName</span></span>|<span data-ttu-id="4bb12-136">String</span><span class="sxs-lookup"><span data-stu-id="4bb12-136">String</span></span>|<span data-ttu-id="4bb12-137">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="4bb12-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-138">description</span><span class="sxs-lookup"><span data-stu-id="4bb12-138">description</span></span>|<span data-ttu-id="4bb12-139">String</span><span class="sxs-lookup"><span data-stu-id="4bb12-139">String</span></span>|<span data-ttu-id="4bb12-140">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="4bb12-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-141">language</span><span class="sxs-lookup"><span data-stu-id="4bb12-141">language</span></span>|<span data-ttu-id="4bb12-142">String</span><span class="sxs-lookup"><span data-stu-id="4bb12-142">String</span></span>|<span data-ttu-id="4bb12-143">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承したデバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="4bb12-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4bb12-144">createdDateTime</span></span>|<span data-ttu-id="4bb12-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bb12-145">DateTimeOffset</span></span>|<span data-ttu-id="4bb12-146">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの作成時刻</span><span class="sxs-lookup"><span data-stu-id="4bb12-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bb12-147">lastModifiedDateTime</span></span>|<span data-ttu-id="4bb12-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bb12-148">DateTimeOffset</span></span>|<span data-ttu-id="4bb12-149">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="4bb12-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="4bb12-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="4bb12-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="4bb12-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="4bb12-152">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された、すぐに使える状態設定</span><span class="sxs-lookup"><span data-stu-id="4bb12-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="4bb12-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="4bb12-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="4bb12-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="4bb12-155">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="4bb12-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="4bb12-156">extractHardwareHash</span></span>|<span data-ttu-id="4bb12-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bb12-157">Boolean</span></span>|<span data-ttu-id="4bb12-158">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルのハードウェアハッシュ抽出</span><span class="sxs-lookup"><span data-stu-id="4bb12-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="4bb12-159">deviceNameTemplate</span></span>|<span data-ttu-id="4bb12-160">String</span><span class="sxs-lookup"><span data-stu-id="4bb12-160">String</span></span>|<span data-ttu-id="4bb12-161">自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。</span><span class="sxs-lookup"><span data-stu-id="4bb12-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="4bb12-162">これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="4bb12-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="4bb12-163">テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="4bb12-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="4bb12-164">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4bb12-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="4bb12-165">deviceType</span></span>|[<span data-ttu-id="4bb12-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="4bb12-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="4bb12-167">このプロファイルを適用できる自動操縦デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="4bb12-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="4bb12-168">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4bb12-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="4bb12-169">可能な値は、`windowsPc`、`surfaceHub2` です。</span><span class="sxs-lookup"><span data-stu-id="4bb12-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="4bb12-170">Enableホワイトグローブ</span><span class="sxs-lookup"><span data-stu-id="4bb12-170">enableWhiteGlove</span></span>|<span data-ttu-id="4bb12-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bb12-171">Boolean</span></span>|<span data-ttu-id="4bb12-172">プロファイルの自動操縦白の手袋を有効にします。</span><span class="sxs-lookup"><span data-stu-id="4bb12-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="4bb12-173">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4bb12-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="4bb12-174">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4bb12-174">roleScopeTagIds</span></span>|<span data-ttu-id="4bb12-175">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="4bb12-175">String collection</span></span>|<span data-ttu-id="4bb12-176">プロファイルのスコープタグ。</span><span class="sxs-lookup"><span data-stu-id="4bb12-176">Scope tags for the profile.</span></span> <span data-ttu-id="4bb12-177">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4bb12-177">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4bb12-178">応答</span><span class="sxs-lookup"><span data-stu-id="4bb12-178">Response</span></span>
<span data-ttu-id="4bb12-179">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4bb12-179">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bb12-180">例</span><span class="sxs-lookup"><span data-stu-id="4bb12-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bb12-181">要求</span><span class="sxs-lookup"><span data-stu-id="4bb12-181">Request</span></span>
<span data-ttu-id="4bb12-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4bb12-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
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

### <a name="response"></a><span data-ttu-id="4bb12-183">応答</span><span class="sxs-lookup"><span data-stu-id="4bb12-183">Response</span></span>
<span data-ttu-id="4bb12-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4bb12-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "id": "e2ec4e69-4e69-e2ec-694e-ece2694eece2",
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





