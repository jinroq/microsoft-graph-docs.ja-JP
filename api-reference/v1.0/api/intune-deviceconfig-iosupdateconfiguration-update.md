---
title: iosUpdateConfiguration の更新
description: iosUpdateConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b84ab0957b3a9cc784b8069ce6a86301fbdeb53d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549819"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="a6796-103">iosUpdateConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="a6796-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="a6796-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6796-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6796-105">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6796-105">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6796-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a6796-106">Prerequisites</span></span>
<span data-ttu-id="a6796-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6796-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6796-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6796-109">Permission type</span></span>|<span data-ttu-id="a6796-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6796-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6796-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6796-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6796-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6796-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6796-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6796-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6796-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6796-114">Not supported.</span></span>|
|<span data-ttu-id="a6796-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6796-115">Application</span></span>|<span data-ttu-id="a6796-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6796-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6796-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6796-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6796-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6796-118">Request headers</span></span>
|<span data-ttu-id="a6796-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6796-119">Header</span></span>|<span data-ttu-id="a6796-120">値</span><span class="sxs-lookup"><span data-stu-id="a6796-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6796-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6796-121">Authorization</span></span>|<span data-ttu-id="a6796-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6796-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6796-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a6796-123">Accept</span></span>|<span data-ttu-id="a6796-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a6796-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6796-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6796-125">Request body</span></span>
<span data-ttu-id="a6796-126">要求本文で、[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6796-126">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="a6796-127">次の表に、[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a6796-127">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="a6796-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6796-128">Property</span></span>|<span data-ttu-id="a6796-129">型</span><span class="sxs-lookup"><span data-stu-id="a6796-129">Type</span></span>|<span data-ttu-id="a6796-130">説明</span><span class="sxs-lookup"><span data-stu-id="a6796-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6796-131">id</span><span class="sxs-lookup"><span data-stu-id="a6796-131">id</span></span>|<span data-ttu-id="a6796-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a6796-132">String</span></span>|<span data-ttu-id="a6796-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a6796-133">Key of the entity.</span></span> <span data-ttu-id="a6796-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6796-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6796-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6796-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a6796-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6796-136">DateTimeOffset</span></span>|<span data-ttu-id="a6796-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a6796-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a6796-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6796-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6796-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6796-139">createdDateTime</span></span>|<span data-ttu-id="a6796-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6796-140">DateTimeOffset</span></span>|<span data-ttu-id="a6796-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a6796-141">DateTime the object was created.</span></span> <span data-ttu-id="a6796-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6796-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6796-143">description</span><span class="sxs-lookup"><span data-stu-id="a6796-143">description</span></span>|<span data-ttu-id="a6796-144">String</span><span class="sxs-lookup"><span data-stu-id="a6796-144">String</span></span>|<span data-ttu-id="a6796-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a6796-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6796-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6796-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6796-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a6796-147">displayName</span></span>|<span data-ttu-id="a6796-148">String</span><span class="sxs-lookup"><span data-stu-id="a6796-148">String</span></span>|<span data-ttu-id="a6796-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a6796-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6796-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6796-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6796-151">version</span><span class="sxs-lookup"><span data-stu-id="a6796-151">version</span></span>|<span data-ttu-id="a6796-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a6796-152">Int32</span></span>|<span data-ttu-id="a6796-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a6796-153">Version of the device configuration.</span></span> <span data-ttu-id="a6796-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a6796-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6796-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a6796-155">activeHoursStart</span></span>|<span data-ttu-id="a6796-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a6796-156">TimeOfDay</span></span>|<span data-ttu-id="a6796-157">アクティブ時間の開始 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="a6796-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a6796-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a6796-158">activeHoursEnd</span></span>|<span data-ttu-id="a6796-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a6796-159">TimeOfDay</span></span>|<span data-ttu-id="a6796-160">アクティブ時間の終了 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="a6796-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a6796-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="a6796-161">scheduledInstallDays</span></span>|<span data-ttu-id="a6796-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a6796-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="a6796-163">アクティブ時間が設定されている曜日。</span><span class="sxs-lookup"><span data-stu-id="a6796-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="a6796-164">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a6796-164">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="a6796-165">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="a6796-165">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a6796-166">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="a6796-166">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="a6796-167">Int32</span><span class="sxs-lookup"><span data-stu-id="a6796-167">Int32</span></span>|<span data-ttu-id="a6796-168">UTC タイム オフセット (分単位で示されます)</span><span class="sxs-lookup"><span data-stu-id="a6796-168">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="a6796-169">応答</span><span class="sxs-lookup"><span data-stu-id="a6796-169">Response</span></span>
<span data-ttu-id="a6796-170">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a6796-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6796-171">例</span><span class="sxs-lookup"><span data-stu-id="a6796-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6796-172">要求</span><span class="sxs-lookup"><span data-stu-id="a6796-172">Request</span></span>
<span data-ttu-id="a6796-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6796-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="a6796-174">応答</span><span class="sxs-lookup"><span data-stu-id="a6796-174">Response</span></span>
<span data-ttu-id="a6796-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6796-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



