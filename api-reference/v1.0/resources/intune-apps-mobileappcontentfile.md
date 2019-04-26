---
title: mobileAppContentFile リソース タイプ
description: 特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8edeebdc3df12d3e1a458ae57e805052e47e3d8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557881"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="cc4e1-103">mobileAppContentFile リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="cc4e1-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="cc4e1-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc4e1-105">特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-105">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>

## <a name="methods"></a><span data-ttu-id="cc4e1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc4e1-106">Methods</span></span>
|<span data-ttu-id="cc4e1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc4e1-107">Method</span></span>|<span data-ttu-id="cc4e1-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cc4e1-108">Return Type</span></span>|<span data-ttu-id="cc4e1-109">説明</span><span class="sxs-lookup"><span data-stu-id="cc4e1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc4e1-110">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="cc4e1-110">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="cc4e1-111">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cc4e1-111">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="cc4e1-112">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-112">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="cc4e1-113">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cc4e1-113">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="cc4e1-114">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cc4e1-114">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="cc4e1-115">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-115">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="cc4e1-116">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cc4e1-116">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="cc4e1-117">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cc4e1-117">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="cc4e1-118">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-118">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="cc4e1-119">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cc4e1-119">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="cc4e1-120">なし</span><span class="sxs-lookup"><span data-stu-id="cc4e1-120">None</span></span>|<span data-ttu-id="cc4e1-121">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-121">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="cc4e1-122">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cc4e1-122">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="cc4e1-123">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cc4e1-123">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="cc4e1-124">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-124">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="cc4e1-125">commit action</span><span class="sxs-lookup"><span data-stu-id="cc4e1-125">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="cc4e1-126">なし</span><span class="sxs-lookup"><span data-stu-id="cc4e1-126">None</span></span>|<span data-ttu-id="cc4e1-127">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-127">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="cc4e1-128">renewUpload action</span><span class="sxs-lookup"><span data-stu-id="cc4e1-128">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="cc4e1-129">なし</span><span class="sxs-lookup"><span data-stu-id="cc4e1-129">None</span></span>|<span data-ttu-id="cc4e1-130">アプリケーション ファイルのアップロード用の SAS URI を更新します。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-130">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc4e1-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc4e1-131">Properties</span></span>
|<span data-ttu-id="cc4e1-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc4e1-132">Property</span></span>|<span data-ttu-id="cc4e1-133">型</span><span class="sxs-lookup"><span data-stu-id="cc4e1-133">Type</span></span>|<span data-ttu-id="cc4e1-134">説明</span><span class="sxs-lookup"><span data-stu-id="cc4e1-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc4e1-135">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="cc4e1-135">azureStorageUri</span></span>|<span data-ttu-id="cc4e1-136">String</span><span class="sxs-lookup"><span data-stu-id="cc4e1-136">String</span></span>|<span data-ttu-id="cc4e1-137">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-137">The Azure Storage URI.</span></span>|
|<span data-ttu-id="cc4e1-138">isCommitted</span><span class="sxs-lookup"><span data-stu-id="cc4e1-138">isCommitted</span></span>|<span data-ttu-id="cc4e1-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc4e1-139">Boolean</span></span>|<span data-ttu-id="cc4e1-140">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-140">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="cc4e1-141">id</span><span class="sxs-lookup"><span data-stu-id="cc4e1-141">id</span></span>|<span data-ttu-id="cc4e1-142">String</span><span class="sxs-lookup"><span data-stu-id="cc4e1-142">String</span></span>|<span data-ttu-id="cc4e1-143">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-143">The File Id.</span></span>|
|<span data-ttu-id="cc4e1-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc4e1-144">createdDateTime</span></span>|<span data-ttu-id="cc4e1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc4e1-145">DateTimeOffset</span></span>|<span data-ttu-id="cc4e1-146">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-146">The time the file was created.</span></span>|
|<span data-ttu-id="cc4e1-147">name</span><span class="sxs-lookup"><span data-stu-id="cc4e1-147">name</span></span>|<span data-ttu-id="cc4e1-148">String</span><span class="sxs-lookup"><span data-stu-id="cc4e1-148">String</span></span>|<span data-ttu-id="cc4e1-149">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-149">the file name.</span></span>|
|<span data-ttu-id="cc4e1-150">size</span><span class="sxs-lookup"><span data-stu-id="cc4e1-150">size</span></span>|<span data-ttu-id="cc4e1-151">Int64</span><span class="sxs-lookup"><span data-stu-id="cc4e1-151">Int64</span></span>|<span data-ttu-id="cc4e1-152">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-152">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="cc4e1-153">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="cc4e1-153">sizeEncrypted</span></span>|<span data-ttu-id="cc4e1-154">Int64</span><span class="sxs-lookup"><span data-stu-id="cc4e1-154">Int64</span></span>|<span data-ttu-id="cc4e1-155">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-155">The size of the file after encryption.</span></span>|
|<span data-ttu-id="cc4e1-156">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cc4e1-156">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="cc4e1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc4e1-157">DateTimeOffset</span></span>|<span data-ttu-id="cc4e1-158">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-158">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="cc4e1-159">manifest</span><span class="sxs-lookup"><span data-stu-id="cc4e1-159">manifest</span></span>|<span data-ttu-id="cc4e1-160">Binary</span><span class="sxs-lookup"><span data-stu-id="cc4e1-160">Binary</span></span>|<span data-ttu-id="cc4e1-161">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-161">The manifest information.</span></span>|
|<span data-ttu-id="cc4e1-162">uploadState</span><span class="sxs-lookup"><span data-stu-id="cc4e1-162">uploadState</span></span>|[<span data-ttu-id="cc4e1-163">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="cc4e1-163">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="cc4e1-164">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-164">The state of the current upload request.</span></span> <span data-ttu-id="cc4e1-165">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-165">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc4e1-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc4e1-166">Relationships</span></span>
<span data-ttu-id="cc4e1-167">なし</span><span class="sxs-lookup"><span data-stu-id="cc4e1-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc4e1-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc4e1-168">JSON Representation</span></span>
<span data-ttu-id="cc4e1-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc4e1-169">Here is a JSON representation of the resource.</span></span>
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
  "uploadState": "String"
}
```



