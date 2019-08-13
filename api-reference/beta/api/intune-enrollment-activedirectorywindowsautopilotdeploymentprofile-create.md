---
title: ActiveDirectoryWindowsAutopilotDeploymentProfile を作成する
description: 新しい activeDirectoryWindowsAutopilotDeploymentProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 615290ffdaad8fcfd315bfccc8f08fe40aa523d6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309815"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="bb54c-103">ActiveDirectoryWindowsAutopilotDeploymentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="bb54c-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="bb54c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb54c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb54c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb54c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb54c-106">新しい[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bb54c-106">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb54c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bb54c-107">Prerequisites</span></span>
<span data-ttu-id="bb54c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb54c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb54c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb54c-110">Permission type</span></span>|<span data-ttu-id="bb54c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb54c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb54c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb54c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb54c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb54c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bb54c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb54c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb54c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb54c-115">Not supported.</span></span>|
|<span data-ttu-id="bb54c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb54c-116">Application</span></span>|<span data-ttu-id="bb54c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb54c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb54c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb54c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="bb54c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb54c-119">Request headers</span></span>
|<span data-ttu-id="bb54c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb54c-120">Header</span></span>|<span data-ttu-id="bb54c-121">値</span><span class="sxs-lookup"><span data-stu-id="bb54c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb54c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb54c-122">Authorization</span></span>|<span data-ttu-id="bb54c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb54c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb54c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bb54c-124">Accept</span></span>|<span data-ttu-id="bb54c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb54c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb54c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb54c-126">Request body</span></span>
<span data-ttu-id="bb54c-127">要求本文で、activeDirectoryWindowsAutopilotDeploymentProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb54c-127">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="bb54c-128">次の表に、activeDirectoryWindowsAutopilotDeploymentProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bb54c-128">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="bb54c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb54c-129">Property</span></span>|<span data-ttu-id="bb54c-130">型</span><span class="sxs-lookup"><span data-stu-id="bb54c-130">Type</span></span>|<span data-ttu-id="bb54c-131">説明</span><span class="sxs-lookup"><span data-stu-id="bb54c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb54c-132">id</span><span class="sxs-lookup"><span data-stu-id="bb54c-132">id</span></span>|<span data-ttu-id="bb54c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="bb54c-133">String</span></span>|<span data-ttu-id="bb54c-134">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルキー</span><span class="sxs-lookup"><span data-stu-id="bb54c-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bb54c-135">displayName</span></span>|<span data-ttu-id="bb54c-136">String</span><span class="sxs-lookup"><span data-stu-id="bb54c-136">String</span></span>|<span data-ttu-id="bb54c-137">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="bb54c-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-138">description</span><span class="sxs-lookup"><span data-stu-id="bb54c-138">description</span></span>|<span data-ttu-id="bb54c-139">String</span><span class="sxs-lookup"><span data-stu-id="bb54c-139">String</span></span>|<span data-ttu-id="bb54c-140">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="bb54c-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-141">language</span><span class="sxs-lookup"><span data-stu-id="bb54c-141">language</span></span>|<span data-ttu-id="bb54c-142">String</span><span class="sxs-lookup"><span data-stu-id="bb54c-142">String</span></span>|<span data-ttu-id="bb54c-143">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承したデバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="bb54c-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb54c-144">createdDateTime</span></span>|<span data-ttu-id="bb54c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb54c-145">DateTimeOffset</span></span>|<span data-ttu-id="bb54c-146">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの作成時刻</span><span class="sxs-lookup"><span data-stu-id="bb54c-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb54c-147">lastModifiedDateTime</span></span>|<span data-ttu-id="bb54c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb54c-148">DateTimeOffset</span></span>|<span data-ttu-id="bb54c-149">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="bb54c-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="bb54c-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="bb54c-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="bb54c-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="bb54c-152">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された、すぐに使える状態設定</span><span class="sxs-lookup"><span data-stu-id="bb54c-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="bb54c-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="bb54c-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="bb54c-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="bb54c-155">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承された登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="bb54c-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="bb54c-156">extractHardwareHash</span></span>|<span data-ttu-id="bb54c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb54c-157">Boolean</span></span>|<span data-ttu-id="bb54c-158">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されたプロファイルのハードウェアハッシュ抽出</span><span class="sxs-lookup"><span data-stu-id="bb54c-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="bb54c-159">deviceNameTemplate</span></span>|<span data-ttu-id="bb54c-160">String</span><span class="sxs-lookup"><span data-stu-id="bb54c-160">String</span></span>|<span data-ttu-id="bb54c-161">自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。</span><span class="sxs-lookup"><span data-stu-id="bb54c-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="bb54c-162">これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="bb54c-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="bb54c-163">テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="bb54c-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="bb54c-164">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bb54c-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="bb54c-165">deviceType</span></span>|[<span data-ttu-id="bb54c-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="bb54c-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="bb54c-167">このプロファイルを適用できる自動操縦デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="bb54c-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="bb54c-168">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="bb54c-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="bb54c-169">可能な値は、`windowsPc`、`surfaceHub2` です。</span><span class="sxs-lookup"><span data-stu-id="bb54c-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="bb54c-170">Enableホワイトグローブ</span><span class="sxs-lookup"><span data-stu-id="bb54c-170">enableWhiteGlove</span></span>|<span data-ttu-id="bb54c-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb54c-171">Boolean</span></span>|<span data-ttu-id="bb54c-172">プロファイルの自動操縦白の手袋を有効にします。</span><span class="sxs-lookup"><span data-stu-id="bb54c-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="bb54c-173">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bb54c-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="bb54c-174">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb54c-174">roleScopeTagIds</span></span>|<span data-ttu-id="bb54c-175">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="bb54c-175">String collection</span></span>|<span data-ttu-id="bb54c-176">プロファイルのスコープタグ。</span><span class="sxs-lookup"><span data-stu-id="bb54c-176">Scope tags for the profile.</span></span> <span data-ttu-id="bb54c-177">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bb54c-177">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bb54c-178">応答</span><span class="sxs-lookup"><span data-stu-id="bb54c-178">Response</span></span>
<span data-ttu-id="bb54c-179">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bb54c-179">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb54c-180">例</span><span class="sxs-lookup"><span data-stu-id="bb54c-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb54c-181">要求</span><span class="sxs-lookup"><span data-stu-id="bb54c-181">Request</span></span>
<span data-ttu-id="bb54c-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bb54c-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb54c-183">応答</span><span class="sxs-lookup"><span data-stu-id="bb54c-183">Response</span></span>
<span data-ttu-id="bb54c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bb54c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






