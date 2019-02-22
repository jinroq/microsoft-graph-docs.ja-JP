---
title: windowsinformationprotectionwipeaction を更新する
description: windowsinformationprotectionwipepeaction オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b198f1387cc3f0806cc6b76953948eca08d88cfc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159102"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="3215f-103">windowsinformationprotectionwipeaction を更新する</span><span class="sxs-lookup"><span data-stu-id="3215f-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="3215f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3215f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3215f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3215f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3215f-106">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3215f-106">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3215f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3215f-107">Prerequisites</span></span>
<span data-ttu-id="3215f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3215f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3215f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3215f-110">Permission type</span></span>|<span data-ttu-id="3215f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3215f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3215f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3215f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3215f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3215f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3215f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3215f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3215f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3215f-115">Not supported.</span></span>|
|<span data-ttu-id="3215f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3215f-116">Application</span></span>|<span data-ttu-id="3215f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3215f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3215f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3215f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="3215f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3215f-119">Request headers</span></span>
|<span data-ttu-id="3215f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3215f-120">Header</span></span>|<span data-ttu-id="3215f-121">値</span><span class="sxs-lookup"><span data-stu-id="3215f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3215f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3215f-122">Authorization</span></span>|<span data-ttu-id="3215f-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3215f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3215f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3215f-124">Accept</span></span>|<span data-ttu-id="3215f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3215f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3215f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3215f-126">Request body</span></span>
<span data-ttu-id="3215f-127">要求本文で、 [windowsinformationprotectionwipepepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3215f-127">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="3215f-128">次の表に、 [windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3215f-128">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="3215f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3215f-129">Property</span></span>|<span data-ttu-id="3215f-130">型</span><span class="sxs-lookup"><span data-stu-id="3215f-130">Type</span></span>|<span data-ttu-id="3215f-131">説明</span><span class="sxs-lookup"><span data-stu-id="3215f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3215f-132">id</span><span class="sxs-lookup"><span data-stu-id="3215f-132">id</span></span>|<span data-ttu-id="3215f-133">String</span><span class="sxs-lookup"><span data-stu-id="3215f-133">String</span></span>|<span data-ttu-id="3215f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3215f-134">Key of the entity.</span></span>|
|<span data-ttu-id="3215f-135">status</span><span class="sxs-lookup"><span data-stu-id="3215f-135">status</span></span>|[<span data-ttu-id="3215f-136">actionState</span><span class="sxs-lookup"><span data-stu-id="3215f-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="3215f-137">ワイプアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="3215f-137">Wipe action status.</span></span> <span data-ttu-id="3215f-138">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="3215f-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3215f-139">targeteduserid</span><span class="sxs-lookup"><span data-stu-id="3215f-139">targetedUserId</span></span>|<span data-ttu-id="3215f-140">String</span><span class="sxs-lookup"><span data-stu-id="3215f-140">String</span></span>|<span data-ttu-id="3215f-141">このワイプアクションの対象となる UserId。</span><span class="sxs-lookup"><span data-stu-id="3215f-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="3215f-142">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="3215f-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="3215f-143">String</span><span class="sxs-lookup"><span data-stu-id="3215f-143">String</span></span>|<span data-ttu-id="3215f-144">このワイプアクションの対象となる DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="3215f-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="3215f-145">targeteddevicename</span><span class="sxs-lookup"><span data-stu-id="3215f-145">targetedDeviceName</span></span>|<span data-ttu-id="3215f-146">String</span><span class="sxs-lookup"><span data-stu-id="3215f-146">String</span></span>|<span data-ttu-id="3215f-147">対象のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="3215f-147">Targeted device name.</span></span>|
|<span data-ttu-id="3215f-148">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="3215f-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="3215f-149">String</span><span class="sxs-lookup"><span data-stu-id="3215f-149">String</span></span>|<span data-ttu-id="3215f-150">対象デバイスの Mac アドレス。</span><span class="sxs-lookup"><span data-stu-id="3215f-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="3215f-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="3215f-151">lastCheckInDateTime</span></span>|<span data-ttu-id="3215f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3215f-152">DateTimeOffset</span></span>|<span data-ttu-id="3215f-153">このワイプアクションの対象となったデバイスの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="3215f-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="3215f-154">応答</span><span class="sxs-lookup"><span data-stu-id="3215f-154">Response</span></span>
<span data-ttu-id="3215f-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3215f-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3215f-156">例</span><span class="sxs-lookup"><span data-stu-id="3215f-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="3215f-157">要求</span><span class="sxs-lookup"><span data-stu-id="3215f-157">Request</span></span>
<span data-ttu-id="3215f-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3215f-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
Content-type: application/json
Content-length: 412

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3215f-159">応答</span><span class="sxs-lookup"><span data-stu-id="3215f-159">Response</span></span>
<span data-ttu-id="3215f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3215f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 461

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "2620a996-a996-2620-96a9-202696a92026",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```




