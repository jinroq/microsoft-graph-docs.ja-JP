---
title: 組織リソースの種類
description: 'Azure Active Directory テナントを表します。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f2b7d83f8c78eb11ad4f22d456d9791982aab5c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345581"
---
# <a name="organization-resource-type"></a><span data-ttu-id="d7b22-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7b22-103">organization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7b22-104">ユーザーやアプリケーションがサインインする Azure Active Directory テナントを表します。</span><span class="sxs-lookup"><span data-stu-id="d7b22-104">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="d7b22-105">このリソースでは読み取りおよび更新操作のみがサポートされ、作成と削除はサポートされません。</span><span class="sxs-lookup"><span data-stu-id="d7b22-105">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="d7b22-106">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="d7b22-106">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="d7b22-107">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="d7b22-107">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="d7b22-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7b22-108">Methods</span></span>

| <span data-ttu-id="d7b22-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7b22-109">Method</span></span>       | <span data-ttu-id="d7b22-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d7b22-110">Return Type</span></span>  |<span data-ttu-id="d7b22-111">説明</span><span class="sxs-lookup"><span data-stu-id="d7b22-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7b22-112">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="d7b22-112">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="d7b22-113">organization</span><span class="sxs-lookup"><span data-stu-id="d7b22-113">organization</span></span>](organization.md) |<span data-ttu-id="d7b22-114">組織オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d7b22-114">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="d7b22-115">Update</span><span class="sxs-lookup"><span data-stu-id="d7b22-115">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="d7b22-116">organization</span><span class="sxs-lookup"><span data-stu-id="d7b22-116">organization</span></span>](organization.md)  |<span data-ttu-id="d7b22-117">organization オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d7b22-117">Update organization object.</span></span> <span data-ttu-id="d7b22-118">更新できるプロパティは、**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones**、**privacyProfile** のみです。</span><span class="sxs-lookup"><span data-stu-id="d7b22-118">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="d7b22-119">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="d7b22-119">**Open extensions**</span></span>| | |
|[<span data-ttu-id="d7b22-120">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="d7b22-120">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="d7b22-121">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="d7b22-121">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="d7b22-122">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="d7b22-122">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="d7b22-123">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="d7b22-123">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="d7b22-124">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b22-124">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="d7b22-125">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="d7b22-125">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="d7b22-126">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="d7b22-126">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="d7b22-127">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="d7b22-127">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="d7b22-128">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="d7b22-128">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7b22-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7b22-129">Properties</span></span>
| <span data-ttu-id="d7b22-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7b22-130">Property</span></span>     | <span data-ttu-id="d7b22-131">型</span><span class="sxs-lookup"><span data-stu-id="d7b22-131">Type</span></span>   |<span data-ttu-id="d7b22-132">説明</span><span class="sxs-lookup"><span data-stu-id="d7b22-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7b22-133">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="d7b22-133">assignedPlans</span></span>|<span data-ttu-id="d7b22-134">[assignedPlan](assignedplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b22-134">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="d7b22-p103">テナントに関連付けられているサービス プランのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d7b22-p103">The collection of service plans associated with the tenant. Not nullable.</span></span>            |
| <span data-ttu-id="d7b22-137">businessPhones</span><span class="sxs-lookup"><span data-stu-id="d7b22-137">businessPhones</span></span>                      | <span data-ttu-id="d7b22-138">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b22-138">String collection</span></span>                                         | <span data-ttu-id="d7b22-139">組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="d7b22-139">Telephone number for the organization.</span></span> <span data-ttu-id="d7b22-140">**メモ:** 文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。</span><span class="sxs-lookup"><span data-stu-id="d7b22-140">**Note:** Although this is a string collection, only one number can be set for this property.</span></span>                                                                                            |
|<span data-ttu-id="d7b22-141">city</span><span class="sxs-lookup"><span data-stu-id="d7b22-141">city</span></span>|<span data-ttu-id="d7b22-142">String</span><span class="sxs-lookup"><span data-stu-id="d7b22-142">String</span></span>| <span data-ttu-id="d7b22-143">組織の住所の市区町村名</span><span class="sxs-lookup"><span data-stu-id="d7b22-143">City name of the address for the organization</span></span> |
|<span data-ttu-id="d7b22-144">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="d7b22-144">companyLastDirSyncTime</span></span>|<span data-ttu-id="d7b22-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7b22-145">DateTimeOffset</span></span>|<span data-ttu-id="d7b22-p105">テナントがオンプレミスのディレクトリと最後に同期した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d7b22-p105">The time and date at which the tenant was last synced with the on-premise directory.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d7b22-148">country</span><span class="sxs-lookup"><span data-stu-id="d7b22-148">country</span></span>|<span data-ttu-id="d7b22-149">String</span><span class="sxs-lookup"><span data-stu-id="d7b22-149">String</span></span>| <span data-ttu-id="d7b22-150">組織の住所の国/地域名</span><span class="sxs-lookup"><span data-stu-id="d7b22-150">Country/region name of the address for the organization</span></span> |
|<span data-ttu-id="d7b22-151">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="d7b22-151">countryLetterCode</span></span>|<span data-ttu-id="d7b22-152">String</span><span class="sxs-lookup"><span data-stu-id="d7b22-152">String</span></span>| <span data-ttu-id="d7b22-153">組織の国/地域の略称</span><span class="sxs-lookup"><span data-stu-id="d7b22-153">Country/region abbreviation for the organization</span></span> |
|<span data-ttu-id="d7b22-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7b22-154">createdDateTime</span></span>|<span data-ttu-id="d7b22-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7b22-155">DateTimeOffset</span></span>| <span data-ttu-id="d7b22-156">組織作成時のタイムスタンプです。</span><span class="sxs-lookup"><span data-stu-id="d7b22-156">Timestamp of when the organization was created.</span></span> <span data-ttu-id="d7b22-157">値は変更できず、組織が作成されると自動的に設定されます。</span><span class="sxs-lookup"><span data-stu-id="d7b22-157">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="d7b22-158">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d7b22-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d7b22-159">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d7b22-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d7b22-160">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d7b22-160">Read-only.</span></span> |
| <span data-ttu-id="d7b22-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7b22-161">deletedDateTime</span></span>                    | <span data-ttu-id="d7b22-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7b22-162">DateTimeOffset</span></span>                                                    | <span data-ttu-id="d7b22-163">ISO 8601 形式を使用して Azure AD テナントが削除されたときの日時を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d7b22-163">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d7b22-164">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります: `'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="d7b22-164">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d7b22-165">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d7b22-165">Read-only.</span></span>                                                                                     |
|<span data-ttu-id="d7b22-166">dirsyncenabled</span><span class="sxs-lookup"><span data-stu-id="d7b22-166">dirSyncEnabled</span></span>|<span data-ttu-id="d7b22-167">ブール値</span><span class="sxs-lookup"><span data-stu-id="d7b22-167">Boolean</span></span>|<span data-ttu-id="d7b22-168">このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。</span><span class="sxs-lookup"><span data-stu-id="d7b22-168">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="d7b22-169">displayName</span><span class="sxs-lookup"><span data-stu-id="d7b22-169">displayName</span></span>|<span data-ttu-id="d7b22-170">文字列</span><span class="sxs-lookup"><span data-stu-id="d7b22-170">String</span></span>|<span data-ttu-id="d7b22-171">テナントの表示名。</span><span class="sxs-lookup"><span data-stu-id="d7b22-171">The display name for the tenant.</span></span>|
|<span data-ttu-id="d7b22-172">id</span><span class="sxs-lookup"><span data-stu-id="d7b22-172">id</span></span>|<span data-ttu-id="d7b22-173">String</span><span class="sxs-lookup"><span data-stu-id="d7b22-173">String</span></span>|<span data-ttu-id="d7b22-174">テナント ID。組織 (またはテナント) を表す一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="d7b22-174">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="d7b22-175">[directoryObject](directoryobject.md) から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d7b22-175">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="d7b22-176">キー。</span><span class="sxs-lookup"><span data-stu-id="d7b22-176">Key.</span></span> <span data-ttu-id="d7b22-177">null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="d7b22-177">Not nullable.</span></span> <span data-ttu-id="d7b22-178">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d7b22-178">Read-only.</span></span>|
|<span data-ttu-id="d7b22-179">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="d7b22-179">isMultipleDataLocationsForServicesEnabled</span></span>|<span data-ttu-id="d7b22-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7b22-180">Boolean</span></span>|<span data-ttu-id="d7b22-181">組織の Multi-Geo が有効の場合 **true**、組織の Multi-Geo が有効ではない場合 **false**、**null** (既定)。</span><span class="sxs-lookup"><span data-stu-id="d7b22-181">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="d7b22-182">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d7b22-182">Read-only.</span></span> <span data-ttu-id="d7b22-183">詳細については、「[OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7b22-183">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span>|
|<span data-ttu-id="d7b22-184">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="d7b22-184">marketingNotificationEmails</span></span>|<span data-ttu-id="d7b22-185">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b22-185">String collection</span></span>| <span data-ttu-id="d7b22-186">null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="d7b22-186">Not nullable.</span></span>            |
|<span data-ttu-id="d7b22-187">objectType</span><span class="sxs-lookup"><span data-stu-id="d7b22-187">objectType</span></span>|<span data-ttu-id="d7b22-188">String</span><span class="sxs-lookup"><span data-stu-id="d7b22-188">String</span></span>|<span data-ttu-id="d7b22-p110">オブジェクトの種類を識別する文字列です。テナントの場合、値は常に「会社」です。</span><span class="sxs-lookup"><span data-stu-id="d7b22-p110">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
|<span data-ttu-id="d7b22-191">postalCode</span><span class="sxs-lookup"><span data-stu-id="d7b22-191">postalCode</span></span>|<span data-ttu-id="d7b22-192">String</span><span class="sxs-lookup"><span data-stu-id="d7b22-192">String</span></span>| <span data-ttu-id="d7b22-193">組織の住所の郵便番号</span><span class="sxs-lookup"><span data-stu-id="d7b22-193">Postal code of the address for the organization</span></span> |
|<span data-ttu-id="d7b22-194">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="d7b22-194">preferredLanguage</span></span>|<span data-ttu-id="d7b22-195">String</span><span class="sxs-lookup"><span data-stu-id="d7b22-195">String</span></span>| <span data-ttu-id="d7b22-196">組織の優先言語。</span><span class="sxs-lookup"><span data-stu-id="d7b22-196">The preferred language for the organization.</span></span> <span data-ttu-id="d7b22-197">ISO 639-1 コードに従う必要があります (例: "en")。</span><span class="sxs-lookup"><span data-stu-id="d7b22-197">Should follow ISO 639-1 Code; for example "en".</span></span> |
|<span data-ttu-id="d7b22-198">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="d7b22-198">privacyProfile</span></span>|[<span data-ttu-id="d7b22-199">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="d7b22-199">privacyProfile</span></span>](privacyprofile.md)| <span data-ttu-id="d7b22-200">組織のプライバシー プロファイル。</span><span class="sxs-lookup"><span data-stu-id="d7b22-200">The privacy profile of an organization.</span></span>            |
|<span data-ttu-id="d7b22-201">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="d7b22-201">provisionedPlans</span></span>|<span data-ttu-id="d7b22-202">[provisionedPlan](provisionedplan.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b22-202">[provisionedPlan](provisionedplan.md) collection</span></span>| <span data-ttu-id="d7b22-203">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d7b22-203">Not nullable.</span></span>            |
|<span data-ttu-id="d7b22-204">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="d7b22-204">securityComplianceNotificationMails</span></span>|<span data-ttu-id="d7b22-205">String collection</span><span class="sxs-lookup"><span data-stu-id="d7b22-205">String collection</span></span>||
|<span data-ttu-id="d7b22-206">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="d7b22-206">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="d7b22-207">String collection</span><span class="sxs-lookup"><span data-stu-id="d7b22-207">String collection</span></span>||
|<span data-ttu-id="d7b22-208">state</span><span class="sxs-lookup"><span data-stu-id="d7b22-208">state</span></span>|<span data-ttu-id="d7b22-209">String</span><span class="sxs-lookup"><span data-stu-id="d7b22-209">String</span></span>| <span data-ttu-id="d7b22-210">組織の住所の都道府県名</span><span class="sxs-lookup"><span data-stu-id="d7b22-210">State name of the address for the organization</span></span> |
|<span data-ttu-id="d7b22-211">street</span><span class="sxs-lookup"><span data-stu-id="d7b22-211">street</span></span>|<span data-ttu-id="d7b22-212">String</span><span class="sxs-lookup"><span data-stu-id="d7b22-212">String</span></span>| <span data-ttu-id="d7b22-213">組織の住所の番地</span><span class="sxs-lookup"><span data-stu-id="d7b22-213">Street name of the address for organization</span></span> |
|<span data-ttu-id="d7b22-214">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="d7b22-214">technicalNotificationMails</span></span>|<span data-ttu-id="d7b22-215">String collection</span><span class="sxs-lookup"><span data-stu-id="d7b22-215">String collection</span></span>| <span data-ttu-id="d7b22-216">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d7b22-216">Not nullable.</span></span> |
|<span data-ttu-id="d7b22-217">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="d7b22-217">verifiedDomains</span></span>|<span data-ttu-id="d7b22-218">[verifiedDomain](verifieddomain.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b22-218">[verifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="d7b22-p112">このテナントに関連付けられているドメインのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d7b22-p112">The collection of domains associated with this tenant. Not nullable.</span></span>            |

## <a name="relationships"></a><span data-ttu-id="d7b22-221">関係</span><span class="sxs-lookup"><span data-stu-id="d7b22-221">Relationships</span></span>

| <span data-ttu-id="d7b22-222">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7b22-222">Relationship</span></span>     | <span data-ttu-id="d7b22-223">型</span><span class="sxs-lookup"><span data-stu-id="d7b22-223">Type</span></span>   |<span data-ttu-id="d7b22-224">説明</span><span class="sxs-lookup"><span data-stu-id="d7b22-224">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7b22-225">extensions</span><span class="sxs-lookup"><span data-stu-id="d7b22-225">extensions</span></span>|<span data-ttu-id="d7b22-226">[extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d7b22-226">[extension](extension.md) collection</span></span>|<span data-ttu-id="d7b22-227">組織リソースに対して定義されているオープン拡張機能のコレクション。</span><span class="sxs-lookup"><span data-stu-id="d7b22-227">The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="d7b22-228">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d7b22-228">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7b22-229">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7b22-229">JSON representation</span></span>

<span data-ttu-id="d7b22-230">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d7b22-230">Here is a JSON representation of the resource</span></span>

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
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}],
  "companyLastDirSyncTime": "2019-02-07T20:33:52.942Z",
  "dirSyncEnabled": true
}
```

## <a name="see-also"></a><span data-ttu-id="d7b22-231">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7b22-231">See also</span></span>

- [<span data-ttu-id="d7b22-232">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="d7b22-232">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d7b22-233">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="d7b22-233">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d7b22-234">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="d7b22-234">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
