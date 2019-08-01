---
title: mobileAppContentFile の更新
description: mobileAppContentFile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e8e14c92ed790deb84bc1bd17036b32644d2331
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001979"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="7fc64-103">mobileAppContentFile の更新</span><span class="sxs-lookup"><span data-stu-id="7fc64-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="7fc64-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7fc64-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fc64-105">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7fc64-105">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fc64-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7fc64-106">Prerequisites</span></span>
<span data-ttu-id="7fc64-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7fc64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fc64-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7fc64-109">Permission type</span></span>|<span data-ttu-id="7fc64-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7fc64-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fc64-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7fc64-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7fc64-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc64-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7fc64-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7fc64-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fc64-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fc64-114">Not supported.</span></span>|
|<span data-ttu-id="7fc64-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7fc64-115">Application</span></span>|<span data-ttu-id="7fc64-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fc64-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fc64-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7fc64-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="7fc64-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7fc64-118">Request headers</span></span>
|<span data-ttu-id="7fc64-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7fc64-119">Header</span></span>|<span data-ttu-id="7fc64-120">値</span><span class="sxs-lookup"><span data-stu-id="7fc64-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fc64-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fc64-121">Authorization</span></span>|<span data-ttu-id="7fc64-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7fc64-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fc64-123">承諾</span><span class="sxs-lookup"><span data-stu-id="7fc64-123">Accept</span></span>|<span data-ttu-id="7fc64-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7fc64-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fc64-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7fc64-125">Request body</span></span>
<span data-ttu-id="7fc64-126">要求本文で、[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7fc64-126">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="7fc64-127">次の表に、[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7fc64-127">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="7fc64-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fc64-128">Property</span></span>|<span data-ttu-id="7fc64-129">型</span><span class="sxs-lookup"><span data-stu-id="7fc64-129">Type</span></span>|<span data-ttu-id="7fc64-130">説明</span><span class="sxs-lookup"><span data-stu-id="7fc64-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fc64-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="7fc64-131">azureStorageUri</span></span>|<span data-ttu-id="7fc64-132">String</span><span class="sxs-lookup"><span data-stu-id="7fc64-132">String</span></span>|<span data-ttu-id="7fc64-133">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="7fc64-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="7fc64-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="7fc64-134">isCommitted</span></span>|<span data-ttu-id="7fc64-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fc64-135">Boolean</span></span>|<span data-ttu-id="7fc64-136">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7fc64-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="7fc64-137">id</span><span class="sxs-lookup"><span data-stu-id="7fc64-137">id</span></span>|<span data-ttu-id="7fc64-138">文字列</span><span class="sxs-lookup"><span data-stu-id="7fc64-138">String</span></span>|<span data-ttu-id="7fc64-139">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="7fc64-139">The File Id.</span></span>|
|<span data-ttu-id="7fc64-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7fc64-140">createdDateTime</span></span>|<span data-ttu-id="7fc64-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fc64-141">DateTimeOffset</span></span>|<span data-ttu-id="7fc64-142">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="7fc64-142">The time the file was created.</span></span>|
|<span data-ttu-id="7fc64-143">name</span><span class="sxs-lookup"><span data-stu-id="7fc64-143">name</span></span>|<span data-ttu-id="7fc64-144">String</span><span class="sxs-lookup"><span data-stu-id="7fc64-144">String</span></span>|<span data-ttu-id="7fc64-145">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="7fc64-145">the file name.</span></span>|
|<span data-ttu-id="7fc64-146">size</span><span class="sxs-lookup"><span data-stu-id="7fc64-146">size</span></span>|<span data-ttu-id="7fc64-147">Int64</span><span class="sxs-lookup"><span data-stu-id="7fc64-147">Int64</span></span>|<span data-ttu-id="7fc64-148">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="7fc64-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="7fc64-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="7fc64-149">sizeEncrypted</span></span>|<span data-ttu-id="7fc64-150">Int64</span><span class="sxs-lookup"><span data-stu-id="7fc64-150">Int64</span></span>|<span data-ttu-id="7fc64-151">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="7fc64-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="7fc64-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7fc64-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="7fc64-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fc64-153">DateTimeOffset</span></span>|<span data-ttu-id="7fc64-154">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="7fc64-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="7fc64-155">manifest</span><span class="sxs-lookup"><span data-stu-id="7fc64-155">manifest</span></span>|<span data-ttu-id="7fc64-156">Binary</span><span class="sxs-lookup"><span data-stu-id="7fc64-156">Binary</span></span>|<span data-ttu-id="7fc64-157">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="7fc64-157">The manifest information.</span></span>|
|<span data-ttu-id="7fc64-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="7fc64-158">uploadState</span></span>|[<span data-ttu-id="7fc64-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="7fc64-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="7fc64-160">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="7fc64-160">The state of the current upload request.</span></span> <span data-ttu-id="7fc64-161">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="7fc64-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="7fc64-162">応答</span><span class="sxs-lookup"><span data-stu-id="7fc64-162">Response</span></span>
<span data-ttu-id="7fc64-163">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="7fc64-163">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fc64-164">例</span><span class="sxs-lookup"><span data-stu-id="7fc64-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fc64-165">要求</span><span class="sxs-lookup"><span data-stu-id="7fc64-165">Request</span></span>
<span data-ttu-id="7fc64-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7fc64-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
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

### <a name="response"></a><span data-ttu-id="7fc64-167">応答</span><span class="sxs-lookup"><span data-stu-id="7fc64-167">Response</span></span>
<span data-ttu-id="7fc64-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7fc64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



