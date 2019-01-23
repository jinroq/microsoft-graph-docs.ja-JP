---
title: mobileAppContentFile リソース タイプ
description: 特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e9f28ea036bbe73fae8e9e59d8d63ea8916f15d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425681"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="0e124-103">mobileAppContentFile リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="0e124-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="0e124-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0e124-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0e124-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e124-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e124-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e124-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e124-107">特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0e124-107">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>

## <a name="methods"></a><span data-ttu-id="0e124-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e124-108">Methods</span></span>
|<span data-ttu-id="0e124-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e124-109">Method</span></span>|<span data-ttu-id="0e124-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0e124-110">Return Type</span></span>|<span data-ttu-id="0e124-111">説明</span><span class="sxs-lookup"><span data-stu-id="0e124-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e124-112">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="0e124-112">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="0e124-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0e124-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="0e124-114">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0e124-114">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="0e124-115">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0e124-115">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="0e124-116">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0e124-116">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="0e124-117">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0e124-117">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="0e124-118">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0e124-118">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="0e124-119">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0e124-119">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="0e124-120">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0e124-120">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="0e124-121">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0e124-121">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="0e124-122">なし</span><span class="sxs-lookup"><span data-stu-id="0e124-122">None</span></span>|<span data-ttu-id="0e124-123">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="0e124-123">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="0e124-124">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0e124-124">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="0e124-125">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0e124-125">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="0e124-126">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0e124-126">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="0e124-127">commit action</span><span class="sxs-lookup"><span data-stu-id="0e124-127">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="0e124-128">なし</span><span class="sxs-lookup"><span data-stu-id="0e124-128">None</span></span>|<span data-ttu-id="0e124-129">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="0e124-129">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="0e124-130">renewUpload action</span><span class="sxs-lookup"><span data-stu-id="0e124-130">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="0e124-131">なし</span><span class="sxs-lookup"><span data-stu-id="0e124-131">None</span></span>|<span data-ttu-id="0e124-132">アプリケーション ファイルのアップロード用の SAS URI を更新します。</span><span class="sxs-lookup"><span data-stu-id="0e124-132">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e124-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e124-133">Properties</span></span>
|<span data-ttu-id="0e124-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e124-134">Property</span></span>|<span data-ttu-id="0e124-135">型</span><span class="sxs-lookup"><span data-stu-id="0e124-135">Type</span></span>|<span data-ttu-id="0e124-136">説明</span><span class="sxs-lookup"><span data-stu-id="0e124-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e124-137">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="0e124-137">azureStorageUri</span></span>|<span data-ttu-id="0e124-138">String</span><span class="sxs-lookup"><span data-stu-id="0e124-138">String</span></span>|<span data-ttu-id="0e124-139">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="0e124-139">The Azure Storage URI.</span></span>|
|<span data-ttu-id="0e124-140">isCommitted</span><span class="sxs-lookup"><span data-stu-id="0e124-140">isCommitted</span></span>|<span data-ttu-id="0e124-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e124-141">Boolean</span></span>|<span data-ttu-id="0e124-142">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0e124-142">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="0e124-143">id</span><span class="sxs-lookup"><span data-stu-id="0e124-143">id</span></span>|<span data-ttu-id="0e124-144">String</span><span class="sxs-lookup"><span data-stu-id="0e124-144">String</span></span>|<span data-ttu-id="0e124-145">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="0e124-145">The File Id.</span></span>|
|<span data-ttu-id="0e124-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e124-146">createdDateTime</span></span>|<span data-ttu-id="0e124-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e124-147">DateTimeOffset</span></span>|<span data-ttu-id="0e124-148">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="0e124-148">The time the file was created.</span></span>|
|<span data-ttu-id="0e124-149">name</span><span class="sxs-lookup"><span data-stu-id="0e124-149">name</span></span>|<span data-ttu-id="0e124-150">String</span><span class="sxs-lookup"><span data-stu-id="0e124-150">String</span></span>|<span data-ttu-id="0e124-151">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="0e124-151">the file name.</span></span>|
|<span data-ttu-id="0e124-152">size</span><span class="sxs-lookup"><span data-stu-id="0e124-152">size</span></span>|<span data-ttu-id="0e124-153">Int64</span><span class="sxs-lookup"><span data-stu-id="0e124-153">Int64</span></span>|<span data-ttu-id="0e124-154">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="0e124-154">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="0e124-155">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="0e124-155">sizeEncrypted</span></span>|<span data-ttu-id="0e124-156">Int64</span><span class="sxs-lookup"><span data-stu-id="0e124-156">Int64</span></span>|<span data-ttu-id="0e124-157">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="0e124-157">The size of the file after encryption.</span></span>|
|<span data-ttu-id="0e124-158">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0e124-158">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="0e124-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e124-159">DateTimeOffset</span></span>|<span data-ttu-id="0e124-160">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="0e124-160">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="0e124-161">manifest</span><span class="sxs-lookup"><span data-stu-id="0e124-161">manifest</span></span>|<span data-ttu-id="0e124-162">Binary</span><span class="sxs-lookup"><span data-stu-id="0e124-162">Binary</span></span>|<span data-ttu-id="0e124-163">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="0e124-163">The manifest information.</span></span>|
|<span data-ttu-id="0e124-164">uploadState</span><span class="sxs-lookup"><span data-stu-id="0e124-164">uploadState</span></span>|[<span data-ttu-id="0e124-165">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="0e124-165">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="0e124-166">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="0e124-166">The state of the current upload request.</span></span> <span data-ttu-id="0e124-167">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="0e124-167">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="0e124-168">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="0e124-168">isFrameworkFile</span></span>|<span data-ttu-id="0e124-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e124-169">Boolean</span></span>|<span data-ttu-id="0e124-170">フレームワーク ファイルのファイルかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="0e124-170">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="0e124-171">isDependency</span><span class="sxs-lookup"><span data-stu-id="0e124-171">isDependency</span></span>|<span data-ttu-id="0e124-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e124-172">Boolean</span></span>|<span data-ttu-id="0e124-173">かどうか、コンテンツ ファイルは、メインのコンテンツ ファイルの依存関係です。</span><span class="sxs-lookup"><span data-stu-id="0e124-173">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e124-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e124-174">Relationships</span></span>
<span data-ttu-id="0e124-175">なし</span><span class="sxs-lookup"><span data-stu-id="0e124-175">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e124-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e124-176">JSON Representation</span></span>
<span data-ttu-id="0e124-177">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e124-177">Here is a JSON representation of the resource.</span></span>
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




