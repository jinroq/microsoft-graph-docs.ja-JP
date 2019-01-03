---
title: ImportedWindowsAutopilotDeviceIdentityUpload を更新します。
description: ImportedWindowsAutopilotDeviceIdentityUpload オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 4fb2274fdb172b6aeceba11364a6460cbe5cce58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324417"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="969b6-103">ImportedWindowsAutopilotDeviceIdentityUpload を更新します。</span><span class="sxs-lookup"><span data-stu-id="969b6-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="969b6-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="969b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="969b6-105">[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="969b6-105">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="969b6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="969b6-106">Prerequisites</span></span>
<span data-ttu-id="969b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="969b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="969b6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="969b6-109">Permission type</span></span>|<span data-ttu-id="969b6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="969b6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="969b6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="969b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="969b6-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="969b6-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="969b6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="969b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="969b6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="969b6-114">Not supported.</span></span>|
|<span data-ttu-id="969b6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="969b6-115">Application</span></span>|<span data-ttu-id="969b6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="969b6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="969b6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="969b6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="969b6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="969b6-118">Request headers</span></span>
|<span data-ttu-id="969b6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="969b6-119">Header</span></span>|<span data-ttu-id="969b6-120">値</span><span class="sxs-lookup"><span data-stu-id="969b6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="969b6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="969b6-121">Authorization</span></span>|<span data-ttu-id="969b6-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="969b6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="969b6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="969b6-123">Accept</span></span>|<span data-ttu-id="969b6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="969b6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="969b6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="969b6-125">Request body</span></span>
<span data-ttu-id="969b6-126">要求の本文に[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="969b6-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="969b6-127">[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="969b6-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="969b6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="969b6-128">Property</span></span>|<span data-ttu-id="969b6-129">種類</span><span class="sxs-lookup"><span data-stu-id="969b6-129">Type</span></span>|<span data-ttu-id="969b6-130">説明</span><span class="sxs-lookup"><span data-stu-id="969b6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="969b6-131">ID</span><span class="sxs-lookup"><span data-stu-id="969b6-131">id</span></span>|<span data-ttu-id="969b6-132">String</span><span class="sxs-lookup"><span data-stu-id="969b6-132">String</span></span>|<span data-ttu-id="969b6-133">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="969b6-133">The GUID for the object</span></span>|
|<span data-ttu-id="969b6-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="969b6-134">createdDateTimeUtc</span></span>|<span data-ttu-id="969b6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="969b6-135">DateTimeOffset</span></span>|<span data-ttu-id="969b6-136">日時を設定すると、エンティティを作成します。</span><span class="sxs-lookup"><span data-stu-id="969b6-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="969b6-137">status</span><span class="sxs-lookup"><span data-stu-id="969b6-137">status</span></span>|[<span data-ttu-id="969b6-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="969b6-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="969b6-139">ステータスをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="969b6-139">Upload status.</span></span> <span data-ttu-id="969b6-140">可能な値は、`noUpload`、`pending`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="969b6-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="969b6-141">応答</span><span class="sxs-lookup"><span data-stu-id="969b6-141">Response</span></span>
<span data-ttu-id="969b6-142">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="969b6-142">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969b6-143">例</span><span class="sxs-lookup"><span data-stu-id="969b6-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="969b6-144">要求</span><span class="sxs-lookup"><span data-stu-id="969b6-144">Request</span></span>
<span data-ttu-id="969b6-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="969b6-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="969b6-146">応答</span><span class="sxs-lookup"><span data-stu-id="969b6-146">Response</span></span>
<span data-ttu-id="969b6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="969b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


