---
title: androidManagedAppRegistration の作成
description: 新しい androidManagedAppRegistration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 83a2fd4c1967da5bdb401ab57bf603dace128f05
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408496"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="2cc06-103">androidManagedAppRegistration の作成</span><span class="sxs-lookup"><span data-stu-id="2cc06-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="2cc06-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2cc06-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2cc06-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cc06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cc06-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2cc06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc06-107">新しい [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2cc06-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cc06-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2cc06-108">Prerequisites</span></span>
<span data-ttu-id="2cc06-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cc06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2cc06-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2cc06-111">Permission type</span></span>|<span data-ttu-id="2cc06-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2cc06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cc06-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2cc06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cc06-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc06-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2cc06-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2cc06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cc06-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cc06-116">Not supported.</span></span>|
|<span data-ttu-id="2cc06-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2cc06-117">Application</span></span>|<span data-ttu-id="2cc06-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cc06-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cc06-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2cc06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="2cc06-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2cc06-120">Request headers</span></span>
|<span data-ttu-id="2cc06-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2cc06-121">Header</span></span>|<span data-ttu-id="2cc06-122">値</span><span class="sxs-lookup"><span data-stu-id="2cc06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cc06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cc06-123">Authorization</span></span>|<span data-ttu-id="2cc06-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2cc06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cc06-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2cc06-125">Accept</span></span>|<span data-ttu-id="2cc06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cc06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cc06-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2cc06-127">Request body</span></span>
<span data-ttu-id="2cc06-128">要求本文で、androidManagedAppRegistration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2cc06-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="2cc06-129">次の表に、androidManagedAppRegistration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2cc06-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="2cc06-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cc06-130">Property</span></span>|<span data-ttu-id="2cc06-131">型</span><span class="sxs-lookup"><span data-stu-id="2cc06-131">Type</span></span>|<span data-ttu-id="2cc06-132">説明</span><span class="sxs-lookup"><span data-stu-id="2cc06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc06-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cc06-133">createdDateTime</span></span>|<span data-ttu-id="2cc06-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cc06-134">DateTimeOffset</span></span>|<span data-ttu-id="2cc06-135">作成日時 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="2cc06-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2cc06-136">lastSyncDateTime</span></span>|<span data-ttu-id="2cc06-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cc06-137">DateTimeOffset</span></span>|<span data-ttu-id="2cc06-138">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="2cc06-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="2cc06-139">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cc06-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="2cc06-140">applicationVersion</span></span>|<span data-ttu-id="2cc06-141">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-141">String</span></span>|<span data-ttu-id="2cc06-142">アプリのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2cc06-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="2cc06-143">managementSdkVersion</span></span>|<span data-ttu-id="2cc06-144">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-144">String</span></span>|<span data-ttu-id="2cc06-145">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2cc06-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="2cc06-146">platformVersion</span></span>|<span data-ttu-id="2cc06-147">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-147">String</span></span>|<span data-ttu-id="2cc06-148">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2cc06-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="2cc06-149">deviceType</span></span>|<span data-ttu-id="2cc06-150">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-150">String</span></span>|<span data-ttu-id="2cc06-151">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2cc06-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="2cc06-152">deviceTag</span></span>|<span data-ttu-id="2cc06-153">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-153">String</span></span>|<span data-ttu-id="2cc06-154">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="2cc06-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="2cc06-155">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="2cc06-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="2cc06-156">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cc06-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="2cc06-157">deviceName</span></span>|<span data-ttu-id="2cc06-158">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-158">String</span></span>|<span data-ttu-id="2cc06-159">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2cc06-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="2cc06-160">managedDeviceId</span></span>|<span data-ttu-id="2cc06-161">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-161">String</span></span>|<span data-ttu-id="2cc06-162">ホスト ・ デバイスの管理デバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="2cc06-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="2cc06-163">ホスト ・ デバイスが管理されている場合にも、値を空にする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2cc06-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="2cc06-164">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cc06-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="2cc06-165">azureADDeviceId</span></span>|<span data-ttu-id="2cc06-166">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-166">String</span></span>|<span data-ttu-id="2cc06-167">ホスト ・ デバイスの Azure Active Directory のデバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="2cc06-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="2cc06-168">ホスト ・ デバイスは、Azure Active Directory が登録されている場合でも、値を空にする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2cc06-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="2cc06-169">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cc06-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2cc06-170">deviceModel</span></span>|<span data-ttu-id="2cc06-171">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-171">String</span></span>|<span data-ttu-id="2cc06-172">[ManagedAppRegistration](../resources/intune-mam-managedappregistration.md)から現在のアプリケーション登録継承用のデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="2cc06-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-173">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="2cc06-173">deviceManufacturer</span></span>|<span data-ttu-id="2cc06-174">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-174">String</span></span>|<span data-ttu-id="2cc06-175">[ManagedAppRegistration](../resources/intune-mam-managedappregistration.md)から現在のアプリケーション登録継承のデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="2cc06-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="2cc06-176">flaggedReasons</span></span>|<span data-ttu-id="2cc06-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2cc06-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="2cc06-178">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="2cc06-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="2cc06-179">例:</span><span class="sxs-lookup"><span data-stu-id="2cc06-179">E.g.</span></span> <span data-ttu-id="2cc06-180">[managedAppRegistration](../resources/intune-mam-managedappregistration.md)から継承のルート デバイス上で実行されているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="2cc06-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="2cc06-181">使用可能な値は、`none`、`rootedDevice` です。</span><span class="sxs-lookup"><span data-stu-id="2cc06-181">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="2cc06-182">userId</span><span class="sxs-lookup"><span data-stu-id="2cc06-182">userId</span></span>|<span data-ttu-id="2cc06-183">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-183">String</span></span>|<span data-ttu-id="2cc06-184">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="2cc06-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="2cc06-185">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cc06-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="2cc06-186">appIdentifier</span></span>|[<span data-ttu-id="2cc06-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="2cc06-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="2cc06-188">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2cc06-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-189">id</span><span class="sxs-lookup"><span data-stu-id="2cc06-189">id</span></span>|<span data-ttu-id="2cc06-190">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-190">String</span></span>|<span data-ttu-id="2cc06-191">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2cc06-191">Key of the entity.</span></span> <span data-ttu-id="2cc06-192">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cc06-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-193">version</span><span class="sxs-lookup"><span data-stu-id="2cc06-193">version</span></span>|<span data-ttu-id="2cc06-194">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-194">String</span></span>|<span data-ttu-id="2cc06-195">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2cc06-195">Version of the entity.</span></span> <span data-ttu-id="2cc06-196">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cc06-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2cc06-197">patchVersion</span><span class="sxs-lookup"><span data-stu-id="2cc06-197">patchVersion</span></span>|<span data-ttu-id="2cc06-198">String</span><span class="sxs-lookup"><span data-stu-id="2cc06-198">String</span></span>|<span data-ttu-id="2cc06-199">現在 android アプリの登録の修正プログラムのバージョン</span><span class="sxs-lookup"><span data-stu-id="2cc06-199">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="2cc06-200">応答</span><span class="sxs-lookup"><span data-stu-id="2cc06-200">Response</span></span>
<span data-ttu-id="2cc06-201">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2cc06-201">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc06-202">例</span><span class="sxs-lookup"><span data-stu-id="2cc06-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cc06-203">要求</span><span class="sxs-lookup"><span data-stu-id="2cc06-203">Request</span></span>
<span data-ttu-id="2cc06-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2cc06-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2cc06-205">応答</span><span class="sxs-lookup"><span data-stu-id="2cc06-205">Response</span></span>
<span data-ttu-id="2cc06-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2cc06-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




