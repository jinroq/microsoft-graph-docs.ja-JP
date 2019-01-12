---
title: mobileAppContentFile の作成
description: 新しい mobileAppContentFile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9061a3b44d80d7182af321502afa84a3a8cb68fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972636"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="89d11-103">mobileAppContentFile の作成</span><span class="sxs-lookup"><span data-stu-id="89d11-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="89d11-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="89d11-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89d11-105">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="89d11-105">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89d11-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="89d11-106">Prerequisites</span></span>
<span data-ttu-id="89d11-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89d11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89d11-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89d11-109">Permission type</span></span>|<span data-ttu-id="89d11-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="89d11-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89d11-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89d11-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89d11-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89d11-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89d11-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89d11-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89d11-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89d11-114">Not supported.</span></span>|
|<span data-ttu-id="89d11-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89d11-115">Application</span></span>|<span data-ttu-id="89d11-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89d11-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89d11-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89d11-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="89d11-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89d11-118">Request headers</span></span>
|<span data-ttu-id="89d11-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89d11-119">Header</span></span>|<span data-ttu-id="89d11-120">値</span><span class="sxs-lookup"><span data-stu-id="89d11-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89d11-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="89d11-121">Authorization</span></span>|<span data-ttu-id="89d11-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="89d11-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89d11-123">Accept</span><span class="sxs-lookup"><span data-stu-id="89d11-123">Accept</span></span>|<span data-ttu-id="89d11-124">application/json</span><span class="sxs-lookup"><span data-stu-id="89d11-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89d11-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="89d11-125">Request body</span></span>
<span data-ttu-id="89d11-126">要求本文で、mobileAppContentFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="89d11-126">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="89d11-127">次の表に、mobileAppContentFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="89d11-127">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="89d11-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89d11-128">Property</span></span>|<span data-ttu-id="89d11-129">型</span><span class="sxs-lookup"><span data-stu-id="89d11-129">Type</span></span>|<span data-ttu-id="89d11-130">説明</span><span class="sxs-lookup"><span data-stu-id="89d11-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d11-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="89d11-131">azureStorageUri</span></span>|<span data-ttu-id="89d11-132">String</span><span class="sxs-lookup"><span data-stu-id="89d11-132">String</span></span>|<span data-ttu-id="89d11-133">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="89d11-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="89d11-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="89d11-134">isCommitted</span></span>|<span data-ttu-id="89d11-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="89d11-135">Boolean</span></span>|<span data-ttu-id="89d11-136">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="89d11-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="89d11-137">id</span><span class="sxs-lookup"><span data-stu-id="89d11-137">id</span></span>|<span data-ttu-id="89d11-138">String</span><span class="sxs-lookup"><span data-stu-id="89d11-138">String</span></span>|<span data-ttu-id="89d11-139">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="89d11-139">The File Id.</span></span>|
|<span data-ttu-id="89d11-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89d11-140">createdDateTime</span></span>|<span data-ttu-id="89d11-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d11-141">DateTimeOffset</span></span>|<span data-ttu-id="89d11-142">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="89d11-142">The time the file was created.</span></span>|
|<span data-ttu-id="89d11-143">name</span><span class="sxs-lookup"><span data-stu-id="89d11-143">name</span></span>|<span data-ttu-id="89d11-144">String</span><span class="sxs-lookup"><span data-stu-id="89d11-144">String</span></span>|<span data-ttu-id="89d11-145">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="89d11-145">the file name.</span></span>|
|<span data-ttu-id="89d11-146">size</span><span class="sxs-lookup"><span data-stu-id="89d11-146">size</span></span>|<span data-ttu-id="89d11-147">Int64</span><span class="sxs-lookup"><span data-stu-id="89d11-147">Int64</span></span>|<span data-ttu-id="89d11-148">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="89d11-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="89d11-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="89d11-149">sizeEncrypted</span></span>|<span data-ttu-id="89d11-150">Int64</span><span class="sxs-lookup"><span data-stu-id="89d11-150">Int64</span></span>|<span data-ttu-id="89d11-151">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="89d11-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="89d11-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="89d11-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="89d11-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d11-153">DateTimeOffset</span></span>|<span data-ttu-id="89d11-154">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="89d11-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="89d11-155">manifest</span><span class="sxs-lookup"><span data-stu-id="89d11-155">manifest</span></span>|<span data-ttu-id="89d11-156">Binary</span><span class="sxs-lookup"><span data-stu-id="89d11-156">Binary</span></span>|<span data-ttu-id="89d11-157">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="89d11-157">The manifest information.</span></span>|
|<span data-ttu-id="89d11-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="89d11-158">uploadState</span></span>|[<span data-ttu-id="89d11-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="89d11-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="89d11-160">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="89d11-160">The state of the current upload request.</span></span> <span data-ttu-id="89d11-161">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="89d11-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="89d11-162">応答</span><span class="sxs-lookup"><span data-stu-id="89d11-162">Response</span></span>
<span data-ttu-id="89d11-163">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89d11-163">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89d11-164">例</span><span class="sxs-lookup"><span data-stu-id="89d11-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="89d11-165">要求</span><span class="sxs-lookup"><span data-stu-id="89d11-165">Request</span></span>
<span data-ttu-id="89d11-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89d11-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="89d11-167">応答</span><span class="sxs-lookup"><span data-stu-id="89d11-167">Response</span></span>
<span data-ttu-id="89d11-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="89d11-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 450

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```



