---
title: mobileAppContentFile リソース タイプ
description: 特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 3ab62a5aa49062209fb18add293344fe68730c66
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337185"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="76ca8-103">mobileAppContentFile リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="76ca8-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="76ca8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="76ca8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76ca8-105">特定の mobileAppContent バージョンに関連付けられている単一のインストーラー ファイルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="76ca8-105">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>
## <a name="methods"></a><span data-ttu-id="76ca8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="76ca8-106">Methods</span></span>
|<span data-ttu-id="76ca8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="76ca8-107">Method</span></span>|<span data-ttu-id="76ca8-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="76ca8-108">Return Type</span></span>|<span data-ttu-id="76ca8-109">説明</span><span class="sxs-lookup"><span data-stu-id="76ca8-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76ca8-110">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="76ca8-110">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="76ca8-111">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="76ca8-111">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="76ca8-112">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="76ca8-112">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="76ca8-113">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="76ca8-113">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="76ca8-114">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="76ca8-114">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="76ca8-115">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="76ca8-115">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="76ca8-116">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="76ca8-116">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="76ca8-117">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="76ca8-117">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="76ca8-118">新しい [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="76ca8-118">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="76ca8-119">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="76ca8-119">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="76ca8-120">なし</span><span class="sxs-lookup"><span data-stu-id="76ca8-120">None</span></span>|<span data-ttu-id="76ca8-121">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="76ca8-121">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="76ca8-122">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="76ca8-122">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="76ca8-123">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="76ca8-123">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="76ca8-124">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="76ca8-124">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="76ca8-125">commit action</span><span class="sxs-lookup"><span data-stu-id="76ca8-125">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="76ca8-126">なし</span><span class="sxs-lookup"><span data-stu-id="76ca8-126">None</span></span>|<span data-ttu-id="76ca8-127">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="76ca8-127">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="76ca8-128">renewUpload action</span><span class="sxs-lookup"><span data-stu-id="76ca8-128">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="76ca8-129">なし</span><span class="sxs-lookup"><span data-stu-id="76ca8-129">None</span></span>|<span data-ttu-id="76ca8-130">アプリケーション ファイルのアップロード用の SAS URI を更新します。</span><span class="sxs-lookup"><span data-stu-id="76ca8-130">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="76ca8-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76ca8-131">Properties</span></span>
|<span data-ttu-id="76ca8-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76ca8-132">Property</span></span>|<span data-ttu-id="76ca8-133">種類</span><span class="sxs-lookup"><span data-stu-id="76ca8-133">Type</span></span>|<span data-ttu-id="76ca8-134">説明</span><span class="sxs-lookup"><span data-stu-id="76ca8-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76ca8-135">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="76ca8-135">azureStorageUri</span></span>|<span data-ttu-id="76ca8-136">String</span><span class="sxs-lookup"><span data-stu-id="76ca8-136">String</span></span>|<span data-ttu-id="76ca8-137">Azure ストレージ URI。</span><span class="sxs-lookup"><span data-stu-id="76ca8-137">The Azure Storage URI.</span></span>|
|<span data-ttu-id="76ca8-138">isCommitted</span><span class="sxs-lookup"><span data-stu-id="76ca8-138">isCommitted</span></span>|<span data-ttu-id="76ca8-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="76ca8-139">Boolean</span></span>|<span data-ttu-id="76ca8-140">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="76ca8-140">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="76ca8-141">id</span><span class="sxs-lookup"><span data-stu-id="76ca8-141">id</span></span>|<span data-ttu-id="76ca8-142">String</span><span class="sxs-lookup"><span data-stu-id="76ca8-142">String</span></span>|<span data-ttu-id="76ca8-143">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="76ca8-143">The File Id.</span></span>|
|<span data-ttu-id="76ca8-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76ca8-144">createdDateTime</span></span>|<span data-ttu-id="76ca8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76ca8-145">DateTimeOffset</span></span>|<span data-ttu-id="76ca8-146">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="76ca8-146">The time the file was created.</span></span>|
|<span data-ttu-id="76ca8-147">name</span><span class="sxs-lookup"><span data-stu-id="76ca8-147">name</span></span>|<span data-ttu-id="76ca8-148">String</span><span class="sxs-lookup"><span data-stu-id="76ca8-148">String</span></span>|<span data-ttu-id="76ca8-149">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="76ca8-149">the file name.</span></span>|
|<span data-ttu-id="76ca8-150">size</span><span class="sxs-lookup"><span data-stu-id="76ca8-150">size</span></span>|<span data-ttu-id="76ca8-151">Int64</span><span class="sxs-lookup"><span data-stu-id="76ca8-151">Int64</span></span>|<span data-ttu-id="76ca8-152">暗号化する前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="76ca8-152">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="76ca8-153">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="76ca8-153">sizeEncrypted</span></span>|<span data-ttu-id="76ca8-154">Int64</span><span class="sxs-lookup"><span data-stu-id="76ca8-154">Int64</span></span>|<span data-ttu-id="76ca8-155">暗号化した後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="76ca8-155">The size of the file after encryption.</span></span>|
|<span data-ttu-id="76ca8-156">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="76ca8-156">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="76ca8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76ca8-157">DateTimeOffset</span></span>|<span data-ttu-id="76ca8-158">Azure ストレージ URI の有効期限が切れる時刻。</span><span class="sxs-lookup"><span data-stu-id="76ca8-158">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="76ca8-159">manifest</span><span class="sxs-lookup"><span data-stu-id="76ca8-159">manifest</span></span>|<span data-ttu-id="76ca8-160">Binary</span><span class="sxs-lookup"><span data-stu-id="76ca8-160">Binary</span></span>|<span data-ttu-id="76ca8-161">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="76ca8-161">The manifest information.</span></span>|
|<span data-ttu-id="76ca8-162">uploadState</span><span class="sxs-lookup"><span data-stu-id="76ca8-162">uploadState</span></span>|[<span data-ttu-id="76ca8-163">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="76ca8-163">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="76ca8-164">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="76ca8-164">The state of the current upload request.</span></span> <span data-ttu-id="76ca8-165">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="76ca8-165">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76ca8-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="76ca8-166">Relationships</span></span>
<span data-ttu-id="76ca8-167">なし</span><span class="sxs-lookup"><span data-stu-id="76ca8-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="76ca8-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76ca8-168">JSON Representation</span></span>
<span data-ttu-id="76ca8-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76ca8-169">Here is a JSON representation of the resource.</span></span>
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



