---
title: mobileAppContentFile の更新
description: mobileAppContentFile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8db4e9544e044f004e3524bf0a0df9af9360f342
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944545"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="db28b-103">mobileAppContentFile の更新</span><span class="sxs-lookup"><span data-stu-id="db28b-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="db28b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="db28b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db28b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db28b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db28b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="db28b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db28b-107">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="db28b-107">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db28b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="db28b-108">Prerequisites</span></span>
<span data-ttu-id="db28b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db28b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db28b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db28b-111">Permission type</span></span>|<span data-ttu-id="db28b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="db28b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db28b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db28b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db28b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db28b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="db28b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db28b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db28b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db28b-116">Not supported.</span></span>|
|<span data-ttu-id="db28b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db28b-117">Application</span></span>|<span data-ttu-id="db28b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db28b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db28b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db28b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="db28b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db28b-120">Request headers</span></span>
|<span data-ttu-id="db28b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db28b-121">Header</span></span>|<span data-ttu-id="db28b-122">値</span><span class="sxs-lookup"><span data-stu-id="db28b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db28b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db28b-123">Authorization</span></span>|<span data-ttu-id="db28b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="db28b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db28b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="db28b-125">Accept</span></span>|<span data-ttu-id="db28b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db28b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db28b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="db28b-127">Request body</span></span>
<span data-ttu-id="db28b-128">要求本文で、[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="db28b-128">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="db28b-129">次の表に、[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="db28b-129">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="db28b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db28b-130">Property</span></span>|<span data-ttu-id="db28b-131">型</span><span class="sxs-lookup"><span data-stu-id="db28b-131">Type</span></span>|<span data-ttu-id="db28b-132">説明</span><span class="sxs-lookup"><span data-stu-id="db28b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db28b-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="db28b-133">azureStorageUri</span></span>|<span data-ttu-id="db28b-134">String</span><span class="sxs-lookup"><span data-stu-id="db28b-134">String</span></span>|<span data-ttu-id="db28b-135">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="db28b-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="db28b-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="db28b-136">isCommitted</span></span>|<span data-ttu-id="db28b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="db28b-137">Boolean</span></span>|<span data-ttu-id="db28b-138">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="db28b-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="db28b-139">id</span><span class="sxs-lookup"><span data-stu-id="db28b-139">id</span></span>|<span data-ttu-id="db28b-140">String</span><span class="sxs-lookup"><span data-stu-id="db28b-140">String</span></span>|<span data-ttu-id="db28b-141">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="db28b-141">The File Id.</span></span>|
|<span data-ttu-id="db28b-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db28b-142">createdDateTime</span></span>|<span data-ttu-id="db28b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db28b-143">DateTimeOffset</span></span>|<span data-ttu-id="db28b-144">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="db28b-144">The time the file was created.</span></span>|
|<span data-ttu-id="db28b-145">name</span><span class="sxs-lookup"><span data-stu-id="db28b-145">name</span></span>|<span data-ttu-id="db28b-146">String</span><span class="sxs-lookup"><span data-stu-id="db28b-146">String</span></span>|<span data-ttu-id="db28b-147">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="db28b-147">the file name.</span></span>|
|<span data-ttu-id="db28b-148">size</span><span class="sxs-lookup"><span data-stu-id="db28b-148">size</span></span>|<span data-ttu-id="db28b-149">Int64</span><span class="sxs-lookup"><span data-stu-id="db28b-149">Int64</span></span>|<span data-ttu-id="db28b-150">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="db28b-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="db28b-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="db28b-151">sizeEncrypted</span></span>|<span data-ttu-id="db28b-152">Int64</span><span class="sxs-lookup"><span data-stu-id="db28b-152">Int64</span></span>|<span data-ttu-id="db28b-153">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="db28b-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="db28b-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="db28b-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="db28b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db28b-155">DateTimeOffset</span></span>|<span data-ttu-id="db28b-156">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="db28b-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="db28b-157">manifest</span><span class="sxs-lookup"><span data-stu-id="db28b-157">manifest</span></span>|<span data-ttu-id="db28b-158">Binary</span><span class="sxs-lookup"><span data-stu-id="db28b-158">Binary</span></span>|<span data-ttu-id="db28b-159">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="db28b-159">The manifest information.</span></span>|
|<span data-ttu-id="db28b-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="db28b-160">uploadState</span></span>|[<span data-ttu-id="db28b-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="db28b-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="db28b-162">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="db28b-162">The state of the current upload request.</span></span> <span data-ttu-id="db28b-163">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="db28b-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="db28b-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="db28b-164">isFrameworkFile</span></span>|<span data-ttu-id="db28b-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="db28b-165">Boolean</span></span>|<span data-ttu-id="db28b-166">フレームワーク ファイルのファイルかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="db28b-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="db28b-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="db28b-167">isDependency</span></span>|<span data-ttu-id="db28b-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="db28b-168">Boolean</span></span>|<span data-ttu-id="db28b-169">かどうか、コンテンツ ファイルは、メインのコンテンツ ファイルの依存関係です。</span><span class="sxs-lookup"><span data-stu-id="db28b-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="db28b-170">応答</span><span class="sxs-lookup"><span data-stu-id="db28b-170">Response</span></span>
<span data-ttu-id="db28b-171">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="db28b-171">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db28b-172">例</span><span class="sxs-lookup"><span data-stu-id="db28b-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="db28b-173">要求</span><span class="sxs-lookup"><span data-stu-id="db28b-173">Request</span></span>
<span data-ttu-id="db28b-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db28b-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 336

{
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

### <a name="response"></a><span data-ttu-id="db28b-175">応答</span><span class="sxs-lookup"><span data-stu-id="db28b-175">Response</span></span>
<span data-ttu-id="db28b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="db28b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





