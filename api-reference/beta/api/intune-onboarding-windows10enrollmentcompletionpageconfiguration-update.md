---
title: Windows10EnrollmentCompletionPageConfiguration の更新
description: Windows10EnrollmentCompletionPageConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e6accf7b452a94a54a1006e3b11b9d9c6cbdec6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899726"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="d8ec6-103">Windows10EnrollmentCompletionPageConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d8ec6-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="d8ec6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8ec6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8ec6-106">[Windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-106">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8ec6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d8ec6-107">Prerequisites</span></span>
<span data-ttu-id="d8ec6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ec6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8ec6-110">Permission type</span></span>|<span data-ttu-id="d8ec6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8ec6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8ec6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8ec6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8ec6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ec6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d8ec6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8ec6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8ec6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-115">Not supported.</span></span>|
|<span data-ttu-id="d8ec6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8ec6-116">Application</span></span>|<span data-ttu-id="d8ec6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8ec6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8ec6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d8ec6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8ec6-119">Request headers</span></span>
|<span data-ttu-id="d8ec6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8ec6-120">Header</span></span>|<span data-ttu-id="d8ec6-121">値</span><span class="sxs-lookup"><span data-stu-id="d8ec6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8ec6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8ec6-122">Authorization</span></span>|<span data-ttu-id="d8ec6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8ec6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d8ec6-124">Accept</span></span>|<span data-ttu-id="d8ec6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8ec6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8ec6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8ec6-126">Request body</span></span>
<span data-ttu-id="d8ec6-127">要求本文で、 [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="d8ec6-128">次の表に、 [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="d8ec6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8ec6-129">Property</span></span>|<span data-ttu-id="d8ec6-130">型</span><span class="sxs-lookup"><span data-stu-id="d8ec6-130">Type</span></span>|<span data-ttu-id="d8ec6-131">説明</span><span class="sxs-lookup"><span data-stu-id="d8ec6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8ec6-132">id</span><span class="sxs-lookup"><span data-stu-id="d8ec6-132">id</span></span>|<span data-ttu-id="d8ec6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d8ec6-133">String</span></span>|<span data-ttu-id="d8ec6-134">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="d8ec6-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8ec6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d8ec6-135">displayName</span></span>|<span data-ttu-id="d8ec6-136">String</span><span class="sxs-lookup"><span data-stu-id="d8ec6-136">String</span></span>|<span data-ttu-id="d8ec6-137">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8ec6-138">description</span><span class="sxs-lookup"><span data-stu-id="d8ec6-138">description</span></span>|<span data-ttu-id="d8ec6-139">String</span><span class="sxs-lookup"><span data-stu-id="d8ec6-139">String</span></span>|<span data-ttu-id="d8ec6-140">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="d8ec6-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8ec6-141">priority</span><span class="sxs-lookup"><span data-stu-id="d8ec6-141">priority</span></span>|<span data-ttu-id="d8ec6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ec6-142">Int32</span></span>|<span data-ttu-id="d8ec6-143">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="d8ec6-144">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="d8ec6-145">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d8ec6-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8ec6-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8ec6-146">createdDateTime</span></span>|<span data-ttu-id="d8ec6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8ec6-147">DateTimeOffset</span></span>|<span data-ttu-id="d8ec6-148">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時</span><span class="sxs-lookup"><span data-stu-id="d8ec6-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8ec6-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8ec6-149">lastModifiedDateTime</span></span>|<span data-ttu-id="d8ec6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8ec6-150">DateTimeOffset</span></span>|<span data-ttu-id="d8ec6-151">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8ec6-152">version</span><span class="sxs-lookup"><span data-stu-id="d8ec6-152">version</span></span>|<span data-ttu-id="d8ec6-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ec6-153">Int32</span></span>|<span data-ttu-id="d8ec6-154">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="d8ec6-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d8ec6-155">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="d8ec6-155">showInstallationProgress</span></span>|<span data-ttu-id="d8ec6-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ec6-156">Boolean</span></span>|<span data-ttu-id="d8ec6-157">ユーザーにインストールの進行状況を表示または非表示にする</span><span class="sxs-lookup"><span data-stu-id="d8ec6-157">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="d8ec6-158">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="d8ec6-158">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="d8ec6-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ec6-159">Boolean</span></span>|<span data-ttu-id="d8ec6-160">ユーザーがインストールエラー時にセットアップを再試行できるようにする</span><span class="sxs-lookup"><span data-stu-id="d8ec6-160">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="d8ec6-161">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d8ec6-161">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="d8ec6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ec6-162">Boolean</span></span>|<span data-ttu-id="d8ec6-163">インストール失敗時にデバイスのリセットを許可またはブロックする</span><span class="sxs-lookup"><span data-stu-id="d8ec6-163">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="d8ec6-164">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d8ec6-164">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="d8ec6-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ec6-165">Boolean</span></span>|<span data-ttu-id="d8ec6-166">インストール失敗時にログ収集を許可またはブロックする</span><span class="sxs-lookup"><span data-stu-id="d8ec6-166">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="d8ec6-167">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="d8ec6-167">customErrorMessage</span></span>|<span data-ttu-id="d8ec6-168">String</span><span class="sxs-lookup"><span data-stu-id="d8ec6-168">String</span></span>|<span data-ttu-id="d8ec6-169">インストールエラーが発生したときに表示するカスタムエラーメッセージを設定する</span><span class="sxs-lookup"><span data-stu-id="d8ec6-169">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="d8ec6-170">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d8ec6-170">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="d8ec6-171">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ec6-171">Int32</span></span>|<span data-ttu-id="d8ec6-172">インストールの進行状況のタイムアウトを分単位で設定する</span><span class="sxs-lookup"><span data-stu-id="d8ec6-172">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="d8ec6-173">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d8ec6-173">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="d8ec6-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8ec6-174">Boolean</span></span>|<span data-ttu-id="d8ec6-175">インストールエラー時にユーザーがデバイスを引き続き使用できるようにする</span><span class="sxs-lookup"><span data-stu-id="d8ec6-175">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="d8ec6-176">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="d8ec6-176">selectedMobileAppIds</span></span>|<span data-ttu-id="d8ec6-177">String collection</span><span class="sxs-lookup"><span data-stu-id="d8ec6-177">String collection</span></span>|<span data-ttu-id="d8ec6-178">インストールの状態を追跡するために選択されたアプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8ec6-178">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="d8ec6-179">応答</span><span class="sxs-lookup"><span data-stu-id="d8ec6-179">Response</span></span>
<span data-ttu-id="d8ec6-180">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-180">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8ec6-181">例</span><span class="sxs-lookup"><span data-stu-id="d8ec6-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8ec6-182">要求</span><span class="sxs-lookup"><span data-stu-id="d8ec6-182">Request</span></span>
<span data-ttu-id="d8ec6-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 583

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d8ec6-184">応答</span><span class="sxs-lookup"><span data-stu-id="d8ec6-184">Response</span></span>
<span data-ttu-id="d8ec6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8ec6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 755

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "77bf8248-8248-77bf-4882-bf774882bf77",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ]
}
```




