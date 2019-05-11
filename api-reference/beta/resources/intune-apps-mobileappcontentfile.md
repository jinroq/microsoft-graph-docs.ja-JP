---
title: mobileAppContentFile リソース タイプ
description: 特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b0b1697bcbf4832b00f40584ebd85644c0052ac
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949961"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="23082-103">mobileAppContentFile リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="23082-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="23082-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23082-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23082-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23082-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23082-106">特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="23082-106">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>

## <a name="methods"></a><span data-ttu-id="23082-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="23082-107">Methods</span></span>
|<span data-ttu-id="23082-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="23082-108">Method</span></span>|<span data-ttu-id="23082-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="23082-109">Return Type</span></span>|<span data-ttu-id="23082-110">説明</span><span class="sxs-lookup"><span data-stu-id="23082-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23082-111">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="23082-111">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="23082-112">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="23082-112">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="23082-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="23082-113">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="23082-114">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23082-114">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="23082-115">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23082-115">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="23082-116">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="23082-116">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="23082-117">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23082-117">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="23082-118">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23082-118">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="23082-119">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="23082-119">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="23082-120">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23082-120">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="23082-121">None</span><span class="sxs-lookup"><span data-stu-id="23082-121">None</span></span>|<span data-ttu-id="23082-122">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="23082-122">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="23082-123">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23082-123">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="23082-124">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23082-124">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="23082-125">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="23082-125">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="23082-126">commit action</span><span class="sxs-lookup"><span data-stu-id="23082-126">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="23082-127">None</span><span class="sxs-lookup"><span data-stu-id="23082-127">None</span></span>|<span data-ttu-id="23082-128">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="23082-128">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="23082-129">renewUpload action</span><span class="sxs-lookup"><span data-stu-id="23082-129">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="23082-130">なし</span><span class="sxs-lookup"><span data-stu-id="23082-130">None</span></span>|<span data-ttu-id="23082-131">アプリケーション ファイルのアップロード用の SAS URI を更新します。</span><span class="sxs-lookup"><span data-stu-id="23082-131">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="23082-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23082-132">Properties</span></span>
|<span data-ttu-id="23082-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23082-133">Property</span></span>|<span data-ttu-id="23082-134">型</span><span class="sxs-lookup"><span data-stu-id="23082-134">Type</span></span>|<span data-ttu-id="23082-135">説明</span><span class="sxs-lookup"><span data-stu-id="23082-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23082-136">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="23082-136">azureStorageUri</span></span>|<span data-ttu-id="23082-137">String</span><span class="sxs-lookup"><span data-stu-id="23082-137">String</span></span>|<span data-ttu-id="23082-138">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="23082-138">The Azure Storage URI.</span></span>|
|<span data-ttu-id="23082-139">isCommitted</span><span class="sxs-lookup"><span data-stu-id="23082-139">isCommitted</span></span>|<span data-ttu-id="23082-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="23082-140">Boolean</span></span>|<span data-ttu-id="23082-141">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="23082-141">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="23082-142">id</span><span class="sxs-lookup"><span data-stu-id="23082-142">id</span></span>|<span data-ttu-id="23082-143">文字列</span><span class="sxs-lookup"><span data-stu-id="23082-143">String</span></span>|<span data-ttu-id="23082-144">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="23082-144">The File Id.</span></span>|
|<span data-ttu-id="23082-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23082-145">createdDateTime</span></span>|<span data-ttu-id="23082-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23082-146">DateTimeOffset</span></span>|<span data-ttu-id="23082-147">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="23082-147">The time the file was created.</span></span>|
|<span data-ttu-id="23082-148">name</span><span class="sxs-lookup"><span data-stu-id="23082-148">name</span></span>|<span data-ttu-id="23082-149">String</span><span class="sxs-lookup"><span data-stu-id="23082-149">String</span></span>|<span data-ttu-id="23082-150">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="23082-150">the file name.</span></span>|
|<span data-ttu-id="23082-151">size</span><span class="sxs-lookup"><span data-stu-id="23082-151">size</span></span>|<span data-ttu-id="23082-152">Int64</span><span class="sxs-lookup"><span data-stu-id="23082-152">Int64</span></span>|<span data-ttu-id="23082-153">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="23082-153">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="23082-154">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="23082-154">sizeEncrypted</span></span>|<span data-ttu-id="23082-155">Int64</span><span class="sxs-lookup"><span data-stu-id="23082-155">Int64</span></span>|<span data-ttu-id="23082-156">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="23082-156">The size of the file after encryption.</span></span>|
|<span data-ttu-id="23082-157">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="23082-157">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="23082-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23082-158">DateTimeOffset</span></span>|<span data-ttu-id="23082-159">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="23082-159">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="23082-160">manifest</span><span class="sxs-lookup"><span data-stu-id="23082-160">manifest</span></span>|<span data-ttu-id="23082-161">Binary</span><span class="sxs-lookup"><span data-stu-id="23082-161">Binary</span></span>|<span data-ttu-id="23082-162">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="23082-162">The manifest information.</span></span>|
|<span data-ttu-id="23082-163">uploadState</span><span class="sxs-lookup"><span data-stu-id="23082-163">uploadState</span></span>|[<span data-ttu-id="23082-164">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="23082-164">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="23082-165">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="23082-165">The state of the current upload request.</span></span> <span data-ttu-id="23082-166">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="23082-166">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="23082-167">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="23082-167">isFrameworkFile</span></span>|<span data-ttu-id="23082-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="23082-168">Boolean</span></span>|<span data-ttu-id="23082-169">ファイルがフレームワークファイルであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="23082-169">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="23082-170">isDependency</span><span class="sxs-lookup"><span data-stu-id="23082-170">isDependency</span></span>|<span data-ttu-id="23082-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="23082-171">Boolean</span></span>|<span data-ttu-id="23082-172">コンテンツファイルがメインコンテンツファイルの依存関係であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="23082-172">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23082-173">関係</span><span class="sxs-lookup"><span data-stu-id="23082-173">Relationships</span></span>
<span data-ttu-id="23082-174">なし</span><span class="sxs-lookup"><span data-stu-id="23082-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23082-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23082-175">JSON Representation</span></span>
<span data-ttu-id="23082-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="23082-176">Here is a JSON representation of the resource.</span></span>
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




