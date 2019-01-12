---
title: mobileAppContentFile リソース タイプ
description: 特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 444c2824755d97b78e2ca2e3f1711f2809dacd30
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972916"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="65f06-103">mobileAppContentFile リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="65f06-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="65f06-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65f06-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65f06-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65f06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65f06-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="65f06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65f06-107">特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="65f06-107">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>
## <a name="methods"></a><span data-ttu-id="65f06-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="65f06-108">Methods</span></span>
|<span data-ttu-id="65f06-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="65f06-109">Method</span></span>|<span data-ttu-id="65f06-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="65f06-110">Return Type</span></span>|<span data-ttu-id="65f06-111">説明</span><span class="sxs-lookup"><span data-stu-id="65f06-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="65f06-112">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="65f06-112">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="65f06-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="65f06-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="65f06-114">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="65f06-114">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="65f06-115">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="65f06-115">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="65f06-116">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="65f06-116">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="65f06-117">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="65f06-117">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="65f06-118">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="65f06-118">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="65f06-119">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="65f06-119">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="65f06-120">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="65f06-120">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="65f06-121">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="65f06-121">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="65f06-122">なし</span><span class="sxs-lookup"><span data-stu-id="65f06-122">None</span></span>|<span data-ttu-id="65f06-123">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="65f06-123">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="65f06-124">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="65f06-124">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="65f06-125">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="65f06-125">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="65f06-126">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="65f06-126">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="65f06-127">commit action</span><span class="sxs-lookup"><span data-stu-id="65f06-127">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="65f06-128">なし</span><span class="sxs-lookup"><span data-stu-id="65f06-128">None</span></span>|<span data-ttu-id="65f06-129">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="65f06-129">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="65f06-130">renewUpload action</span><span class="sxs-lookup"><span data-stu-id="65f06-130">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="65f06-131">なし</span><span class="sxs-lookup"><span data-stu-id="65f06-131">None</span></span>|<span data-ttu-id="65f06-132">アプリケーション ファイルのアップロード用の SAS URI を更新します。</span><span class="sxs-lookup"><span data-stu-id="65f06-132">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="65f06-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65f06-133">Properties</span></span>
|<span data-ttu-id="65f06-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65f06-134">Property</span></span>|<span data-ttu-id="65f06-135">型</span><span class="sxs-lookup"><span data-stu-id="65f06-135">Type</span></span>|<span data-ttu-id="65f06-136">説明</span><span class="sxs-lookup"><span data-stu-id="65f06-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f06-137">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="65f06-137">azureStorageUri</span></span>|<span data-ttu-id="65f06-138">String</span><span class="sxs-lookup"><span data-stu-id="65f06-138">String</span></span>|<span data-ttu-id="65f06-139">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="65f06-139">The Azure Storage URI.</span></span>|
|<span data-ttu-id="65f06-140">isCommitted</span><span class="sxs-lookup"><span data-stu-id="65f06-140">isCommitted</span></span>|<span data-ttu-id="65f06-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f06-141">Boolean</span></span>|<span data-ttu-id="65f06-142">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="65f06-142">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="65f06-143">id</span><span class="sxs-lookup"><span data-stu-id="65f06-143">id</span></span>|<span data-ttu-id="65f06-144">String</span><span class="sxs-lookup"><span data-stu-id="65f06-144">String</span></span>|<span data-ttu-id="65f06-145">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="65f06-145">The File Id.</span></span>|
|<span data-ttu-id="65f06-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65f06-146">createdDateTime</span></span>|<span data-ttu-id="65f06-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65f06-147">DateTimeOffset</span></span>|<span data-ttu-id="65f06-148">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="65f06-148">The time the file was created.</span></span>|
|<span data-ttu-id="65f06-149">name</span><span class="sxs-lookup"><span data-stu-id="65f06-149">name</span></span>|<span data-ttu-id="65f06-150">String</span><span class="sxs-lookup"><span data-stu-id="65f06-150">String</span></span>|<span data-ttu-id="65f06-151">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="65f06-151">the file name.</span></span>|
|<span data-ttu-id="65f06-152">size</span><span class="sxs-lookup"><span data-stu-id="65f06-152">size</span></span>|<span data-ttu-id="65f06-153">Int64</span><span class="sxs-lookup"><span data-stu-id="65f06-153">Int64</span></span>|<span data-ttu-id="65f06-154">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="65f06-154">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="65f06-155">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="65f06-155">sizeEncrypted</span></span>|<span data-ttu-id="65f06-156">Int64</span><span class="sxs-lookup"><span data-stu-id="65f06-156">Int64</span></span>|<span data-ttu-id="65f06-157">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="65f06-157">The size of the file after encryption.</span></span>|
|<span data-ttu-id="65f06-158">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="65f06-158">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="65f06-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65f06-159">DateTimeOffset</span></span>|<span data-ttu-id="65f06-160">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="65f06-160">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="65f06-161">manifest</span><span class="sxs-lookup"><span data-stu-id="65f06-161">manifest</span></span>|<span data-ttu-id="65f06-162">Binary</span><span class="sxs-lookup"><span data-stu-id="65f06-162">Binary</span></span>|<span data-ttu-id="65f06-163">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="65f06-163">The manifest information.</span></span>|
|<span data-ttu-id="65f06-164">uploadState</span><span class="sxs-lookup"><span data-stu-id="65f06-164">uploadState</span></span>|[<span data-ttu-id="65f06-165">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="65f06-165">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="65f06-166">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="65f06-166">The state of the current upload request.</span></span> <span data-ttu-id="65f06-167">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="65f06-167">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="65f06-168">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="65f06-168">isFrameworkFile</span></span>|<span data-ttu-id="65f06-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f06-169">Boolean</span></span>|<span data-ttu-id="65f06-170">フレームワーク ファイルのファイルかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="65f06-170">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="65f06-171">isDependency</span><span class="sxs-lookup"><span data-stu-id="65f06-171">isDependency</span></span>|<span data-ttu-id="65f06-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f06-172">Boolean</span></span>|<span data-ttu-id="65f06-173">かどうか、コンテンツ ファイルは、メインのコンテンツ ファイルの依存関係です。</span><span class="sxs-lookup"><span data-stu-id="65f06-173">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65f06-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65f06-174">Relationships</span></span>
<span data-ttu-id="65f06-175">なし</span><span class="sxs-lookup"><span data-stu-id="65f06-175">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65f06-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65f06-176">JSON Representation</span></span>
<span data-ttu-id="65f06-177">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65f06-177">Here is a JSON representation of the resource.</span></span>
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





