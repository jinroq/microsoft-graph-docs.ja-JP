---
title: iosUpdateConfiguration の作成
description: 新しい iosUpdateConfiguration オブジェクトを作成します。
ms.openlocfilehash: 65acd8334cc53e637563cae45d4a6d5721405843
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023365"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="56e00-103">iosUpdateConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="56e00-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="56e00-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="56e00-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56e00-105">新しい [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="56e00-105">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56e00-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="56e00-106">Prerequisites</span></span>
<span data-ttu-id="56e00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56e00-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56e00-109">Permission type</span></span>|<span data-ttu-id="56e00-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="56e00-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56e00-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56e00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56e00-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56e00-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56e00-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56e00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56e00-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56e00-114">Not supported.</span></span>|
|<span data-ttu-id="56e00-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56e00-115">Application</span></span>|<span data-ttu-id="56e00-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56e00-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56e00-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56e00-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="56e00-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56e00-118">Request headers</span></span>
|<span data-ttu-id="56e00-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56e00-119">Header</span></span>|<span data-ttu-id="56e00-120">値</span><span class="sxs-lookup"><span data-stu-id="56e00-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56e00-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56e00-121">Authorization</span></span>|<span data-ttu-id="56e00-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="56e00-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56e00-123">Accept</span><span class="sxs-lookup"><span data-stu-id="56e00-123">Accept</span></span>|<span data-ttu-id="56e00-124">application/json</span><span class="sxs-lookup"><span data-stu-id="56e00-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56e00-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="56e00-125">Request body</span></span>
<span data-ttu-id="56e00-126">要求本文で、iosUpdateConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56e00-126">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="56e00-127">次の表に、iosUpdateConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="56e00-127">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="56e00-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56e00-128">Property</span></span>|<span data-ttu-id="56e00-129">型</span><span class="sxs-lookup"><span data-stu-id="56e00-129">Type</span></span>|<span data-ttu-id="56e00-130">説明</span><span class="sxs-lookup"><span data-stu-id="56e00-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56e00-131">id</span><span class="sxs-lookup"><span data-stu-id="56e00-131">id</span></span>|<span data-ttu-id="56e00-132">String</span><span class="sxs-lookup"><span data-stu-id="56e00-132">String</span></span>|<span data-ttu-id="56e00-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="56e00-133">Key of the entity.</span></span> <span data-ttu-id="56e00-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56e00-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56e00-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56e00-135">lastModifiedDateTime</span></span>|<span data-ttu-id="56e00-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56e00-136">DateTimeOffset</span></span>|<span data-ttu-id="56e00-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="56e00-137">DateTime the object was last modified.</span></span> <span data-ttu-id="56e00-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56e00-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56e00-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56e00-139">createdDateTime</span></span>|<span data-ttu-id="56e00-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56e00-140">DateTimeOffset</span></span>|<span data-ttu-id="56e00-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="56e00-141">DateTime the object was created.</span></span> <span data-ttu-id="56e00-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56e00-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56e00-143">説明</span><span class="sxs-lookup"><span data-stu-id="56e00-143">description</span></span>|<span data-ttu-id="56e00-144">String</span><span class="sxs-lookup"><span data-stu-id="56e00-144">String</span></span>|<span data-ttu-id="56e00-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="56e00-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="56e00-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56e00-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56e00-147">displayName</span><span class="sxs-lookup"><span data-stu-id="56e00-147">displayName</span></span>|<span data-ttu-id="56e00-148">String</span><span class="sxs-lookup"><span data-stu-id="56e00-148">String</span></span>|<span data-ttu-id="56e00-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="56e00-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="56e00-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56e00-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56e00-151">version</span><span class="sxs-lookup"><span data-stu-id="56e00-151">version</span></span>|<span data-ttu-id="56e00-152">Int32</span><span class="sxs-lookup"><span data-stu-id="56e00-152">Int32</span></span>|<span data-ttu-id="56e00-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="56e00-153">Version of the device configuration.</span></span> <span data-ttu-id="56e00-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="56e00-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56e00-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="56e00-155">activeHoursStart</span></span>|<span data-ttu-id="56e00-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="56e00-156">TimeOfDay</span></span>|<span data-ttu-id="56e00-157">アクティブ時間の開始 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="56e00-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="56e00-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="56e00-158">activeHoursEnd</span></span>|<span data-ttu-id="56e00-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="56e00-159">TimeOfDay</span></span>|<span data-ttu-id="56e00-160">アクティブ時間の終了 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="56e00-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="56e00-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="56e00-161">scheduledInstallDays</span></span>|<span data-ttu-id="56e00-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="56e00-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="56e00-163">アクティブ時間が設定されている曜日。</span><span class="sxs-lookup"><span data-stu-id="56e00-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="56e00-164">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="56e00-164">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="56e00-165">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="56e00-165">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="56e00-166">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="56e00-166">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="56e00-167">Int32</span><span class="sxs-lookup"><span data-stu-id="56e00-167">Int32</span></span>|<span data-ttu-id="56e00-168">UTC タイム オフセット (分単位で示されます)</span><span class="sxs-lookup"><span data-stu-id="56e00-168">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="56e00-169">応答</span><span class="sxs-lookup"><span data-stu-id="56e00-169">Response</span></span>
<span data-ttu-id="56e00-170">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56e00-170">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56e00-171">例</span><span class="sxs-lookup"><span data-stu-id="56e00-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="56e00-172">要求</span><span class="sxs-lookup"><span data-stu-id="56e00-172">Request</span></span>
<span data-ttu-id="56e00-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56e00-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="56e00-174">応答</span><span class="sxs-lookup"><span data-stu-id="56e00-174">Response</span></span>
<span data-ttu-id="56e00-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56e00-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```



