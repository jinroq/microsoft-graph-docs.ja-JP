---
title: Update windows10GeneralConfiguration
description: windows10GeneralConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a83940e3892ea02a9416ccbf97d99de63a57a3c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578800"
---
# <a name="update-windows10generalconfiguration"></a><span data-ttu-id="f3e33-103">Update windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3e33-103">Update windows10GeneralConfiguration</span></span>

> <span data-ttu-id="f3e33-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3e33-105">[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-105">Update the properties of a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3e33-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3e33-106">Prerequisites</span></span>
<span data-ttu-id="f3e33-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3e33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3e33-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3e33-109">Permission type</span></span>|<span data-ttu-id="f3e33-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3e33-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3e33-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3e33-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3e33-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3e33-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3e33-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3e33-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3e33-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3e33-114">Not supported.</span></span>|
|<span data-ttu-id="f3e33-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3e33-115">Application</span></span>|<span data-ttu-id="f3e33-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3e33-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3e33-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3e33-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f3e33-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3e33-118">Request headers</span></span>
|<span data-ttu-id="f3e33-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3e33-119">Header</span></span>|<span data-ttu-id="f3e33-120">値</span><span class="sxs-lookup"><span data-stu-id="f3e33-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3e33-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3e33-121">Authorization</span></span>|<span data-ttu-id="f3e33-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3e33-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f3e33-123">Accept</span></span>|<span data-ttu-id="f3e33-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3e33-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3e33-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3e33-125">Request body</span></span>
<span data-ttu-id="f3e33-126">要求本文で、[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-126">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

<span data-ttu-id="f3e33-127">次の表に、[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-127">The following table shows the properties that are required when you create the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

|<span data-ttu-id="f3e33-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3e33-128">Property</span></span>|<span data-ttu-id="f3e33-129">型</span><span class="sxs-lookup"><span data-stu-id="f3e33-129">Type</span></span>|<span data-ttu-id="f3e33-130">説明</span><span class="sxs-lookup"><span data-stu-id="f3e33-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3e33-131">id</span><span class="sxs-lookup"><span data-stu-id="f3e33-131">id</span></span>|<span data-ttu-id="f3e33-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f3e33-132">String</span></span>|<span data-ttu-id="f3e33-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f3e33-133">Key of the entity.</span></span> <span data-ttu-id="f3e33-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3e33-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3e33-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3e33-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f3e33-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3e33-136">DateTimeOffset</span></span>|<span data-ttu-id="f3e33-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f3e33-137">DateTime the object was last modified.</span></span> <span data-ttu-id="f3e33-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3e33-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3e33-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3e33-139">createdDateTime</span></span>|<span data-ttu-id="f3e33-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3e33-140">DateTimeOffset</span></span>|<span data-ttu-id="f3e33-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f3e33-141">DateTime the object was created.</span></span> <span data-ttu-id="f3e33-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3e33-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3e33-143">説明</span><span class="sxs-lookup"><span data-stu-id="f3e33-143">description</span></span>|<span data-ttu-id="f3e33-144">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-144">String</span></span>|<span data-ttu-id="f3e33-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f3e33-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3e33-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3e33-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3e33-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f3e33-147">displayName</span></span>|<span data-ttu-id="f3e33-148">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-148">String</span></span>|<span data-ttu-id="f3e33-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f3e33-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3e33-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3e33-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3e33-151">version</span><span class="sxs-lookup"><span data-stu-id="f3e33-151">version</span></span>|<span data-ttu-id="f3e33-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-152">Int32</span></span>|<span data-ttu-id="f3e33-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f3e33-153">Version of the device configuration.</span></span> <span data-ttu-id="f3e33-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3e33-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3e33-155">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="f3e33-155">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="f3e33-156">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-156">String</span></span>|<span data-ttu-id="f3e33-157">クラウド プリンターを検出するエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="f3e33-157">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="f3e33-158">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="f3e33-158">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="f3e33-159">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-159">String</span></span>|<span data-ttu-id="f3e33-160">OAuth トークンを取得するための認証エンドポイント。</span><span class="sxs-lookup"><span data-stu-id="f3e33-160">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="f3e33-161">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3e33-161">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="f3e33-162">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-162">String</span></span>|<span data-ttu-id="f3e33-163">OAuth 認証機関から OAuth トークンを取得することを承認されているクライアント アプリケーションの GUID。</span><span class="sxs-lookup"><span data-stu-id="f3e33-163">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="f3e33-164">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3e33-164">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="f3e33-165">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-165">String</span></span>|<span data-ttu-id="f3e33-166">Azure Portal で構成されている印刷サービスの OAuth リソース URI。</span><span class="sxs-lookup"><span data-stu-id="f3e33-166">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="f3e33-167">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="f3e33-167">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="f3e33-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-168">Int32</span></span>|<span data-ttu-id="f3e33-169">検出エンドポイントからクエリを実行する必要があるプリンターの最大数。</span><span class="sxs-lookup"><span data-stu-id="f3e33-169">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="f3e33-170">これはモバイルのみでの設定です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-170">This is a mobile only setting.</span></span> <span data-ttu-id="f3e33-171">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-171">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="f3e33-172">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3e33-172">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="f3e33-173">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-173">String</span></span>|<span data-ttu-id="f3e33-174">Azure Portal で構成されているプリンター検出サービスの OAuth リソース URI。</span><span class="sxs-lookup"><span data-stu-id="f3e33-174">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="f3e33-175">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="f3e33-175">searchBlockDiacritics</span></span>|<span data-ttu-id="f3e33-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-176">Boolean</span></span>|<span data-ttu-id="f3e33-177">検索で分音記号を使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-177">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="f3e33-178">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="f3e33-178">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="f3e33-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-179">Boolean</span></span>|<span data-ttu-id="f3e33-180">コンテンツとプロパティのインデックスを作成するときに、自動言語検出を使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-180">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="f3e33-181">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="f3e33-181">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="f3e33-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-182">Boolean</span></span>|<span data-ttu-id="f3e33-183">Cortana またはエクスプローラーの検索結果に表示されないようにするため、WIP で保護されているアイテムのインデックス作成を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-183">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="f3e33-184">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="f3e33-184">searchEnableRemoteQueries</span></span>|<span data-ttu-id="f3e33-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-185">Boolean</span></span>|<span data-ttu-id="f3e33-186">このコンピューターのインデックスに対するリモート クエリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-186">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="f3e33-187">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="f3e33-187">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="f3e33-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-188">Boolean</span></span>|<span data-ttu-id="f3e33-189">インデクサー バックオフの検索機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-189">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="f3e33-190">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="f3e33-190">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="f3e33-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-191">Boolean</span></span>|<span data-ttu-id="f3e33-192">リムーバブル ドライブ上の場所をライブラリに追加してインデックスを作成することをユーザーに許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-192">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="f3e33-193">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="f3e33-193">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="f3e33-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-194">Boolean</span></span>|<span data-ttu-id="f3e33-195">インデックスの場所と同じドライブ上のハード ドライブ領域の最小値を指定して、その最小値を下回ったらインデックス作成を停止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-195">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="f3e33-196">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="f3e33-196">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="f3e33-197">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="f3e33-197">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="f3e33-198">診断データと利用統計情報データ (Watson など) の送信をデバイスに許可する値を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-198">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="f3e33-199">可能な値は、`userDefined`、`none`、`basic`、`enhanced`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-199">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="f3e33-200">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="f3e33-200">oneDriveDisableFileSync</span></span>|<span data-ttu-id="f3e33-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-201">Boolean</span></span>|<span data-ttu-id="f3e33-202">アプリや機能から OneDrive 上のファイルを操作することを IT 管理者が禁止できるかどうかを示す値を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-202">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="f3e33-203">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="f3e33-203">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="f3e33-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-204">Boolean</span></span>|<span data-ttu-id="f3e33-205">ユーザーがストア以外の場所からアプリをインストールできるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-205">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="f3e33-206">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="f3e33-206">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="f3e33-207">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-207">String</span></span>|<span data-ttu-id="f3e33-208">ダウンロードしてデスクトップ画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはデスクトップ画像として使用する必要があるファイル システム上のローカル画像のファイル URL。</span><span class="sxs-lookup"><span data-stu-id="f3e33-208">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="f3e33-209">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="f3e33-209">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="f3e33-210">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-210">String</span></span>|<span data-ttu-id="f3e33-211">ダウンロードしてロック画面画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはロック画面画像として使用する必要があるファイル システム上のローカル画像のファイル URL。</span><span class="sxs-lookup"><span data-stu-id="f3e33-211">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="f3e33-212">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="f3e33-212">bluetoothAllowedServices</span></span>|<span data-ttu-id="f3e33-213">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f3e33-213">String collection</span></span>|<span data-ttu-id="f3e33-214">許可されている Bluetooth サービスおよびプロファイルの一覧を 16 進形式の文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-214">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="f3e33-215">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="f3e33-215">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="f3e33-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-216">Boolean</span></span>|<span data-ttu-id="f3e33-217">ユーザーが Bluetooth 広告を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-217">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="f3e33-218">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="f3e33-218">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="f3e33-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-219">Boolean</span></span>|<span data-ttu-id="f3e33-220">ユーザーが Bluetooth の発見可能モードを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-220">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="f3e33-221">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="f3e33-221">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="f3e33-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-222">Boolean</span></span>|<span data-ttu-id="f3e33-223">バンドルされた特定のいくつかの Bluetooth 周辺機器を自動的にホスト デバイスとペアにすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-223">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="f3e33-224">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="f3e33-224">edgeBlockAutofill</span></span>|<span data-ttu-id="f3e33-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-225">Boolean</span></span>|<span data-ttu-id="f3e33-226">自動入力を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-226">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="f3e33-227">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-227">edgeBlocked</span></span>|<span data-ttu-id="f3e33-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-228">Boolean</span></span>|<span data-ttu-id="f3e33-229">ユーザーが Edge ブラウザーを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-229">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="f3e33-230">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="f3e33-230">edgeCookiePolicy</span></span>|[<span data-ttu-id="f3e33-231">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="f3e33-231">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="f3e33-232">Edge ブラウザーでどの Cookie を禁止するかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-232">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="f3e33-233">可能な値は、`userDefined`、`allow`、`blockThirdParty`、`blockAll` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-233">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="f3e33-234">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="f3e33-234">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="f3e33-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-235">Boolean</span></span>|<span data-ttu-id="f3e33-236">Edge ブラウザー内の開発者ツールを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-236">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="f3e33-237">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="f3e33-237">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="f3e33-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-238">Boolean</span></span>|<span data-ttu-id="f3e33-239">ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-239">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="f3e33-240">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="f3e33-240">edgeBlockExtensions</span></span>|<span data-ttu-id="f3e33-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-241">Boolean</span></span>|<span data-ttu-id="f3e33-242">Edge ブラウザーの拡張機能を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-242">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="f3e33-243">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="f3e33-243">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="f3e33-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-244">Boolean</span></span>|<span data-ttu-id="f3e33-245">Edge ブラウザーで会社のネットワークの InPrivate ブラウズを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-245">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="f3e33-246">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="f3e33-246">edgeBlockJavaScript</span></span>|<span data-ttu-id="f3e33-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-247">Boolean</span></span>|<span data-ttu-id="f3e33-248">ユーザーが JavaScript を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-248">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="f3e33-249">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="f3e33-249">edgeBlockPasswordManager</span></span>|<span data-ttu-id="f3e33-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-250">Boolean</span></span>|<span data-ttu-id="f3e33-251">パスワード マネージャーを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-251">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="f3e33-252">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="f3e33-252">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="f3e33-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-253">Boolean</span></span>|<span data-ttu-id="f3e33-254">Microsoft Edge のアドレス バー ドロップダウン機能を禁止します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-254">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="f3e33-255">Microsoft Edge から Microsoft サービスへのネットワーク接続を最小限に抑えるには、この設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="f3e33-255">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="f3e33-256">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="f3e33-256">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="f3e33-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-257">Boolean</span></span>|<span data-ttu-id="f3e33-258">Microsoft Edge での Microsoft 互換性リストを禁止します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-258">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="f3e33-259">Microsoft ではこのリストを利用して、既知の互換性の問題があるサイトを Edge で正しく表示できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f3e33-259">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="f3e33-260">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="f3e33-260">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="f3e33-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-261">Boolean</span></span>|<span data-ttu-id="f3e33-262">Microsoft Edge の終了時にブラウズ データを消去します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-262">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="f3e33-263">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="f3e33-263">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="f3e33-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-264">Boolean</span></span>|<span data-ttu-id="f3e33-265">Edge のスタート ページをユーザーが変更することを許可します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-265">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="f3e33-266">ユーザーが Edge を開いたときに既定で表示されるスタート ページを指定するには、EdgeHomepageUrls を使用します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-266">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="f3e33-267">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-267">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="f3e33-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-268">Boolean</span></span>|<span data-ttu-id="f3e33-269">Microsoft Edge の初回使用時に表示される Microsoft の Web ページを禁止します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-269">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="f3e33-270">このポリシーでは、ゼロ エミッション構成に登録している企業などが、このページの表示を禁止できます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-270">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="f3e33-271">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="f3e33-271">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="f3e33-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-272">Boolean</span></span>|<span data-ttu-id="f3e33-273">ユーザーが Microsoft Edge からスタートにサイトをピン留めしたときに、ライブ タイルを作成するために Microsoft が情報を収集することを禁止します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-273">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="f3e33-274">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="f3e33-274">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="f3e33-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-275">Boolean</span></span>|<span data-ttu-id="f3e33-276">Internet Explorer と Microsoft Edge の間でお気に入りの同期を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f3e33-276">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="f3e33-277">お気に入りの追加、削除、変更、順序変更が、ブラウザー間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-277">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="f3e33-278">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="f3e33-278">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="f3e33-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-279">Boolean</span></span>|<span data-ttu-id="f3e33-280">ローミング中に携帯電話上でユーザーがデータを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-280">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="f3e33-281">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="f3e33-281">cellularBlockVpn</span></span>|<span data-ttu-id="f3e33-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-282">Boolean</span></span>|<span data-ttu-id="f3e33-283">携帯電話上でユーザーが VPN を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-283">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="f3e33-284">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="f3e33-284">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="f3e33-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-285">Boolean</span></span>|<span data-ttu-id="f3e33-286">ローミング時に携帯電話上でユーザーが VPN を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-286">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="f3e33-287">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="f3e33-287">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="f3e33-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-288">Boolean</span></span>|<span data-ttu-id="f3e33-289">エンド ユーザーが Defender にアクセスすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-289">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="f3e33-290">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="f3e33-290">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="f3e33-291">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-291">Int32</span></span>|<span data-ttu-id="f3e33-292">検疫済みのマルウェアを削除するまでの日数。</span><span class="sxs-lookup"><span data-stu-id="f3e33-292">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="f3e33-293">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-293">Valid values 0 to 90</span></span>|
|<span data-ttu-id="f3e33-294">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="f3e33-294">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="f3e33-295">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="f3e33-295">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="f3e33-296">検出されたマルウェアに対する Defender のアクションを脅威レベルごとに取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-296">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="f3e33-297">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="f3e33-297">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="f3e33-298">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="f3e33-298">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="f3e33-299">Defender がシステムをスキャンする曜日。</span><span class="sxs-lookup"><span data-stu-id="f3e33-299">Defender day of the week for the system scan.</span></span> <span data-ttu-id="f3e33-300">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-300">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="f3e33-301">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="f3e33-301">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="f3e33-302">String collection</span><span class="sxs-lookup"><span data-stu-id="f3e33-302">String collection</span></span>|<span data-ttu-id="f3e33-303">スキャンとリアルタイム保護から除外するファイルとフォルダー。</span><span class="sxs-lookup"><span data-stu-id="f3e33-303">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="f3e33-304">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="f3e33-304">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="f3e33-305">String collection</span><span class="sxs-lookup"><span data-stu-id="f3e33-305">String collection</span></span>|<span data-ttu-id="f3e33-306">スキャンとリアルタイム保護から除外するファイル拡張子。</span><span class="sxs-lookup"><span data-stu-id="f3e33-306">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="f3e33-307">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="f3e33-307">defenderScanMaxCpu</span></span>|<span data-ttu-id="f3e33-308">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-308">Int32</span></span>|<span data-ttu-id="f3e33-309">スキャン中の最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="f3e33-309">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="f3e33-310">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-310">Valid values 0 to 100</span></span>|
|<span data-ttu-id="f3e33-311">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="f3e33-311">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="f3e33-312">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="f3e33-312">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="f3e33-313">ファイル アクティビティを監視する値。</span><span class="sxs-lookup"><span data-stu-id="f3e33-313">Value for monitoring file activity.</span></span> <span data-ttu-id="f3e33-314">可能な値は、`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-314">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="f3e33-315">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="f3e33-315">defenderProcessesToExclude</span></span>|<span data-ttu-id="f3e33-316">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f3e33-316">String collection</span></span>|<span data-ttu-id="f3e33-317">スキャンとリアルタイム保護から除外するプロセス。</span><span class="sxs-lookup"><span data-stu-id="f3e33-317">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="f3e33-318">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="f3e33-318">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="f3e33-319">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="f3e33-319">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="f3e33-320">ユーザーにサンプルの送信を要求する方法の構成。</span><span class="sxs-lookup"><span data-stu-id="f3e33-320">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="f3e33-321">可能な値は、`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-321">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="f3e33-322">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="f3e33-322">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="f3e33-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-323">Boolean</span></span>|<span data-ttu-id="f3e33-324">動作の監視が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-324">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="f3e33-325">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="f3e33-325">defenderRequireCloudProtection</span></span>|<span data-ttu-id="f3e33-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-326">Boolean</span></span>|<span data-ttu-id="f3e33-327">クラウドの保護が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-327">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="f3e33-328">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="f3e33-328">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="f3e33-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-329">Boolean</span></span>|<span data-ttu-id="f3e33-330">ネットワーク検査システムが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-330">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="f3e33-331">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="f3e33-331">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="f3e33-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-332">Boolean</span></span>|<span data-ttu-id="f3e33-333">リアルタイムの監視が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-333">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="f3e33-334">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="f3e33-334">defenderScanArchiveFiles</span></span>|<span data-ttu-id="f3e33-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-335">Boolean</span></span>|<span data-ttu-id="f3e33-336">アーカイブ ファイルをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-336">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="f3e33-337">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="f3e33-337">defenderScanDownloads</span></span>|<span data-ttu-id="f3e33-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-338">Boolean</span></span>|<span data-ttu-id="f3e33-339">ダウンロードをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-339">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="f3e33-340">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="f3e33-340">defenderScanNetworkFiles</span></span>|<span data-ttu-id="f3e33-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-341">Boolean</span></span>|<span data-ttu-id="f3e33-342">ネットワーク フォルダーから開かれたファイルをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-342">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="f3e33-343">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="f3e33-343">defenderScanIncomingMail</span></span>|<span data-ttu-id="f3e33-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-344">Boolean</span></span>|<span data-ttu-id="f3e33-345">受信メール メッセージをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-345">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="f3e33-346">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="f3e33-346">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="f3e33-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-347">Boolean</span></span>|<span data-ttu-id="f3e33-348">フル スキャン時に、マップされたネットワーク ドライブをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-348">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="f3e33-349">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="f3e33-349">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="f3e33-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-350">Boolean</span></span>|<span data-ttu-id="f3e33-351">フル スキャン時に、リムーバブル ドライブをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-351">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="f3e33-352">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="f3e33-352">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="f3e33-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-353">Boolean</span></span>|<span data-ttu-id="f3e33-354">Internet Explorer ブラウザーに読み込まれるスクリプトをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-354">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="f3e33-355">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="f3e33-355">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="f3e33-356">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-356">Int32</span></span>|<span data-ttu-id="f3e33-357">署名を更新する間隔 (時間)。</span><span class="sxs-lookup"><span data-stu-id="f3e33-357">The signature update interval in hours.</span></span> <span data-ttu-id="f3e33-358">確認しない場合は 0 を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-358">Specify 0 not to check.</span></span> <span data-ttu-id="f3e33-359">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-359">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f3e33-360">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="f3e33-360">defenderScanType</span></span>|[<span data-ttu-id="f3e33-361">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="f3e33-361">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="f3e33-362">Defender システム スキャンの種類。</span><span class="sxs-lookup"><span data-stu-id="f3e33-362">The defender system scan type.</span></span> <span data-ttu-id="f3e33-363">使用可能な値は、`userDefined`、`disabled`、`quick`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-363">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="f3e33-364">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="f3e33-364">defenderScheduledScanTime</span></span>|<span data-ttu-id="f3e33-365">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f3e33-365">TimeOfDay</span></span>|<span data-ttu-id="f3e33-366">システムのスキャンの Defender 時刻。</span><span class="sxs-lookup"><span data-stu-id="f3e33-366">The defender time for the system scan.</span></span>|
|<span data-ttu-id="f3e33-367">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="f3e33-367">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="f3e33-368">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f3e33-368">TimeOfDay</span></span>|<span data-ttu-id="f3e33-369">毎日のクイック スキャンを実行する時刻。</span><span class="sxs-lookup"><span data-stu-id="f3e33-369">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="f3e33-370">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="f3e33-370">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="f3e33-371">defendercloudblockleveltype</span><span class="sxs-lookup"><span data-stu-id="f3e33-371">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="f3e33-372">クラウド配信の保護レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-372">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="f3e33-373">可能な値は、`notConfigured`、`high`、`highPlus`、`zeroTolerance` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-373">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="f3e33-374">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3e33-374">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="f3e33-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-375">Boolean</span></span>|<span data-ttu-id="f3e33-376">Windows 10 Mobile デバイスのロック画面で、画面のタイムアウトを制御するユーザー構成可能な設定を表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-376">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="f3e33-377">このポリシーが [許可] に設定されている場合は、lockScreenTimeoutInSeconds によって設定された値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-377">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="f3e33-378">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="f3e33-378">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="f3e33-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-379">Boolean</span></span>|<span data-ttu-id="f3e33-380">ロック画面上のアクション センター通知を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-380">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="f3e33-381">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="f3e33-381">lockScreenBlockCortana</span></span>|<span data-ttu-id="f3e33-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-382">Boolean</span></span>|<span data-ttu-id="f3e33-383">システムのロック中にユーザーが音声認識を使用して Cortana と対話できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-383">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="f3e33-384">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="f3e33-384">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="f3e33-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-385">Boolean</span></span>|<span data-ttu-id="f3e33-386">デバイスのロック画面へのトースト通知を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-386">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="f3e33-387">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="f3e33-387">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="f3e33-388">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-388">Int32</span></span>|<span data-ttu-id="f3e33-389">Windows 10 Mobile デバイスで画面をロックしてから画面をオフにするまでの時間 (秒) を設定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-389">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="f3e33-390">サポートされている値は 11 から 1800 までです。</span><span class="sxs-lookup"><span data-stu-id="f3e33-390">Supported values are 11-1800.</span></span> <span data-ttu-id="f3e33-391">有効な値は 11 から 1800 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-391">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="f3e33-392">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f3e33-392">passwordBlockSimple</span></span>|<span data-ttu-id="f3e33-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-393">Boolean</span></span>|<span data-ttu-id="f3e33-394">"1111" や "1234" などの PIN またはパスワードを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-394">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="f3e33-395">Windows 10 デスクトップでは、ピクチャ パスワードの使用も制御します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-395">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="f3e33-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f3e33-396">passwordExpirationDays</span></span>|<span data-ttu-id="f3e33-397">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-397">Int32</span></span>|<span data-ttu-id="f3e33-398">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="f3e33-398">The password expiration in days.</span></span> <span data-ttu-id="f3e33-399">有効な値は 0 から 730 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-399">Valid values 0 to 730</span></span>|
|<span data-ttu-id="f3e33-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f3e33-400">passwordMinimumLength</span></span>|<span data-ttu-id="f3e33-401">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-401">Int32</span></span>|<span data-ttu-id="f3e33-402">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="f3e33-402">The minimum password length.</span></span> <span data-ttu-id="f3e33-403">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f3e33-404">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f3e33-404">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f3e33-405">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-405">Int32</span></span>|<span data-ttu-id="f3e33-406">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="f3e33-406">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f3e33-407">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f3e33-407">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f3e33-408">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-408">Int32</span></span>|<span data-ttu-id="f3e33-409">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="f3e33-409">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f3e33-410">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f3e33-410">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f3e33-411">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-411">Int32</span></span>|<span data-ttu-id="f3e33-412">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="f3e33-412">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="f3e33-413">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-413">Valid values 0 to 50</span></span>|
|<span data-ttu-id="f3e33-414">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f3e33-414">passwordRequired</span></span>|<span data-ttu-id="f3e33-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-415">Boolean</span></span>|<span data-ttu-id="f3e33-416">ユーザーにパスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-416">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="f3e33-417">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="f3e33-417">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="f3e33-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-418">Boolean</span></span>|<span data-ttu-id="f3e33-419">アイドル状態からの再開時にパスワードを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-419">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="f3e33-420">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f3e33-420">passwordRequiredType</span></span>|[<span data-ttu-id="f3e33-421">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="f3e33-421">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f3e33-422">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="f3e33-422">The required password type.</span></span> <span data-ttu-id="f3e33-423">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-423">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f3e33-424">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f3e33-424">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f3e33-425">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-425">Int32</span></span>|<span data-ttu-id="f3e33-426">出荷時の設定にリセットされるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="f3e33-426">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="f3e33-427">有効な値は 0 から 999 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-427">Valid values 0 to 999</span></span>|
|<span data-ttu-id="f3e33-428">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="f3e33-428">privacyAdvertisingId</span></span>|[<span data-ttu-id="f3e33-429">statemanagementsetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-429">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="f3e33-430">広告識別子の使用を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="f3e33-430">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="f3e33-431">Windows 10 バージョン 1607 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="f3e33-431">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="f3e33-432">可能な値は `notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-432">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="f3e33-433">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="f3e33-433">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="f3e33-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-434">Boolean</span></span>|<span data-ttu-id="f3e33-435">アプリの起動時に、ペアリングとプライバシーに関するユーザーの同意ダイアログの自動受け入れを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-435">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="f3e33-436">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="f3e33-436">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="f3e33-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-437">Boolean</span></span>|<span data-ttu-id="f3e33-438">Cortana、音声入力、ストア アプリケーションに対するクラウド ベースの音声サービスの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-438">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="f3e33-439">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="f3e33-439">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="f3e33-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-440">Boolean</span></span>|<span data-ttu-id="f3e33-441">ユーザーがタスク バーからアプリのピン留めを外すことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-441">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="f3e33-442">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="f3e33-442">startMenuAppListVisibility</span></span>|[<span data-ttu-id="f3e33-443">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="f3e33-443">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="f3e33-444">この値を設定すると、アプリ リストを折りたたんだり、アプリ リスト全体を削除したり、設定アプリで対応する切り替えを無効にしたりできます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-444">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="f3e33-445">可能な値は、`userDefined`、`collapse`、`remove`、`disableSettingsApp` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-445">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="f3e33-446">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="f3e33-446">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="f3e33-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-447">Boolean</span></span>|<span data-ttu-id="f3e33-448">このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウント設定の変更] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-448">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="f3e33-449">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="f3e33-449">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="f3e33-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-450">Boolean</span></span>|<span data-ttu-id="f3e33-451">このポリシーを有効にすると、よく使われるアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-451">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="f3e33-452">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="f3e33-452">startMenuHideHibernate</span></span>|<span data-ttu-id="f3e33-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-453">Boolean</span></span>|<span data-ttu-id="f3e33-454">このポリシーを有効にすると、スタート メニューの電源ボタンに [休止状態] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-454">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="f3e33-455">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="f3e33-455">startMenuHideLock</span></span>|<span data-ttu-id="f3e33-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-456">Boolean</span></span>|<span data-ttu-id="f3e33-457">このポリシーを有効にすると、スタート メニューのユーザー タイルに [ロック] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-457">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="f3e33-458">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="f3e33-458">startMenuHidePowerButton</span></span>|<span data-ttu-id="f3e33-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-459">Boolean</span></span>|<span data-ttu-id="f3e33-460">このポリシーを有効にすると、スタート メニューに電源ボタンが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-460">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="f3e33-461">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="f3e33-461">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="f3e33-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-462">Boolean</span></span>|<span data-ttu-id="f3e33-463">このポリシーを有効にすると、最近開いた項目のジャンプ リストがスタート メニュー/タスクバーに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-463">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="f3e33-464">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="f3e33-464">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="f3e33-465">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-465">Boolean</span></span>|<span data-ttu-id="f3e33-466">このポリシーを有効にすると、最近追加したアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-466">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="f3e33-467">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="f3e33-467">startMenuHideRestartOptions</span></span>|<span data-ttu-id="f3e33-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-468">Boolean</span></span>|<span data-ttu-id="f3e33-469">このポリシーを有効にすると、スタート メニューの電源ボタンに [再起動]/[更新して再起動] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-469">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="f3e33-470">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="f3e33-470">startMenuHideShutDown</span></span>|<span data-ttu-id="f3e33-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-471">Boolean</span></span>|<span data-ttu-id="f3e33-472">このポリシーを有効にすると、スタート メニューの電源ボタンに [シャットダウン]/[更新してシャットダウン] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-472">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="f3e33-473">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="f3e33-473">startMenuHideSignOut</span></span>|<span data-ttu-id="f3e33-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-474">Boolean</span></span>|<span data-ttu-id="f3e33-475">このポリシーを有効にすると、スタート メニューのユーザー タイルに [サインアウト] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-475">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="f3e33-476">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="f3e33-476">startMenuHideSleep</span></span>|<span data-ttu-id="f3e33-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-477">Boolean</span></span>|<span data-ttu-id="f3e33-478">このポリシーを有効にすると、スタート メニューの電源ボタンに [スリープ] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-478">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="f3e33-479">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="f3e33-479">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="f3e33-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-480">Boolean</span></span>|<span data-ttu-id="f3e33-481">このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウントの切り替え] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-481">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="f3e33-482">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="f3e33-482">startMenuHideUserTile</span></span>|<span data-ttu-id="f3e33-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-483">Boolean</span></span>|<span data-ttu-id="f3e33-484">このポリシーを有効にすると、スタート メニューにユーザー タイルが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-484">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="f3e33-485">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="f3e33-485">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="f3e33-486">Binary</span><span class="sxs-lookup"><span data-stu-id="f3e33-486">Binary</span></span>|<span data-ttu-id="f3e33-487">このポリシー設定では、Edge アセットをインポートして startMenuLayoutXml ポリシーで使用することができます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-487">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="f3e33-488">スタートのレイアウトには、Edge アプリからのセカンダリ タイルを含めることができ、このタイルは Edge のローカル アセット ファイルを検索します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-488">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="f3e33-489">Edge のローカル アセットは存在しないことがあり、その場合は Edge のセカンダリ タイルが空で表示されます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-489">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="f3e33-490">このポリシーは、startMenuLayoutXml ポリシーが変更された場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-490">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="f3e33-491">値は、UTF-8 の Base64 でエンコードされたバイト配列にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-491">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="f3e33-492">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="f3e33-492">startMenuLayoutXml</span></span>|<span data-ttu-id="f3e33-493">Binary</span><span class="sxs-lookup"><span data-stu-id="f3e33-493">Binary</span></span>|<span data-ttu-id="f3e33-494">管理者がスタート メニューの既定のレイアウトを上書きし、ユーザーがこれを変更できないようにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-494">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="f3e33-495">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-495">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="f3e33-496">XML は、UTF8 エンコードのバイト配列形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3e33-496">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="f3e33-497">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="f3e33-497">startMenuMode</span></span>|[<span data-ttu-id="f3e33-498">windowsstartmenumodetype</span><span class="sxs-lookup"><span data-stu-id="f3e33-498">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="f3e33-499">管理者がスタート メニューの表示方法を決めることを許可します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-499">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="f3e33-500">可能な値は `userDefined`、`fullScreen`、`nonFullScreen` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-500">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="f3e33-501">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="f3e33-501">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="f3e33-502">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-502">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-503">スタート メニューへのドキュメント フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-503">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-504">可能な値は `notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-504">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-505">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="f3e33-505">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="f3e33-506">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-506">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-507">スタート メニューへのダウンロード フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-507">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-508">可能な値は `notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-508">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-509">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="f3e33-509">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="f3e33-510">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-510">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-511">スタート メニューへのエクスプローラー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-511">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-512">可能な値は `notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-512">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-513">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="f3e33-513">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="f3e33-514">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-514">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-515">スタート メニューへのホームグループ フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-515">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-516">可能な値は `notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-516">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-517">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="f3e33-517">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="f3e33-518">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-518">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-519">スタート メニューへのミュージック フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-519">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-520">可能な値は `notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-520">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-521">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="f3e33-521">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="f3e33-522">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-522">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-523">スタート メニューへのネットワーク フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-523">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-524">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-524">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-525">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="f3e33-525">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="f3e33-526">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-526">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-527">スタート メニューへの個人用フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-527">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-528">可能な値は `notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-528">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-529">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="f3e33-529">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="f3e33-530">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-530">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-531">スタート メニューへのピクチャ フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-531">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-532">可能な値は `notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-532">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-533">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="f3e33-533">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="f3e33-534">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-534">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-535">スタート メニューへの設定フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-535">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-536">可能な値は `notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-536">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-537">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="f3e33-537">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="f3e33-538">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-538">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="f3e33-539">スタート メニューへのビデオ フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-539">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="f3e33-540">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-540">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="f3e33-541">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="f3e33-541">settingsBlockSettingsApp</span></span>|<span data-ttu-id="f3e33-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-542">Boolean</span></span>|<span data-ttu-id="f3e33-543">設定アプリへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-543">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="f3e33-544">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-544">settingsBlockSystemPage</span></span>|<span data-ttu-id="f3e33-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-545">Boolean</span></span>|<span data-ttu-id="f3e33-546">設定アプリ内の [システム] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-546">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="f3e33-547">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-547">settingsBlockDevicesPage</span></span>|<span data-ttu-id="f3e33-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-548">Boolean</span></span>|<span data-ttu-id="f3e33-549">設定アプリ内の [デバイス] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-549">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="f3e33-550">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-550">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="f3e33-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-551">Boolean</span></span>|<span data-ttu-id="f3e33-552">設定アプリ内の [ネットワークとインターネット] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-552">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="f3e33-553">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-553">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="f3e33-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-554">Boolean</span></span>|<span data-ttu-id="f3e33-555">設定アプリ内の [個人用設定] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-555">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="f3e33-556">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-556">settingsBlockAccountsPage</span></span>|<span data-ttu-id="f3e33-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-557">Boolean</span></span>|<span data-ttu-id="f3e33-558">設定アプリ内の [アカウント] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-558">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="f3e33-559">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="f3e33-559">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="f3e33-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-560">Boolean</span></span>|<span data-ttu-id="f3e33-561">設定アプリ内の [時刻と言語] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-561">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="f3e33-562">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-562">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="f3e33-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-563">Boolean</span></span>|<span data-ttu-id="f3e33-564">設定アプリ内の [簡単操作] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-564">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="f3e33-565">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-565">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="f3e33-566">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-566">Boolean</span></span>|<span data-ttu-id="f3e33-567">設定アプリ内の [プライバシー] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-567">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="f3e33-568">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-568">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="f3e33-569">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-569">Boolean</span></span>|<span data-ttu-id="f3e33-570">設定アプリ内の [更新とセキュリティ] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-570">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="f3e33-571">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-571">settingsBlockAppsPage</span></span>|<span data-ttu-id="f3e33-572">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-572">Boolean</span></span>|<span data-ttu-id="f3e33-573">設定アプリ内の [アプリ] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-573">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="f3e33-574">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="f3e33-574">settingsBlockGamingPage</span></span>|<span data-ttu-id="f3e33-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-575">Boolean</span></span>|<span data-ttu-id="f3e33-576">設定アプリ内の [ゲーム] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-576">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="f3e33-577">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="f3e33-577">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="f3e33-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-578">Boolean</span></span>|<span data-ttu-id="f3e33-579">通常はコンシューマー向けのエクスペリエンスを IT 管理者が禁止できるようにします。たとえば、開始時の提案、メンバーシップ通知、OOBE 後のアプリ インストール、リダイレクト タイルなどです。</span><span class="sxs-lookup"><span data-stu-id="f3e33-579">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="f3e33-580">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-580">windowsSpotlightBlocked</span></span>|<span data-ttu-id="f3e33-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-581">Boolean</span></span>|<span data-ttu-id="f3e33-582">IT 管理者が Windows スポットライトのすべての機能をオフにできるようにします</span><span class="sxs-lookup"><span data-stu-id="f3e33-582">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="f3e33-583">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="f3e33-583">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="f3e33-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-584">Boolean</span></span>|<span data-ttu-id="f3e33-585">各 OS のクリーン インストールやアップグレードの後、またはその後も継続的に、新しい機能や変更された機能を Microsoft からユーザーに紹介することを禁止します</span><span class="sxs-lookup"><span data-stu-id="f3e33-585">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="f3e33-586">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="f3e33-586">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="f3e33-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-587">Boolean</span></span>|<span data-ttu-id="f3e33-588">ユーザーのデバイスの使用状況に基づいて Windows スポットライトのコンテンツをカスタマイズすることを禁止します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-588">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="f3e33-589">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="f3e33-589">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="f3e33-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-590">Boolean</span></span>|<span data-ttu-id="f3e33-591">Windows スポットライト経由でサード パーティのコンテンツを配信することを禁止します</span><span class="sxs-lookup"><span data-stu-id="f3e33-591">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="f3e33-592">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="f3e33-592">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="f3e33-593">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-593">Boolean</span></span>|<span data-ttu-id="f3e33-594">Windows スポットライトからの Windows へようこそのエクスペリエンスを禁止します</span><span class="sxs-lookup"><span data-stu-id="f3e33-594">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="f3e33-595">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="f3e33-595">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="f3e33-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-596">Boolean</span></span>|<span data-ttu-id="f3e33-597">Windows のヒントのポップアップを IT 管理者がオフにできるようにします。</span><span class="sxs-lookup"><span data-stu-id="f3e33-597">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="f3e33-598">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f3e33-598">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="f3e33-599">windowsスポットライト enablementsettings</span><span class="sxs-lookup"><span data-stu-id="f3e33-599">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="f3e33-600">スポットライトの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-600">Specifies the type of Spotlight.</span></span> <span data-ttu-id="f3e33-601">可能な値は `notConfigured`、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-601">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="f3e33-602">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="f3e33-602">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="f3e33-603">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-603">Boolean</span></span>|<span data-ttu-id="f3e33-604">オンに設定すると、プロキシの設定がデバイスのすべてのプロセスとアカウントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-604">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="f3e33-605">それ以外の場合は、MDM に登録されているユーザー アカウントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-605">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="f3e33-606">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="f3e33-606">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="f3e33-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-607">Boolean</span></span>|<span data-ttu-id="f3e33-608">設定の自動検出を無効にします。</span><span class="sxs-lookup"><span data-stu-id="f3e33-608">Disable automatic detection of settings.</span></span> <span data-ttu-id="f3e33-609">有効にした場合、システムはプロキシ自動構成 (PAC) スクリプトへのパスを検索します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-609">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="f3e33-610">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="f3e33-610">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="f3e33-611">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-611">String</span></span>|<span data-ttu-id="f3e33-612">使用するプロキシ自動構成 (PAC) スクリプトのアドレス。</span><span class="sxs-lookup"><span data-stu-id="f3e33-612">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="f3e33-613">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="f3e33-613">networkProxyServer</span></span>|[<span data-ttu-id="f3e33-614">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="f3e33-614">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="f3e33-615">プロキシ サーバーの設定を手動で指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-615">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="f3e33-616">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="f3e33-616">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="f3e33-617">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-617">Boolean</span></span>|<span data-ttu-id="f3e33-618">Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-618">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="f3e33-619">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-619">antiTheftModeBlocked</span></span>|<span data-ttu-id="f3e33-620">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-620">Boolean</span></span>|<span data-ttu-id="f3e33-621">ユーザーが盗難防止モードの設定を選択することを禁止するかどうかを示します (Windows 10 Mobile のみ)。</span><span class="sxs-lookup"><span data-stu-id="f3e33-621">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="f3e33-622">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-622">bluetoothBlocked</span></span>|<span data-ttu-id="f3e33-623">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-623">Boolean</span></span>|<span data-ttu-id="f3e33-624">ユーザーが Bluetooth を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-624">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="f3e33-625">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-625">cameraBlocked</span></span>|<span data-ttu-id="f3e33-626">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-626">Boolean</span></span>|<span data-ttu-id="f3e33-627">ユーザーがデバイスのカメラにアクセスすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-627">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="f3e33-628">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-628">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="f3e33-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-629">Boolean</span></span>|<span data-ttu-id="f3e33-630">他のデバイスの検出と接続、リモート メッセージング、リモート アプリ セッション、その他のデバイス間エクスペリエンスを可能にする、接続されているデバイスのサービスを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-630">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="f3e33-631">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="f3e33-631">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="f3e33-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-632">Boolean</span></span>|<span data-ttu-id="f3e33-633">ユーザーが手動でルート証明書をインストールすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-633">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="f3e33-634">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-634">copyPasteBlocked</span></span>|<span data-ttu-id="f3e33-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-635">Boolean</span></span>|<span data-ttu-id="f3e33-636">ユーザーがコピーと貼り付けを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-636">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="f3e33-637">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-637">cortanaBlocked</span></span>|<span data-ttu-id="f3e33-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-638">Boolean</span></span>|<span data-ttu-id="f3e33-639">ユーザーが Cortana を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-639">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="f3e33-640">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="f3e33-640">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="f3e33-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-641">Boolean</span></span>|<span data-ttu-id="f3e33-642">ユーザーが携帯電話をリセットすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-642">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="f3e33-643">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="f3e33-643">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="f3e33-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-644">Boolean</span></span>|<span data-ttu-id="f3e33-645">ユーザーがデバイス管理から手動で登録解除を行うことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-645">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="f3e33-646">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="f3e33-646">safeSearchFilter</span></span>|[<span data-ttu-id="f3e33-647">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="f3e33-647">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="f3e33-648">セーフ サーチに必要なフィルター レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-648">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="f3e33-649">可能な値は、`userDefined`、`strict`、`moderate` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-649">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="f3e33-650">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="f3e33-650">edgeBlockPopups</span></span>|<span data-ttu-id="f3e33-651">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-651">Boolean</span></span>|<span data-ttu-id="f3e33-652">ポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-652">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="f3e33-653">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="f3e33-653">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="f3e33-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-654">Boolean</span></span>|<span data-ttu-id="f3e33-655">ユーザーがアドレスバーの検索候補を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-655">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="f3e33-656">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="f3e33-656">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="f3e33-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-657">Boolean</span></span>|<span data-ttu-id="f3e33-658">イントラネットトラフィックをエッジから Internet Explorer に切り替えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-658">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="f3e33-659">注: このプロパティの名前は誤解されています。このプロパティは現在使用されていません。代わりに EdgeSendIntranetTrafficToInternetExplorer を使用してください。</span><span class="sxs-lookup"><span data-stu-id="f3e33-659">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="f3e33-660">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="f3e33-660">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="f3e33-661">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-661">Boolean</span></span>|<span data-ttu-id="f3e33-662">イントラネットトラフィックをエッジから Internet Explorer に切り替えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-662">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="f3e33-663">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="f3e33-663">edgeRequireSmartScreen</span></span>|<span data-ttu-id="f3e33-664">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-664">Boolean</span></span>|<span data-ttu-id="f3e33-665">スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-665">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="f3e33-666">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="f3e33-666">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="f3e33-667">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-667">String</span></span>|<span data-ttu-id="f3e33-668">エンタープライズ モードのサイト リストの場所を示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-668">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="f3e33-669">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-669">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="f3e33-670">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="f3e33-670">edgeFirstRunUrl</span></span>|<span data-ttu-id="f3e33-671">String</span><span class="sxs-lookup"><span data-stu-id="f3e33-671">String</span></span>|<span data-ttu-id="f3e33-672">Edge ブラウザーを初めて開いたときに最初に実行される URL です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-672">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="f3e33-673">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="f3e33-673">edgeSearchEngine</span></span>|[<span data-ttu-id="f3e33-674">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="f3e33-674">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="f3e33-675">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f3e33-675">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="f3e33-676">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-676">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="f3e33-677">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="f3e33-677">edgeHomepageUrls</span></span>|<span data-ttu-id="f3e33-678">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f3e33-678">String collection</span></span>|<span data-ttu-id="f3e33-679">MDM に登録されているデバイスの Edge ブラウザーに表示されるホームページの URL の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-679">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="f3e33-680">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="f3e33-680">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="f3e33-681">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-681">Boolean</span></span>|<span data-ttu-id="f3e33-682">Edge ブラウザーの about:flags へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-682">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="f3e33-683">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="f3e33-683">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="f3e33-684">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-684">Boolean</span></span>|<span data-ttu-id="f3e33-685">悪意のある Web サイトの可能性があるサイトに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-685">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="f3e33-686">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="f3e33-686">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="f3e33-687">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-687">Boolean</span></span>|<span data-ttu-id="f3e33-688">未検証のファイルのダウンロードに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="f3e33-688">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="f3e33-689">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="f3e33-689">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="f3e33-690">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-690">Boolean</span></span>|<span data-ttu-id="f3e33-691">WebRTC を使用して通話を発信しているときにユーザーのローカル ホストの IP アドレスが表示されるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="f3e33-691">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="f3e33-692">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-692">internetSharingBlocked</span></span>|<span data-ttu-id="f3e33-693">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-693">Boolean</span></span>|<span data-ttu-id="f3e33-694">ユーザーがインターネット共有を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-694">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="f3e33-695">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="f3e33-695">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="f3e33-696">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-696">Boolean</span></span>|<span data-ttu-id="f3e33-697">ユーザーがプロビジョニング パッケージをインストールすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-697">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="f3e33-698">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="f3e33-698">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="f3e33-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-699">Boolean</span></span>|<span data-ttu-id="f3e33-700">ランタイム構成エージェントがプロビジョニング パッケージを削除することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-700">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="f3e33-701">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="f3e33-701">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="f3e33-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-702">Boolean</span></span>|<span data-ttu-id="f3e33-703">ユーザーが日付と時刻の設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-703">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="f3e33-704">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="f3e33-704">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="f3e33-705">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-705">Boolean</span></span>|<span data-ttu-id="f3e33-706">ユーザーがデバイス名を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-706">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="f3e33-707">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="f3e33-707">settingsBlockChangeRegion</span></span>|<span data-ttu-id="f3e33-708">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-708">Boolean</span></span>|<span data-ttu-id="f3e33-709">ユーザーがリージョン設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-709">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="f3e33-710">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="f3e33-710">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="f3e33-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-711">Boolean</span></span>|<span data-ttu-id="f3e33-712">ユーザーが言語の設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-712">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="f3e33-713">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="f3e33-713">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="f3e33-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-714">Boolean</span></span>|<span data-ttu-id="f3e33-715">ユーザーが電源とスリープの設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-715">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="f3e33-716">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-716">locationServicesBlocked</span></span>|<span data-ttu-id="f3e33-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-717">Boolean</span></span>|<span data-ttu-id="f3e33-718">ユーザーが位置情報サービスを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-718">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="f3e33-719">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-719">microsoftAccountBlocked</span></span>|<span data-ttu-id="f3e33-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-720">Boolean</span></span>|<span data-ttu-id="f3e33-721">Microsoft アカウントを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-721">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="f3e33-722">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="f3e33-722">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="f3e33-723">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-723">Boolean</span></span>|<span data-ttu-id="f3e33-724">Microsoft アカウントの設定の同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-724">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="f3e33-725">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-725">nfcBlocked</span></span>|<span data-ttu-id="f3e33-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-726">Boolean</span></span>|<span data-ttu-id="f3e33-727">ユーザーが近距離無線通信を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-727">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="f3e33-728">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-728">resetProtectionModeBlocked</span></span>|<span data-ttu-id="f3e33-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-729">Boolean</span></span>|<span data-ttu-id="f3e33-730">ユーザーが保護モードをリセットすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-730">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="f3e33-731">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-731">screenCaptureBlocked</span></span>|<span data-ttu-id="f3e33-732">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-732">Boolean</span></span>|<span data-ttu-id="f3e33-733">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-733">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="f3e33-734">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="f3e33-734">storageBlockRemovableStorage</span></span>|<span data-ttu-id="f3e33-735">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-735">Boolean</span></span>|<span data-ttu-id="f3e33-736">ユーザーがリムーバブル記憶域を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-736">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="f3e33-737">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="f3e33-737">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="f3e33-738">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-738">Boolean</span></span>|<span data-ttu-id="f3e33-739">モバイル デバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-739">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="f3e33-740">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-740">usbBlocked</span></span>|<span data-ttu-id="f3e33-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-741">Boolean</span></span>|<span data-ttu-id="f3e33-742">ユーザーが USB 接続を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-742">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="f3e33-743">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-743">voiceRecordingBlocked</span></span>|<span data-ttu-id="f3e33-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-744">Boolean</span></span>|<span data-ttu-id="f3e33-745">ユーザーが音声録音を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-745">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="f3e33-746">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="f3e33-746">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="f3e33-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-747">Boolean</span></span>|<span data-ttu-id="f3e33-748">Wi-Fi ホットスポットへの自動接続を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-748">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="f3e33-749">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="f3e33-749">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f3e33-750">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-750">wiFiBlocked</span></span>|<span data-ttu-id="f3e33-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-751">Boolean</span></span>|<span data-ttu-id="f3e33-752">ユーザーが Wi-Fi を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-752">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="f3e33-753">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3e33-753">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="f3e33-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-754">Boolean</span></span>|<span data-ttu-id="f3e33-755">ユーザーが Wi-Fi の手動構成を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-755">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="f3e33-756">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="f3e33-756">wiFiScanInterval</span></span>|<span data-ttu-id="f3e33-757">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e33-757">Int32</span></span>|<span data-ttu-id="f3e33-758">Wi-Fi ネットワークに対するデバイス スキャンの頻度を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-758">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="f3e33-759">サポートされている値は 1 から 500 まで、既定値は 100、500 は最低頻度です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-759">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="f3e33-760">有効な値は 1 から 500 までです</span><span class="sxs-lookup"><span data-stu-id="f3e33-760">Valid values 1 to 500</span></span>|
|<span data-ttu-id="f3e33-761">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="f3e33-761">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="f3e33-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-762">Boolean</span></span>|<span data-ttu-id="f3e33-763">他のデバイスがこの PC をプロジェクター用に検出することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-763">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="f3e33-764">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="f3e33-764">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="f3e33-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-765">Boolean</span></span>|<span data-ttu-id="f3e33-766">ワイヤレス ディスプレイ レシーバーからのユーザー入力を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-766">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="f3e33-767">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="f3e33-767">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="f3e33-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-768">Boolean</span></span>|<span data-ttu-id="f3e33-769">新しいデバイスがペアリングを開始するときに PIN が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-769">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="f3e33-770">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-770">windowsStoreBlocked</span></span>|<span data-ttu-id="f3e33-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-771">Boolean</span></span>|<span data-ttu-id="f3e33-772">ユーザーが Windows ストアを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-772">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="f3e33-773">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="f3e33-773">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="f3e33-774">statemanagementsetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-774">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="f3e33-775">信頼された証明書で署名した AppX パッケージからアプリをサイドローディングできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-775">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="f3e33-776">可能な値は `notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-776">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="f3e33-777">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="f3e33-777">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="f3e33-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-778">Boolean</span></span>|<span data-ttu-id="f3e33-779">Windows ストアからのアプリの自動更新を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-779">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="f3e33-780">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-780">developerUnlockSetting</span></span>|[<span data-ttu-id="f3e33-781">statemanagementsetting</span><span class="sxs-lookup"><span data-stu-id="f3e33-781">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="f3e33-782">開発者によるロック解除を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-782">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="f3e33-783">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-783">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="f3e33-784">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="f3e33-784">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="f3e33-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-785">Boolean</span></span>|<span data-ttu-id="f3e33-786">同じアプリの複数のユーザーによるデータ共有を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-786">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="f3e33-787">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="f3e33-787">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="f3e33-788">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-788">Boolean</span></span>|<span data-ttu-id="f3e33-789">プレインストールまたはダウンロードによって取得したすべての Windows ストア アプリの起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-789">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="f3e33-790">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="f3e33-790">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="f3e33-791">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-791">Boolean</span></span>|<span data-ttu-id="f3e33-792">プライベート ストアのみを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-792">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="f3e33-793">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="f3e33-793">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="f3e33-794">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-794">Boolean</span></span>|<span data-ttu-id="f3e33-795">アプリケーションのデータがシステム ドライブに制限されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-795">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="f3e33-796">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="f3e33-796">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="f3e33-797">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-797">Boolean</span></span>|<span data-ttu-id="f3e33-798">アプリケーションのインストールがシステム ドライブに制限されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-798">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="f3e33-799">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="f3e33-799">gameDvrBlocked</span></span>|<span data-ttu-id="f3e33-800">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-800">Boolean</span></span>|<span data-ttu-id="f3e33-801">DVR とブロードキャストを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-801">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="f3e33-802">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="f3e33-802">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="f3e33-803">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-803">Boolean</span></span>|<span data-ttu-id="f3e33-804">デバイス検出 UX を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-804">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="f3e33-805">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="f3e33-805">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="f3e33-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-806">Boolean</span></span>|<span data-ttu-id="f3e33-807">SIM カードが検出されない場合にエラー ダイアログを表示することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-807">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="f3e33-808">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="f3e33-808">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="f3e33-809">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-809">Boolean</span></span>|<span data-ttu-id="f3e33-810">デバイスでのタスクの切り替えを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-810">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="f3e33-811">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="f3e33-811">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="f3e33-812">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-812">Boolean</span></span>|<span data-ttu-id="f3e33-813">同時にログオンしているユーザー間での切り替えをログオフなしで迅速に行う機能を無効にします。</span><span class="sxs-lookup"><span data-stu-id="f3e33-813">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="f3e33-814">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="f3e33-814">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="f3e33-815">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3e33-815">Boolean</span></span>|<span data-ttu-id="f3e33-816">ネットワークへの接続にデバイスが必要かどうか。</span><span class="sxs-lookup"><span data-stu-id="f3e33-816">Whether the device is required to connect to the network.</span></span>|



## <a name="response"></a><span data-ttu-id="f3e33-817">応答</span><span class="sxs-lookup"><span data-stu-id="f3e33-817">Response</span></span>
<span data-ttu-id="f3e33-818">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3e33-818">If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3e33-819">例</span><span class="sxs-lookup"><span data-stu-id="f3e33-819">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3e33-820">要求</span><span class="sxs-lookup"><span data-stu-id="f3e33-820">Request</span></span>
<span data-ttu-id="f3e33-821">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3e33-821">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9822

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
  "edgeSendIntranetTrafficToInternetExplorer": true,
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

### <a name="response"></a><span data-ttu-id="f3e33-822">応答</span><span class="sxs-lookup"><span data-stu-id="f3e33-822">Response</span></span>
<span data-ttu-id="f3e33-p158">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3e33-p158">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9994

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
  "edgeSendIntranetTrafficToInternetExplorer": true,
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



