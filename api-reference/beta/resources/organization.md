---
title: 組織リソースの種類
description: 'Azure Active Directory のテナント型を表します。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b0e1e0563b0e29d49fbf5dece0f62f70e7a71c52
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574993"
---
# <a name="organization-resource-type"></a><span data-ttu-id="d95ac-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d95ac-103">organization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d95ac-104">ユーザーやアプリケーションがサインインする Azure Active Directory テナントを表します。</span><span class="sxs-lookup"><span data-stu-id="d95ac-104">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="d95ac-105">このリソースでは読み取りおよび更新操作のみがサポートされ、作成と削除はサポートされません。</span><span class="sxs-lookup"><span data-stu-id="d95ac-105">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="d95ac-106">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="d95ac-106">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="d95ac-107">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="d95ac-107">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="d95ac-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d95ac-108">Methods</span></span>

| <span data-ttu-id="d95ac-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d95ac-109">Method</span></span>       | <span data-ttu-id="d95ac-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d95ac-110">Return Type</span></span>  |<span data-ttu-id="d95ac-111">説明</span><span class="sxs-lookup"><span data-stu-id="d95ac-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d95ac-112">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="d95ac-112">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="d95ac-113">organization</span><span class="sxs-lookup"><span data-stu-id="d95ac-113">organization</span></span>](organization.md) |<span data-ttu-id="d95ac-114">組織オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d95ac-114">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="d95ac-115">Update</span><span class="sxs-lookup"><span data-stu-id="d95ac-115">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="d95ac-116">organization</span><span class="sxs-lookup"><span data-stu-id="d95ac-116">organization</span></span>](organization.md)  |<span data-ttu-id="d95ac-117">organization オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d95ac-117">Update organization object.</span></span> <span data-ttu-id="d95ac-118">更新できるプロパティは、**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones**、**privacyProfile** のみです。</span><span class="sxs-lookup"><span data-stu-id="d95ac-118">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="d95ac-119">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="d95ac-119">**Open extensions**</span></span>| | |
|[<span data-ttu-id="d95ac-120">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="d95ac-120">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="d95ac-121">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="d95ac-121">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="d95ac-122">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="d95ac-122">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="d95ac-123">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="d95ac-123">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="d95ac-124">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-124">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="d95ac-125">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="d95ac-125">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="d95ac-126">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="d95ac-126">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="d95ac-127">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="d95ac-127">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="d95ac-128">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="d95ac-128">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="d95ac-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d95ac-129">Properties</span></span>
| <span data-ttu-id="d95ac-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d95ac-130">Property</span></span>     | <span data-ttu-id="d95ac-131">型</span><span class="sxs-lookup"><span data-stu-id="d95ac-131">Type</span></span>   |<span data-ttu-id="d95ac-132">説明</span><span class="sxs-lookup"><span data-stu-id="d95ac-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d95ac-133">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="d95ac-133">assignedPlans</span></span>|<span data-ttu-id="d95ac-134">[assignedPlan](assignedplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-134">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="d95ac-p103">テナントに関連付けられているサービス プランのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d95ac-p103">The collection of service plans associated with the tenant. Not nullable.</span></span>            |
| <span data-ttu-id="d95ac-137">businessPhones</span><span class="sxs-lookup"><span data-stu-id="d95ac-137">businessPhones</span></span>                      | <span data-ttu-id="d95ac-138">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-138">String collection</span></span>                                         | <span data-ttu-id="d95ac-139">組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="d95ac-139">Telephone number for the organization.</span></span> <span data-ttu-id="d95ac-140">**メモ:** 文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。</span><span class="sxs-lookup"><span data-stu-id="d95ac-140">**Note:** Although this is a string collection, only one number can be set for this property.</span></span>                                                                                            |
|<span data-ttu-id="d95ac-141">city</span><span class="sxs-lookup"><span data-stu-id="d95ac-141">city</span></span>|<span data-ttu-id="d95ac-142">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-142">String</span></span>| <span data-ttu-id="d95ac-143">組織の住所の市区町村名</span><span class="sxs-lookup"><span data-stu-id="d95ac-143">City name of the address for the organization</span></span> |
|<span data-ttu-id="d95ac-144">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="d95ac-144">companyLastDirSyncTime</span></span>|<span data-ttu-id="d95ac-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d95ac-145">DateTimeOffset</span></span>|<span data-ttu-id="d95ac-p105">テナントがオンプレミスのディレクトリと最後に同期した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d95ac-p105">The time and date at which the tenant was last synced with the on-premise directory.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d95ac-148">country</span><span class="sxs-lookup"><span data-stu-id="d95ac-148">country</span></span>|<span data-ttu-id="d95ac-149">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-149">String</span></span>| <span data-ttu-id="d95ac-150">組織の住所の国/地域名</span><span class="sxs-lookup"><span data-stu-id="d95ac-150">Country/region name of the address for the organization</span></span> |
|<span data-ttu-id="d95ac-151">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="d95ac-151">countryLetterCode</span></span>|<span data-ttu-id="d95ac-152">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-152">String</span></span>| <span data-ttu-id="d95ac-153">組織の国/地域の略称</span><span class="sxs-lookup"><span data-stu-id="d95ac-153">Country/region abbreviation for the organization</span></span> |
|<span data-ttu-id="d95ac-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d95ac-154">createdDateTime</span></span>|<span data-ttu-id="d95ac-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d95ac-155">DateTimeOffset</span></span>| <span data-ttu-id="d95ac-156">組織作成時のタイムスタンプです。</span><span class="sxs-lookup"><span data-stu-id="d95ac-156">Timestamp of when the organization was created.</span></span> <span data-ttu-id="d95ac-157">値は変更できず、組織が作成されると自動的に設定されます。</span><span class="sxs-lookup"><span data-stu-id="d95ac-157">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="d95ac-158">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d95ac-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d95ac-159">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d95ac-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d95ac-160">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d95ac-160">Read-only.</span></span> |
| <span data-ttu-id="d95ac-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="d95ac-161">deletedDateTime</span></span>                    | <span data-ttu-id="d95ac-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d95ac-162">DateTimeOffset</span></span>                                                    | <span data-ttu-id="d95ac-163">ISO 8601 形式を使用して Azure AD テナントが削除されたときの日時を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d95ac-163">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d95ac-164">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります: `'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="d95ac-164">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d95ac-165">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d95ac-165">Read-only.</span></span>                                                                                     |
|<span data-ttu-id="d95ac-166">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="d95ac-166">dirSyncEnabled</span></span>|<span data-ttu-id="d95ac-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="d95ac-167">Boolean</span></span>|<span data-ttu-id="d95ac-168">このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。</span><span class="sxs-lookup"><span data-stu-id="d95ac-168">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="d95ac-169">displayName</span><span class="sxs-lookup"><span data-stu-id="d95ac-169">displayName</span></span>|<span data-ttu-id="d95ac-170">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-170">String</span></span>|<span data-ttu-id="d95ac-171">テナントの表示名。</span><span class="sxs-lookup"><span data-stu-id="d95ac-171">The display name for the tenant.</span></span>|
|<span data-ttu-id="d95ac-172">id</span><span class="sxs-lookup"><span data-stu-id="d95ac-172">id</span></span>|<span data-ttu-id="d95ac-173">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-173">String</span></span>|<span data-ttu-id="d95ac-174">テナント ID。組織 (またはテナント) を表す一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="d95ac-174">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="d95ac-175">[directoryObject](directoryobject.md) から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d95ac-175">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="d95ac-176">キー。</span><span class="sxs-lookup"><span data-stu-id="d95ac-176">Key.</span></span> <span data-ttu-id="d95ac-177">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d95ac-177">Not nullable.</span></span> <span data-ttu-id="d95ac-178">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d95ac-178">Read-only.</span></span>|
|<span data-ttu-id="d95ac-179">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="d95ac-179">isMultipleDataLocationsForServicesEnabled</span></span>|<span data-ttu-id="d95ac-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="d95ac-180">Boolean</span></span>|<span data-ttu-id="d95ac-181">組織の Multi-Geo が有効の場合 **true**、組織の Multi-Geo が有効ではない場合 **false**、**null** (既定)。</span><span class="sxs-lookup"><span data-stu-id="d95ac-181">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="d95ac-182">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d95ac-182">Read-only.</span></span> <span data-ttu-id="d95ac-183">詳細については、「[OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d95ac-183">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span>|
|<span data-ttu-id="d95ac-184">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="d95ac-184">marketingNotificationEmails</span></span>|<span data-ttu-id="d95ac-185">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-185">String collection</span></span>| <span data-ttu-id="d95ac-186">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d95ac-186">Not nullable.</span></span>            |
|<span data-ttu-id="d95ac-187">objectType</span><span class="sxs-lookup"><span data-stu-id="d95ac-187">objectType</span></span>|<span data-ttu-id="d95ac-188">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-188">String</span></span>|<span data-ttu-id="d95ac-p110">オブジェクトの種類を識別する文字列です。テナントの場合、値は常に「会社」です。</span><span class="sxs-lookup"><span data-stu-id="d95ac-p110">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
|<span data-ttu-id="d95ac-191">postalCode</span><span class="sxs-lookup"><span data-stu-id="d95ac-191">postalCode</span></span>|<span data-ttu-id="d95ac-192">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-192">String</span></span>| <span data-ttu-id="d95ac-193">組織の住所の郵便番号</span><span class="sxs-lookup"><span data-stu-id="d95ac-193">Postal code of the address for the organization</span></span> |
|<span data-ttu-id="d95ac-194">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="d95ac-194">preferredLanguage</span></span>|<span data-ttu-id="d95ac-195">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-195">String</span></span>| <span data-ttu-id="d95ac-196">組織の優先言語。</span><span class="sxs-lookup"><span data-stu-id="d95ac-196">The preferred language for the organization.</span></span> <span data-ttu-id="d95ac-197">ISO 639-1 コードに従う必要があります (例: "en")。</span><span class="sxs-lookup"><span data-stu-id="d95ac-197">Should follow ISO 639-1 Code; for example "en".</span></span> |
|<span data-ttu-id="d95ac-198">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="d95ac-198">privacyProfile</span></span>|[<span data-ttu-id="d95ac-199">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="d95ac-199">privacyProfile</span></span>](privacyprofile.md)| <span data-ttu-id="d95ac-200">組織のプライバシー プロファイル。</span><span class="sxs-lookup"><span data-stu-id="d95ac-200">The privacy profile of an organization.</span></span>            |
|<span data-ttu-id="d95ac-201">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="d95ac-201">provisionedPlans</span></span>|<span data-ttu-id="d95ac-202">[provisionedPlan](provisionedplan.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-202">[provisionedPlan](provisionedplan.md) collection</span></span>| <span data-ttu-id="d95ac-203">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d95ac-203">Not nullable.</span></span>            |
|<span data-ttu-id="d95ac-204">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="d95ac-204">provisioningErrors</span></span>|<span data-ttu-id="d95ac-205">onPremisesProvisioningError コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-205">onPremisesProvisioningError collection</span></span>| <span data-ttu-id="d95ac-206">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d95ac-206">Not nullable.</span></span>            |
|<span data-ttu-id="d95ac-207">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="d95ac-207">securityComplianceNotificationMails</span></span>|<span data-ttu-id="d95ac-208">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-208">String collection</span></span>||
|<span data-ttu-id="d95ac-209">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="d95ac-209">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="d95ac-210">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-210">String collection</span></span>||
|<span data-ttu-id="d95ac-211">state</span><span class="sxs-lookup"><span data-stu-id="d95ac-211">state</span></span>|<span data-ttu-id="d95ac-212">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-212">String</span></span>| <span data-ttu-id="d95ac-213">組織の住所の都道府県名</span><span class="sxs-lookup"><span data-stu-id="d95ac-213">State name of the address for the organization</span></span> |
|<span data-ttu-id="d95ac-214">street</span><span class="sxs-lookup"><span data-stu-id="d95ac-214">street</span></span>|<span data-ttu-id="d95ac-215">String</span><span class="sxs-lookup"><span data-stu-id="d95ac-215">String</span></span>| <span data-ttu-id="d95ac-216">組織の住所の番地</span><span class="sxs-lookup"><span data-stu-id="d95ac-216">Street name of the address for organization</span></span> |
|<span data-ttu-id="d95ac-217">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="d95ac-217">technicalNotificationMails</span></span>|<span data-ttu-id="d95ac-218">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-218">String collection</span></span>| <span data-ttu-id="d95ac-219">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d95ac-219">Not nullable.</span></span> |
|<span data-ttu-id="d95ac-220">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="d95ac-220">verifiedDomains</span></span>|<span data-ttu-id="d95ac-221">[VerifiedDomain](verifieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-221">[VerifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="d95ac-p112">このテナントに関連付けられているドメインのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d95ac-p112">The collection of domains associated with this tenant. Not nullable.</span></span>            |

## <a name="relationships"></a><span data-ttu-id="d95ac-224">関係</span><span class="sxs-lookup"><span data-stu-id="d95ac-224">Relationships</span></span>

| <span data-ttu-id="d95ac-225">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d95ac-225">Relationship</span></span>     | <span data-ttu-id="d95ac-226">型</span><span class="sxs-lookup"><span data-stu-id="d95ac-226">Type</span></span>   |<span data-ttu-id="d95ac-227">説明</span><span class="sxs-lookup"><span data-stu-id="d95ac-227">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d95ac-228">extensions</span><span class="sxs-lookup"><span data-stu-id="d95ac-228">extensions</span></span>|<span data-ttu-id="d95ac-229">[extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d95ac-229">[extension](extension.md) collection</span></span>|<span data-ttu-id="d95ac-230">組織のリソースに対して定義されている、開いている拡張機能のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d95ac-230">The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="d95ac-231">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d95ac-231">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d95ac-232">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d95ac-232">JSON representation</span></span>

<span data-ttu-id="d95ac-233">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d95ac-233">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
  "objectType": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}
```

## <a name="see-also"></a><span data-ttu-id="d95ac-234">関連項目</span><span class="sxs-lookup"><span data-stu-id="d95ac-234">See also</span></span>

- [<span data-ttu-id="d95ac-235">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="d95ac-235">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d95ac-236">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="d95ac-236">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d95ac-237">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="d95ac-237">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/organization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
