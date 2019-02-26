---
title: importedWindowsAutopilotDeviceIdentityUpload を作成する
description: 新しい importedWindowsAutopilotDeviceIdentityUpload オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fd4230b0ecdb4279380255b1fa62cbe697a4843
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264394"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="53a0c-103">importedWindowsAutopilotDeviceIdentityUpload を作成する</span><span class="sxs-lookup"><span data-stu-id="53a0c-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="53a0c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53a0c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53a0c-105">新しい[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="53a0c-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53a0c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="53a0c-106">Prerequisites</span></span>
<span data-ttu-id="53a0c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53a0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53a0c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53a0c-109">Permission type</span></span>|<span data-ttu-id="53a0c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="53a0c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53a0c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53a0c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53a0c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53a0c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53a0c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53a0c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53a0c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53a0c-114">Not supported.</span></span>|
|<span data-ttu-id="53a0c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53a0c-115">Application</span></span>|<span data-ttu-id="53a0c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53a0c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53a0c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53a0c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="53a0c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53a0c-118">Request headers</span></span>
|<span data-ttu-id="53a0c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53a0c-119">Header</span></span>|<span data-ttu-id="53a0c-120">値</span><span class="sxs-lookup"><span data-stu-id="53a0c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53a0c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53a0c-121">Authorization</span></span>|<span data-ttu-id="53a0c-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="53a0c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53a0c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="53a0c-123">Accept</span></span>|<span data-ttu-id="53a0c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53a0c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53a0c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="53a0c-125">Request body</span></span>
<span data-ttu-id="53a0c-126">要求本文で、importedWindowsAutopilotDeviceIdentityUpload オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="53a0c-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="53a0c-127">次の表に、importedWindowsAutopilotDeviceIdentityUpload の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="53a0c-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="53a0c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53a0c-128">Property</span></span>|<span data-ttu-id="53a0c-129">型</span><span class="sxs-lookup"><span data-stu-id="53a0c-129">Type</span></span>|<span data-ttu-id="53a0c-130">説明</span><span class="sxs-lookup"><span data-stu-id="53a0c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53a0c-131">id</span><span class="sxs-lookup"><span data-stu-id="53a0c-131">id</span></span>|<span data-ttu-id="53a0c-132">String</span><span class="sxs-lookup"><span data-stu-id="53a0c-132">String</span></span>|<span data-ttu-id="53a0c-133">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="53a0c-133">The GUID for the object</span></span>|
|<span data-ttu-id="53a0c-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="53a0c-134">createdDateTimeUtc</span></span>|<span data-ttu-id="53a0c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a0c-135">DateTimeOffset</span></span>|<span data-ttu-id="53a0c-136">エンティティが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="53a0c-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="53a0c-137">status</span><span class="sxs-lookup"><span data-stu-id="53a0c-137">status</span></span>|[<span data-ttu-id="53a0c-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="53a0c-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="53a0c-139">アップロードの状態。</span><span class="sxs-lookup"><span data-stu-id="53a0c-139">Upload status.</span></span> <span data-ttu-id="53a0c-140">可能な値は、`noUpload`、`pending`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="53a0c-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="53a0c-141">応答</span><span class="sxs-lookup"><span data-stu-id="53a0c-141">Response</span></span>
<span data-ttu-id="53a0c-142">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53a0c-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53a0c-143">例</span><span class="sxs-lookup"><span data-stu-id="53a0c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="53a0c-144">要求</span><span class="sxs-lookup"><span data-stu-id="53a0c-144">Request</span></span>
<span data-ttu-id="53a0c-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53a0c-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="53a0c-146">応答</span><span class="sxs-lookup"><span data-stu-id="53a0c-146">Response</span></span>
<span data-ttu-id="53a0c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53a0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



