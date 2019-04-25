---
title: windows10EnrollmentCompletionPageConfiguration を作成する
description: 新しい windows10EnrollmentCompletionPageConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c2edde71ba4ec8b61fe8894f05b0a6501df053c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528044"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="d9356-103">windows10EnrollmentCompletionPageConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="d9356-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="d9356-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9356-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9356-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9356-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9356-106">新しい[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d9356-106">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9356-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d9356-107">Prerequisites</span></span>
<span data-ttu-id="d9356-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9356-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9356-110">Permission type</span></span>|<span data-ttu-id="d9356-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9356-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9356-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9356-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9356-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9356-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d9356-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9356-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9356-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9356-115">Not supported.</span></span>|
|<span data-ttu-id="d9356-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9356-116">Application</span></span>|<span data-ttu-id="d9356-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9356-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9356-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9356-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d9356-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9356-119">Request headers</span></span>
|<span data-ttu-id="d9356-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9356-120">Header</span></span>|<span data-ttu-id="d9356-121">値</span><span class="sxs-lookup"><span data-stu-id="d9356-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9356-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9356-122">Authorization</span></span>|<span data-ttu-id="d9356-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9356-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9356-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d9356-124">Accept</span></span>|<span data-ttu-id="d9356-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9356-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9356-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9356-126">Request body</span></span>
<span data-ttu-id="d9356-127">要求本文で、windows10EnrollmentCompletionPageConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d9356-127">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="d9356-128">次の表に、windows10EnrollmentCompletionPageConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d9356-128">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="d9356-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9356-129">Property</span></span>|<span data-ttu-id="d9356-130">型</span><span class="sxs-lookup"><span data-stu-id="d9356-130">Type</span></span>|<span data-ttu-id="d9356-131">説明</span><span class="sxs-lookup"><span data-stu-id="d9356-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9356-132">id</span><span class="sxs-lookup"><span data-stu-id="d9356-132">id</span></span>|<span data-ttu-id="d9356-133">String</span><span class="sxs-lookup"><span data-stu-id="d9356-133">String</span></span>|<span data-ttu-id="d9356-134">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id</span><span class="sxs-lookup"><span data-stu-id="d9356-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9356-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d9356-135">displayName</span></span>|<span data-ttu-id="d9356-136">String</span><span class="sxs-lookup"><span data-stu-id="d9356-136">String</span></span>|<span data-ttu-id="d9356-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d9356-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9356-138">description</span><span class="sxs-lookup"><span data-stu-id="d9356-138">description</span></span>|<span data-ttu-id="d9356-139">String</span><span class="sxs-lookup"><span data-stu-id="d9356-139">String</span></span>|<span data-ttu-id="d9356-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d9356-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9356-141">priority</span><span class="sxs-lookup"><span data-stu-id="d9356-141">priority</span></span>|<span data-ttu-id="d9356-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d9356-142">Int32</span></span>|<span data-ttu-id="d9356-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d9356-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9356-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9356-144">createdDateTime</span></span>|<span data-ttu-id="d9356-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9356-145">DateTimeOffset</span></span>|<span data-ttu-id="d9356-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d9356-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9356-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9356-147">lastModifiedDateTime</span></span>|<span data-ttu-id="d9356-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9356-148">DateTimeOffset</span></span>|<span data-ttu-id="d9356-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d9356-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9356-150">version</span><span class="sxs-lookup"><span data-stu-id="d9356-150">version</span></span>|<span data-ttu-id="d9356-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d9356-151">Int32</span></span>|<span data-ttu-id="d9356-152">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d9356-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d9356-153">showinstallationprogress</span><span class="sxs-lookup"><span data-stu-id="d9356-153">showInstallationProgress</span></span>|<span data-ttu-id="d9356-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="d9356-154">Boolean</span></span>|<span data-ttu-id="d9356-155">ユーザーにインストールの進行状況を表示または非表示にする</span><span class="sxs-lookup"><span data-stu-id="d9356-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="d9356-156">blockdevicesetupretrybyuser</span><span class="sxs-lookup"><span data-stu-id="d9356-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="d9356-157">ブール値</span><span class="sxs-lookup"><span data-stu-id="d9356-157">Boolean</span></span>|<span data-ttu-id="d9356-158">ユーザーがインストールエラー時にセットアップを再試行できるようにする</span><span class="sxs-lookup"><span data-stu-id="d9356-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="d9356-159">allowdeviceresetoninstallfailure</span><span class="sxs-lookup"><span data-stu-id="d9356-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="d9356-160">ブール値</span><span class="sxs-lookup"><span data-stu-id="d9356-160">Boolean</span></span>|<span data-ttu-id="d9356-161">インストール失敗時にデバイスのリセットを許可またはブロックする</span><span class="sxs-lookup"><span data-stu-id="d9356-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="d9356-162">allowlogcollectiononinstallfailure</span><span class="sxs-lookup"><span data-stu-id="d9356-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="d9356-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="d9356-163">Boolean</span></span>|<span data-ttu-id="d9356-164">インストール失敗時にログ収集を許可またはブロックする</span><span class="sxs-lookup"><span data-stu-id="d9356-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="d9356-165">customerrormessage</span><span class="sxs-lookup"><span data-stu-id="d9356-165">customErrorMessage</span></span>|<span data-ttu-id="d9356-166">String</span><span class="sxs-lookup"><span data-stu-id="d9356-166">String</span></span>|<span data-ttu-id="d9356-167">インストールエラーが発生したときに表示するカスタムエラーメッセージを設定する</span><span class="sxs-lookup"><span data-stu-id="d9356-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="d9356-168">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d9356-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="d9356-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d9356-169">Int32</span></span>|<span data-ttu-id="d9356-170">インストールの進行状況のタイムアウトを分単位で設定する</span><span class="sxs-lookup"><span data-stu-id="d9356-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="d9356-171">allowdeviceuseoninstallfailure</span><span class="sxs-lookup"><span data-stu-id="d9356-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="d9356-172">ブール値</span><span class="sxs-lookup"><span data-stu-id="d9356-172">Boolean</span></span>|<span data-ttu-id="d9356-173">インストールエラー時にユーザーがデバイスを引き続き使用できるようにする</span><span class="sxs-lookup"><span data-stu-id="d9356-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="d9356-174">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="d9356-174">selectedMobileAppIds</span></span>|<span data-ttu-id="d9356-175">String collection</span><span class="sxs-lookup"><span data-stu-id="d9356-175">String collection</span></span>|<span data-ttu-id="d9356-176">インストールの状態を追跡するために選択されたアプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9356-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="d9356-177">応答</span><span class="sxs-lookup"><span data-stu-id="d9356-177">Response</span></span>
<span data-ttu-id="d9356-178">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d9356-178">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9356-179">例</span><span class="sxs-lookup"><span data-stu-id="d9356-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9356-180">要求</span><span class="sxs-lookup"><span data-stu-id="d9356-180">Request</span></span>
<span data-ttu-id="d9356-181">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d9356-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="d9356-182">応答</span><span class="sxs-lookup"><span data-stu-id="d9356-182">Response</span></span>
<span data-ttu-id="d9356-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d9356-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





