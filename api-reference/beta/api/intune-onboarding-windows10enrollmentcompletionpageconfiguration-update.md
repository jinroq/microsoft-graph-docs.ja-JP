---
title: Windows10EnrollmentCompletionPageConfiguration を更新します。
description: Windows10EnrollmentCompletionPageConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c7d3937ac02ae0a16a48bfaeea170310bbc3833
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416245"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="a6d1f-103">Windows10EnrollmentCompletionPageConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="a6d1f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a6d1f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6d1f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6d1f-107">[Windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6d1f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a6d1f-108">Prerequisites</span></span>
<span data-ttu-id="a6d1f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6d1f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6d1f-111">Permission type</span></span>|<span data-ttu-id="a6d1f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6d1f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6d1f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6d1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6d1f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6d1f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6d1f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6d1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6d1f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-116">Not supported.</span></span>|
|<span data-ttu-id="a6d1f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6d1f-117">Application</span></span>|<span data-ttu-id="a6d1f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6d1f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6d1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6d1f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6d1f-120">Request headers</span></span>
|<span data-ttu-id="a6d1f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6d1f-121">Header</span></span>|<span data-ttu-id="a6d1f-122">値</span><span class="sxs-lookup"><span data-stu-id="a6d1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6d1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6d1f-123">Authorization</span></span>|<span data-ttu-id="a6d1f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6d1f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6d1f-125">Accept</span></span>|<span data-ttu-id="a6d1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6d1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6d1f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6d1f-127">Request body</span></span>
<span data-ttu-id="a6d1f-128">要求の本文に[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="a6d1f-129">[Windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="a6d1f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6d1f-130">Property</span></span>|<span data-ttu-id="a6d1f-131">型</span><span class="sxs-lookup"><span data-stu-id="a6d1f-131">Type</span></span>|<span data-ttu-id="a6d1f-132">説明</span><span class="sxs-lookup"><span data-stu-id="a6d1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6d1f-133">id</span><span class="sxs-lookup"><span data-stu-id="a6d1f-133">id</span></span>|<span data-ttu-id="a6d1f-134">String</span><span class="sxs-lookup"><span data-stu-id="a6d1f-134">String</span></span>|<span data-ttu-id="a6d1f-135">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6d1f-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6d1f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a6d1f-136">displayName</span></span>|<span data-ttu-id="a6d1f-137">String</span><span class="sxs-lookup"><span data-stu-id="a6d1f-137">String</span></span>|<span data-ttu-id="a6d1f-138">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6d1f-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6d1f-139">説明</span><span class="sxs-lookup"><span data-stu-id="a6d1f-139">description</span></span>|<span data-ttu-id="a6d1f-140">String</span><span class="sxs-lookup"><span data-stu-id="a6d1f-140">String</span></span>|<span data-ttu-id="a6d1f-141">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6d1f-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6d1f-142">priority</span><span class="sxs-lookup"><span data-stu-id="a6d1f-142">priority</span></span>|<span data-ttu-id="a6d1f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d1f-143">Int32</span></span>|<span data-ttu-id="a6d1f-144">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6d1f-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6d1f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6d1f-145">createdDateTime</span></span>|<span data-ttu-id="a6d1f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6d1f-146">DateTimeOffset</span></span>|<span data-ttu-id="a6d1f-147">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6d1f-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6d1f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6d1f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a6d1f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6d1f-149">DateTimeOffset</span></span>|<span data-ttu-id="a6d1f-150">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6d1f-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6d1f-151">version</span><span class="sxs-lookup"><span data-stu-id="a6d1f-151">version</span></span>|<span data-ttu-id="a6d1f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d1f-152">Int32</span></span>|<span data-ttu-id="a6d1f-153">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6d1f-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6d1f-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="a6d1f-154">showInstallationProgress</span></span>|<span data-ttu-id="a6d1f-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6d1f-155">Boolean</span></span>|<span data-ttu-id="a6d1f-156">ユーザーにインストールの進行状況の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="a6d1f-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="a6d1f-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="a6d1f-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="a6d1f-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6d1f-158">Boolean</span></span>|<span data-ttu-id="a6d1f-159">インストールの失敗時にセットアップを再実行するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="a6d1f-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="a6d1f-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="a6d1f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6d1f-161">Boolean</span></span>|<span data-ttu-id="a6d1f-162">許可またはブロック デバイスのインストールの失敗時にリセット</span><span class="sxs-lookup"><span data-stu-id="a6d1f-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="a6d1f-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="a6d1f-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="a6d1f-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6d1f-164">Boolean</span></span>|<span data-ttu-id="a6d1f-165">許可またはブロックのインストールの失敗時にログの収集</span><span class="sxs-lookup"><span data-stu-id="a6d1f-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="a6d1f-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="a6d1f-166">customErrorMessage</span></span>|<span data-ttu-id="a6d1f-167">String</span><span class="sxs-lookup"><span data-stu-id="a6d1f-167">String</span></span>|<span data-ttu-id="a6d1f-168">インストールの失敗時に表示するカスタム エラー メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="a6d1f-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a6d1f-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="a6d1f-170">Int32</span><span class="sxs-lookup"><span data-stu-id="a6d1f-170">Int32</span></span>|<span data-ttu-id="a6d1f-171">インストールの進行状況のタイムアウトを分単位で設定します。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="a6d1f-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="a6d1f-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="a6d1f-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6d1f-173">Boolean</span></span>|<span data-ttu-id="a6d1f-174">インストールの失敗時にデバイスを使用するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="a6d1f-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="a6d1f-175">selectedMobileAppIds</span></span>|<span data-ttu-id="a6d1f-176">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a6d1f-176">String collection</span></span>|<span data-ttu-id="a6d1f-177">インストールのステータスを追跡するために選択したアプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6d1f-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="a6d1f-178">応答</span><span class="sxs-lookup"><span data-stu-id="a6d1f-178">Response</span></span>
<span data-ttu-id="a6d1f-179">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-179">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6d1f-180">例</span><span class="sxs-lookup"><span data-stu-id="a6d1f-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6d1f-181">要求</span><span class="sxs-lookup"><span data-stu-id="a6d1f-181">Request</span></span>
<span data-ttu-id="a6d1f-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6d1f-183">応答</span><span class="sxs-lookup"><span data-stu-id="a6d1f-183">Response</span></span>
<span data-ttu-id="a6d1f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6d1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




