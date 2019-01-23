---
title: mdmWindowsInformationProtectionPolicy リソース タイプ
description: MDM を使用する Windows 情報保護のポリシー
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 60bd38174777342436095d222a36dadeb2d67437
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424785"
---
# <a name="mdmwindowsinformationprotectionpolicy-resource-type"></a><span data-ttu-id="c1c11-103">mdmWindowsInformationProtectionPolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c1c11-103">mdmWindowsInformationProtectionPolicy resource type</span></span>

> <span data-ttu-id="c1c11-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1c11-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1c11-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1c11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1c11-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1c11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1c11-107">MDM を使用する Windows 情報保護のポリシー</span><span class="sxs-lookup"><span data-stu-id="c1c11-107">Policy for Windows information protection with MDM</span></span>


<span data-ttu-id="c1c11-108">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-108">Inherits from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c1c11-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1c11-109">Methods</span></span>
|<span data-ttu-id="c1c11-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1c11-110">Method</span></span>|<span data-ttu-id="c1c11-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c1c11-111">Return Type</span></span>|<span data-ttu-id="c1c11-112">説明</span><span class="sxs-lookup"><span data-stu-id="c1c11-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c1c11-113">List mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="c1c11-113">List mdmWindowsInformationProtectionPolicies</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-list.md)|<span data-ttu-id="c1c11-114">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-114">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="c1c11-115">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c1c11-115">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>|
|[<span data-ttu-id="c1c11-116">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c1c11-116">Get mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-get.md)|[<span data-ttu-id="c1c11-117">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c1c11-117">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="c1c11-118">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c1c11-118">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="c1c11-119">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c1c11-119">Create mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-create.md)|[<span data-ttu-id="c1c11-120">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c1c11-120">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="c1c11-121">新しい [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c1c11-121">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="c1c11-122">Delete mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c1c11-122">Delete mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-delete.md)|<span data-ttu-id="c1c11-123">なし</span><span class="sxs-lookup"><span data-stu-id="c1c11-123">None</span></span>|<span data-ttu-id="c1c11-124">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c1c11-124">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>|
|[<span data-ttu-id="c1c11-125">Update mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c1c11-125">Update mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-update.md)|[<span data-ttu-id="c1c11-126">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c1c11-126">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="c1c11-127">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c1c11-127">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1c11-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1c11-128">Properties</span></span>
|<span data-ttu-id="c1c11-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1c11-129">Property</span></span>|<span data-ttu-id="c1c11-130">型</span><span class="sxs-lookup"><span data-stu-id="c1c11-130">Type</span></span>|<span data-ttu-id="c1c11-131">説明</span><span class="sxs-lookup"><span data-stu-id="c1c11-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c11-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c1c11-132">displayName</span></span>|<span data-ttu-id="c1c11-133">String</span><span class="sxs-lookup"><span data-stu-id="c1c11-133">String</span></span>|<span data-ttu-id="c1c11-134">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="c1c11-134">Policy display name.</span></span> <span data-ttu-id="c1c11-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c1c11-136">説明</span><span class="sxs-lookup"><span data-stu-id="c1c11-136">description</span></span>|<span data-ttu-id="c1c11-137">String</span><span class="sxs-lookup"><span data-stu-id="c1c11-137">String</span></span>|<span data-ttu-id="c1c11-138">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="c1c11-138">The policy's description.</span></span> <span data-ttu-id="c1c11-139">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c1c11-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1c11-140">createdDateTime</span></span>|<span data-ttu-id="c1c11-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1c11-141">DateTimeOffset</span></span>|<span data-ttu-id="c1c11-142">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c1c11-142">The date and time the policy was created.</span></span> <span data-ttu-id="c1c11-143">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c1c11-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1c11-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c1c11-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1c11-145">DateTimeOffset</span></span>|<span data-ttu-id="c1c11-146">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="c1c11-146">Last time the policy was modified.</span></span> <span data-ttu-id="c1c11-147">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c1c11-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1c11-148">roleScopeTagIds</span></span>|<span data-ttu-id="c1c11-149">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-149">String collection</span></span>|<span data-ttu-id="c1c11-150">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="c1c11-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1c11-151">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c1c11-152">id</span><span class="sxs-lookup"><span data-stu-id="c1c11-152">id</span></span>|<span data-ttu-id="c1c11-153">String</span><span class="sxs-lookup"><span data-stu-id="c1c11-153">String</span></span>|<span data-ttu-id="c1c11-154">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c1c11-154">Key of the entity.</span></span> <span data-ttu-id="c1c11-155">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c1c11-156">version</span><span class="sxs-lookup"><span data-stu-id="c1c11-156">version</span></span>|<span data-ttu-id="c1c11-157">String</span><span class="sxs-lookup"><span data-stu-id="c1c11-157">String</span></span>|<span data-ttu-id="c1c11-158">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c1c11-158">Version of the entity.</span></span> <span data-ttu-id="c1c11-159">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c1c11-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="c1c11-160">enforcementLevel</span></span>|[<span data-ttu-id="c1c11-161">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="c1c11-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="c1c11-162">WIP の適用レベルです。[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)からサポートされている値継承の列挙型定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1c11-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="c1c11-163">可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="c1c11-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="c1c11-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="c1c11-164">enterpriseDomain</span></span>|<span data-ttu-id="c1c11-165">String</span><span class="sxs-lookup"><span data-stu-id="c1c11-165">String</span></span>|<span data-ttu-id="c1c11-166">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="c1c11-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="c1c11-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c1c11-169">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="c1c11-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="c1c11-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1c11-171">Boolean</span></span>|<span data-ttu-id="c1c11-172">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="c1c11-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="c1c11-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="c1c11-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="c1c11-175">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="c1c11-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="c1c11-176">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="c1c11-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="c1c11-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1c11-178">Boolean</span></span>|<span data-ttu-id="c1c11-179">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="c1c11-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="c1c11-180">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="c1c11-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="c1c11-181">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="c1c11-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="c1c11-182">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="c1c11-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="c1c11-184">Guid</span><span class="sxs-lookup"><span data-stu-id="c1c11-184">Guid</span></span>|<span data-ttu-id="c1c11-185">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="c1c11-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="c1c11-186">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="c1c11-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="c1c11-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1c11-188">Boolean</span></span>|<span data-ttu-id="c1c11-189">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="c1c11-190">iconsVisible</span></span>|<span data-ttu-id="c1c11-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1c11-191">Boolean</span></span>|<span data-ttu-id="c1c11-192">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="c1c11-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="c1c11-193">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="c1c11-194">protectedApps</span></span>|<span data-ttu-id="c1c11-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="c1c11-196">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="c1c11-197">exemptApps</span></span>|<span data-ttu-id="c1c11-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="c1c11-199">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="c1c11-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="c1c11-200">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="c1c11-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="c1c11-201">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="c1c11-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="c1c11-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c1c11-204">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="c1c11-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="c1c11-205">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="c1c11-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="c1c11-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="c1c11-208">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c1c11-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="c1c11-209">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="c1c11-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="c1c11-210">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="c1c11-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="c1c11-211">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="c1c11-212">enterpriseIPRanges</span></span>|<span data-ttu-id="c1c11-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="c1c11-214">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="c1c11-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="c1c11-215">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="c1c11-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="c1c11-216">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="c1c11-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="c1c11-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1c11-218">Boolean</span></span>|<span data-ttu-id="c1c11-219">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="c1c11-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="c1c11-220">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="c1c11-221">enterpriseProxyServers</span></span>|<span data-ttu-id="c1c11-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c1c11-223">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="c1c11-223">This is a list of proxy servers.</span></span> <span data-ttu-id="c1c11-224">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="c1c11-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="c1c11-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c1c11-227">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="c1c11-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="c1c11-228">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="c1c11-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="c1c11-229">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="c1c11-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="c1c11-230">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="c1c11-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="c1c11-231">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="c1c11-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="c1c11-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1c11-233">Boolean</span></span>|<span data-ttu-id="c1c11-234">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="c1c11-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="c1c11-235">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="c1c11-236">neutralDomainResources</span></span>|<span data-ttu-id="c1c11-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c1c11-238">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="c1c11-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="c1c11-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1c11-240">Boolean</span></span>|<span data-ttu-id="c1c11-241">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="c1c11-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="c1c11-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c1c11-244">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c1c11-245">isAssigned</span></span>|<span data-ttu-id="c1c11-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1c11-246">Boolean</span></span>|<span data-ttu-id="c1c11-247">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c1c11-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="c1c11-248">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1c11-249">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1c11-249">Relationships</span></span>
|<span data-ttu-id="c1c11-250">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1c11-250">Relationship</span></span>|<span data-ttu-id="c1c11-251">型</span><span class="sxs-lookup"><span data-stu-id="c1c11-251">Type</span></span>|<span data-ttu-id="c1c11-252">説明</span><span class="sxs-lookup"><span data-stu-id="c1c11-252">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c11-253">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="c1c11-253">protectedAppLockerFiles</span></span>|<span data-ttu-id="c1c11-254">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-254">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="c1c11-255">xml ファイルを使用して、保護されたアプリを入力する別の方法 ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-255">Another way to input protected apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-256">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="c1c11-256">exemptAppLockerFiles</span></span>|<span data-ttu-id="c1c11-257">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-257">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="c1c11-258">xml ファイルを使用して、保護されていないアプリを入力する別の方法 ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c1c11-258">Another way to input exempt apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c1c11-259">assignments</span><span class="sxs-lookup"><span data-stu-id="c1c11-259">assignments</span></span>|<span data-ttu-id="c1c11-260">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c1c11-260">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="c1c11-261">ポリシーを対象とするセキュリティ グループのリストへのナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="c1c11-261">Navigation property to list of security groups targeted for policy.</span></span> <span data-ttu-id="c1c11-262">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1c11-262">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1c11-263">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1c11-263">JSON Representation</span></span>
<span data-ttu-id="c1c11-264">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1c11-264">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```




