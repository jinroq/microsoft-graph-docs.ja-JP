---
title: mobileAppContentFile リソース タイプ
description: 特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。
ms.openlocfilehash: 72467995e4d586df54a6c3cb2295e37cd9b9c6ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071457"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="fc6c5-103">mobileAppContentFile リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="fc6c5-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="fc6c5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc6c5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc6c5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc6c5-107">特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-107">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>
## <a name="methods"></a><span data-ttu-id="fc6c5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fc6c5-108">Methods</span></span>
|<span data-ttu-id="fc6c5-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="fc6c5-109">Method</span></span>|<span data-ttu-id="fc6c5-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fc6c5-110">Return Type</span></span>|<span data-ttu-id="fc6c5-111">説明</span><span class="sxs-lookup"><span data-stu-id="fc6c5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fc6c5-112">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="fc6c5-112">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="fc6c5-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fc6c5-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="fc6c5-114">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-114">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="fc6c5-115">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="fc6c5-115">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="fc6c5-116">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="fc6c5-116">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="fc6c5-117">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-117">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="fc6c5-118">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="fc6c5-118">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="fc6c5-119">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="fc6c5-119">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="fc6c5-120">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-120">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="fc6c5-121">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="fc6c5-121">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="fc6c5-122">なし</span><span class="sxs-lookup"><span data-stu-id="fc6c5-122">None</span></span>|<span data-ttu-id="fc6c5-123">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-123">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="fc6c5-124">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="fc6c5-124">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="fc6c5-125">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="fc6c5-125">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="fc6c5-126">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-126">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="fc6c5-127">commit action</span><span class="sxs-lookup"><span data-stu-id="fc6c5-127">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="fc6c5-128">なし</span><span class="sxs-lookup"><span data-stu-id="fc6c5-128">None</span></span>|<span data-ttu-id="fc6c5-129">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-129">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="fc6c5-130">renewUpload action</span><span class="sxs-lookup"><span data-stu-id="fc6c5-130">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="fc6c5-131">なし</span><span class="sxs-lookup"><span data-stu-id="fc6c5-131">None</span></span>|<span data-ttu-id="fc6c5-132">アプリケーション ファイルのアップロード用の SAS URI を更新します。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-132">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc6c5-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc6c5-133">Properties</span></span>
|<span data-ttu-id="fc6c5-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc6c5-134">Property</span></span>|<span data-ttu-id="fc6c5-135">型</span><span class="sxs-lookup"><span data-stu-id="fc6c5-135">Type</span></span>|<span data-ttu-id="fc6c5-136">説明</span><span class="sxs-lookup"><span data-stu-id="fc6c5-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc6c5-137">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="fc6c5-137">azureStorageUri</span></span>|<span data-ttu-id="fc6c5-138">String</span><span class="sxs-lookup"><span data-stu-id="fc6c5-138">String</span></span>|<span data-ttu-id="fc6c5-139">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-139">The Azure Storage URI.</span></span>|
|<span data-ttu-id="fc6c5-140">isCommitted</span><span class="sxs-lookup"><span data-stu-id="fc6c5-140">isCommitted</span></span>|<span data-ttu-id="fc6c5-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc6c5-141">Boolean</span></span>|<span data-ttu-id="fc6c5-142">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-142">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="fc6c5-143">id</span><span class="sxs-lookup"><span data-stu-id="fc6c5-143">id</span></span>|<span data-ttu-id="fc6c5-144">String</span><span class="sxs-lookup"><span data-stu-id="fc6c5-144">String</span></span>|<span data-ttu-id="fc6c5-145">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-145">The File Id.</span></span>|
|<span data-ttu-id="fc6c5-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc6c5-146">createdDateTime</span></span>|<span data-ttu-id="fc6c5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc6c5-147">DateTimeOffset</span></span>|<span data-ttu-id="fc6c5-148">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-148">The time the file was created.</span></span>|
|<span data-ttu-id="fc6c5-149">name</span><span class="sxs-lookup"><span data-stu-id="fc6c5-149">name</span></span>|<span data-ttu-id="fc6c5-150">String</span><span class="sxs-lookup"><span data-stu-id="fc6c5-150">String</span></span>|<span data-ttu-id="fc6c5-151">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-151">the file name.</span></span>|
|<span data-ttu-id="fc6c5-152">size</span><span class="sxs-lookup"><span data-stu-id="fc6c5-152">size</span></span>|<span data-ttu-id="fc6c5-153">Int64</span><span class="sxs-lookup"><span data-stu-id="fc6c5-153">Int64</span></span>|<span data-ttu-id="fc6c5-154">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-154">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="fc6c5-155">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="fc6c5-155">sizeEncrypted</span></span>|<span data-ttu-id="fc6c5-156">Int64</span><span class="sxs-lookup"><span data-stu-id="fc6c5-156">Int64</span></span>|<span data-ttu-id="fc6c5-157">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-157">The size of the file after encryption.</span></span>|
|<span data-ttu-id="fc6c5-158">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fc6c5-158">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="fc6c5-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc6c5-159">DateTimeOffset</span></span>|<span data-ttu-id="fc6c5-160">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-160">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="fc6c5-161">manifest</span><span class="sxs-lookup"><span data-stu-id="fc6c5-161">manifest</span></span>|<span data-ttu-id="fc6c5-162">バイナリ</span><span class="sxs-lookup"><span data-stu-id="fc6c5-162">Binary</span></span>|<span data-ttu-id="fc6c5-163">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-163">The manifest information.</span></span>|
|<span data-ttu-id="fc6c5-164">uploadState</span><span class="sxs-lookup"><span data-stu-id="fc6c5-164">uploadState</span></span>|[<span data-ttu-id="fc6c5-165">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="fc6c5-165">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="fc6c5-166">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-166">The state of the current upload request.</span></span> <span data-ttu-id="fc6c5-167">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-167">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="fc6c5-168">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="fc6c5-168">isFrameworkFile</span></span>|<span data-ttu-id="fc6c5-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="fc6c5-169">Boolean</span></span>|<span data-ttu-id="fc6c5-170">フレームワーク ファイルのファイルかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-170">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="fc6c5-171">isDependency</span><span class="sxs-lookup"><span data-stu-id="fc6c5-171">isDependency</span></span>|<span data-ttu-id="fc6c5-172">ブール値</span><span class="sxs-lookup"><span data-stu-id="fc6c5-172">Boolean</span></span>|<span data-ttu-id="fc6c5-173">かどうか、コンテンツ ファイルは、メインのコンテンツ ファイルの依存関係です。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-173">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc6c5-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fc6c5-174">Relationships</span></span>
<span data-ttu-id="fc6c5-175">なし</span><span class="sxs-lookup"><span data-stu-id="fc6c5-175">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc6c5-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc6c5-176">JSON Representation</span></span>
<span data-ttu-id="fc6c5-177">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fc6c5-177">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": true,
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String",
  "isFrameworkFile": true,
  "isDependency": true
}
```





