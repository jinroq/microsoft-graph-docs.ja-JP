---
title: androidManagedAppRegistration の作成
description: 新しい androidManagedAppRegistration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c05ba7fa13577134b148c8af836e3ba453a1e40
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571460"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="c8381-103">androidManagedAppRegistration の作成</span><span class="sxs-lookup"><span data-stu-id="c8381-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="c8381-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8381-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8381-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8381-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8381-106">新しい [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8381-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8381-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8381-107">Prerequisites</span></span>
<span data-ttu-id="c8381-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8381-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8381-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8381-110">Permission type</span></span>|<span data-ttu-id="c8381-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8381-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8381-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8381-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8381-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8381-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8381-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8381-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8381-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8381-115">Not supported.</span></span>|
|<span data-ttu-id="c8381-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8381-116">Application</span></span>|<span data-ttu-id="c8381-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8381-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8381-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8381-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="c8381-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8381-119">Request headers</span></span>
|<span data-ttu-id="c8381-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8381-120">Header</span></span>|<span data-ttu-id="c8381-121">値</span><span class="sxs-lookup"><span data-stu-id="c8381-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8381-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8381-122">Authorization</span></span>|<span data-ttu-id="c8381-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8381-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8381-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c8381-124">Accept</span></span>|<span data-ttu-id="c8381-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8381-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8381-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8381-126">Request body</span></span>
<span data-ttu-id="c8381-127">要求本文で、androidManagedAppRegistration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8381-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="c8381-128">次の表に、androidManagedAppRegistration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c8381-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="c8381-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8381-129">Property</span></span>|<span data-ttu-id="c8381-130">型</span><span class="sxs-lookup"><span data-stu-id="c8381-130">Type</span></span>|<span data-ttu-id="c8381-131">説明</span><span class="sxs-lookup"><span data-stu-id="c8381-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8381-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8381-132">createdDateTime</span></span>|<span data-ttu-id="c8381-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8381-133">DateTimeOffset</span></span>|<span data-ttu-id="c8381-134">作成日時 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="c8381-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c8381-135">lastSyncDateTime</span></span>|<span data-ttu-id="c8381-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8381-136">DateTimeOffset</span></span>|<span data-ttu-id="c8381-137">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="c8381-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="c8381-138">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8381-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="c8381-139">applicationVersion</span></span>|<span data-ttu-id="c8381-140">String</span><span class="sxs-lookup"><span data-stu-id="c8381-140">String</span></span>|<span data-ttu-id="c8381-141">アプリのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c8381-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c8381-142">managementSdkVersion</span></span>|<span data-ttu-id="c8381-143">String</span><span class="sxs-lookup"><span data-stu-id="c8381-143">String</span></span>|<span data-ttu-id="c8381-144">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c8381-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="c8381-145">platformVersion</span></span>|<span data-ttu-id="c8381-146">String</span><span class="sxs-lookup"><span data-stu-id="c8381-146">String</span></span>|<span data-ttu-id="c8381-147">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c8381-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="c8381-148">deviceType</span></span>|<span data-ttu-id="c8381-149">String</span><span class="sxs-lookup"><span data-stu-id="c8381-149">String</span></span>|<span data-ttu-id="c8381-150">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c8381-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c8381-151">deviceTag</span></span>|<span data-ttu-id="c8381-152">String</span><span class="sxs-lookup"><span data-stu-id="c8381-152">String</span></span>|<span data-ttu-id="c8381-153">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="c8381-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="c8381-154">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="c8381-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="c8381-155">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8381-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="c8381-156">deviceName</span></span>|<span data-ttu-id="c8381-157">String</span><span class="sxs-lookup"><span data-stu-id="c8381-157">String</span></span>|<span data-ttu-id="c8381-158">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c8381-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-159">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="c8381-159">managedDeviceId</span></span>|<span data-ttu-id="c8381-160">String</span><span class="sxs-lookup"><span data-stu-id="c8381-160">String</span></span>|<span data-ttu-id="c8381-161">ホストデバイスの管理デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="c8381-161">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="c8381-162">ホストデバイスが管理されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c8381-162">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="c8381-163">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8381-163">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-164">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="c8381-164">azureADDeviceId</span></span>|<span data-ttu-id="c8381-165">String</span><span class="sxs-lookup"><span data-stu-id="c8381-165">String</span></span>|<span data-ttu-id="c8381-166">ホストデバイスの Azure Active Directory デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="c8381-166">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="c8381-167">ホストデバイスが Azure Active Directory に登録されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c8381-167">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="c8381-168">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8381-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-169">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c8381-169">deviceModel</span></span>|<span data-ttu-id="c8381-170">String</span><span class="sxs-lookup"><span data-stu-id="c8381-170">String</span></span>|<span data-ttu-id="c8381-171">[managedAppRegistration](../resources/intune-mam-managedappregistration.md)から継承された現在のアプリの登録のデバイスモデル。</span><span class="sxs-lookup"><span data-stu-id="c8381-171">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-172">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="c8381-172">deviceManufacturer</span></span>|<span data-ttu-id="c8381-173">String</span><span class="sxs-lookup"><span data-stu-id="c8381-173">String</span></span>|<span data-ttu-id="c8381-174">[managedAppRegistration](../resources/intune-mam-managedappregistration.md)から継承された現在のアプリの登録のデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="c8381-174">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-175">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="c8381-175">flaggedReasons</span></span>|<span data-ttu-id="c8381-176">[managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c8381-176">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="c8381-177">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="c8381-177">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="c8381-178">例:</span><span class="sxs-lookup"><span data-stu-id="c8381-178">E.g.</span></span> <span data-ttu-id="c8381-179">[managedAppRegistration](../resources/intune-mam-managedappregistration.md)から継承されたルートデバイスで実行されているアプリ。</span><span class="sxs-lookup"><span data-stu-id="c8381-179">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="c8381-180">可能な値は、`none`、`rootedDevice`、`androidBootloaderUnlocked`、`androidFactoryRomModified` です。</span><span class="sxs-lookup"><span data-stu-id="c8381-180">Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span></span>|
|<span data-ttu-id="c8381-181">userId</span><span class="sxs-lookup"><span data-stu-id="c8381-181">userId</span></span>|<span data-ttu-id="c8381-182">String</span><span class="sxs-lookup"><span data-stu-id="c8381-182">String</span></span>|<span data-ttu-id="c8381-183">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="c8381-183">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="c8381-184">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8381-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-185">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c8381-185">appIdentifier</span></span>|[<span data-ttu-id="c8381-186">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c8381-186">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c8381-187">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c8381-187">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-188">id</span><span class="sxs-lookup"><span data-stu-id="c8381-188">id</span></span>|<span data-ttu-id="c8381-189">String</span><span class="sxs-lookup"><span data-stu-id="c8381-189">String</span></span>|<span data-ttu-id="c8381-190">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c8381-190">Key of the entity.</span></span> <span data-ttu-id="c8381-191">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8381-191">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-192">version</span><span class="sxs-lookup"><span data-stu-id="c8381-192">version</span></span>|<span data-ttu-id="c8381-193">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c8381-193">String</span></span>|<span data-ttu-id="c8381-194">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c8381-194">Version of the entity.</span></span> <span data-ttu-id="c8381-195">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c8381-195">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c8381-196">パッチバージョン</span><span class="sxs-lookup"><span data-stu-id="c8381-196">patchVersion</span></span>|<span data-ttu-id="c8381-197">String</span><span class="sxs-lookup"><span data-stu-id="c8381-197">String</span></span>|<span data-ttu-id="c8381-198">現在の android アプリの登録のパッチバージョン</span><span class="sxs-lookup"><span data-stu-id="c8381-198">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="c8381-199">応答</span><span class="sxs-lookup"><span data-stu-id="c8381-199">Response</span></span>
<span data-ttu-id="c8381-200">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8381-200">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8381-201">例</span><span class="sxs-lookup"><span data-stu-id="c8381-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8381-202">要求</span><span class="sxs-lookup"><span data-stu-id="c8381-202">Request</span></span>
<span data-ttu-id="c8381-203">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8381-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 879

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### <a name="response"></a><span data-ttu-id="c8381-204">応答</span><span class="sxs-lookup"><span data-stu-id="c8381-204">Response</span></span>
<span data-ttu-id="c8381-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8381-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 987

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```




