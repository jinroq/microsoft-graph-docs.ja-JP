---
title: ActiveDirectoryWindowsAutopilotDeploymentProfile を更新します。
description: ActiveDirectoryWindowsAutopilotDeploymentProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 929ab9b026052422187eb4e94446011f3abb6f26
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404366"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="ff339-103">ActiveDirectoryWindowsAutopilotDeploymentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="ff339-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="ff339-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff339-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff339-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff339-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff339-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff339-107">[ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ff339-107">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff339-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ff339-108">Prerequisites</span></span>
<span data-ttu-id="ff339-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff339-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ff339-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff339-111">Permission type</span></span>|<span data-ttu-id="ff339-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff339-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff339-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff339-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff339-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff339-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ff339-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff339-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff339-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff339-116">Not supported.</span></span>|
|<span data-ttu-id="ff339-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff339-117">Application</span></span>|<span data-ttu-id="ff339-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff339-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff339-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff339-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="ff339-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff339-120">Request headers</span></span>
|<span data-ttu-id="ff339-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff339-121">Header</span></span>|<span data-ttu-id="ff339-122">値</span><span class="sxs-lookup"><span data-stu-id="ff339-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff339-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff339-123">Authorization</span></span>|<span data-ttu-id="ff339-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ff339-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff339-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff339-125">Accept</span></span>|<span data-ttu-id="ff339-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff339-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff339-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff339-127">Request body</span></span>
<span data-ttu-id="ff339-128">要求の本文に[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ff339-128">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="ff339-129">[ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="ff339-129">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="ff339-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff339-130">Property</span></span>|<span data-ttu-id="ff339-131">型</span><span class="sxs-lookup"><span data-stu-id="ff339-131">Type</span></span>|<span data-ttu-id="ff339-132">説明</span><span class="sxs-lookup"><span data-stu-id="ff339-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff339-133">id</span><span class="sxs-lookup"><span data-stu-id="ff339-133">id</span></span>|<span data-ttu-id="ff339-134">String</span><span class="sxs-lookup"><span data-stu-id="ff339-134">String</span></span>|<span data-ttu-id="ff339-135">プロファイル キーは、 [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="ff339-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ff339-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ff339-136">displayName</span></span>|<span data-ttu-id="ff339-137">String</span><span class="sxs-lookup"><span data-stu-id="ff339-137">String</span></span>|<span data-ttu-id="ff339-138">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるプロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="ff339-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ff339-139">説明</span><span class="sxs-lookup"><span data-stu-id="ff339-139">description</span></span>|<span data-ttu-id="ff339-140">String</span><span class="sxs-lookup"><span data-stu-id="ff339-140">String</span></span>|<span data-ttu-id="ff339-141">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるプロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="ff339-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ff339-142">language</span><span class="sxs-lookup"><span data-stu-id="ff339-142">language</span></span>|<span data-ttu-id="ff339-143">String</span><span class="sxs-lookup"><span data-stu-id="ff339-143">String</span></span>|<span data-ttu-id="ff339-144">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるデバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="ff339-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ff339-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff339-145">createdDateTime</span></span>|<span data-ttu-id="ff339-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff339-146">DateTimeOffset</span></span>|<span data-ttu-id="ff339-147">継承されるプロファイル作成時は、 [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から</span><span class="sxs-lookup"><span data-stu-id="ff339-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ff339-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff339-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ff339-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff339-149">DateTimeOffset</span></span>|<span data-ttu-id="ff339-150">プロファイルは、 [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)からの継承の時間を最終更新日</span><span class="sxs-lookup"><span data-stu-id="ff339-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ff339-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="ff339-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="ff339-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="ff339-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="ff339-153">ボックス発生[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)からの継承を設定します。</span><span class="sxs-lookup"><span data-stu-id="ff339-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ff339-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="ff339-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="ff339-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="ff339-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="ff339-156">登録ステータス画面が[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)からの継承を設定します。</span><span class="sxs-lookup"><span data-stu-id="ff339-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ff339-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="ff339-157">extractHardwareHash</span></span>|<span data-ttu-id="ff339-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff339-158">Boolean</span></span>|<span data-ttu-id="ff339-159">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されるプロファイルの HardwareHash の抽出</span><span class="sxs-lookup"><span data-stu-id="ff339-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ff339-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="ff339-160">deviceNameTemplate</span></span>|<span data-ttu-id="ff339-161">String</span><span class="sxs-lookup"><span data-stu-id="ff339-161">String</span></span>|<span data-ttu-id="ff339-162">自動操縦装置のデバイスの名前を指定するために使用するテンプレートです。</span><span class="sxs-lookup"><span data-stu-id="ff339-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="ff339-163">これは、ユーザー設定のテキスト、デバイスのシリアル番号またはランダムに生成された番号のいずれかが含まれていることもできます。</span><span class="sxs-lookup"><span data-stu-id="ff339-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="ff339-164">テンプレートによって生成されたテキストの長さの合計は、15 個以内の文字を使用できます。</span><span class="sxs-lookup"><span data-stu-id="ff339-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="ff339-165">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="ff339-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ff339-166">応答</span><span class="sxs-lookup"><span data-stu-id="ff339-166">Response</span></span>
<span data-ttu-id="ff339-167">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ff339-167">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff339-168">例</span><span class="sxs-lookup"><span data-stu-id="ff339-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff339-169">要求</span><span class="sxs-lookup"><span data-stu-id="ff339-169">Request</span></span>
<span data-ttu-id="ff339-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff339-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1044

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
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a><span data-ttu-id="ff339-171">応答</span><span class="sxs-lookup"><span data-stu-id="ff339-171">Response</span></span>
<span data-ttu-id="ff339-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff339-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

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
  "deviceNameTemplate": "Device Name Template value"
}
```




