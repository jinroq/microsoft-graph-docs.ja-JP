---
title: mobileAppContentFile の作成
description: 新しい mobileAppContentFile オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c815cfcb272e0eb79465d81702e158934ec8c42a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394244"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="15d56-103">mobileAppContentFile の作成</span><span class="sxs-lookup"><span data-stu-id="15d56-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="15d56-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15d56-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15d56-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15d56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15d56-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15d56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15d56-107">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="15d56-107">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15d56-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="15d56-108">Prerequisites</span></span>
<span data-ttu-id="15d56-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15d56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15d56-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15d56-111">Permission type</span></span>|<span data-ttu-id="15d56-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="15d56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15d56-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15d56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15d56-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15d56-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15d56-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15d56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15d56-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15d56-116">Not supported.</span></span>|
|<span data-ttu-id="15d56-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15d56-117">Application</span></span>|<span data-ttu-id="15d56-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15d56-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15d56-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15d56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="15d56-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15d56-120">Request headers</span></span>
|<span data-ttu-id="15d56-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15d56-121">Header</span></span>|<span data-ttu-id="15d56-122">値</span><span class="sxs-lookup"><span data-stu-id="15d56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15d56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15d56-123">Authorization</span></span>|<span data-ttu-id="15d56-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="15d56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15d56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15d56-125">Accept</span></span>|<span data-ttu-id="15d56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15d56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15d56-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="15d56-127">Request body</span></span>
<span data-ttu-id="15d56-128">要求本文で、mobileAppContentFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="15d56-128">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="15d56-129">次の表に、mobileAppContentFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="15d56-129">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="15d56-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15d56-130">Property</span></span>|<span data-ttu-id="15d56-131">型</span><span class="sxs-lookup"><span data-stu-id="15d56-131">Type</span></span>|<span data-ttu-id="15d56-132">説明</span><span class="sxs-lookup"><span data-stu-id="15d56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15d56-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="15d56-133">azureStorageUri</span></span>|<span data-ttu-id="15d56-134">String</span><span class="sxs-lookup"><span data-stu-id="15d56-134">String</span></span>|<span data-ttu-id="15d56-135">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="15d56-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="15d56-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="15d56-136">isCommitted</span></span>|<span data-ttu-id="15d56-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="15d56-137">Boolean</span></span>|<span data-ttu-id="15d56-138">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="15d56-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="15d56-139">id</span><span class="sxs-lookup"><span data-stu-id="15d56-139">id</span></span>|<span data-ttu-id="15d56-140">String</span><span class="sxs-lookup"><span data-stu-id="15d56-140">String</span></span>|<span data-ttu-id="15d56-141">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="15d56-141">The File Id.</span></span>|
|<span data-ttu-id="15d56-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15d56-142">createdDateTime</span></span>|<span data-ttu-id="15d56-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15d56-143">DateTimeOffset</span></span>|<span data-ttu-id="15d56-144">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="15d56-144">The time the file was created.</span></span>|
|<span data-ttu-id="15d56-145">name</span><span class="sxs-lookup"><span data-stu-id="15d56-145">name</span></span>|<span data-ttu-id="15d56-146">String</span><span class="sxs-lookup"><span data-stu-id="15d56-146">String</span></span>|<span data-ttu-id="15d56-147">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="15d56-147">the file name.</span></span>|
|<span data-ttu-id="15d56-148">size</span><span class="sxs-lookup"><span data-stu-id="15d56-148">size</span></span>|<span data-ttu-id="15d56-149">Int64</span><span class="sxs-lookup"><span data-stu-id="15d56-149">Int64</span></span>|<span data-ttu-id="15d56-150">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="15d56-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="15d56-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="15d56-151">sizeEncrypted</span></span>|<span data-ttu-id="15d56-152">Int64</span><span class="sxs-lookup"><span data-stu-id="15d56-152">Int64</span></span>|<span data-ttu-id="15d56-153">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="15d56-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="15d56-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="15d56-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="15d56-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15d56-155">DateTimeOffset</span></span>|<span data-ttu-id="15d56-156">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="15d56-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="15d56-157">manifest</span><span class="sxs-lookup"><span data-stu-id="15d56-157">manifest</span></span>|<span data-ttu-id="15d56-158">Binary</span><span class="sxs-lookup"><span data-stu-id="15d56-158">Binary</span></span>|<span data-ttu-id="15d56-159">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="15d56-159">The manifest information.</span></span>|
|<span data-ttu-id="15d56-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="15d56-160">uploadState</span></span>|[<span data-ttu-id="15d56-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="15d56-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="15d56-162">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="15d56-162">The state of the current upload request.</span></span> <span data-ttu-id="15d56-163">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="15d56-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="15d56-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="15d56-164">isFrameworkFile</span></span>|<span data-ttu-id="15d56-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="15d56-165">Boolean</span></span>|<span data-ttu-id="15d56-166">フレームワーク ファイルのファイルかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="15d56-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="15d56-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="15d56-167">isDependency</span></span>|<span data-ttu-id="15d56-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="15d56-168">Boolean</span></span>|<span data-ttu-id="15d56-169">かどうか、コンテンツ ファイルは、メインのコンテンツ ファイルの依存関係です。</span><span class="sxs-lookup"><span data-stu-id="15d56-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="15d56-170">応答</span><span class="sxs-lookup"><span data-stu-id="15d56-170">Response</span></span>
<span data-ttu-id="15d56-171">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="15d56-171">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15d56-172">例</span><span class="sxs-lookup"><span data-stu-id="15d56-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="15d56-173">要求</span><span class="sxs-lookup"><span data-stu-id="15d56-173">Request</span></span>
<span data-ttu-id="15d56-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15d56-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="15d56-175">応答</span><span class="sxs-lookup"><span data-stu-id="15d56-175">Response</span></span>
<span data-ttu-id="15d56-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="15d56-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




