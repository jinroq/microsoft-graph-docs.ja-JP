---
title: WindowsInformationProtectionWipeAction を作成する
description: 新しい windowsInformationProtectionWipeAction オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2468da2e3f27bc4538dd9137ec3041a6c0962c99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994300"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="ffdba-103">WindowsInformationProtectionWipeAction を作成する</span><span class="sxs-lookup"><span data-stu-id="ffdba-103">Create windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="ffdba-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffdba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffdba-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffdba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffdba-106">新しい[Windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ffdba-106">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffdba-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ffdba-107">Prerequisites</span></span>
<span data-ttu-id="ffdba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffdba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffdba-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ffdba-110">Permission type</span></span>|<span data-ttu-id="ffdba-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ffdba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffdba-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ffdba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffdba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffdba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ffdba-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ffdba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffdba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffdba-115">Not supported.</span></span>|
|<span data-ttu-id="ffdba-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ffdba-116">Application</span></span>|<span data-ttu-id="ffdba-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffdba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffdba-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffdba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="ffdba-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffdba-119">Request headers</span></span>
|<span data-ttu-id="ffdba-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffdba-120">Header</span></span>|<span data-ttu-id="ffdba-121">値</span><span class="sxs-lookup"><span data-stu-id="ffdba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffdba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffdba-122">Authorization</span></span>|<span data-ttu-id="ffdba-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffdba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffdba-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ffdba-124">Accept</span></span>|<span data-ttu-id="ffdba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffdba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffdba-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ffdba-126">Request body</span></span>
<span data-ttu-id="ffdba-127">要求本文で、Windowsinformationprotectionwipepepeaction オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ffdba-127">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="ffdba-128">次の表に、Windowsinformationprotectionwipepeaction の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ffdba-128">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="ffdba-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffdba-129">Property</span></span>|<span data-ttu-id="ffdba-130">型</span><span class="sxs-lookup"><span data-stu-id="ffdba-130">Type</span></span>|<span data-ttu-id="ffdba-131">説明</span><span class="sxs-lookup"><span data-stu-id="ffdba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffdba-132">id</span><span class="sxs-lookup"><span data-stu-id="ffdba-132">id</span></span>|<span data-ttu-id="ffdba-133">String</span><span class="sxs-lookup"><span data-stu-id="ffdba-133">String</span></span>|<span data-ttu-id="ffdba-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ffdba-134">Key of the entity.</span></span>|
|<span data-ttu-id="ffdba-135">status</span><span class="sxs-lookup"><span data-stu-id="ffdba-135">status</span></span>|[<span data-ttu-id="ffdba-136">actionState</span><span class="sxs-lookup"><span data-stu-id="ffdba-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ffdba-137">ワイプアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="ffdba-137">Wipe action status.</span></span> <span data-ttu-id="ffdba-138">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="ffdba-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ffdba-139">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="ffdba-139">targetedUserId</span></span>|<span data-ttu-id="ffdba-140">String</span><span class="sxs-lookup"><span data-stu-id="ffdba-140">String</span></span>|<span data-ttu-id="ffdba-141">このワイプアクションの対象となる UserId。</span><span class="sxs-lookup"><span data-stu-id="ffdba-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="ffdba-142">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="ffdba-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="ffdba-143">String</span><span class="sxs-lookup"><span data-stu-id="ffdba-143">String</span></span>|<span data-ttu-id="ffdba-144">このワイプアクションの対象となる DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="ffdba-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="ffdba-145">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ffdba-145">targetedDeviceName</span></span>|<span data-ttu-id="ffdba-146">String</span><span class="sxs-lookup"><span data-stu-id="ffdba-146">String</span></span>|<span data-ttu-id="ffdba-147">対象のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="ffdba-147">Targeted device name.</span></span>|
|<span data-ttu-id="ffdba-148">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="ffdba-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="ffdba-149">String</span><span class="sxs-lookup"><span data-stu-id="ffdba-149">String</span></span>|<span data-ttu-id="ffdba-150">対象デバイスの Mac アドレス。</span><span class="sxs-lookup"><span data-stu-id="ffdba-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="ffdba-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="ffdba-151">lastCheckInDateTime</span></span>|<span data-ttu-id="ffdba-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffdba-152">DateTimeOffset</span></span>|<span data-ttu-id="ffdba-153">このワイプアクションの対象となったデバイスの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="ffdba-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="ffdba-154">応答</span><span class="sxs-lookup"><span data-stu-id="ffdba-154">Response</span></span>
<span data-ttu-id="ffdba-155">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ffdba-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffdba-156">例</span><span class="sxs-lookup"><span data-stu-id="ffdba-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffdba-157">要求</span><span class="sxs-lookup"><span data-stu-id="ffdba-157">Request</span></span>
<span data-ttu-id="ffdba-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ffdba-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
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

### <a name="response"></a><span data-ttu-id="ffdba-159">応答</span><span class="sxs-lookup"><span data-stu-id="ffdba-159">Response</span></span>
<span data-ttu-id="ffdba-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ffdba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





