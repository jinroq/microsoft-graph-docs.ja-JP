---
title: 連絡先を更新する
description: 連絡先オブジェクトのプロパティを更新します。
ms.openlocfilehash: baf563530dc174418169efdd7f7bb48d81048a6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022622"
---
# <a name="update-contact"></a><span data-ttu-id="5132d-103">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="5132d-103">Update contact</span></span>

<span data-ttu-id="5132d-104">連絡先オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5132d-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5132d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5132d-105">Permissions</span></span>
<span data-ttu-id="5132d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5132d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5132d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5132d-108">Permission type</span></span>      | <span data-ttu-id="5132d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5132d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5132d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5132d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5132d-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5132d-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5132d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5132d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5132d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5132d-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5132d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5132d-114">Application</span></span> | <span data-ttu-id="5132d-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5132d-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5132d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5132d-116">HTTP request</span></span>
<span data-ttu-id="5132d-117"><!-- { "blockType": "ignored" } -->[連絡先](../resources/contact.md)ユーザーの既定の[contactFolder](../resources/contactfolder.md)からです。</span><span class="sxs-lookup"><span data-stu-id="5132d-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="5132d-118">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="5132d-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="5132d-p102">[contactFolder](../resources/mailfolder.md) の子フォルダー内に含まれる [連絡先](../resources/contact.md)。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="5132d-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5132d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5132d-121">Request headers</span></span>
| <span data-ttu-id="5132d-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5132d-122">Header</span></span>       | <span data-ttu-id="5132d-123">値</span><span class="sxs-lookup"><span data-stu-id="5132d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5132d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5132d-124">Authorization</span></span>  | <span data-ttu-id="5132d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5132d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5132d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5132d-127">Content-Type</span></span>  | <span data-ttu-id="5132d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5132d-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5132d-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="5132d-130">Request body</span></span>
<span data-ttu-id="5132d-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="5132d-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5132d-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5132d-134">Property</span></span>     | <span data-ttu-id="5132d-135">型</span><span class="sxs-lookup"><span data-stu-id="5132d-135">Type</span></span>   |<span data-ttu-id="5132d-136">説明</span><span class="sxs-lookup"><span data-stu-id="5132d-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5132d-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="5132d-137">assistantName</span></span>|<span data-ttu-id="5132d-138">String</span><span class="sxs-lookup"><span data-stu-id="5132d-138">String</span></span>|<span data-ttu-id="5132d-139">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="5132d-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="5132d-140">birthday</span><span class="sxs-lookup"><span data-stu-id="5132d-140">birthday</span></span>|<span data-ttu-id="5132d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5132d-141">DateTimeOffset</span></span>|<span data-ttu-id="5132d-142">連絡先の誕生日です。</span><span class="sxs-lookup"><span data-stu-id="5132d-142">The contact's birthday.</span></span>|
|<span data-ttu-id="5132d-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="5132d-143">businessAddress</span></span>|[<span data-ttu-id="5132d-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="5132d-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="5132d-145">連絡先の勤務先の住所。</span><span class="sxs-lookup"><span data-stu-id="5132d-145">The contact's business address.</span></span>|
|<span data-ttu-id="5132d-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="5132d-146">businessHomePage</span></span>|<span data-ttu-id="5132d-147">String</span><span class="sxs-lookup"><span data-stu-id="5132d-147">String</span></span>|<span data-ttu-id="5132d-148">連絡先の勤務先のホーム ページ。</span><span class="sxs-lookup"><span data-stu-id="5132d-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="5132d-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="5132d-149">businessPhones</span></span>|<span data-ttu-id="5132d-150">String</span><span class="sxs-lookup"><span data-stu-id="5132d-150">String</span></span>|<span data-ttu-id="5132d-151">連絡先の勤務先の電話番号。</span><span class="sxs-lookup"><span data-stu-id="5132d-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="5132d-152">categories</span><span class="sxs-lookup"><span data-stu-id="5132d-152">categories</span></span>|<span data-ttu-id="5132d-153">String</span><span class="sxs-lookup"><span data-stu-id="5132d-153">String</span></span>|<span data-ttu-id="5132d-154">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="5132d-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="5132d-155">children</span><span class="sxs-lookup"><span data-stu-id="5132d-155">children</span></span>|<span data-ttu-id="5132d-156">String</span><span class="sxs-lookup"><span data-stu-id="5132d-156">String</span></span>|<span data-ttu-id="5132d-157">連絡先の子供の名前。</span><span class="sxs-lookup"><span data-stu-id="5132d-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="5132d-158">companyName</span><span class="sxs-lookup"><span data-stu-id="5132d-158">companyName</span></span>|<span data-ttu-id="5132d-159">String</span><span class="sxs-lookup"><span data-stu-id="5132d-159">String</span></span>|<span data-ttu-id="5132d-160">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="5132d-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="5132d-161">department</span><span class="sxs-lookup"><span data-stu-id="5132d-161">department</span></span>|<span data-ttu-id="5132d-162">String</span><span class="sxs-lookup"><span data-stu-id="5132d-162">String</span></span>|<span data-ttu-id="5132d-163">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="5132d-163">The contact's department.</span></span>|
|<span data-ttu-id="5132d-164">displayName</span><span class="sxs-lookup"><span data-stu-id="5132d-164">displayName</span></span>|<span data-ttu-id="5132d-165">String</span><span class="sxs-lookup"><span data-stu-id="5132d-165">String</span></span>|<span data-ttu-id="5132d-166">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="5132d-166">The contact's display name.</span></span> <span data-ttu-id="5132d-167">その他のプロパティを後で更新プログラムが原因で、自動的に生成された値を指定した表示名の値を上書きすることに注意します。</span><span class="sxs-lookup"><span data-stu-id="5132d-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="5132d-168">既存の値を保持するには、必ず、更新操作の表示名としてです。</span><span class="sxs-lookup"><span data-stu-id="5132d-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="5132d-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="5132d-169">emailAddresses</span></span>|<span data-ttu-id="5132d-170">[EmailAddress](../resources/emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="5132d-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="5132d-171">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="5132d-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="5132d-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="5132d-172">fileAs</span></span>|<span data-ttu-id="5132d-173">String</span><span class="sxs-lookup"><span data-stu-id="5132d-173">String</span></span>|<span data-ttu-id="5132d-174">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="5132d-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="5132d-175">generation</span><span class="sxs-lookup"><span data-stu-id="5132d-175">generation</span></span>|<span data-ttu-id="5132d-176">String</span><span class="sxs-lookup"><span data-stu-id="5132d-176">String</span></span>|<span data-ttu-id="5132d-177">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="5132d-177">The contact's generation.</span></span>|
|<span data-ttu-id="5132d-178">givenName</span><span class="sxs-lookup"><span data-stu-id="5132d-178">givenName</span></span>|<span data-ttu-id="5132d-179">String</span><span class="sxs-lookup"><span data-stu-id="5132d-179">String</span></span>|<span data-ttu-id="5132d-180">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="5132d-180">The contact's given name.</span></span>|
|<span data-ttu-id="5132d-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="5132d-181">homeAddress</span></span>|[<span data-ttu-id="5132d-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="5132d-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="5132d-183">連絡先の自宅住所。</span><span class="sxs-lookup"><span data-stu-id="5132d-183">The contact's home address.</span></span>|
|<span data-ttu-id="5132d-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="5132d-184">homePhones</span></span>|<span data-ttu-id="5132d-185">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5132d-185">String collection</span></span>|<span data-ttu-id="5132d-186">連絡先の自宅の電話番号。</span><span class="sxs-lookup"><span data-stu-id="5132d-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="5132d-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="5132d-187">imAddresses</span></span>|<span data-ttu-id="5132d-188">String</span><span class="sxs-lookup"><span data-stu-id="5132d-188">String</span></span>|<span data-ttu-id="5132d-189">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="5132d-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="5132d-190">initials</span><span class="sxs-lookup"><span data-stu-id="5132d-190">initials</span></span>|<span data-ttu-id="5132d-191">String</span><span class="sxs-lookup"><span data-stu-id="5132d-191">String</span></span>|<span data-ttu-id="5132d-192">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="5132d-192">The contact's initials.</span></span>|
|<span data-ttu-id="5132d-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="5132d-193">jobTitle</span></span>|<span data-ttu-id="5132d-194">String</span><span class="sxs-lookup"><span data-stu-id="5132d-194">String</span></span>|<span data-ttu-id="5132d-195">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="5132d-195">The contact’s job title.</span></span>|
|<span data-ttu-id="5132d-196">manager</span><span class="sxs-lookup"><span data-stu-id="5132d-196">manager</span></span>|<span data-ttu-id="5132d-197">String</span><span class="sxs-lookup"><span data-stu-id="5132d-197">String</span></span>|<span data-ttu-id="5132d-198">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="5132d-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="5132d-199">middleName</span><span class="sxs-lookup"><span data-stu-id="5132d-199">middleName</span></span>|<span data-ttu-id="5132d-200">String</span><span class="sxs-lookup"><span data-stu-id="5132d-200">String</span></span>|<span data-ttu-id="5132d-201">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="5132d-201">The contact's middle name.</span></span>|
|<span data-ttu-id="5132d-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="5132d-202">mobilePhone</span></span>|<span data-ttu-id="5132d-203">String</span><span class="sxs-lookup"><span data-stu-id="5132d-203">String</span></span>|<span data-ttu-id="5132d-204">連絡先の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="5132d-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="5132d-205">nickName</span><span class="sxs-lookup"><span data-stu-id="5132d-205">nickName</span></span>|<span data-ttu-id="5132d-206">String</span><span class="sxs-lookup"><span data-stu-id="5132d-206">String</span></span>|<span data-ttu-id="5132d-207">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="5132d-207">The contact's nickname.</span></span>|
|<span data-ttu-id="5132d-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="5132d-208">officeLocation</span></span>|<span data-ttu-id="5132d-209">String</span><span class="sxs-lookup"><span data-stu-id="5132d-209">String</span></span>|<span data-ttu-id="5132d-210">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="5132d-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="5132d-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="5132d-211">otherAddress</span></span>|[<span data-ttu-id="5132d-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="5132d-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="5132d-213">連絡先の別の住所。</span><span class="sxs-lookup"><span data-stu-id="5132d-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="5132d-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="5132d-214">parentFolderId</span></span>|<span data-ttu-id="5132d-215">String</span><span class="sxs-lookup"><span data-stu-id="5132d-215">String</span></span>|<span data-ttu-id="5132d-216">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="5132d-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="5132d-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="5132d-217">personalNotes</span></span>|<span data-ttu-id="5132d-218">String</span><span class="sxs-lookup"><span data-stu-id="5132d-218">String</span></span>|<span data-ttu-id="5132d-219">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="5132d-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="5132d-220">profession</span><span class="sxs-lookup"><span data-stu-id="5132d-220">profession</span></span>|<span data-ttu-id="5132d-221">String</span><span class="sxs-lookup"><span data-stu-id="5132d-221">String</span></span>|<span data-ttu-id="5132d-222">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="5132d-222">The contact's profession.</span></span>|
|<span data-ttu-id="5132d-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="5132d-223">spouseName</span></span>|<span data-ttu-id="5132d-224">String</span><span class="sxs-lookup"><span data-stu-id="5132d-224">String</span></span>|<span data-ttu-id="5132d-225">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="5132d-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="5132d-226">姓</span><span class="sxs-lookup"><span data-stu-id="5132d-226">surname</span></span>|<span data-ttu-id="5132d-227">String</span><span class="sxs-lookup"><span data-stu-id="5132d-227">String</span></span>|<span data-ttu-id="5132d-228">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="5132d-228">The contact's surname.</span></span>|
|<span data-ttu-id="5132d-229">タイトル</span><span class="sxs-lookup"><span data-stu-id="5132d-229">title</span></span>|<span data-ttu-id="5132d-230">String</span><span class="sxs-lookup"><span data-stu-id="5132d-230">String</span></span>|<span data-ttu-id="5132d-231">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="5132d-231">The contact's title.</span></span>|
|<span data-ttu-id="5132d-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="5132d-232">yomiCompanyName</span></span>|<span data-ttu-id="5132d-233">String</span><span class="sxs-lookup"><span data-stu-id="5132d-233">String</span></span>|<span data-ttu-id="5132d-p107">連絡先の会社名の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="5132d-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="5132d-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="5132d-236">yomiGivenName</span></span>|<span data-ttu-id="5132d-237">String</span><span class="sxs-lookup"><span data-stu-id="5132d-237">String</span></span>|<span data-ttu-id="5132d-p108">連絡先の名 (ファースト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="5132d-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="5132d-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="5132d-240">yomiSurname</span></span>|<span data-ttu-id="5132d-241">String</span><span class="sxs-lookup"><span data-stu-id="5132d-241">String</span></span>|<span data-ttu-id="5132d-p109">連絡先の姓 (ラスト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="5132d-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="5132d-244">応答</span><span class="sxs-lookup"><span data-stu-id="5132d-244">Response</span></span>

<span data-ttu-id="5132d-245">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5132d-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5132d-246">例</span><span class="sxs-lookup"><span data-stu-id="5132d-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5132d-247">要求</span><span class="sxs-lookup"><span data-stu-id="5132d-247">Request</span></span>
<span data-ttu-id="5132d-248">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5132d-248">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contacts/{id}
Content-type: application/json
Content-length: 1977

{
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "birthday": "1974-07-22"
}
```
##### <a name="response"></a><span data-ttu-id="5132d-249">応答</span><span class="sxs-lookup"><span data-stu-id="5132d-249">Response</span></span>
<span data-ttu-id="5132d-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5132d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "https://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
