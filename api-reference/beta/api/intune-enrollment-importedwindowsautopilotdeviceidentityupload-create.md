---
title: ImportedWindowsAutopilotDeviceIdentityUpload を作成する
description: 新しい importedWindowsAutopilotDeviceIdentityUpload オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19f1cfce3f44c49a2da5e31fa791574be1d5eb69
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908407"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="22e44-103">ImportedWindowsAutopilotDeviceIdentityUpload を作成する</span><span class="sxs-lookup"><span data-stu-id="22e44-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="22e44-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22e44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22e44-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22e44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22e44-106">新しい[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="22e44-106">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22e44-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="22e44-107">Prerequisites</span></span>
<span data-ttu-id="22e44-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22e44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22e44-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22e44-110">Permission type</span></span>|<span data-ttu-id="22e44-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22e44-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22e44-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22e44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22e44-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22e44-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="22e44-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22e44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22e44-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22e44-115">Not supported.</span></span>|
|<span data-ttu-id="22e44-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22e44-116">Application</span></span>|<span data-ttu-id="22e44-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22e44-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22e44-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22e44-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="22e44-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22e44-119">Request headers</span></span>
|<span data-ttu-id="22e44-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22e44-120">Header</span></span>|<span data-ttu-id="22e44-121">値</span><span class="sxs-lookup"><span data-stu-id="22e44-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22e44-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22e44-122">Authorization</span></span>|<span data-ttu-id="22e44-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="22e44-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22e44-124">承諾</span><span class="sxs-lookup"><span data-stu-id="22e44-124">Accept</span></span>|<span data-ttu-id="22e44-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22e44-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22e44-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="22e44-126">Request body</span></span>
<span data-ttu-id="22e44-127">要求本文で、importedWindowsAutopilotDeviceIdentityUpload オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22e44-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="22e44-128">次の表に、importedWindowsAutopilotDeviceIdentityUpload の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="22e44-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="22e44-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22e44-129">Property</span></span>|<span data-ttu-id="22e44-130">型</span><span class="sxs-lookup"><span data-stu-id="22e44-130">Type</span></span>|<span data-ttu-id="22e44-131">説明</span><span class="sxs-lookup"><span data-stu-id="22e44-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22e44-132">id</span><span class="sxs-lookup"><span data-stu-id="22e44-132">id</span></span>|<span data-ttu-id="22e44-133">String</span><span class="sxs-lookup"><span data-stu-id="22e44-133">String</span></span>|<span data-ttu-id="22e44-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="22e44-134">The GUID for the object</span></span>|
|<span data-ttu-id="22e44-135">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="22e44-135">createdDateTimeUtc</span></span>|<span data-ttu-id="22e44-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22e44-136">DateTimeOffset</span></span>|<span data-ttu-id="22e44-137">エンティティが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="22e44-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="22e44-138">status</span><span class="sxs-lookup"><span data-stu-id="22e44-138">status</span></span>|[<span data-ttu-id="22e44-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="22e44-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="22e44-140">アップロードの状態。</span><span class="sxs-lookup"><span data-stu-id="22e44-140">Upload status.</span></span> <span data-ttu-id="22e44-141">可能な値は、`noUpload`、`pending`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="22e44-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="22e44-142">応答</span><span class="sxs-lookup"><span data-stu-id="22e44-142">Response</span></span>
<span data-ttu-id="22e44-143">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="22e44-143">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22e44-144">例</span><span class="sxs-lookup"><span data-stu-id="22e44-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="22e44-145">要求</span><span class="sxs-lookup"><span data-stu-id="22e44-145">Request</span></span>
<span data-ttu-id="22e44-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22e44-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="22e44-147">応答</span><span class="sxs-lookup"><span data-stu-id="22e44-147">Response</span></span>
<span data-ttu-id="22e44-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22e44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```




