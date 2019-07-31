---
title: mobileAppContentFile リソース タイプ
description: 特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dfefbf506adfcccf750077e6997ad14524564659
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012465"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="c83c8-103">mobileAppContentFile リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c83c8-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="c83c8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c83c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c83c8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c83c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c83c8-106">特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c83c8-106">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>

## <a name="methods"></a><span data-ttu-id="c83c8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c83c8-107">Methods</span></span>
|<span data-ttu-id="c83c8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c83c8-108">Method</span></span>|<span data-ttu-id="c83c8-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c83c8-109">Return Type</span></span>|<span data-ttu-id="c83c8-110">説明</span><span class="sxs-lookup"><span data-stu-id="c83c8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c83c8-111">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="c83c8-111">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="c83c8-112">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c83c8-112">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="c83c8-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c83c8-113">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="c83c8-114">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c83c8-114">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="c83c8-115">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c83c8-115">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="c83c8-116">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c83c8-116">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="c83c8-117">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c83c8-117">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="c83c8-118">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c83c8-118">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="c83c8-119">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c83c8-119">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="c83c8-120">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c83c8-120">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="c83c8-121">None</span><span class="sxs-lookup"><span data-stu-id="c83c8-121">None</span></span>|<span data-ttu-id="c83c8-122">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c83c8-122">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="c83c8-123">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c83c8-123">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="c83c8-124">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c83c8-124">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="c83c8-125">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c83c8-125">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="c83c8-126">commit action</span><span class="sxs-lookup"><span data-stu-id="c83c8-126">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="c83c8-127">None</span><span class="sxs-lookup"><span data-stu-id="c83c8-127">None</span></span>|<span data-ttu-id="c83c8-128">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="c83c8-128">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="c83c8-129">renewUpload action</span><span class="sxs-lookup"><span data-stu-id="c83c8-129">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="c83c8-130">なし</span><span class="sxs-lookup"><span data-stu-id="c83c8-130">None</span></span>|<span data-ttu-id="c83c8-131">アプリケーション ファイルのアップロード用の SAS URI を更新します。</span><span class="sxs-lookup"><span data-stu-id="c83c8-131">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="c83c8-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c83c8-132">Properties</span></span>
|<span data-ttu-id="c83c8-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c83c8-133">Property</span></span>|<span data-ttu-id="c83c8-134">型</span><span class="sxs-lookup"><span data-stu-id="c83c8-134">Type</span></span>|<span data-ttu-id="c83c8-135">説明</span><span class="sxs-lookup"><span data-stu-id="c83c8-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c83c8-136">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="c83c8-136">azureStorageUri</span></span>|<span data-ttu-id="c83c8-137">String</span><span class="sxs-lookup"><span data-stu-id="c83c8-137">String</span></span>|<span data-ttu-id="c83c8-138">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="c83c8-138">The Azure Storage URI.</span></span>|
|<span data-ttu-id="c83c8-139">isCommitted</span><span class="sxs-lookup"><span data-stu-id="c83c8-139">isCommitted</span></span>|<span data-ttu-id="c83c8-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c83c8-140">Boolean</span></span>|<span data-ttu-id="c83c8-141">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c83c8-141">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="c83c8-142">id</span><span class="sxs-lookup"><span data-stu-id="c83c8-142">id</span></span>|<span data-ttu-id="c83c8-143">文字列</span><span class="sxs-lookup"><span data-stu-id="c83c8-143">String</span></span>|<span data-ttu-id="c83c8-144">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="c83c8-144">The File Id.</span></span>|
|<span data-ttu-id="c83c8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c83c8-145">createdDateTime</span></span>|<span data-ttu-id="c83c8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c83c8-146">DateTimeOffset</span></span>|<span data-ttu-id="c83c8-147">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="c83c8-147">The time the file was created.</span></span>|
|<span data-ttu-id="c83c8-148">name</span><span class="sxs-lookup"><span data-stu-id="c83c8-148">name</span></span>|<span data-ttu-id="c83c8-149">String</span><span class="sxs-lookup"><span data-stu-id="c83c8-149">String</span></span>|<span data-ttu-id="c83c8-150">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="c83c8-150">the file name.</span></span>|
|<span data-ttu-id="c83c8-151">size</span><span class="sxs-lookup"><span data-stu-id="c83c8-151">size</span></span>|<span data-ttu-id="c83c8-152">Int64</span><span class="sxs-lookup"><span data-stu-id="c83c8-152">Int64</span></span>|<span data-ttu-id="c83c8-153">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="c83c8-153">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="c83c8-154">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="c83c8-154">sizeEncrypted</span></span>|<span data-ttu-id="c83c8-155">Int64</span><span class="sxs-lookup"><span data-stu-id="c83c8-155">Int64</span></span>|<span data-ttu-id="c83c8-156">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="c83c8-156">The size of the file after encryption.</span></span>|
|<span data-ttu-id="c83c8-157">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c83c8-157">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="c83c8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c83c8-158">DateTimeOffset</span></span>|<span data-ttu-id="c83c8-159">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="c83c8-159">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="c83c8-160">manifest</span><span class="sxs-lookup"><span data-stu-id="c83c8-160">manifest</span></span>|<span data-ttu-id="c83c8-161">Binary</span><span class="sxs-lookup"><span data-stu-id="c83c8-161">Binary</span></span>|<span data-ttu-id="c83c8-162">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="c83c8-162">The manifest information.</span></span>|
|<span data-ttu-id="c83c8-163">uploadState</span><span class="sxs-lookup"><span data-stu-id="c83c8-163">uploadState</span></span>|[<span data-ttu-id="c83c8-164">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="c83c8-164">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="c83c8-165">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="c83c8-165">The state of the current upload request.</span></span> <span data-ttu-id="c83c8-166">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="c83c8-166">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="c83c8-167">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="c83c8-167">isFrameworkFile</span></span>|<span data-ttu-id="c83c8-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="c83c8-168">Boolean</span></span>|<span data-ttu-id="c83c8-169">ファイルがフレームワークファイルであるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c83c8-169">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="c83c8-170">isDependency</span><span class="sxs-lookup"><span data-stu-id="c83c8-170">isDependency</span></span>|<span data-ttu-id="c83c8-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="c83c8-171">Boolean</span></span>|<span data-ttu-id="c83c8-172">コンテンツファイルがメインコンテンツファイルの依存関係であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c83c8-172">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c83c8-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c83c8-173">Relationships</span></span>
<span data-ttu-id="c83c8-174">なし</span><span class="sxs-lookup"><span data-stu-id="c83c8-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c83c8-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c83c8-175">JSON Representation</span></span>
<span data-ttu-id="c83c8-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c83c8-176">Here is a JSON representation of the resource.</span></span>
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





