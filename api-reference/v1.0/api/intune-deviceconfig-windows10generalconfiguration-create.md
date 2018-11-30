---
title: Create windows10GeneralConfiguration
description: 新しい windows10GeneralConfiguration オブジェクトを作成します。
ms.openlocfilehash: a727bb9da70b78e6e6c43957364e585c1b2b6f3a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023821"
---
# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="7b291-103">Create windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b291-103">Create windows10GeneralConfiguration</span></span>

> <span data-ttu-id="7b291-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b291-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b291-105">新しい [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7b291-105">Create a new [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b291-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7b291-106">Prerequisites</span></span>
<span data-ttu-id="7b291-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b291-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b291-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b291-109">Permission type</span></span>|<span data-ttu-id="7b291-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b291-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b291-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b291-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b291-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b291-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b291-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b291-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b291-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b291-114">Not supported.</span></span>|
|<span data-ttu-id="7b291-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b291-115">Application</span></span>|<span data-ttu-id="7b291-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b291-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b291-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b291-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7b291-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b291-118">Request headers</span></span>
|<span data-ttu-id="7b291-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b291-119">Header</span></span>|<span data-ttu-id="7b291-120">値</span><span class="sxs-lookup"><span data-stu-id="7b291-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b291-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b291-121">Authorization</span></span>|<span data-ttu-id="7b291-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7b291-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b291-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7b291-123">Accept</span></span>|<span data-ttu-id="7b291-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7b291-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b291-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b291-125">Request body</span></span>
<span data-ttu-id="7b291-126">要求本文で、windows10GeneralConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-126">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="7b291-127">次の表に、windows10GeneralConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-127">The following table shows the properties that are required when you create the windows10GeneralConfiguration.</span></span>

|<span data-ttu-id="7b291-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b291-128">Property</span></span>|<span data-ttu-id="7b291-129">型</span><span class="sxs-lookup"><span data-stu-id="7b291-129">Type</span></span>|<span data-ttu-id="7b291-130">説明</span><span class="sxs-lookup"><span data-stu-id="7b291-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b291-131">id</span><span class="sxs-lookup"><span data-stu-id="7b291-131">id</span></span>|<span data-ttu-id="7b291-132">String</span><span class="sxs-lookup"><span data-stu-id="7b291-132">String</span></span>|<span data-ttu-id="7b291-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7b291-133">Key of the entity.</span></span> <span data-ttu-id="7b291-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b291-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b291-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b291-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7b291-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b291-136">DateTimeOffset</span></span>|<span data-ttu-id="7b291-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7b291-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7b291-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b291-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b291-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b291-139">createdDateTime</span></span>|<span data-ttu-id="7b291-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b291-140">DateTimeOffset</span></span>|<span data-ttu-id="7b291-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7b291-141">DateTime the object was created.</span></span> <span data-ttu-id="7b291-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b291-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b291-143">説明</span><span class="sxs-lookup"><span data-stu-id="7b291-143">description</span></span>|<span data-ttu-id="7b291-144">String</span><span class="sxs-lookup"><span data-stu-id="7b291-144">String</span></span>|<span data-ttu-id="7b291-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7b291-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b291-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b291-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b291-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7b291-147">displayName</span></span>|<span data-ttu-id="7b291-148">String</span><span class="sxs-lookup"><span data-stu-id="7b291-148">String</span></span>|<span data-ttu-id="7b291-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7b291-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b291-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b291-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b291-151">version</span><span class="sxs-lookup"><span data-stu-id="7b291-151">version</span></span>|<span data-ttu-id="7b291-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-152">Int32</span></span>|<span data-ttu-id="7b291-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7b291-153">Version of the device configuration.</span></span> <span data-ttu-id="7b291-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b291-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b291-155">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="7b291-155">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="7b291-156">String</span><span class="sxs-lookup"><span data-stu-id="7b291-156">String</span></span>|<span data-ttu-id="7b291-157">クラウド プリンターを検出するエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="7b291-157">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="7b291-158">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="7b291-158">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="7b291-159">String</span><span class="sxs-lookup"><span data-stu-id="7b291-159">String</span></span>|<span data-ttu-id="7b291-160">OAuth トークンを取得するための認証エンドポイント。</span><span class="sxs-lookup"><span data-stu-id="7b291-160">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="7b291-161">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b291-161">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="7b291-162">String</span><span class="sxs-lookup"><span data-stu-id="7b291-162">String</span></span>|<span data-ttu-id="7b291-163">OAuth 認証機関から OAuth トークンを取得することを承認されているクライアント アプリケーションの GUID。</span><span class="sxs-lookup"><span data-stu-id="7b291-163">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="7b291-164">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b291-164">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="7b291-165">String</span><span class="sxs-lookup"><span data-stu-id="7b291-165">String</span></span>|<span data-ttu-id="7b291-166">Azure Portal で構成されている印刷サービスの OAuth リソース URI。</span><span class="sxs-lookup"><span data-stu-id="7b291-166">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="7b291-167">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="7b291-167">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="7b291-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-168">Int32</span></span>|<span data-ttu-id="7b291-169">検出エンドポイントからクエリを実行する必要があるプリンターの最大数。</span><span class="sxs-lookup"><span data-stu-id="7b291-169">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="7b291-170">これはモバイルのみでの設定です。</span><span class="sxs-lookup"><span data-stu-id="7b291-170">This is a mobile only setting.</span></span> <span data-ttu-id="7b291-171">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-171">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="7b291-172">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b291-172">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="7b291-173">String</span><span class="sxs-lookup"><span data-stu-id="7b291-173">String</span></span>|<span data-ttu-id="7b291-174">Azure Portal で構成されているプリンター検出サービスの OAuth リソース URI。</span><span class="sxs-lookup"><span data-stu-id="7b291-174">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="7b291-175">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="7b291-175">searchBlockDiacritics</span></span>|<span data-ttu-id="7b291-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-176">Boolean</span></span>|<span data-ttu-id="7b291-177">検索で分音記号を使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-177">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="7b291-178">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="7b291-178">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="7b291-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-179">Boolean</span></span>|<span data-ttu-id="7b291-180">コンテンツとプロパティのインデックスを作成するときに、自動言語検出を使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-180">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="7b291-181">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="7b291-181">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="7b291-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-182">Boolean</span></span>|<span data-ttu-id="7b291-183">Cortana またはエクスプローラーの検索結果に表示されないようにするため、WIP で保護されているアイテムのインデックス作成を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-183">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="7b291-184">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="7b291-184">searchEnableRemoteQueries</span></span>|<span data-ttu-id="7b291-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-185">Boolean</span></span>|<span data-ttu-id="7b291-186">このコンピューターのインデックスに対するリモート クエリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-186">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="7b291-187">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="7b291-187">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="7b291-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-188">Boolean</span></span>|<span data-ttu-id="7b291-189">インデクサー バックオフの検索機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-189">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="7b291-190">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="7b291-190">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="7b291-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-191">Boolean</span></span>|<span data-ttu-id="7b291-192">リムーバブル ドライブ上の場所をライブラリに追加してインデックスを作成することをユーザーに許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-192">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="7b291-193">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="7b291-193">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="7b291-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-194">Boolean</span></span>|<span data-ttu-id="7b291-195">インデックスの場所と同じドライブ上のハード ドライブ領域の最小値を指定して、その最小値を下回ったらインデックス作成を停止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-195">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="7b291-196">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="7b291-196">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="7b291-197">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="7b291-197">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="7b291-198">診断データと利用統計情報データ (Watson など) の送信をデバイスに許可する値を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-198">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="7b291-199">可能な値は、`userDefined`、`none`、`basic`、`enhanced`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-199">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="7b291-200">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="7b291-200">oneDriveDisableFileSync</span></span>|<span data-ttu-id="7b291-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-201">Boolean</span></span>|<span data-ttu-id="7b291-202">アプリや機能から OneDrive 上のファイルを操作することを IT 管理者が禁止できるかどうかを示す値を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-202">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="7b291-203">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="7b291-203">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="7b291-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-204">Boolean</span></span>|<span data-ttu-id="7b291-205">ユーザーがストア以外の場所からアプリをインストールできるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="7b291-205">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="7b291-206">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="7b291-206">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="7b291-207">String</span><span class="sxs-lookup"><span data-stu-id="7b291-207">String</span></span>|<span data-ttu-id="7b291-208">ダウンロードしてデスクトップ画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはデスクトップ画像として使用する必要があるファイル システム上のローカル画像のファイル URL。</span><span class="sxs-lookup"><span data-stu-id="7b291-208">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="7b291-209">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="7b291-209">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="7b291-210">String</span><span class="sxs-lookup"><span data-stu-id="7b291-210">String</span></span>|<span data-ttu-id="7b291-211">ダウンロードしてロック画面画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはロック画面画像として使用する必要があるファイル システム上のローカル画像のファイル URL。</span><span class="sxs-lookup"><span data-stu-id="7b291-211">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="7b291-212">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="7b291-212">bluetoothAllowedServices</span></span>|<span data-ttu-id="7b291-213">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7b291-213">String collection</span></span>|<span data-ttu-id="7b291-214">許可されている Bluetooth サービスおよびプロファイルの一覧を 16 進形式の文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-214">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="7b291-215">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="7b291-215">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="7b291-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-216">Boolean</span></span>|<span data-ttu-id="7b291-217">ユーザーが Bluetooth 広告を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-217">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="7b291-218">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="7b291-218">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="7b291-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-219">Boolean</span></span>|<span data-ttu-id="7b291-220">ユーザーが Bluetooth の発見可能モードを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-220">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="7b291-221">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="7b291-221">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="7b291-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-222">Boolean</span></span>|<span data-ttu-id="7b291-223">バンドルされた特定のいくつかの Bluetooth 周辺機器を自動的にホスト デバイスとペアにすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-223">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="7b291-224">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="7b291-224">edgeBlockAutofill</span></span>|<span data-ttu-id="7b291-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-225">Boolean</span></span>|<span data-ttu-id="7b291-226">自動入力を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-226">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="7b291-227">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-227">edgeBlocked</span></span>|<span data-ttu-id="7b291-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-228">Boolean</span></span>|<span data-ttu-id="7b291-229">ユーザーが Edge ブラウザーを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-229">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="7b291-230">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="7b291-230">edgeCookiePolicy</span></span>|[<span data-ttu-id="7b291-231">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="7b291-231">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="7b291-232">Edge ブラウザーでどの Cookie を禁止するかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-232">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="7b291-233">可能な値は、`userDefined`、`allow`、`blockThirdParty`、`blockAll` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-233">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="7b291-234">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="7b291-234">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="7b291-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-235">Boolean</span></span>|<span data-ttu-id="7b291-236">Edge ブラウザー内の開発者ツールを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-236">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="7b291-237">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="7b291-237">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="7b291-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-238">Boolean</span></span>|<span data-ttu-id="7b291-239">ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-239">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="7b291-240">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="7b291-240">edgeBlockExtensions</span></span>|<span data-ttu-id="7b291-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-241">Boolean</span></span>|<span data-ttu-id="7b291-242">Edge ブラウザーの拡張機能を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-242">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="7b291-243">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="7b291-243">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="7b291-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-244">Boolean</span></span>|<span data-ttu-id="7b291-245">Edge ブラウザーで会社のネットワークの InPrivate ブラウズを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-245">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="7b291-246">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="7b291-246">edgeBlockJavaScript</span></span>|<span data-ttu-id="7b291-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-247">Boolean</span></span>|<span data-ttu-id="7b291-248">ユーザーが JavaScript を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-248">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="7b291-249">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="7b291-249">edgeBlockPasswordManager</span></span>|<span data-ttu-id="7b291-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-250">Boolean</span></span>|<span data-ttu-id="7b291-251">パスワード マネージャーを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-251">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="7b291-252">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="7b291-252">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="7b291-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-253">Boolean</span></span>|<span data-ttu-id="7b291-254">Microsoft Edge のアドレス バー ドロップダウン機能を禁止します。</span><span class="sxs-lookup"><span data-stu-id="7b291-254">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="7b291-255">Microsoft Edge から Microsoft サービスへのネットワーク接続を最小限に抑えるには、この設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="7b291-255">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="7b291-256">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="7b291-256">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="7b291-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-257">Boolean</span></span>|<span data-ttu-id="7b291-258">Microsoft Edge での Microsoft 互換性リストを禁止します。</span><span class="sxs-lookup"><span data-stu-id="7b291-258">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="7b291-259">Microsoft ではこのリストを利用して、既知の互換性の問題があるサイトを Edge で正しく表示できるようにします。</span><span class="sxs-lookup"><span data-stu-id="7b291-259">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="7b291-260">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="7b291-260">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="7b291-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-261">Boolean</span></span>|<span data-ttu-id="7b291-262">Microsoft Edge の終了時にブラウズ データを消去します。</span><span class="sxs-lookup"><span data-stu-id="7b291-262">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="7b291-263">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="7b291-263">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="7b291-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-264">Boolean</span></span>|<span data-ttu-id="7b291-265">Edge のスタート ページをユーザーが変更することを許可します。</span><span class="sxs-lookup"><span data-stu-id="7b291-265">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="7b291-266">ユーザーが Edge を開いたときに既定で表示されるスタート ページを指定するには、EdgeHomepageUrls を使用します。</span><span class="sxs-lookup"><span data-stu-id="7b291-266">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="7b291-267">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="7b291-267">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="7b291-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-268">Boolean</span></span>|<span data-ttu-id="7b291-269">Microsoft Edge の初回使用時に表示される Microsoft の Web ページを禁止します。</span><span class="sxs-lookup"><span data-stu-id="7b291-269">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="7b291-270">このポリシーでは、ゼロ エミッション構成に登録している企業などが、このページの表示を禁止できます。</span><span class="sxs-lookup"><span data-stu-id="7b291-270">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="7b291-271">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="7b291-271">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="7b291-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-272">Boolean</span></span>|<span data-ttu-id="7b291-273">ユーザーが Microsoft Edge からスタートにサイトをピン留めしたときに、ライブ タイルを作成するために Microsoft が情報を収集することを禁止します。</span><span class="sxs-lookup"><span data-stu-id="7b291-273">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="7b291-274">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="7b291-274">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="7b291-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-275">Boolean</span></span>|<span data-ttu-id="7b291-276">Internet Explorer と Microsoft Edge の間でお気に入りの同期を有効にします。</span><span class="sxs-lookup"><span data-stu-id="7b291-276">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="7b291-277">お気に入りの追加、削除、変更、順序変更が、ブラウザー間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="7b291-277">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="7b291-278">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="7b291-278">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="7b291-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-279">Boolean</span></span>|<span data-ttu-id="7b291-280">ローミング中に携帯電話上でユーザーがデータを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-280">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="7b291-281">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="7b291-281">cellularBlockVpn</span></span>|<span data-ttu-id="7b291-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-282">Boolean</span></span>|<span data-ttu-id="7b291-283">携帯電話上でユーザーが VPN を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-283">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="7b291-284">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="7b291-284">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="7b291-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-285">Boolean</span></span>|<span data-ttu-id="7b291-286">ローミング時に携帯電話上でユーザーが VPN を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-286">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="7b291-287">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="7b291-287">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="7b291-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-288">Boolean</span></span>|<span data-ttu-id="7b291-289">エンド ユーザーが Defender にアクセスすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-289">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="7b291-290">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="7b291-290">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="7b291-291">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-291">Int32</span></span>|<span data-ttu-id="7b291-292">検疫済みのマルウェアを削除するまでの日数。</span><span class="sxs-lookup"><span data-stu-id="7b291-292">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="7b291-293">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-293">Valid values 0 to 90</span></span>|
|<span data-ttu-id="7b291-294">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="7b291-294">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="7b291-295">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="7b291-295">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="7b291-296">検出されたマルウェアに対する Defender のアクションを脅威レベルごとに取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-296">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="7b291-297">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="7b291-297">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="7b291-298">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="7b291-298">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="7b291-299">Defender がシステムをスキャンする曜日。</span><span class="sxs-lookup"><span data-stu-id="7b291-299">Defender day of the week for the system scan.</span></span> <span data-ttu-id="7b291-300">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-300">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="7b291-301">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="7b291-301">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="7b291-302">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7b291-302">String collection</span></span>|<span data-ttu-id="7b291-303">スキャンとリアルタイム保護から除外するファイルとフォルダー。</span><span class="sxs-lookup"><span data-stu-id="7b291-303">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="7b291-304">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="7b291-304">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="7b291-305">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7b291-305">String collection</span></span>|<span data-ttu-id="7b291-306">スキャンとリアルタイム保護から除外するファイル拡張子。</span><span class="sxs-lookup"><span data-stu-id="7b291-306">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="7b291-307">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="7b291-307">defenderScanMaxCpu</span></span>|<span data-ttu-id="7b291-308">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-308">Int32</span></span>|<span data-ttu-id="7b291-309">スキャン中の最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="7b291-309">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="7b291-310">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-310">Valid values 0 to 100</span></span>|
|<span data-ttu-id="7b291-311">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="7b291-311">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="7b291-312">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="7b291-312">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="7b291-313">ファイル アクティビティを監視する値。</span><span class="sxs-lookup"><span data-stu-id="7b291-313">Value for monitoring file activity.</span></span> <span data-ttu-id="7b291-314">可能な値は、`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-314">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="7b291-315">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="7b291-315">defenderProcessesToExclude</span></span>|<span data-ttu-id="7b291-316">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7b291-316">String collection</span></span>|<span data-ttu-id="7b291-317">スキャンとリアルタイム保護から除外するプロセス。</span><span class="sxs-lookup"><span data-stu-id="7b291-317">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="7b291-318">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="7b291-318">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="7b291-319">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="7b291-319">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="7b291-320">ユーザーにサンプルの送信を要求する方法の構成。</span><span class="sxs-lookup"><span data-stu-id="7b291-320">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="7b291-321">可能な値は、`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-321">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="7b291-322">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="7b291-322">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="7b291-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-323">Boolean</span></span>|<span data-ttu-id="7b291-324">動作の監視が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-324">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="7b291-325">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="7b291-325">defenderRequireCloudProtection</span></span>|<span data-ttu-id="7b291-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-326">Boolean</span></span>|<span data-ttu-id="7b291-327">クラウドの保護が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-327">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="7b291-328">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="7b291-328">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="7b291-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-329">Boolean</span></span>|<span data-ttu-id="7b291-330">ネットワーク検査システムが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-330">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="7b291-331">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="7b291-331">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="7b291-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-332">Boolean</span></span>|<span data-ttu-id="7b291-333">リアルタイムの監視が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-333">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="7b291-334">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="7b291-334">defenderScanArchiveFiles</span></span>|<span data-ttu-id="7b291-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-335">Boolean</span></span>|<span data-ttu-id="7b291-336">アーカイブ ファイルをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-336">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="7b291-337">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="7b291-337">defenderScanDownloads</span></span>|<span data-ttu-id="7b291-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-338">Boolean</span></span>|<span data-ttu-id="7b291-339">ダウンロードをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-339">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="7b291-340">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="7b291-340">defenderScanNetworkFiles</span></span>|<span data-ttu-id="7b291-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-341">Boolean</span></span>|<span data-ttu-id="7b291-342">ネットワーク フォルダーから開かれたファイルをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-342">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="7b291-343">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="7b291-343">defenderScanIncomingMail</span></span>|<span data-ttu-id="7b291-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-344">Boolean</span></span>|<span data-ttu-id="7b291-345">受信メール メッセージをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-345">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="7b291-346">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="7b291-346">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="7b291-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-347">Boolean</span></span>|<span data-ttu-id="7b291-348">フル スキャン時に、マップされたネットワーク ドライブをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-348">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="7b291-349">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="7b291-349">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="7b291-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-350">Boolean</span></span>|<span data-ttu-id="7b291-351">フル スキャン時に、リムーバブル ドライブをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-351">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="7b291-352">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="7b291-352">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="7b291-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-353">Boolean</span></span>|<span data-ttu-id="7b291-354">Internet Explorer ブラウザーに読み込まれるスクリプトをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-354">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="7b291-355">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="7b291-355">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="7b291-356">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-356">Int32</span></span>|<span data-ttu-id="7b291-357">署名を更新する間隔 (時間)。</span><span class="sxs-lookup"><span data-stu-id="7b291-357">The signature update interval in hours.</span></span> <span data-ttu-id="7b291-358">確認しない場合は 0 を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-358">Specify 0 not to check.</span></span> <span data-ttu-id="7b291-359">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-359">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7b291-360">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="7b291-360">defenderScanType</span></span>|[<span data-ttu-id="7b291-361">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="7b291-361">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="7b291-362">Defender システム スキャンの種類。</span><span class="sxs-lookup"><span data-stu-id="7b291-362">The defender system scan type.</span></span> <span data-ttu-id="7b291-363">可能な値は、`userDefined`、`disabled`、`quick`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-363">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="7b291-364">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="7b291-364">defenderScheduledScanTime</span></span>|<span data-ttu-id="7b291-365">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7b291-365">TimeOfDay</span></span>|<span data-ttu-id="7b291-366">システムのスキャンの Defender 時刻。</span><span class="sxs-lookup"><span data-stu-id="7b291-366">The defender time for the system scan.</span></span>|
|<span data-ttu-id="7b291-367">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="7b291-367">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="7b291-368">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7b291-368">TimeOfDay</span></span>|<span data-ttu-id="7b291-369">毎日のクイック スキャンを実行する時刻。</span><span class="sxs-lookup"><span data-stu-id="7b291-369">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="7b291-370">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="7b291-370">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="7b291-371">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="7b291-371">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="7b291-372">クラウド配信の保護レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-372">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="7b291-373">可能な値は、`notConfigured`、`high`、`highPlus`、`zeroTolerance` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-373">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="7b291-374">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b291-374">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="7b291-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-375">Boolean</span></span>|<span data-ttu-id="7b291-376">Windows 10 Mobile デバイスのロック画面で、画面のタイムアウトを制御するユーザー構成可能な設定を表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-376">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="7b291-377">このポリシーが [許可] に設定されている場合は、lockScreenTimeoutInSeconds によって設定された値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="7b291-377">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="7b291-378">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="7b291-378">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="7b291-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-379">Boolean</span></span>|<span data-ttu-id="7b291-380">ロック画面上のアクション センター通知を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-380">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="7b291-381">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="7b291-381">lockScreenBlockCortana</span></span>|<span data-ttu-id="7b291-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-382">Boolean</span></span>|<span data-ttu-id="7b291-383">システムのロック中にユーザーが音声認識を使用して Cortana と対話できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-383">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="7b291-384">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="7b291-384">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="7b291-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-385">Boolean</span></span>|<span data-ttu-id="7b291-386">デバイスのロック画面へのトースト通知を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-386">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="7b291-387">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="7b291-387">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="7b291-388">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-388">Int32</span></span>|<span data-ttu-id="7b291-389">Windows 10 Mobile デバイスで画面をロックしてから画面をオフにするまでの時間 (秒) を設定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-389">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="7b291-390">サポートされている値は 11 から 1800 までです。</span><span class="sxs-lookup"><span data-stu-id="7b291-390">Supported values are 11-1800.</span></span> <span data-ttu-id="7b291-391">有効な値は 11 から 1800 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-391">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="7b291-392">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7b291-392">passwordBlockSimple</span></span>|<span data-ttu-id="7b291-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-393">Boolean</span></span>|<span data-ttu-id="7b291-394">"1111" や "1234" などの PIN またはパスワードを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-394">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="7b291-395">Windows 10 デスクトップでは、ピクチャ パスワードの使用も制御します。</span><span class="sxs-lookup"><span data-stu-id="7b291-395">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="7b291-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7b291-396">passwordExpirationDays</span></span>|<span data-ttu-id="7b291-397">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-397">Int32</span></span>|<span data-ttu-id="7b291-398">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="7b291-398">The password expiration in days.</span></span> <span data-ttu-id="7b291-399">有効な値は 0 から 730 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-399">Valid values 0 to 730</span></span>|
|<span data-ttu-id="7b291-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7b291-400">passwordMinimumLength</span></span>|<span data-ttu-id="7b291-401">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-401">Int32</span></span>|<span data-ttu-id="7b291-402">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="7b291-402">The minimum password length.</span></span> <span data-ttu-id="7b291-403">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7b291-404">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7b291-404">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7b291-405">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-405">Int32</span></span>|<span data-ttu-id="7b291-406">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="7b291-406">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7b291-407">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7b291-407">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7b291-408">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-408">Int32</span></span>|<span data-ttu-id="7b291-409">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="7b291-409">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7b291-410">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7b291-410">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7b291-411">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-411">Int32</span></span>|<span data-ttu-id="7b291-412">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="7b291-412">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="7b291-413">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-413">Valid values 0 to 50</span></span>|
|<span data-ttu-id="7b291-414">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7b291-414">passwordRequired</span></span>|<span data-ttu-id="7b291-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-415">Boolean</span></span>|<span data-ttu-id="7b291-416">ユーザーにパスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-416">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="7b291-417">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="7b291-417">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="7b291-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-418">Boolean</span></span>|<span data-ttu-id="7b291-419">アイドル状態からの再開時にパスワードを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-419">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="7b291-420">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7b291-420">passwordRequiredType</span></span>|[<span data-ttu-id="7b291-421">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7b291-421">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7b291-422">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="7b291-422">The required password type.</span></span> <span data-ttu-id="7b291-423">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-423">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7b291-424">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="7b291-424">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="7b291-425">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-425">Int32</span></span>|<span data-ttu-id="7b291-426">出荷時の設定にリセットされるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="7b291-426">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="7b291-427">有効な値は 0 から 999 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-427">Valid values 0 to 999</span></span>|
|<span data-ttu-id="7b291-428">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="7b291-428">privacyAdvertisingId</span></span>|[<span data-ttu-id="7b291-429">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="7b291-429">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="7b291-430">広告識別子の使用を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="7b291-430">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="7b291-431">Windows 10 バージョン 1607 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="7b291-431">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="7b291-432">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-432">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="7b291-433">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="7b291-433">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="7b291-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-434">Boolean</span></span>|<span data-ttu-id="7b291-435">アプリの起動時に、ペアリングとプライバシーに関するユーザーの同意ダイアログの自動受け入れを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-435">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="7b291-436">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="7b291-436">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="7b291-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-437">Boolean</span></span>|<span data-ttu-id="7b291-438">Cortana、音声入力、ストア アプリケーションに対するクラウド ベースの音声サービスの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-438">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="7b291-439">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="7b291-439">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="7b291-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-440">Boolean</span></span>|<span data-ttu-id="7b291-441">ユーザーがタスク バーからアプリのピン留めを外すことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-441">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="7b291-442">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="7b291-442">startMenuAppListVisibility</span></span>|[<span data-ttu-id="7b291-443">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="7b291-443">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="7b291-444">この値を設定すると、アプリ リストを折りたたんだり、アプリ リスト全体を削除したり、設定アプリで対応する切り替えを無効にしたりできます。</span><span class="sxs-lookup"><span data-stu-id="7b291-444">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="7b291-445">可能な値は、`userDefined`、`collapse`、`remove`、`disableSettingsApp` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-445">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="7b291-446">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="7b291-446">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="7b291-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-447">Boolean</span></span>|<span data-ttu-id="7b291-448">このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウント設定の変更] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-448">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="7b291-449">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="7b291-449">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="7b291-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-450">Boolean</span></span>|<span data-ttu-id="7b291-451">このポリシーを有効にすると、よく使われるアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="7b291-451">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="7b291-452">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="7b291-452">startMenuHideHibernate</span></span>|<span data-ttu-id="7b291-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-453">Boolean</span></span>|<span data-ttu-id="7b291-454">このポリシーを有効にすると、スタート メニューの電源ボタンに [休止状態] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-454">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="7b291-455">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="7b291-455">startMenuHideLock</span></span>|<span data-ttu-id="7b291-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-456">Boolean</span></span>|<span data-ttu-id="7b291-457">このポリシーを有効にすると、スタート メニューのユーザー タイルに [ロック] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-457">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="7b291-458">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="7b291-458">startMenuHidePowerButton</span></span>|<span data-ttu-id="7b291-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-459">Boolean</span></span>|<span data-ttu-id="7b291-460">このポリシーを有効にすると、スタート メニューに電源ボタンが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-460">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="7b291-461">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="7b291-461">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="7b291-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-462">Boolean</span></span>|<span data-ttu-id="7b291-463">このポリシーを有効にすると、最近開いた項目のジャンプ リストがスタート メニュー/タスクバーに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="7b291-463">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="7b291-464">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="7b291-464">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="7b291-465">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-465">Boolean</span></span>|<span data-ttu-id="7b291-466">このポリシーを有効にすると、最近追加したアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="7b291-466">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="7b291-467">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="7b291-467">startMenuHideRestartOptions</span></span>|<span data-ttu-id="7b291-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-468">Boolean</span></span>|<span data-ttu-id="7b291-469">このポリシーを有効にすると、スタート メニューの電源ボタンに [再起動]/[更新して再起動] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-469">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="7b291-470">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="7b291-470">startMenuHideShutDown</span></span>|<span data-ttu-id="7b291-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-471">Boolean</span></span>|<span data-ttu-id="7b291-472">このポリシーを有効にすると、スタート メニューの電源ボタンに [シャットダウン]/[更新してシャットダウン] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-472">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="7b291-473">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="7b291-473">startMenuHideSignOut</span></span>|<span data-ttu-id="7b291-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-474">Boolean</span></span>|<span data-ttu-id="7b291-475">このポリシーを有効にすると、スタート メニューのユーザー タイルに [サインアウト] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-475">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="7b291-476">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="7b291-476">startMenuHideSleep</span></span>|<span data-ttu-id="7b291-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-477">Boolean</span></span>|<span data-ttu-id="7b291-478">このポリシーを有効にすると、スタート メニューの電源ボタンに [スリープ] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-478">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="7b291-479">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="7b291-479">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="7b291-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-480">Boolean</span></span>|<span data-ttu-id="7b291-481">このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウントの切り替え] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-481">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="7b291-482">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="7b291-482">startMenuHideUserTile</span></span>|<span data-ttu-id="7b291-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-483">Boolean</span></span>|<span data-ttu-id="7b291-484">このポリシーを有効にすると、スタート メニューにユーザー タイルが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b291-484">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="7b291-485">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="7b291-485">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="7b291-486">Binary</span><span class="sxs-lookup"><span data-stu-id="7b291-486">Binary</span></span>|<span data-ttu-id="7b291-487">このポリシー設定では、Edge アセットをインポートして startMenuLayoutXml ポリシーで使用することができます。</span><span class="sxs-lookup"><span data-stu-id="7b291-487">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="7b291-488">スタートのレイアウトには、Edge アプリからのセカンダリ タイルを含めることができ、このタイルは Edge のローカル アセット ファイルを検索します。</span><span class="sxs-lookup"><span data-stu-id="7b291-488">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="7b291-489">Edge のローカル アセットは存在しないことがあり、その場合は Edge のセカンダリ タイルが空で表示されます。</span><span class="sxs-lookup"><span data-stu-id="7b291-489">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="7b291-490">このポリシーは、startMenuLayoutXml ポリシーが変更された場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="7b291-490">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="7b291-491">値は、UTF-8 の Base64 でエンコードされたバイト配列にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b291-491">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="7b291-492">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="7b291-492">startMenuLayoutXml</span></span>|<span data-ttu-id="7b291-493">Binary</span><span class="sxs-lookup"><span data-stu-id="7b291-493">Binary</span></span>|<span data-ttu-id="7b291-494">管理者がスタート メニューの既定のレイアウトを上書きし、ユーザーがこれを変更できないようにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="7b291-494">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="7b291-495">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-495">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="7b291-496">XML は、UTF8 エンコードのバイト配列形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b291-496">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="7b291-497">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="7b291-497">startMenuMode</span></span>|[<span data-ttu-id="7b291-498">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="7b291-498">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="7b291-499">管理者がスタート メニューの表示方法を決めることを許可します。</span><span class="sxs-lookup"><span data-stu-id="7b291-499">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="7b291-500">可能な値は、`userDefined`、`fullScreen`、`nonFullScreen` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-500">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="7b291-501">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="7b291-501">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="7b291-502">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-502">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-503">スタート メニューへのドキュメント フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-503">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-504">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-504">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-505">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="7b291-505">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="7b291-506">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-506">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-507">スタート メニューへのダウンロード フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-507">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-508">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-508">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-509">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="7b291-509">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="7b291-510">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-510">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-511">スタート メニューへのエクスプローラー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-511">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-512">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-512">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-513">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="7b291-513">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="7b291-514">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-514">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-515">スタート メニューへのホームグループ フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-515">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-516">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-516">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-517">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="7b291-517">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="7b291-518">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-518">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-519">スタート メニューへのミュージック フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-519">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-520">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-520">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-521">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="7b291-521">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="7b291-522">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-522">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-523">スタート メニューへのネットワーク フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-523">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-524">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-524">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-525">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="7b291-525">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="7b291-526">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-526">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-527">スタート メニューへの個人用フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-527">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-528">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-528">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-529">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="7b291-529">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="7b291-530">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-530">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-531">スタート メニューへのピクチャ フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-531">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-532">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-532">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-533">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="7b291-533">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="7b291-534">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-534">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-535">スタート メニューへの設定フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-535">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-536">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-536">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-537">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="7b291-537">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="7b291-538">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="7b291-538">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="7b291-539">スタート メニューへのビデオ フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="7b291-539">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="7b291-540">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-540">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="7b291-541">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="7b291-541">settingsBlockSettingsApp</span></span>|<span data-ttu-id="7b291-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-542">Boolean</span></span>|<span data-ttu-id="7b291-543">設定アプリへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-543">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="7b291-544">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="7b291-544">settingsBlockSystemPage</span></span>|<span data-ttu-id="7b291-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-545">Boolean</span></span>|<span data-ttu-id="7b291-546">設定アプリ内の [システム] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-546">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="7b291-547">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="7b291-547">settingsBlockDevicesPage</span></span>|<span data-ttu-id="7b291-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-548">Boolean</span></span>|<span data-ttu-id="7b291-549">設定アプリ内の [デバイス] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-549">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="7b291-550">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="7b291-550">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="7b291-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-551">Boolean</span></span>|<span data-ttu-id="7b291-552">設定アプリ内の [ネットワークとインターネット] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-552">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="7b291-553">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="7b291-553">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="7b291-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-554">Boolean</span></span>|<span data-ttu-id="7b291-555">設定アプリ内の [個人用設定] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-555">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="7b291-556">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="7b291-556">settingsBlockAccountsPage</span></span>|<span data-ttu-id="7b291-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-557">Boolean</span></span>|<span data-ttu-id="7b291-558">設定アプリ内の [アカウント] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-558">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="7b291-559">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="7b291-559">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="7b291-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-560">Boolean</span></span>|<span data-ttu-id="7b291-561">設定アプリ内の [時刻と言語] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-561">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="7b291-562">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="7b291-562">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="7b291-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-563">Boolean</span></span>|<span data-ttu-id="7b291-564">設定アプリ内の [簡単操作] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-564">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="7b291-565">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="7b291-565">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="7b291-566">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-566">Boolean</span></span>|<span data-ttu-id="7b291-567">設定アプリ内の [プライバシー] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-567">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="7b291-568">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="7b291-568">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="7b291-569">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-569">Boolean</span></span>|<span data-ttu-id="7b291-570">設定アプリ内の [更新とセキュリティ] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-570">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="7b291-571">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="7b291-571">settingsBlockAppsPage</span></span>|<span data-ttu-id="7b291-572">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-572">Boolean</span></span>|<span data-ttu-id="7b291-573">設定アプリ内の [アプリ] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-573">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="7b291-574">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="7b291-574">settingsBlockGamingPage</span></span>|<span data-ttu-id="7b291-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-575">Boolean</span></span>|<span data-ttu-id="7b291-576">設定アプリ内の [ゲーム] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-576">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="7b291-577">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="7b291-577">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="7b291-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-578">Boolean</span></span>|<span data-ttu-id="7b291-579">通常はコンシューマー向けのエクスペリエンスを IT 管理者が禁止できるようにします。たとえば、開始時の提案、メンバーシップ通知、OOBE 後のアプリ インストール、リダイレクト タイルなどです。</span><span class="sxs-lookup"><span data-stu-id="7b291-579">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="7b291-580">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-580">windowsSpotlightBlocked</span></span>|<span data-ttu-id="7b291-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-581">Boolean</span></span>|<span data-ttu-id="7b291-582">IT 管理者が Windows スポットライトのすべての機能をオフにできるようにします</span><span class="sxs-lookup"><span data-stu-id="7b291-582">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="7b291-583">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="7b291-583">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="7b291-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-584">Boolean</span></span>|<span data-ttu-id="7b291-585">各 OS のクリーン インストールやアップグレードの後、またはその後も継続的に、新しい機能や変更された機能を Microsoft からユーザーに紹介することを禁止します</span><span class="sxs-lookup"><span data-stu-id="7b291-585">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="7b291-586">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="7b291-586">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="7b291-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-587">Boolean</span></span>|<span data-ttu-id="7b291-588">ユーザーのデバイスの使用状況に基づいて Windows スポットライトのコンテンツをカスタマイズすることを禁止します。</span><span class="sxs-lookup"><span data-stu-id="7b291-588">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="7b291-589">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="7b291-589">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="7b291-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-590">Boolean</span></span>|<span data-ttu-id="7b291-591">Windows スポットライト経由でサード パーティのコンテンツを配信することを禁止します</span><span class="sxs-lookup"><span data-stu-id="7b291-591">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="7b291-592">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="7b291-592">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="7b291-593">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-593">Boolean</span></span>|<span data-ttu-id="7b291-594">Windows スポットライトからの Windows へようこそのエクスペリエンスを禁止します</span><span class="sxs-lookup"><span data-stu-id="7b291-594">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="7b291-595">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="7b291-595">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="7b291-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-596">Boolean</span></span>|<span data-ttu-id="7b291-597">Windows のヒントのポップアップを IT 管理者がオフにできるようにします。</span><span class="sxs-lookup"><span data-stu-id="7b291-597">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="7b291-598">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="7b291-598">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="7b291-599">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="7b291-599">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="7b291-600">スポット ライトの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-600">Specifies the type of Spotlight.</span></span> <span data-ttu-id="7b291-601">可能な値は、`notConfigured`、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-601">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="7b291-602">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="7b291-602">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="7b291-603">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-603">Boolean</span></span>|<span data-ttu-id="7b291-604">オンに設定すると、プロキシの設定がデバイスのすべてのプロセスとアカウントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="7b291-604">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="7b291-605">それ以外の場合は、MDM に登録されているユーザー アカウントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="7b291-605">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="7b291-606">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="7b291-606">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="7b291-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-607">Boolean</span></span>|<span data-ttu-id="7b291-608">設定の自動検出を無効にします。</span><span class="sxs-lookup"><span data-stu-id="7b291-608">Disable automatic detection of settings.</span></span> <span data-ttu-id="7b291-609">有効にした場合、システムはプロキシ自動構成 (PAC) スクリプトへのパスを検索します。</span><span class="sxs-lookup"><span data-stu-id="7b291-609">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="7b291-610">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="7b291-610">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="7b291-611">String</span><span class="sxs-lookup"><span data-stu-id="7b291-611">String</span></span>|<span data-ttu-id="7b291-612">使用するプロキシ自動構成 (PAC) スクリプトのアドレス。</span><span class="sxs-lookup"><span data-stu-id="7b291-612">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="7b291-613">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="7b291-613">networkProxyServer</span></span>|[<span data-ttu-id="7b291-614">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="7b291-614">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="7b291-615">プロキシ サーバーの設定を手動で指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-615">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="7b291-616">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="7b291-616">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="7b291-617">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-617">Boolean</span></span>|<span data-ttu-id="7b291-618">Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-618">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="7b291-619">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-619">antiTheftModeBlocked</span></span>|<span data-ttu-id="7b291-620">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-620">Boolean</span></span>|<span data-ttu-id="7b291-621">ユーザーが盗難防止モードの設定を選択することを禁止するかどうかを示します (Windows 10 Mobile のみ)。</span><span class="sxs-lookup"><span data-stu-id="7b291-621">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="7b291-622">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-622">bluetoothBlocked</span></span>|<span data-ttu-id="7b291-623">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-623">Boolean</span></span>|<span data-ttu-id="7b291-624">ユーザーが Bluetooth を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-624">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="7b291-625">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-625">cameraBlocked</span></span>|<span data-ttu-id="7b291-626">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-626">Boolean</span></span>|<span data-ttu-id="7b291-627">ユーザーがデバイスのカメラにアクセスすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-627">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="7b291-628">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-628">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="7b291-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-629">Boolean</span></span>|<span data-ttu-id="7b291-630">他のデバイスの検出と接続、リモート メッセージング、リモート アプリ セッション、その他のデバイス間エクスペリエンスを可能にする、接続されているデバイスのサービスを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-630">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="7b291-631">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="7b291-631">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="7b291-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-632">Boolean</span></span>|<span data-ttu-id="7b291-633">ユーザーが手動でルート証明書をインストールすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-633">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="7b291-634">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-634">copyPasteBlocked</span></span>|<span data-ttu-id="7b291-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-635">Boolean</span></span>|<span data-ttu-id="7b291-636">ユーザーがコピーと貼り付けを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-636">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="7b291-637">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-637">cortanaBlocked</span></span>|<span data-ttu-id="7b291-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-638">Boolean</span></span>|<span data-ttu-id="7b291-639">ユーザーが Cortana を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="7b291-639">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="7b291-640">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="7b291-640">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="7b291-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-641">Boolean</span></span>|<span data-ttu-id="7b291-642">ユーザーが携帯電話をリセットすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-642">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="7b291-643">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="7b291-643">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="7b291-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-644">Boolean</span></span>|<span data-ttu-id="7b291-645">ユーザーがデバイス管理から手動で登録解除を行うことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-645">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="7b291-646">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="7b291-646">safeSearchFilter</span></span>|[<span data-ttu-id="7b291-647">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="7b291-647">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="7b291-648">セーフ サーチに必要なフィルター レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-648">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="7b291-649">可能な値は、`userDefined`、`strict`、`moderate` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-649">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="7b291-650">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="7b291-650">edgeBlockPopups</span></span>|<span data-ttu-id="7b291-651">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-651">Boolean</span></span>|<span data-ttu-id="7b291-652">ポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-652">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="7b291-653">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="7b291-653">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="7b291-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-654">Boolean</span></span>|<span data-ttu-id="7b291-655">ユーザーがアドレス バーで検索候補を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-655">Indicates whether or not to Block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="7b291-656">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="7b291-656">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="7b291-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-657">Boolean</span></span>|<span data-ttu-id="7b291-658">ユーザーが Edge から Internet Explorer にイントラネット トラフィックを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-658">Indicates whether or not to Block the user from sending Intranet traffic to Internet Explorer from Edge.</span></span>|
|<span data-ttu-id="7b291-659">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="7b291-659">edgeRequireSmartScreen</span></span>|<span data-ttu-id="7b291-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-660">Boolean</span></span>|<span data-ttu-id="7b291-661">スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-661">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="7b291-662">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="7b291-662">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="7b291-663">String</span><span class="sxs-lookup"><span data-stu-id="7b291-663">String</span></span>|<span data-ttu-id="7b291-664">エンタープライズ モードのサイト リストの場所を示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-664">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="7b291-665">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="7b291-665">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="7b291-666">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="7b291-666">edgeFirstRunUrl</span></span>|<span data-ttu-id="7b291-667">String</span><span class="sxs-lookup"><span data-stu-id="7b291-667">String</span></span>|<span data-ttu-id="7b291-668">Edge ブラウザーを初めて開いたときに最初に実行される URL です。</span><span class="sxs-lookup"><span data-stu-id="7b291-668">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="7b291-669">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="7b291-669">edgeSearchEngine</span></span>|[<span data-ttu-id="7b291-670">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="7b291-670">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="7b291-671">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="7b291-671">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="7b291-672">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="7b291-672">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="7b291-673">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="7b291-673">edgeHomepageUrls</span></span>|<span data-ttu-id="7b291-674">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7b291-674">String collection</span></span>|<span data-ttu-id="7b291-675">MDM に登録されているデバイスの Edge ブラウザーに表示されるホームページの URL の一覧です。</span><span class="sxs-lookup"><span data-stu-id="7b291-675">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="7b291-676">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="7b291-676">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="7b291-677">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-677">Boolean</span></span>|<span data-ttu-id="7b291-678">Edge ブラウザーの about:flags へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-678">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="7b291-679">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="7b291-679">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="7b291-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-680">Boolean</span></span>|<span data-ttu-id="7b291-681">悪意のある Web サイトの可能性があるサイトに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-681">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="7b291-682">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="7b291-682">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="7b291-683">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-683">Boolean</span></span>|<span data-ttu-id="7b291-684">未検証のファイルのダウンロードに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7b291-684">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="7b291-685">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="7b291-685">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="7b291-686">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-686">Boolean</span></span>|<span data-ttu-id="7b291-687">WebRTC を使用して通話を発信しているときにユーザーのローカル ホストの IP アドレスが表示されるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="7b291-687">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="7b291-688">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-688">internetSharingBlocked</span></span>|<span data-ttu-id="7b291-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-689">Boolean</span></span>|<span data-ttu-id="7b291-690">ユーザーがインターネット共有を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-690">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="7b291-691">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="7b291-691">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="7b291-692">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-692">Boolean</span></span>|<span data-ttu-id="7b291-693">ユーザーがプロビジョニング パッケージをインストールすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-693">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="7b291-694">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="7b291-694">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="7b291-695">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-695">Boolean</span></span>|<span data-ttu-id="7b291-696">ランタイム構成エージェントがプロビジョニング パッケージを削除することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-696">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="7b291-697">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="7b291-697">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="7b291-698">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-698">Boolean</span></span>|<span data-ttu-id="7b291-699">ユーザーが日付と時刻の設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-699">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="7b291-700">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="7b291-700">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="7b291-701">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-701">Boolean</span></span>|<span data-ttu-id="7b291-702">ユーザーがデバイス名を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-702">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="7b291-703">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="7b291-703">settingsBlockChangeRegion</span></span>|<span data-ttu-id="7b291-704">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-704">Boolean</span></span>|<span data-ttu-id="7b291-705">ユーザーがリージョン設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-705">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="7b291-706">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="7b291-706">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="7b291-707">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-707">Boolean</span></span>|<span data-ttu-id="7b291-708">ユーザーが言語の設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-708">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="7b291-709">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="7b291-709">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="7b291-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-710">Boolean</span></span>|<span data-ttu-id="7b291-711">ユーザーが電源とスリープの設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-711">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="7b291-712">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-712">locationServicesBlocked</span></span>|<span data-ttu-id="7b291-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-713">Boolean</span></span>|<span data-ttu-id="7b291-714">ユーザーが位置情報サービスを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-714">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="7b291-715">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-715">microsoftAccountBlocked</span></span>|<span data-ttu-id="7b291-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-716">Boolean</span></span>|<span data-ttu-id="7b291-717">Microsoft アカウントを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-717">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="7b291-718">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="7b291-718">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="7b291-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-719">Boolean</span></span>|<span data-ttu-id="7b291-720">Microsoft アカウントの設定の同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-720">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="7b291-721">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-721">nfcBlocked</span></span>|<span data-ttu-id="7b291-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-722">Boolean</span></span>|<span data-ttu-id="7b291-723">ユーザーが近距離無線通信を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-723">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="7b291-724">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-724">resetProtectionModeBlocked</span></span>|<span data-ttu-id="7b291-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-725">Boolean</span></span>|<span data-ttu-id="7b291-726">ユーザーが保護モードをリセットすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-726">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="7b291-727">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-727">screenCaptureBlocked</span></span>|<span data-ttu-id="7b291-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-728">Boolean</span></span>|<span data-ttu-id="7b291-729">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-729">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="7b291-730">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="7b291-730">storageBlockRemovableStorage</span></span>|<span data-ttu-id="7b291-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-731">Boolean</span></span>|<span data-ttu-id="7b291-732">ユーザーがリムーバブル記憶域を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-732">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="7b291-733">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="7b291-733">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="7b291-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-734">Boolean</span></span>|<span data-ttu-id="7b291-735">モバイル デバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-735">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="7b291-736">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-736">usbBlocked</span></span>|<span data-ttu-id="7b291-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-737">Boolean</span></span>|<span data-ttu-id="7b291-738">ユーザーが USB 接続を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-738">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="7b291-739">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-739">voiceRecordingBlocked</span></span>|<span data-ttu-id="7b291-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-740">Boolean</span></span>|<span data-ttu-id="7b291-741">ユーザーが音声録音を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-741">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="7b291-742">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="7b291-742">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="7b291-743">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-743">Boolean</span></span>|<span data-ttu-id="7b291-744">Wi-Fi ホットスポットへの自動接続を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-744">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="7b291-745">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="7b291-745">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="7b291-746">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-746">wiFiBlocked</span></span>|<span data-ttu-id="7b291-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-747">Boolean</span></span>|<span data-ttu-id="7b291-748">ユーザーが Wi-Fi を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-748">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="7b291-749">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b291-749">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="7b291-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-750">Boolean</span></span>|<span data-ttu-id="7b291-751">ユーザーが Wi-Fi の手動構成を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-751">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="7b291-752">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="7b291-752">wiFiScanInterval</span></span>|<span data-ttu-id="7b291-753">Int32</span><span class="sxs-lookup"><span data-stu-id="7b291-753">Int32</span></span>|<span data-ttu-id="7b291-754">Wi-Fi ネットワークに対するデバイス スキャンの頻度を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b291-754">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="7b291-755">サポートされている値は 1 から 500 まで、既定値は 100、500 は最低頻度です。</span><span class="sxs-lookup"><span data-stu-id="7b291-755">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="7b291-756">有効な値は 1 から 500 までです</span><span class="sxs-lookup"><span data-stu-id="7b291-756">Valid values 1 to 500</span></span>|
|<span data-ttu-id="7b291-757">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="7b291-757">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="7b291-758">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-758">Boolean</span></span>|<span data-ttu-id="7b291-759">他のデバイスがこの PC をプロジェクター用に検出することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-759">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="7b291-760">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="7b291-760">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="7b291-761">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-761">Boolean</span></span>|<span data-ttu-id="7b291-762">ワイヤレス ディスプレイ レシーバーからのユーザー入力を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-762">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="7b291-763">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="7b291-763">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="7b291-764">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-764">Boolean</span></span>|<span data-ttu-id="7b291-765">新しいデバイスがペアリングを開始するときに PIN が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-765">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="7b291-766">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-766">windowsStoreBlocked</span></span>|<span data-ttu-id="7b291-767">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-767">Boolean</span></span>|<span data-ttu-id="7b291-768">ユーザーが Windows ストアを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-768">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="7b291-769">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="7b291-769">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="7b291-770">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="7b291-770">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="7b291-771">信頼された証明書で署名した AppX パッケージからアプリをサイドローディングできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-771">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="7b291-772">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-772">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="7b291-773">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="7b291-773">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="7b291-774">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-774">Boolean</span></span>|<span data-ttu-id="7b291-775">Windows ストアからのアプリの自動更新を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-775">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="7b291-776">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="7b291-776">developerUnlockSetting</span></span>|[<span data-ttu-id="7b291-777">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="7b291-777">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="7b291-778">開発者によるロック解除を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-778">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="7b291-779">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="7b291-779">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="7b291-780">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="7b291-780">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="7b291-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-781">Boolean</span></span>|<span data-ttu-id="7b291-782">同じアプリの複数のユーザーによるデータ共有を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-782">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="7b291-783">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="7b291-783">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="7b291-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-784">Boolean</span></span>|<span data-ttu-id="7b291-785">プレインストールまたはダウンロードによって取得したすべての Windows ストア アプリの起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-785">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="7b291-786">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="7b291-786">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="7b291-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-787">Boolean</span></span>|<span data-ttu-id="7b291-788">プライベート ストアのみを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-788">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="7b291-789">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="7b291-789">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="7b291-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-790">Boolean</span></span>|<span data-ttu-id="7b291-791">アプリケーションのデータがシステム ドライブに制限されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-791">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="7b291-792">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="7b291-792">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="7b291-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-793">Boolean</span></span>|<span data-ttu-id="7b291-794">アプリケーションのインストールがシステム ドライブに制限されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-794">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="7b291-795">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="7b291-795">gameDvrBlocked</span></span>|<span data-ttu-id="7b291-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-796">Boolean</span></span>|<span data-ttu-id="7b291-797">DVR とブロードキャストを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-797">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="7b291-798">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="7b291-798">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="7b291-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-799">Boolean</span></span>|<span data-ttu-id="7b291-800">デバイス検出 UX を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-800">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="7b291-801">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="7b291-801">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="7b291-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-802">Boolean</span></span>|<span data-ttu-id="7b291-803">SIM カードが検出されない場合にエラー ダイアログを表示することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-803">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="7b291-804">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="7b291-804">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="7b291-805">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-805">Boolean</span></span>|<span data-ttu-id="7b291-806">デバイスでのタスクの切り替えを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7b291-806">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="7b291-807">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="7b291-807">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="7b291-808">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b291-808">Boolean</span></span>|<span data-ttu-id="7b291-809">同時にログオンしているユーザー間での切り替えをログオフなしで迅速に行う機能を無効にします。</span><span class="sxs-lookup"><span data-stu-id="7b291-809">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="7b291-810">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="7b291-810">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="7b291-811">ブール値</span><span class="sxs-lookup"><span data-stu-id="7b291-811">Boolean</span></span>|<span data-ttu-id="7b291-812">かどうか、デバイスがネットワークに接続する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b291-812">Whether the device is required to connect to the network.</span></span>|



## <a name="response"></a><span data-ttu-id="7b291-813">応答</span><span class="sxs-lookup"><span data-stu-id="7b291-813">Response</span></span>
<span data-ttu-id="7b291-814">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7b291-814">If successful, this method returns a `201 Created` response code and a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b291-815">例</span><span class="sxs-lookup"><span data-stu-id="7b291-815">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b291-816">要求</span><span class="sxs-lookup"><span data-stu-id="7b291-816">Request</span></span>
<span data-ttu-id="7b291-817">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b291-817">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9768

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```

### <a name="response"></a><span data-ttu-id="7b291-818">応答</span><span class="sxs-lookup"><span data-stu-id="7b291-818">Response</span></span>
<span data-ttu-id="7b291-p157">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7b291-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9940

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```



