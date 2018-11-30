---
title: 連絡先を更新する
description: 連絡先オブジェクトのプロパティを更新します。
ms.openlocfilehash: 2fbf597ebc8a6c65141c64ae42ae42266f14cbde
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068972"
---
# <a name="update-contact"></a><span data-ttu-id="b5e3d-103">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="b5e3d-103">Update contact</span></span>

> <span data-ttu-id="b5e3d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5e3d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5e3d-106">連絡先オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-106">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5e3d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b5e3d-107">Permissions</span></span>
<span data-ttu-id="b5e3d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5e3d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5e3d-110">Permission type</span></span>      | <span data-ttu-id="b5e3d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5e3d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5e3d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b5e3d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b5e3d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e3d-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b5e3d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5e3d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e3d-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e3d-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b5e3d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5e3d-116">Application</span></span> | <span data-ttu-id="b5e3d-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e3d-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5e3d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5e3d-118">HTTP request</span></span>
<span data-ttu-id="b5e3d-119"><!-- { "blockType": "ignored" } -->[連絡先](../resources/contact.md)ユーザーの既定の[contactFolder](../resources/contactfolder.md)からです。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="b5e3d-120">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="b5e3d-121">[にお問い合わせください](../resources/contact.md) [contactFolder](../resources/mailfolder.md)の子フォルダーに含まれています。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="b5e3d-122">次の例は、入れ子のレベルを 1 つを示していますが、連絡先を子の子でというように配置できます。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b5e3d-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5e3d-123">Request headers</span></span>
| <span data-ttu-id="b5e3d-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5e3d-124">Header</span></span>       | <span data-ttu-id="b5e3d-125">値</span><span class="sxs-lookup"><span data-stu-id="b5e3d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b5e3d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5e3d-126">Authorization</span></span>  | <span data-ttu-id="b5e3d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b5e3d-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5e3d-129">Content-Type</span></span>  | <span data-ttu-id="b5e3d-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b5e3d-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5e3d-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="b5e3d-132">Request body</span></span>
<span data-ttu-id="b5e3d-p106">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b5e3d-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5e3d-136">Property</span></span>     | <span data-ttu-id="b5e3d-137">型</span><span class="sxs-lookup"><span data-stu-id="b5e3d-137">Type</span></span>   |<span data-ttu-id="b5e3d-138">説明</span><span class="sxs-lookup"><span data-stu-id="b5e3d-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5e3d-139">assistantName</span><span class="sxs-lookup"><span data-stu-id="b5e3d-139">assistantName</span></span>|<span data-ttu-id="b5e3d-140">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-140">String</span></span>|<span data-ttu-id="b5e3d-141">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-141">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="b5e3d-142">birthday</span><span class="sxs-lookup"><span data-stu-id="b5e3d-142">birthday</span></span>|<span data-ttu-id="b5e3d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5e3d-143">DateTimeOffset</span></span>|<span data-ttu-id="b5e3d-144">連絡先の誕生日です。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-144">The contact's birthday.</span></span>|
|<span data-ttu-id="b5e3d-145">categories</span><span class="sxs-lookup"><span data-stu-id="b5e3d-145">categories</span></span>|<span data-ttu-id="b5e3d-146">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-146">String</span></span>|<span data-ttu-id="b5e3d-147">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-147">The categories associated with the contact.</span></span>|
|<span data-ttu-id="b5e3d-148">children</span><span class="sxs-lookup"><span data-stu-id="b5e3d-148">children</span></span>|<span data-ttu-id="b5e3d-149">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-149">String</span></span>||
|<span data-ttu-id="b5e3d-150">companyName</span><span class="sxs-lookup"><span data-stu-id="b5e3d-150">companyName</span></span>|<span data-ttu-id="b5e3d-151">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-151">String</span></span>|<span data-ttu-id="b5e3d-152">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-152">The name of the contact's company.</span></span>|
|<span data-ttu-id="b5e3d-153">department</span><span class="sxs-lookup"><span data-stu-id="b5e3d-153">department</span></span>|<span data-ttu-id="b5e3d-154">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-154">String</span></span>|<span data-ttu-id="b5e3d-155">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-155">The contact's department.</span></span>|
|<span data-ttu-id="b5e3d-156">displayName</span><span class="sxs-lookup"><span data-stu-id="b5e3d-156">displayName</span></span>|<span data-ttu-id="b5e3d-157">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-157">String</span></span>|<span data-ttu-id="b5e3d-158">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-158">The contact's display name.</span></span> <span data-ttu-id="b5e3d-159">その他のプロパティを後で更新プログラムが原因で、自動的に生成された値を指定した表示名の値を上書きすることに注意します。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-159">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="b5e3d-160">既存の値を保持するには、必ず、更新操作の表示名としてです。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-160">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="b5e3d-161">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="b5e3d-161">emailAddresses</span></span>|<span data-ttu-id="b5e3d-162">[typedEmailAddress](../resources/typedemailaddress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b5e3d-162">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="b5e3d-163">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-163">The contact's email addresses.</span></span>|
|<span data-ttu-id="b5e3d-164">fileAs</span><span class="sxs-lookup"><span data-stu-id="b5e3d-164">fileAs</span></span>|<span data-ttu-id="b5e3d-165">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-165">String</span></span>|<span data-ttu-id="b5e3d-166">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-166">The name the contact is filed under.</span></span>|
|<span data-ttu-id="b5e3d-167">gender</span><span class="sxs-lookup"><span data-stu-id="b5e3d-167">gender</span></span> |<span data-ttu-id="b5e3d-168">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-168">String</span></span> |<span data-ttu-id="b5e3d-169">連絡先の性別。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-169">The contact's gender.</span></span> |
|<span data-ttu-id="b5e3d-170">generation</span><span class="sxs-lookup"><span data-stu-id="b5e3d-170">generation</span></span>|<span data-ttu-id="b5e3d-171">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-171">String</span></span>|<span data-ttu-id="b5e3d-172">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-172">The contact's generation.</span></span>|
|<span data-ttu-id="b5e3d-173">givenName</span><span class="sxs-lookup"><span data-stu-id="b5e3d-173">givenName</span></span>|<span data-ttu-id="b5e3d-174">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-174">String</span></span>|<span data-ttu-id="b5e3d-175">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-175">The contact's given name.</span></span>|
|<span data-ttu-id="b5e3d-176">imAddresses</span><span class="sxs-lookup"><span data-stu-id="b5e3d-176">imAddresses</span></span>|<span data-ttu-id="b5e3d-177">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-177">String</span></span>|<span data-ttu-id="b5e3d-178">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-178">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="b5e3d-179">initials</span><span class="sxs-lookup"><span data-stu-id="b5e3d-179">initials</span></span>|<span data-ttu-id="b5e3d-180">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-180">String</span></span>|<span data-ttu-id="b5e3d-181">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-181">The contact's initials.</span></span>|
|<span data-ttu-id="b5e3d-182">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b5e3d-182">jobTitle</span></span>|<span data-ttu-id="b5e3d-183">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-183">String</span></span>|<span data-ttu-id="b5e3d-184">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-184">The contact’s job title.</span></span>|
|<span data-ttu-id="b5e3d-185">manager</span><span class="sxs-lookup"><span data-stu-id="b5e3d-185">manager</span></span>|<span data-ttu-id="b5e3d-186">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-186">String</span></span>|<span data-ttu-id="b5e3d-187">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-187">The name of the contact's manager.</span></span>
|<span data-ttu-id="b5e3d-188">middleName</span><span class="sxs-lookup"><span data-stu-id="b5e3d-188">middleName</span></span>|<span data-ttu-id="b5e3d-189">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-189">String</span></span>|<span data-ttu-id="b5e3d-190">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-190">The contact's middle name.</span></span>|
|<span data-ttu-id="b5e3d-191">nickName</span><span class="sxs-lookup"><span data-stu-id="b5e3d-191">nickName</span></span>|<span data-ttu-id="b5e3d-192">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-192">String</span></span>|<span data-ttu-id="b5e3d-193">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-193">The contact's nickname.</span></span>|
|<span data-ttu-id="b5e3d-194">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b5e3d-194">officeLocation</span></span>|<span data-ttu-id="b5e3d-195">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-195">String</span></span>|<span data-ttu-id="b5e3d-196">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-196">The location of the contact's office.</span></span>|
|<span data-ttu-id="b5e3d-197">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b5e3d-197">parentFolderId</span></span>|<span data-ttu-id="b5e3d-198">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-198">String</span></span>|<span data-ttu-id="b5e3d-199">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-199">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="b5e3d-200">personalNotes</span><span class="sxs-lookup"><span data-stu-id="b5e3d-200">personalNotes</span></span>|<span data-ttu-id="b5e3d-201">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-201">String</span></span>|<span data-ttu-id="b5e3d-202">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-202">The user's notes about the contact.</span></span>|
|<span data-ttu-id="b5e3d-203">phones</span><span class="sxs-lookup"><span data-stu-id="b5e3d-203">phones</span></span> |<span data-ttu-id="b5e3d-204">[phone](../resources/phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5e3d-204">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="b5e3d-205">自宅電話、携帯電話、勤務先電話など、連絡先に関連付けられた電話番号。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-205">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="b5e3d-206">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="b5e3d-206">postalAddresses</span></span> |<span data-ttu-id="b5e3d-207">[physicalAddress](../resources/physicaladdress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b5e3d-207">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="b5e3d-208">自宅住所や勤務先住所など、連絡先に関連付けられた住所。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-208">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="b5e3d-209">profession</span><span class="sxs-lookup"><span data-stu-id="b5e3d-209">profession</span></span>|<span data-ttu-id="b5e3d-210">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-210">String</span></span>|<span data-ttu-id="b5e3d-211">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-211">The contact's profession.</span></span>|
|<span data-ttu-id="b5e3d-212">spouseName</span><span class="sxs-lookup"><span data-stu-id="b5e3d-212">spouseName</span></span>|<span data-ttu-id="b5e3d-213">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-213">String</span></span>|<span data-ttu-id="b5e3d-214">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-214">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="b5e3d-215">姓</span><span class="sxs-lookup"><span data-stu-id="b5e3d-215">surname</span></span>|<span data-ttu-id="b5e3d-216">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-216">String</span></span>|<span data-ttu-id="b5e3d-217">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-217">The contact's surname.</span></span>|
|<span data-ttu-id="b5e3d-218">タイトル</span><span class="sxs-lookup"><span data-stu-id="b5e3d-218">title</span></span>|<span data-ttu-id="b5e3d-219">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-219">String</span></span>|<span data-ttu-id="b5e3d-220">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-220">The contact's title.</span></span>|
|<span data-ttu-id="b5e3d-221">websites</span><span class="sxs-lookup"><span data-stu-id="b5e3d-221">websites</span></span> |<span data-ttu-id="b5e3d-222">[website](../resources/website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5e3d-222">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="b5e3d-223">連絡先に関連付けられた Web サイト。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-223">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="b5e3d-224">weddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="b5e3d-224">weddingAnniversary</span></span> |<span data-ttu-id="b5e3d-225">日付</span><span class="sxs-lookup"><span data-stu-id="b5e3d-225">Date</span></span> |<span data-ttu-id="b5e3d-226">連絡先の結婚記念日。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-226">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="b5e3d-227">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="b5e3d-227">yomiCompanyName</span></span>|<span data-ttu-id="b5e3d-228">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-228">String</span></span>|<span data-ttu-id="b5e3d-p108">連絡先の会社名の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-p108">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="b5e3d-231">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="b5e3d-231">yomiGivenName</span></span>|<span data-ttu-id="b5e3d-232">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-232">String</span></span>|<span data-ttu-id="b5e3d-p109">連絡先の名 (ファースト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-p109">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="b5e3d-235">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="b5e3d-235">yomiSurname</span></span>|<span data-ttu-id="b5e3d-236">String</span><span class="sxs-lookup"><span data-stu-id="b5e3d-236">String</span></span>|<span data-ttu-id="b5e3d-p110">連絡先の姓 (ラスト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-p110">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="b5e3d-239">使用することができます**お問い合わせください**リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または既存の**連絡先**のインスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-239">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="b5e3d-240">応答</span><span class="sxs-lookup"><span data-stu-id="b5e3d-240">Response</span></span>

<span data-ttu-id="b5e3d-241">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文のオブジェクトの更新に[お問い合わせください](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-241">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5e3d-242">例</span><span class="sxs-lookup"><span data-stu-id="b5e3d-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5e3d-243">要求</span><span class="sxs-lookup"><span data-stu-id="b5e3d-243">Request</span></span>
<span data-ttu-id="b5e3d-244">次の例では、指定した連絡先の個人用の電子メール アドレスを更新します。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-244">The following example updates the personal email address of the specified contact.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
##### <a name="response"></a><span data-ttu-id="b5e3d-245">応答</span><span class="sxs-lookup"><span data-stu-id="b5e3d-245">Response</span></span>
<span data-ttu-id="b5e3d-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b5e3d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="b5e3d-249">関連項目</span><span class="sxs-lookup"><span data-stu-id="b5e3d-249">See also</span></span>

- [<span data-ttu-id="b5e3d-250">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="b5e3d-250">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b5e3d-251">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="b5e3d-251">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->