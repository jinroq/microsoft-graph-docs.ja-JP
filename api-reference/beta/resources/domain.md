---
title: ドメイン リソースの種類
description: テナントに関連付けられているドメインを表します。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 3aeede3a796bfdf6019e4cb840e6b7a949d96b20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849512"
---
# <a name="domain-resource-type"></a><span data-ttu-id="6c583-103">ドメイン リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c583-103">domain resource type</span></span>

> <span data-ttu-id="6c583-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c583-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c583-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c583-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c583-106">テナントに関連付けられているドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="6c583-106">Represents a domain associated with the tenant.</span></span>

<span data-ttu-id="6c583-p102">ドメイン操作を使用して、テナントにドメインを関連付け、ドメインの所有権を確認し、サポートされているサービスを構成します。ドメイン操作によって Office 365 などのサービスのドメインの関連付けを自動化するレジストラーを有効にします。たとえば、ドメインのサインアップの一部として、レジストラーは電子メール、Web サイト、認証などのバニティ ドメインを有効化することができます。</span><span class="sxs-lookup"><span data-stu-id="6c583-p102">Use domain operations to associate domains to a tenant, verify domain ownership, and configure supported services.  Domain operations enable registrars to automate domain association for services such as Office 365. For example, as part of domain sign up, a registrar can enable a vanity domain for email, websites, authentication, etc.</span></span>

<span data-ttu-id="6c583-110">ドメインをテナントに関連付ける方法：</span><span class="sxs-lookup"><span data-stu-id="6c583-110">To associate a domain with a tenant:</span></span>

1. <span data-ttu-id="6c583-111">ドメインをテナントに[関連付ける](../api/domain-post-domains.md)。</span><span class="sxs-lookup"><span data-stu-id="6c583-111">[Associate](../api/domain-post-domains.md) a domain with a tenant.</span></span>

2. <span data-ttu-id="6c583-p103">ドメインの検証レコードを[取得する](../api/domain-list-verificationdnsrecords.md)。ドメイン レジストラーまたは DNS サーバー構成を使用して、検証レコードの詳細情報をドメインのゾーン ファイルに追加します。</span><span class="sxs-lookup"><span data-stu-id="6c583-p103">[Retrieve](../api/domain-list-verificationdnsrecords.md) the domain verification records. Add the verification record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

3. <span data-ttu-id="6c583-p104">ドメインの所有権を[検証する](../api/domain-verify.md)。ドメインを確認し、*isVerified* プロパティを *true* に設定します。</span><span class="sxs-lookup"><span data-stu-id="6c583-p104">[Verify](../api/domain-verify.md) the ownership of the domain. This will verify the domain and set the *isVerified* property to *true*.</span></span>

4. <span data-ttu-id="6c583-116">ドメインと共に使用する、サポートされているサービスを[指定する](../api/domain-update.md)。</span><span class="sxs-lookup"><span data-stu-id="6c583-116">[Indicate](../api/domain-update.md) the supported services you plan to use with the domain.</span></span>

5. <span data-ttu-id="6c583-p105">ドメイン向けのサービスを有効にするのに必要なレコードの一覧を取得して、サポートされているサービスを[構成する](../api/domain-list-serviceconfigurationrecords.md)。ドメイン レジストラーまたは DNS サーバー構成を使用して、構成レコードの詳細情報をドメインのゾーン ファイルに追加します。</span><span class="sxs-lookup"><span data-stu-id="6c583-p105">[Configure](../api/domain-list-serviceconfigurationrecords.md) supported services by retrieving a list of records needed to enable services for the domain. Add the configuration record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="6c583-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c583-119">Methods</span></span>

| <span data-ttu-id="6c583-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c583-120">Method</span></span>   | <span data-ttu-id="6c583-121">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6c583-121">Return Type</span></span> |<span data-ttu-id="6c583-122">説明</span><span class="sxs-lookup"><span data-stu-id="6c583-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c583-123">Get domain</span><span class="sxs-lookup"><span data-stu-id="6c583-123">Get domain</span></span>](../api/domain-get.md) | [<span data-ttu-id="6c583-124">domain</span><span class="sxs-lookup"><span data-stu-id="6c583-124">domain</span></span>](domain.md) | <span data-ttu-id="6c583-125">ドメイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6c583-125">Read properties and relationships of a domain object.</span></span>|
|[<span data-ttu-id="6c583-126">Create domain</span><span class="sxs-lookup"><span data-stu-id="6c583-126">Create domain</span></span>](../api/domain-post-domains.md) | [<span data-ttu-id="6c583-127">domain</span><span class="sxs-lookup"><span data-stu-id="6c583-127">domain</span></span>](domain.md) | <span data-ttu-id="6c583-128">テナントにドメインを追加します。</span><span class="sxs-lookup"><span data-stu-id="6c583-128">Adds a domain to the tenant.</span></span> |
|[<span data-ttu-id="6c583-129">List domainNameReference</span><span class="sxs-lookup"><span data-stu-id="6c583-129">List domainNameReference</span></span>](../api/domain-list-domainnamereferences.md) |<span data-ttu-id="6c583-130">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c583-130">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="6c583-131">ドメインへの参照付きのディレクトリ オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="6c583-131">Retrieve a list of directory objects with a reference to the domain.</span></span>|
|[<span data-ttu-id="6c583-132">List serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="6c583-132">List serviceConfigurationRecords</span></span>](../api/domain-list-serviceconfigurationrecords.md) |<span data-ttu-id="6c583-133">[domainDnsRecord](domaindnsrecord.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c583-133">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="6c583-134">ドメイン構成のためドメインの DNS レコードの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="6c583-134">Retrieve a list of domain DNS records for domain configuration.</span></span>|
|[<span data-ttu-id="6c583-135">List verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="6c583-135">List verificationDnsRecords</span></span>](../api/domain-list-verificationdnsrecords.md) |<span data-ttu-id="6c583-136">[domainDnsRecord](domaindnsrecord.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c583-136">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="6c583-137">ドメイン検証のためドメインの DNS レコードの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="6c583-137">Retrieve a list of domain DNS records for domain verification.</span></span>|
|[<span data-ttu-id="6c583-138">Update domain</span><span class="sxs-lookup"><span data-stu-id="6c583-138">Update domain</span></span>](../api/domain-update.md) | [<span data-ttu-id="6c583-139">domain</span><span class="sxs-lookup"><span data-stu-id="6c583-139">domain</span></span>](domain.md) |<span data-ttu-id="6c583-140">ドメインを更新します</span><span class="sxs-lookup"><span data-stu-id="6c583-140">Updates a domain.</span></span>|
|[<span data-ttu-id="6c583-141">Delete domain</span><span class="sxs-lookup"><span data-stu-id="6c583-141">Delete domain</span></span>](../api/domain-delete.md) | <span data-ttu-id="6c583-142">なし</span><span class="sxs-lookup"><span data-stu-id="6c583-142">None</span></span> |<span data-ttu-id="6c583-143">ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="6c583-143">Deletes a domain.</span></span>|
|[<span data-ttu-id="6c583-144">ForceDelete ドメイン</span><span class="sxs-lookup"><span data-stu-id="6c583-144">ForceDelete domain</span></span>](../api/domain-forcedelete.md)|<span data-ttu-id="6c583-145">なし</span><span class="sxs-lookup"><span data-stu-id="6c583-145">None</span></span>|<span data-ttu-id="6c583-146">非同期操作を使用してドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="6c583-146">Deletes a domain using an asynchronous operation.</span></span>|
|[<span data-ttu-id="6c583-147">Verify domain</span><span class="sxs-lookup"><span data-stu-id="6c583-147">Verify domain</span></span>](../api/domain-verify.md)|[<span data-ttu-id="6c583-148">domain</span><span class="sxs-lookup"><span data-stu-id="6c583-148">domain</span></span>](domain.md)|<span data-ttu-id="6c583-149">ドメインの所有権を検証します。</span><span class="sxs-lookup"><span data-stu-id="6c583-149">Validates the ownership of the domain.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c583-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c583-150">Properties</span></span>

| <span data-ttu-id="6c583-151">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c583-151">Property</span></span>   | <span data-ttu-id="6c583-152">種類</span><span class="sxs-lookup"><span data-stu-id="6c583-152">Type</span></span> | <span data-ttu-id="6c583-153">説明</span><span class="sxs-lookup"><span data-stu-id="6c583-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6c583-154">authenticationType</span><span class="sxs-lookup"><span data-stu-id="6c583-154">authenticationType</span></span>|<span data-ttu-id="6c583-155">String</span><span class="sxs-lookup"><span data-stu-id="6c583-155">String</span></span>| <span data-ttu-id="6c583-p106">ドメインに対して構成されている認証の種類を示します。値は、*Managed* または *Federated* のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="6c583-p106">Indicates the configured authentication type for the domain. The value is either *Managed* or *Federated*.</span></span><br> <span data-ttu-id="6c583-158">*Managed* の場合、Azure AD がユーザー認証を実行するクラウド管理のドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="6c583-158">*Managed* indicates a cloud managed domain where Azure AD performs user authentication.</span></span><br><span data-ttu-id="6c583-p107">*Federated* の場合、Active Directory フェデレーション サービスを経由したテナントのオンプレミスの Active Directory のように、認証が ID プロバイダーとフェデレーションを行うことを表します。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="6c583-p107">*Federated* indicates authentication is federated with an identity provider such as the tenant's on-premises Active Directory via Active Directory Federation Services. Not nullable</span></span> |
|<span data-ttu-id="6c583-161">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="6c583-161">availabilityStatus</span></span>|<span data-ttu-id="6c583-162">String</span><span class="sxs-lookup"><span data-stu-id="6c583-162">String</span></span>| <span data-ttu-id="6c583-p108">[確認](../api/domain-verify.md)操作を使用する場合を除き、このプロパティは常に null です。[確認](../api/domain-verify.md)操作を使用する場合、応答で**ドメイン** エンティティが返されます。応答内の、**ドメイン** エンティティの **availabilityStatus** プロパティは、*AvailableImmediately* または *EmailVerifiedDomainTakeoverScheduled* のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="6c583-p108">This property is always null except when the [verify](../api/domain-verify.md) action is used. When the [verify](../api/domain-verify.md) action is used, a **domain** entity is returned in the response. The **availabilityStatus** property of the **domain** entity in the response is either *AvailableImmediately* or *EmailVerifiedDomainTakeoverScheduled*.</span></span>|
|<span data-ttu-id="6c583-166">id</span><span class="sxs-lookup"><span data-stu-id="6c583-166">id</span></span>|<span data-ttu-id="6c583-167">String</span><span class="sxs-lookup"><span data-stu-id="6c583-167">String</span></span>| <span data-ttu-id="6c583-p109">ドメインの完全修飾名です。キー、不変、Null 許容ではない、一意</span><span class="sxs-lookup"><span data-stu-id="6c583-p109">The fully qualified name of the domain. Key, immutable, not nullable, unique</span></span> |
|<span data-ttu-id="6c583-170">isAdminManaged</span><span class="sxs-lookup"><span data-stu-id="6c583-170">isAdminManaged</span></span>|<span data-ttu-id="6c583-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c583-171">Boolean</span></span>| <span data-ttu-id="6c583-p110">ドメインの DNS レコードの管理が Office 365 に委任されている場合、プロパティの値は false です。それ以外の場合、値は true です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="6c583-p110">The value of the property is false if the DNS record management of the domain has been delegated to Office 365. Otherwise, the value is true. Not nullable</span></span> |
|<span data-ttu-id="6c583-175">isDefault</span><span class="sxs-lookup"><span data-stu-id="6c583-175">isDefault</span></span>|<span data-ttu-id="6c583-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c583-176">Boolean</span></span>| <span data-ttu-id="6c583-p111">ユーザーの作成に使用する既定のドメインの場合は true です。会社ごとに 1 つだけの既定のドメインがあります。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="6c583-p111">True if this is the default domain that is used for user creation. There is only one default domain per company. Not nullable</span></span> |
|<span data-ttu-id="6c583-180">isInitial</span><span class="sxs-lookup"><span data-stu-id="6c583-180">isInitial</span></span>|<span data-ttu-id="6c583-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c583-181">Boolean</span></span>| <span data-ttu-id="6c583-p112">Microsoft Online Services (companyname.onmicrosoft.com) によって作成された初期ドメインがある場合は true です。会社ごとに 1 つだけの初期ドメインがあります。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="6c583-p112">True if this is the initial domain created by Microsoft Online Services (companyname.onmicrosoft.com). There is only one initial domain per company. Not nullable</span></span> |
|<span data-ttu-id="6c583-185">isRoot</span><span class="sxs-lookup"><span data-stu-id="6c583-185">isRoot</span></span>|<span data-ttu-id="6c583-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c583-186">Boolean</span></span>| <span data-ttu-id="6c583-p113">ドメインが検証済みのルート ドメインである場合は true です。それ以外に、ドメインがサブドメインまたは未確認である場合は false です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="6c583-p113">True if the domain is a verified root domain. Otherwise, false if the domain is a subdomain or unverified. Not nullable</span></span> |
|<span data-ttu-id="6c583-190">isVerified</span><span class="sxs-lookup"><span data-stu-id="6c583-190">isVerified</span></span>|<span data-ttu-id="6c583-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c583-191">Boolean</span></span>| <span data-ttu-id="6c583-p114">そのドメインが、ドメイン所有権の確認を完了している場合は true です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="6c583-p114">True if the domain has completed domain ownership verification. Not nullable</span></span> |
|<span data-ttu-id="6c583-194">supportedServices</span><span class="sxs-lookup"><span data-stu-id="6c583-194">supportedServices</span></span>|<span data-ttu-id="6c583-195">String collection</span><span class="sxs-lookup"><span data-stu-id="6c583-195">String collection</span></span>| <span data-ttu-id="6c583-196">ドメインに割り当てられている機能です。</span><span class="sxs-lookup"><span data-stu-id="6c583-196">The capabilities assigned to the domain.</span></span><br><br><span data-ttu-id="6c583-197">0、1 または次の値を含めることができます。*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="6c583-197">Can include 0, 1 or more of following values: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span><br><br> <span data-ttu-id="6c583-198">Graph API を使用して追加または削除できる値は次のとおりです。*Email*、*OfficeCommunicationsOnline*、*Yammer*</span><span class="sxs-lookup"><span data-stu-id="6c583-198">The values which you can add/remove using Graph API include: *Email*, *OfficeCommunicationsOnline*, *Yammer*</span></span><br><span data-ttu-id="6c583-199">null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="6c583-199">Not nullable</span></span>|
|<span data-ttu-id="6c583-200">state</span><span class="sxs-lookup"><span data-stu-id="6c583-200">state</span></span>|[<span data-ttu-id="6c583-201">domainState</span><span class="sxs-lookup"><span data-stu-id="6c583-201">domainState</span></span>](domainstate.md)| <span data-ttu-id="6c583-202">ドメインのためにスケジュールされている非同期操作の状態です。</span><span class="sxs-lookup"><span data-stu-id="6c583-202">Status of asynchronous operations scheduled for the domain.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6c583-203">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c583-203">Relationships</span></span>

<span data-ttu-id="6c583-p115">検証レコードやサービス構成のレコードなど、ディレクトリ内のドメインと他のオブジェクト間のリレーションシップは、ナビゲーション プロパティを介して公開されます。要求でこれらのナビゲーション プロパティを対象にすれば、そのリレーションシップを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="6c583-p115">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties. You can read these relationships by targeting these navigation properties in your requests.</span></span>

| <span data-ttu-id="6c583-206">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c583-206">Relationship</span></span> | <span data-ttu-id="6c583-207">型</span><span class="sxs-lookup"><span data-stu-id="6c583-207">Type</span></span> |<span data-ttu-id="6c583-208">説明</span><span class="sxs-lookup"><span data-stu-id="6c583-208">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c583-209">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="6c583-209">domainNameReferences</span></span>|<span data-ttu-id="6c583-210">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c583-210">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="6c583-211">読み取り専用、Null 許容型</span><span class="sxs-lookup"><span data-stu-id="6c583-211">Read-only, Nullable</span></span>|
|<span data-ttu-id="6c583-212">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="6c583-212">serviceConfigurationRecords</span></span>|<span data-ttu-id="6c583-213">[domainDnsRecord](domaindnsrecord.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c583-213">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="6c583-214">ドメインを Microsoft Online Services で使用する前に、顧客がそのドメインの DNS ゾーン ファイルに追加する DNS レコードです。</span><span class="sxs-lookup"><span data-stu-id="6c583-214">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="6c583-215">読み取り専用、Null 許容型</span><span class="sxs-lookup"><span data-stu-id="6c583-215">Read-only, Nullable</span></span> |
|<span data-ttu-id="6c583-216">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="6c583-216">verificationDnsRecords</span></span>|<span data-ttu-id="6c583-217">[domainDnsRecord](domaindnsrecord.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c583-217">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="6c583-218">顧客が Azure AD のドメイン所有権の確認を完了する前に、顧客がそのドメインの DNS ゾーン ファイルに追加する DNS レコード。</span><span class="sxs-lookup"><span data-stu-id="6c583-218">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="6c583-219">読み取り専用、Null 許容型</span><span class="sxs-lookup"><span data-stu-id="6c583-219">Read-only, Nullable</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c583-220">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c583-220">JSON representation</span></span>
<span data-ttu-id="6c583-221">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c583-221">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
