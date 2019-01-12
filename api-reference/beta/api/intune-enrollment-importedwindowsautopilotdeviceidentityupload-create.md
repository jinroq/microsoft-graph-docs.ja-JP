---
title: ImportedWindowsAutopilotDeviceIdentityUpload を作成します。
description: 新しい importedWindowsAutopilotDeviceIdentityUpload オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 414191348a6654e59a81c8e46c48bb3e7728a303
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913891"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="8897e-103">ImportedWindowsAutopilotDeviceIdentityUpload を作成します。</span><span class="sxs-lookup"><span data-stu-id="8897e-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="8897e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8897e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8897e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8897e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8897e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8897e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8897e-107">新しい[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8897e-107">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8897e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8897e-108">Prerequisites</span></span>
<span data-ttu-id="8897e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8897e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8897e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8897e-111">Permission type</span></span>|<span data-ttu-id="8897e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8897e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8897e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8897e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8897e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8897e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8897e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8897e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8897e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8897e-116">Not supported.</span></span>|
|<span data-ttu-id="8897e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8897e-117">Application</span></span>|<span data-ttu-id="8897e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8897e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8897e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8897e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="8897e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8897e-120">Request headers</span></span>
|<span data-ttu-id="8897e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8897e-121">Header</span></span>|<span data-ttu-id="8897e-122">値</span><span class="sxs-lookup"><span data-stu-id="8897e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8897e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8897e-123">Authorization</span></span>|<span data-ttu-id="8897e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8897e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8897e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8897e-125">Accept</span></span>|<span data-ttu-id="8897e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8897e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8897e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8897e-127">Request body</span></span>
<span data-ttu-id="8897e-128">要求の本文に importedWindowsAutopilotDeviceIdentityUpload オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8897e-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="8897e-129">次の表は、importedWindowsAutopilotDeviceIdentityUpload を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8897e-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="8897e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8897e-130">Property</span></span>|<span data-ttu-id="8897e-131">型</span><span class="sxs-lookup"><span data-stu-id="8897e-131">Type</span></span>|<span data-ttu-id="8897e-132">説明</span><span class="sxs-lookup"><span data-stu-id="8897e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8897e-133">ID</span><span class="sxs-lookup"><span data-stu-id="8897e-133">id</span></span>|<span data-ttu-id="8897e-134">String</span><span class="sxs-lookup"><span data-stu-id="8897e-134">String</span></span>|<span data-ttu-id="8897e-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="8897e-135">The GUID for the object</span></span>|
|<span data-ttu-id="8897e-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="8897e-136">createdDateTimeUtc</span></span>|<span data-ttu-id="8897e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8897e-137">DateTimeOffset</span></span>|<span data-ttu-id="8897e-138">日時を設定すると、エンティティを作成します。</span><span class="sxs-lookup"><span data-stu-id="8897e-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="8897e-139">status</span><span class="sxs-lookup"><span data-stu-id="8897e-139">status</span></span>|[<span data-ttu-id="8897e-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="8897e-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="8897e-141">ステータスをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="8897e-141">Upload status.</span></span> <span data-ttu-id="8897e-142">可能な値は、`noUpload`、`pending`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="8897e-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="8897e-143">応答</span><span class="sxs-lookup"><span data-stu-id="8897e-143">Response</span></span>
<span data-ttu-id="8897e-144">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8897e-144">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8897e-145">例</span><span class="sxs-lookup"><span data-stu-id="8897e-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="8897e-146">要求</span><span class="sxs-lookup"><span data-stu-id="8897e-146">Request</span></span>
<span data-ttu-id="8897e-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8897e-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8897e-148">応答</span><span class="sxs-lookup"><span data-stu-id="8897e-148">Response</span></span>
<span data-ttu-id="8897e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8897e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





