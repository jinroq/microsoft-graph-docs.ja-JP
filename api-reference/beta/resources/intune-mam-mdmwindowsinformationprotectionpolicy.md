---
title: mdmWindowsInformationProtectionPolicy リソース タイプ
description: MDM を使用する Windows 情報保護のポリシー
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 600d01f780274ba00b17355f83692cb1a9581e43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998330"
---
# <a name="mdmwindowsinformationprotectionpolicy-resource-type"></a><span data-ttu-id="b39eb-103">mdmWindowsInformationProtectionPolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="b39eb-103">mdmWindowsInformationProtectionPolicy resource type</span></span>

> <span data-ttu-id="b39eb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b39eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b39eb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b39eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b39eb-106">MDM を使用する Windows 情報保護のポリシー</span><span class="sxs-lookup"><span data-stu-id="b39eb-106">Policy for Windows information protection with MDM</span></span>


<span data-ttu-id="b39eb-107">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-107">Inherits from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b39eb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b39eb-108">Methods</span></span>
|<span data-ttu-id="b39eb-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b39eb-109">Method</span></span>|<span data-ttu-id="b39eb-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b39eb-110">Return Type</span></span>|<span data-ttu-id="b39eb-111">説明</span><span class="sxs-lookup"><span data-stu-id="b39eb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b39eb-112">List mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="b39eb-112">List mdmWindowsInformationProtectionPolicies</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-list.md)|<span data-ttu-id="b39eb-113">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-113">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="b39eb-114">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b39eb-114">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>|
|[<span data-ttu-id="b39eb-115">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b39eb-115">Get mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-get.md)|[<span data-ttu-id="b39eb-116">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b39eb-116">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="b39eb-117">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b39eb-117">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="b39eb-118">Create mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b39eb-118">Create mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-create.md)|[<span data-ttu-id="b39eb-119">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b39eb-119">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="b39eb-120">新しい [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b39eb-120">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|
|[<span data-ttu-id="b39eb-121">Delete mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b39eb-121">Delete mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-delete.md)|<span data-ttu-id="b39eb-122">なし</span><span class="sxs-lookup"><span data-stu-id="b39eb-122">None</span></span>|<span data-ttu-id="b39eb-123">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b39eb-123">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>|
|[<span data-ttu-id="b39eb-124">Update mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b39eb-124">Update mdmWindowsInformationProtectionPolicy</span></span>](../api/intune-mam-mdmwindowsinformationprotectionpolicy-update.md)|[<span data-ttu-id="b39eb-125">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b39eb-125">mdmWindowsInformationProtectionPolicy</span></span>](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|<span data-ttu-id="b39eb-126">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b39eb-126">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b39eb-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b39eb-127">Properties</span></span>
|<span data-ttu-id="b39eb-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b39eb-128">Property</span></span>|<span data-ttu-id="b39eb-129">型</span><span class="sxs-lookup"><span data-stu-id="b39eb-129">Type</span></span>|<span data-ttu-id="b39eb-130">説明</span><span class="sxs-lookup"><span data-stu-id="b39eb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b39eb-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b39eb-131">displayName</span></span>|<span data-ttu-id="b39eb-132">String</span><span class="sxs-lookup"><span data-stu-id="b39eb-132">String</span></span>|<span data-ttu-id="b39eb-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="b39eb-133">Policy display name.</span></span> <span data-ttu-id="b39eb-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b39eb-135">description</span><span class="sxs-lookup"><span data-stu-id="b39eb-135">description</span></span>|<span data-ttu-id="b39eb-136">String</span><span class="sxs-lookup"><span data-stu-id="b39eb-136">String</span></span>|<span data-ttu-id="b39eb-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="b39eb-137">The policy's description.</span></span> <span data-ttu-id="b39eb-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b39eb-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b39eb-139">createdDateTime</span></span>|<span data-ttu-id="b39eb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b39eb-140">DateTimeOffset</span></span>|<span data-ttu-id="b39eb-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b39eb-141">The date and time the policy was created.</span></span> <span data-ttu-id="b39eb-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b39eb-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b39eb-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b39eb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b39eb-144">DateTimeOffset</span></span>|<span data-ttu-id="b39eb-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="b39eb-145">Last time the policy was modified.</span></span> <span data-ttu-id="b39eb-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b39eb-147">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b39eb-147">roleScopeTagIds</span></span>|<span data-ttu-id="b39eb-148">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-148">String collection</span></span>|<span data-ttu-id="b39eb-149">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b39eb-149">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b39eb-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b39eb-151">id</span><span class="sxs-lookup"><span data-stu-id="b39eb-151">id</span></span>|<span data-ttu-id="b39eb-152">文字列</span><span class="sxs-lookup"><span data-stu-id="b39eb-152">String</span></span>|<span data-ttu-id="b39eb-153">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b39eb-153">Key of the entity.</span></span> <span data-ttu-id="b39eb-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b39eb-155">version</span><span class="sxs-lookup"><span data-stu-id="b39eb-155">version</span></span>|<span data-ttu-id="b39eb-156">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b39eb-156">String</span></span>|<span data-ttu-id="b39eb-157">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b39eb-157">Version of the entity.</span></span> <span data-ttu-id="b39eb-158">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b39eb-159">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="b39eb-159">enforcementLevel</span></span>|[<span data-ttu-id="b39eb-160">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="b39eb-160">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="b39eb-161">仕掛品の実施レベル。[Windowsinformationprotection](../resources/intune-mam-windowsinformationprotection.md)から継承した、サポートされている値の列挙定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b39eb-161">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="b39eb-162">使用可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。</span><span class="sxs-lookup"><span data-stu-id="b39eb-162">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="b39eb-163">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="b39eb-163">enterpriseDomain</span></span>|<span data-ttu-id="b39eb-164">String</span><span class="sxs-lookup"><span data-stu-id="b39eb-164">String</span></span>|<span data-ttu-id="b39eb-165">プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-165">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-166">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="b39eb-166">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="b39eb-167">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-167">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b39eb-168">保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-168">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-169">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="b39eb-169">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="b39eb-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39eb-170">Boolean</span></span>|<span data-ttu-id="b39eb-171">ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-171">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-172">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="b39eb-172">dataRecoveryCertificate</span></span>|[<span data-ttu-id="b39eb-173">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="b39eb-173">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="b39eb-174">暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。</span><span class="sxs-lookup"><span data-stu-id="b39eb-174">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="b39eb-175">これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-175">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-176">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="b39eb-176">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="b39eb-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39eb-177">Boolean</span></span>|<span data-ttu-id="b39eb-178">このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="b39eb-178">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="b39eb-179">1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b39eb-179">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="b39eb-180">キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。</span><span class="sxs-lookup"><span data-stu-id="b39eb-180">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="b39eb-181">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-181">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-182">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="b39eb-182">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="b39eb-183">GUID</span><span class="sxs-lookup"><span data-stu-id="b39eb-183">Guid</span></span>|<span data-ttu-id="b39eb-184">RMS の暗号化に使用する TemplateID GUID。</span><span class="sxs-lookup"><span data-stu-id="b39eb-184">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="b39eb-185">RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-185">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-186">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="b39eb-186">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="b39eb-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39eb-187">Boolean</span></span>|<span data-ttu-id="b39eb-188">WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-188">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-189">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="b39eb-189">iconsVisible</span></span>|<span data-ttu-id="b39eb-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39eb-190">Boolean</span></span>|<span data-ttu-id="b39eb-191">エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b39eb-191">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="b39eb-192">Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-192">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-193">protectedApps</span><span class="sxs-lookup"><span data-stu-id="b39eb-193">protectedApps</span></span>|<span data-ttu-id="b39eb-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="b39eb-195">保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-195">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-196">exemptApps</span><span class="sxs-lookup"><span data-stu-id="b39eb-196">exemptApps</span></span>|<span data-ttu-id="b39eb-197">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-197">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="b39eb-198">適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。</span><span class="sxs-lookup"><span data-stu-id="b39eb-198">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="b39eb-199">これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="b39eb-199">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="b39eb-200">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-200">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-201">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="b39eb-201">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="b39eb-202">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-202">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b39eb-203">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="b39eb-203">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="b39eb-204">デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-204">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-205">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="b39eb-205">enterpriseProxiedDomains</span></span>|<span data-ttu-id="b39eb-206">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-206">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="b39eb-207">保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b39eb-207">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="b39eb-208">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="b39eb-208">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="b39eb-209">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="b39eb-209">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="b39eb-210">この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-210">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-211">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="b39eb-211">enterpriseIPRanges</span></span>|<span data-ttu-id="b39eb-212">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-212">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="b39eb-213">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="b39eb-213">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="b39eb-214">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="b39eb-214">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="b39eb-215">これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-215">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-216">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="b39eb-216">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="b39eb-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39eb-217">Boolean</span></span>|<span data-ttu-id="b39eb-218">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="b39eb-218">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="b39eb-219">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-219">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-220">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="b39eb-220">enterpriseProxyServers</span></span>|<span data-ttu-id="b39eb-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b39eb-222">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="b39eb-222">This is a list of proxy servers.</span></span> <span data-ttu-id="b39eb-223">このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-223">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-224">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="b39eb-224">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="b39eb-225">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-225">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b39eb-226">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="b39eb-226">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="b39eb-227">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="b39eb-227">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="b39eb-228">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="b39eb-228">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="b39eb-229">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="b39eb-229">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="b39eb-230">これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-230">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-231">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="b39eb-231">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="b39eb-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39eb-232">Boolean</span></span>|<span data-ttu-id="b39eb-233">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="b39eb-233">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="b39eb-234">既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-234">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-235">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="b39eb-235">neutralDomainResources</span></span>|<span data-ttu-id="b39eb-236">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-236">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b39eb-237">職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-237">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-238">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="b39eb-238">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="b39eb-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39eb-239">Boolean</span></span>|<span data-ttu-id="b39eb-240">このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-240">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-241">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="b39eb-241">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="b39eb-242">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-242">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b39eb-243">企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-243">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-244">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b39eb-244">isAssigned</span></span>|<span data-ttu-id="b39eb-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39eb-245">Boolean</span></span>|<span data-ttu-id="b39eb-246">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b39eb-246">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="b39eb-247">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-247">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b39eb-248">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b39eb-248">Relationships</span></span>
|<span data-ttu-id="b39eb-249">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b39eb-249">Relationship</span></span>|<span data-ttu-id="b39eb-250">型</span><span class="sxs-lookup"><span data-stu-id="b39eb-250">Type</span></span>|<span data-ttu-id="b39eb-251">説明</span><span class="sxs-lookup"><span data-stu-id="b39eb-251">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b39eb-252">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="b39eb-252">protectedAppLockerFiles</span></span>|<span data-ttu-id="b39eb-253">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-253">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="b39eb-254">xml ファイルを使用して、保護されたアプリを入力する別の方法 ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-254">Another way to input protected apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-255">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="b39eb-255">exemptAppLockerFiles</span></span>|<span data-ttu-id="b39eb-256">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-256">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="b39eb-257">xml ファイルを使用して、保護されていないアプリを入力する別の方法 ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b39eb-257">Another way to input exempt apps through xml files Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b39eb-258">assignments</span><span class="sxs-lookup"><span data-stu-id="b39eb-258">assignments</span></span>|<span data-ttu-id="b39eb-259">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b39eb-259">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="b39eb-260">ポリシーを対象とするセキュリティ グループのリストへのナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="b39eb-260">Navigation property to list of security groups targeted for policy.</span></span> <span data-ttu-id="b39eb-261">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b39eb-261">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b39eb-262">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b39eb-262">JSON Representation</span></span>
<span data-ttu-id="b39eb-263">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b39eb-263">Here is a JSON representation of the resource.</span></span>
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





