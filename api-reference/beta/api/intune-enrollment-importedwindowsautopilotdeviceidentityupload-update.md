---
title: importedWindowsAutopilotDeviceIdentityUpload の更新
description: importedWindowsAutopilotDeviceIdentityUpload オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e75ec2ea82aa28cfab5a1d29b9ead6e8a409c64c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532430"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="883cd-103">importedWindowsAutopilotDeviceIdentityUpload の更新</span><span class="sxs-lookup"><span data-stu-id="883cd-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="883cd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="883cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="883cd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="883cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="883cd-106">[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="883cd-106">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="883cd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="883cd-107">Prerequisites</span></span>
<span data-ttu-id="883cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="883cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="883cd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="883cd-110">Permission type</span></span>|<span data-ttu-id="883cd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="883cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="883cd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="883cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="883cd-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="883cd-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="883cd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="883cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="883cd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="883cd-115">Not supported.</span></span>|
|<span data-ttu-id="883cd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="883cd-116">Application</span></span>|<span data-ttu-id="883cd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="883cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="883cd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="883cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="883cd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="883cd-119">Request headers</span></span>
|<span data-ttu-id="883cd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="883cd-120">Header</span></span>|<span data-ttu-id="883cd-121">値</span><span class="sxs-lookup"><span data-stu-id="883cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="883cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="883cd-122">Authorization</span></span>|<span data-ttu-id="883cd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="883cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="883cd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="883cd-124">Accept</span></span>|<span data-ttu-id="883cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="883cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="883cd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="883cd-126">Request body</span></span>
<span data-ttu-id="883cd-127">要求本文で、 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="883cd-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="883cd-128">次の表に、 [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="883cd-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="883cd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="883cd-129">Property</span></span>|<span data-ttu-id="883cd-130">型</span><span class="sxs-lookup"><span data-stu-id="883cd-130">Type</span></span>|<span data-ttu-id="883cd-131">説明</span><span class="sxs-lookup"><span data-stu-id="883cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="883cd-132">id</span><span class="sxs-lookup"><span data-stu-id="883cd-132">id</span></span>|<span data-ttu-id="883cd-133">String</span><span class="sxs-lookup"><span data-stu-id="883cd-133">String</span></span>|<span data-ttu-id="883cd-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="883cd-134">The GUID for the object</span></span>|
|<span data-ttu-id="883cd-135">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="883cd-135">createdDateTimeUtc</span></span>|<span data-ttu-id="883cd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="883cd-136">DateTimeOffset</span></span>|<span data-ttu-id="883cd-137">エンティティが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="883cd-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="883cd-138">status</span><span class="sxs-lookup"><span data-stu-id="883cd-138">status</span></span>|[<span data-ttu-id="883cd-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="883cd-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="883cd-140">アップロードの状態。</span><span class="sxs-lookup"><span data-stu-id="883cd-140">Upload status.</span></span> <span data-ttu-id="883cd-141">可能な値は、`noUpload`、`pending`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="883cd-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="883cd-142">応答</span><span class="sxs-lookup"><span data-stu-id="883cd-142">Response</span></span>
<span data-ttu-id="883cd-143">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="883cd-143">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="883cd-144">例</span><span class="sxs-lookup"><span data-stu-id="883cd-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="883cd-145">要求</span><span class="sxs-lookup"><span data-stu-id="883cd-145">Request</span></span>
<span data-ttu-id="883cd-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="883cd-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="883cd-147">応答</span><span class="sxs-lookup"><span data-stu-id="883cd-147">Response</span></span>
<span data-ttu-id="883cd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="883cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```





