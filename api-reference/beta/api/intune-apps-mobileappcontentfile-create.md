---
title: mobileAppContentFile の作成
description: 新しい mobileAppContentFile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 221222dc6ea212d02fd89cd83a528e022f873cc9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960819"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="d1310-103">mobileAppContentFile の作成</span><span class="sxs-lookup"><span data-stu-id="d1310-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="d1310-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1310-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1310-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1310-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1310-106">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1310-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1310-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d1310-107">Prerequisites</span></span>
<span data-ttu-id="d1310-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1310-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1310-110">Permission type</span></span>|<span data-ttu-id="d1310-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1310-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1310-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1310-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1310-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1310-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d1310-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1310-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1310-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1310-115">Not supported.</span></span>|
|<span data-ttu-id="d1310-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1310-116">Application</span></span>|<span data-ttu-id="d1310-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1310-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1310-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1310-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="d1310-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1310-119">Request headers</span></span>
|<span data-ttu-id="d1310-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1310-120">Header</span></span>|<span data-ttu-id="d1310-121">値</span><span class="sxs-lookup"><span data-stu-id="d1310-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1310-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1310-122">Authorization</span></span>|<span data-ttu-id="d1310-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1310-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1310-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d1310-124">Accept</span></span>|<span data-ttu-id="d1310-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1310-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1310-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1310-126">Request body</span></span>
<span data-ttu-id="d1310-127">要求本文で、mobileAppContentFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d1310-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="d1310-128">次の表に、mobileAppContentFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d1310-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="d1310-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1310-129">Property</span></span>|<span data-ttu-id="d1310-130">型</span><span class="sxs-lookup"><span data-stu-id="d1310-130">Type</span></span>|<span data-ttu-id="d1310-131">説明</span><span class="sxs-lookup"><span data-stu-id="d1310-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1310-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="d1310-132">azureStorageUri</span></span>|<span data-ttu-id="d1310-133">String</span><span class="sxs-lookup"><span data-stu-id="d1310-133">String</span></span>|<span data-ttu-id="d1310-134">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="d1310-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="d1310-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="d1310-135">isCommitted</span></span>|<span data-ttu-id="d1310-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1310-136">Boolean</span></span>|<span data-ttu-id="d1310-137">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="d1310-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="d1310-138">id</span><span class="sxs-lookup"><span data-stu-id="d1310-138">id</span></span>|<span data-ttu-id="d1310-139">文字列</span><span class="sxs-lookup"><span data-stu-id="d1310-139">String</span></span>|<span data-ttu-id="d1310-140">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="d1310-140">The File Id.</span></span>|
|<span data-ttu-id="d1310-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1310-141">createdDateTime</span></span>|<span data-ttu-id="d1310-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1310-142">DateTimeOffset</span></span>|<span data-ttu-id="d1310-143">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="d1310-143">The time the file was created.</span></span>|
|<span data-ttu-id="d1310-144">name</span><span class="sxs-lookup"><span data-stu-id="d1310-144">name</span></span>|<span data-ttu-id="d1310-145">String</span><span class="sxs-lookup"><span data-stu-id="d1310-145">String</span></span>|<span data-ttu-id="d1310-146">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="d1310-146">the file name.</span></span>|
|<span data-ttu-id="d1310-147">size</span><span class="sxs-lookup"><span data-stu-id="d1310-147">size</span></span>|<span data-ttu-id="d1310-148">Int64</span><span class="sxs-lookup"><span data-stu-id="d1310-148">Int64</span></span>|<span data-ttu-id="d1310-149">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="d1310-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="d1310-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="d1310-150">sizeEncrypted</span></span>|<span data-ttu-id="d1310-151">Int64</span><span class="sxs-lookup"><span data-stu-id="d1310-151">Int64</span></span>|<span data-ttu-id="d1310-152">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="d1310-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="d1310-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d1310-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="d1310-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1310-154">DateTimeOffset</span></span>|<span data-ttu-id="d1310-155">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="d1310-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="d1310-156">manifest</span><span class="sxs-lookup"><span data-stu-id="d1310-156">manifest</span></span>|<span data-ttu-id="d1310-157">Binary</span><span class="sxs-lookup"><span data-stu-id="d1310-157">Binary</span></span>|<span data-ttu-id="d1310-158">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="d1310-158">The manifest information.</span></span>|
|<span data-ttu-id="d1310-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="d1310-159">uploadState</span></span>|[<span data-ttu-id="d1310-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="d1310-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="d1310-161">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="d1310-161">The state of the current upload request.</span></span> <span data-ttu-id="d1310-162">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="d1310-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="d1310-163">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="d1310-163">isFrameworkFile</span></span>|<span data-ttu-id="d1310-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1310-164">Boolean</span></span>|<span data-ttu-id="d1310-165">ファイルがフレームワークファイルであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="d1310-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="d1310-166">isDependency</span><span class="sxs-lookup"><span data-stu-id="d1310-166">isDependency</span></span>|<span data-ttu-id="d1310-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1310-167">Boolean</span></span>|<span data-ttu-id="d1310-168">コンテンツファイルがメインコンテンツファイルの依存関係であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d1310-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="d1310-169">応答</span><span class="sxs-lookup"><span data-stu-id="d1310-169">Response</span></span>
<span data-ttu-id="d1310-170">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d1310-170">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1310-171">例</span><span class="sxs-lookup"><span data-stu-id="d1310-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1310-172">要求</span><span class="sxs-lookup"><span data-stu-id="d1310-172">Request</span></span>
<span data-ttu-id="d1310-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1310-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-type: application/json
Content-length: 395

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```

### <a name="response"></a><span data-ttu-id="d1310-174">応答</span><span class="sxs-lookup"><span data-stu-id="d1310-174">Response</span></span>
<span data-ttu-id="d1310-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d1310-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 503

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
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```





