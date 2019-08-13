---
title: WindowsInformationProtectionWipeAction を更新する
description: Windowsinformationprotectionwipepeaction オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a75930ba8cfe90b102b062427c156757b363179
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353366"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="899e9-103">WindowsInformationProtectionWipeAction を更新する</span><span class="sxs-lookup"><span data-stu-id="899e9-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="899e9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="899e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="899e9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="899e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="899e9-106">[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="899e9-106">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="899e9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="899e9-107">Prerequisites</span></span>
<span data-ttu-id="899e9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="899e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="899e9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="899e9-110">Permission type</span></span>|<span data-ttu-id="899e9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="899e9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="899e9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="899e9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="899e9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="899e9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="899e9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="899e9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="899e9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="899e9-115">Not supported.</span></span>|
|<span data-ttu-id="899e9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="899e9-116">Application</span></span>|<span data-ttu-id="899e9-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="899e9-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="899e9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="899e9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="899e9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="899e9-119">Request headers</span></span>
|<span data-ttu-id="899e9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="899e9-120">Header</span></span>|<span data-ttu-id="899e9-121">値</span><span class="sxs-lookup"><span data-stu-id="899e9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="899e9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="899e9-122">Authorization</span></span>|<span data-ttu-id="899e9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="899e9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="899e9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="899e9-124">Accept</span></span>|<span data-ttu-id="899e9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="899e9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="899e9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="899e9-126">Request body</span></span>
<span data-ttu-id="899e9-127">要求本文で、 [Windowsinformationprotectionwipepepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="899e9-127">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="899e9-128">次の表に、 [Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="899e9-128">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="899e9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="899e9-129">Property</span></span>|<span data-ttu-id="899e9-130">型</span><span class="sxs-lookup"><span data-stu-id="899e9-130">Type</span></span>|<span data-ttu-id="899e9-131">説明</span><span class="sxs-lookup"><span data-stu-id="899e9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="899e9-132">id</span><span class="sxs-lookup"><span data-stu-id="899e9-132">id</span></span>|<span data-ttu-id="899e9-133">String</span><span class="sxs-lookup"><span data-stu-id="899e9-133">String</span></span>|<span data-ttu-id="899e9-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="899e9-134">Key of the entity.</span></span>|
|<span data-ttu-id="899e9-135">status</span><span class="sxs-lookup"><span data-stu-id="899e9-135">status</span></span>|[<span data-ttu-id="899e9-136">actionState</span><span class="sxs-lookup"><span data-stu-id="899e9-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="899e9-137">ワイプアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="899e9-137">Wipe action status.</span></span> <span data-ttu-id="899e9-138">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="899e9-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="899e9-139">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="899e9-139">targetedUserId</span></span>|<span data-ttu-id="899e9-140">String</span><span class="sxs-lookup"><span data-stu-id="899e9-140">String</span></span>|<span data-ttu-id="899e9-141">このワイプアクションの対象となる UserId。</span><span class="sxs-lookup"><span data-stu-id="899e9-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="899e9-142">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="899e9-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="899e9-143">String</span><span class="sxs-lookup"><span data-stu-id="899e9-143">String</span></span>|<span data-ttu-id="899e9-144">このワイプアクションの対象となる DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="899e9-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="899e9-145">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="899e9-145">targetedDeviceName</span></span>|<span data-ttu-id="899e9-146">String</span><span class="sxs-lookup"><span data-stu-id="899e9-146">String</span></span>|<span data-ttu-id="899e9-147">対象のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="899e9-147">Targeted device name.</span></span>|
|<span data-ttu-id="899e9-148">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="899e9-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="899e9-149">String</span><span class="sxs-lookup"><span data-stu-id="899e9-149">String</span></span>|<span data-ttu-id="899e9-150">対象デバイスの Mac アドレス。</span><span class="sxs-lookup"><span data-stu-id="899e9-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="899e9-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="899e9-151">lastCheckInDateTime</span></span>|<span data-ttu-id="899e9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="899e9-152">DateTimeOffset</span></span>|<span data-ttu-id="899e9-153">このワイプアクションの対象となったデバイスの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="899e9-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="899e9-154">応答</span><span class="sxs-lookup"><span data-stu-id="899e9-154">Response</span></span>
<span data-ttu-id="899e9-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="899e9-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="899e9-156">例</span><span class="sxs-lookup"><span data-stu-id="899e9-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="899e9-157">要求</span><span class="sxs-lookup"><span data-stu-id="899e9-157">Request</span></span>
<span data-ttu-id="899e9-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="899e9-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="899e9-159">応答</span><span class="sxs-lookup"><span data-stu-id="899e9-159">Response</span></span>
<span data-ttu-id="899e9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="899e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






