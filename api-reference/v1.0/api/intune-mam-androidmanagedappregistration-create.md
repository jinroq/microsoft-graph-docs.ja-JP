---
title: androidManagedAppRegistration の作成
description: 新しい androidManagedAppRegistration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4485ab59a2a1bc4658a12e9bff4fae57fae2c898
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931994"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="b2eb4-103">androidManagedAppRegistration の作成</span><span class="sxs-lookup"><span data-stu-id="b2eb4-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="b2eb4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2eb4-105">新しい [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2eb4-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b2eb4-106">Prerequisites</span></span>
<span data-ttu-id="b2eb4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2eb4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2eb4-109">Permission type</span></span>|<span data-ttu-id="b2eb4-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2eb4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2eb4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2eb4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2eb4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2eb4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2eb4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2eb4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2eb4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-114">Not supported.</span></span>|
|<span data-ttu-id="b2eb4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2eb4-115">Application</span></span>|<span data-ttu-id="b2eb4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2eb4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2eb4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="b2eb4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2eb4-118">Request headers</span></span>
|<span data-ttu-id="b2eb4-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2eb4-119">Header</span></span>|<span data-ttu-id="b2eb4-120">値</span><span class="sxs-lookup"><span data-stu-id="b2eb4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2eb4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2eb4-121">Authorization</span></span>|<span data-ttu-id="b2eb4-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2eb4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b2eb4-123">Accept</span></span>|<span data-ttu-id="b2eb4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b2eb4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2eb4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2eb4-125">Request body</span></span>
<span data-ttu-id="b2eb4-126">要求本文で、androidManagedAppRegistration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="b2eb4-127">次の表に、androidManagedAppRegistration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="b2eb4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2eb4-128">Property</span></span>|<span data-ttu-id="b2eb4-129">種類</span><span class="sxs-lookup"><span data-stu-id="b2eb4-129">Type</span></span>|<span data-ttu-id="b2eb4-130">説明</span><span class="sxs-lookup"><span data-stu-id="b2eb4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2eb4-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2eb4-131">createdDateTime</span></span>|<span data-ttu-id="b2eb4-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2eb4-132">DateTimeOffset</span></span>|<span data-ttu-id="b2eb4-133">作成日時 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b2eb4-134">lastSyncDateTime</span></span>|<span data-ttu-id="b2eb4-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2eb4-135">DateTimeOffset</span></span>|<span data-ttu-id="b2eb4-136">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="b2eb4-137">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2eb4-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="b2eb4-138">applicationVersion</span></span>|<span data-ttu-id="b2eb4-139">String</span><span class="sxs-lookup"><span data-stu-id="b2eb4-139">String</span></span>|<span data-ttu-id="b2eb4-140">アプリのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b2eb4-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="b2eb4-141">managementSdkVersion</span></span>|<span data-ttu-id="b2eb4-142">String</span><span class="sxs-lookup"><span data-stu-id="b2eb4-142">String</span></span>|<span data-ttu-id="b2eb4-143">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b2eb4-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="b2eb4-144">platformVersion</span></span>|<span data-ttu-id="b2eb4-145">String</span><span class="sxs-lookup"><span data-stu-id="b2eb4-145">String</span></span>|<span data-ttu-id="b2eb4-146">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b2eb4-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="b2eb4-147">deviceType</span></span>|<span data-ttu-id="b2eb4-148">String</span><span class="sxs-lookup"><span data-stu-id="b2eb4-148">String</span></span>|<span data-ttu-id="b2eb4-149">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b2eb4-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="b2eb4-150">deviceTag</span></span>|<span data-ttu-id="b2eb4-151">String</span><span class="sxs-lookup"><span data-stu-id="b2eb4-151">String</span></span>|<span data-ttu-id="b2eb4-152">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="b2eb4-153">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="b2eb4-154">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2eb4-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="b2eb4-155">deviceName</span></span>|<span data-ttu-id="b2eb4-156">String</span><span class="sxs-lookup"><span data-stu-id="b2eb4-156">String</span></span>|<span data-ttu-id="b2eb4-157">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b2eb4-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="b2eb4-158">flaggedReasons</span></span>|<span data-ttu-id="b2eb4-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b2eb4-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="b2eb4-160">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="b2eb4-161">例:</span><span class="sxs-lookup"><span data-stu-id="b2eb4-161">E.g.</span></span> <span data-ttu-id="b2eb4-162">[managedAppRegistration](../resources/intune-mam-managedappregistration.md)から継承のルート デバイス上で実行されているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="b2eb4-163">使用可能な値は、`none`、`rootedDevice` です。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="b2eb4-164">userId</span><span class="sxs-lookup"><span data-stu-id="b2eb4-164">userId</span></span>|<span data-ttu-id="b2eb4-165">String</span><span class="sxs-lookup"><span data-stu-id="b2eb4-165">String</span></span>|<span data-ttu-id="b2eb4-166">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="b2eb4-167">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2eb4-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="b2eb4-168">appIdentifier</span></span>|[<span data-ttu-id="b2eb4-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b2eb4-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b2eb4-170">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b2eb4-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-171">id</span><span class="sxs-lookup"><span data-stu-id="b2eb4-171">id</span></span>|<span data-ttu-id="b2eb4-172">String</span><span class="sxs-lookup"><span data-stu-id="b2eb4-172">String</span></span>|<span data-ttu-id="b2eb4-173">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-173">Key of the entity.</span></span> <span data-ttu-id="b2eb4-174">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2eb4-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b2eb4-175">version</span><span class="sxs-lookup"><span data-stu-id="b2eb4-175">version</span></span>|<span data-ttu-id="b2eb4-176">String</span><span class="sxs-lookup"><span data-stu-id="b2eb4-176">String</span></span>|<span data-ttu-id="b2eb4-177">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-177">Version of the entity.</span></span> <span data-ttu-id="b2eb4-178">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2eb4-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b2eb4-179">応答</span><span class="sxs-lookup"><span data-stu-id="b2eb4-179">Response</span></span>
<span data-ttu-id="b2eb4-180">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2eb4-181">例</span><span class="sxs-lookup"><span data-stu-id="b2eb4-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2eb4-182">要求</span><span class="sxs-lookup"><span data-stu-id="b2eb4-182">Request</span></span>
<span data-ttu-id="b2eb4-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="b2eb4-184">応答</span><span class="sxs-lookup"><span data-stu-id="b2eb4-184">Response</span></span>
<span data-ttu-id="b2eb4-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b2eb4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

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
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```



