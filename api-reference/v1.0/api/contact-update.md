---
title: 連絡先を更新する
description: 連絡先オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0d8a6d344326d1dfb03a23fc21e7e21680a827dd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277498"
---
# <a name="update-contact"></a><span data-ttu-id="161d3-103">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="161d3-103">Update contact</span></span>

<span data-ttu-id="161d3-104">連絡先オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="161d3-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="161d3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="161d3-105">Permissions</span></span>
<span data-ttu-id="161d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="161d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="161d3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="161d3-108">Permission type</span></span>      | <span data-ttu-id="161d3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="161d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="161d3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="161d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="161d3-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="161d3-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="161d3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="161d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="161d3-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="161d3-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="161d3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="161d3-114">Application</span></span> | <span data-ttu-id="161d3-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="161d3-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="161d3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="161d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="161d3-117">ユーザーの既定 [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="161d3-117">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="161d3-118">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="161d3-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="161d3-p102">[contactFolder](../resources/mailfolder.md) の子フォルダー内に含まれる [連絡先](../resources/contact.md)。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="161d3-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="161d3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="161d3-121">Request headers</span></span>
| <span data-ttu-id="161d3-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="161d3-122">Header</span></span>       | <span data-ttu-id="161d3-123">値</span><span class="sxs-lookup"><span data-stu-id="161d3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="161d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="161d3-124">Authorization</span></span>  | <span data-ttu-id="161d3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="161d3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="161d3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="161d3-127">Content-Type</span></span>  | <span data-ttu-id="161d3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="161d3-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="161d3-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="161d3-130">Request body</span></span>
<span data-ttu-id="161d3-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="161d3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="161d3-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="161d3-134">Property</span></span>     | <span data-ttu-id="161d3-135">型</span><span class="sxs-lookup"><span data-stu-id="161d3-135">Type</span></span>   |<span data-ttu-id="161d3-136">説明</span><span class="sxs-lookup"><span data-stu-id="161d3-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="161d3-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="161d3-137">assistantName</span></span>|<span data-ttu-id="161d3-138">String</span><span class="sxs-lookup"><span data-stu-id="161d3-138">String</span></span>|<span data-ttu-id="161d3-139">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="161d3-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="161d3-140">birthday</span><span class="sxs-lookup"><span data-stu-id="161d3-140">birthday</span></span>|<span data-ttu-id="161d3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="161d3-141">DateTimeOffset</span></span>|<span data-ttu-id="161d3-142">連絡先の誕生日です。</span><span class="sxs-lookup"><span data-stu-id="161d3-142">The contact's birthday.</span></span>|
|<span data-ttu-id="161d3-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="161d3-143">businessAddress</span></span>|[<span data-ttu-id="161d3-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="161d3-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="161d3-145">連絡先の勤務先の住所。</span><span class="sxs-lookup"><span data-stu-id="161d3-145">The contact's business address.</span></span>|
|<span data-ttu-id="161d3-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="161d3-146">businessHomePage</span></span>|<span data-ttu-id="161d3-147">String</span><span class="sxs-lookup"><span data-stu-id="161d3-147">String</span></span>|<span data-ttu-id="161d3-148">連絡先の勤務先のホーム ページ。</span><span class="sxs-lookup"><span data-stu-id="161d3-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="161d3-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="161d3-149">businessPhones</span></span>|<span data-ttu-id="161d3-150">String</span><span class="sxs-lookup"><span data-stu-id="161d3-150">String</span></span>|<span data-ttu-id="161d3-151">連絡先の勤務先の電話番号。</span><span class="sxs-lookup"><span data-stu-id="161d3-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="161d3-152">categories</span><span class="sxs-lookup"><span data-stu-id="161d3-152">categories</span></span>|<span data-ttu-id="161d3-153">String</span><span class="sxs-lookup"><span data-stu-id="161d3-153">String</span></span>|<span data-ttu-id="161d3-154">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="161d3-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="161d3-155">children</span><span class="sxs-lookup"><span data-stu-id="161d3-155">children</span></span>|<span data-ttu-id="161d3-156">String</span><span class="sxs-lookup"><span data-stu-id="161d3-156">String</span></span>|<span data-ttu-id="161d3-157">連絡先の子供の名前。</span><span class="sxs-lookup"><span data-stu-id="161d3-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="161d3-158">companyName</span><span class="sxs-lookup"><span data-stu-id="161d3-158">companyName</span></span>|<span data-ttu-id="161d3-159">String</span><span class="sxs-lookup"><span data-stu-id="161d3-159">String</span></span>|<span data-ttu-id="161d3-160">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="161d3-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="161d3-161">department</span><span class="sxs-lookup"><span data-stu-id="161d3-161">department</span></span>|<span data-ttu-id="161d3-162">String</span><span class="sxs-lookup"><span data-stu-id="161d3-162">String</span></span>|<span data-ttu-id="161d3-163">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="161d3-163">The contact's department.</span></span>|
|<span data-ttu-id="161d3-164">displayName</span><span class="sxs-lookup"><span data-stu-id="161d3-164">displayName</span></span>|<span data-ttu-id="161d3-165">文字列</span><span class="sxs-lookup"><span data-stu-id="161d3-165">String</span></span>|<span data-ttu-id="161d3-166">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="161d3-166">The contact's display name.</span></span> <span data-ttu-id="161d3-167">後で他のプロパティを更新すると、指定した displayName 値が自動的に生成された値に上書きされますので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="161d3-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="161d3-168">既存の値を保持するには、[更新] 操作で必ずその値を displayName として含めてください。</span><span class="sxs-lookup"><span data-stu-id="161d3-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="161d3-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="161d3-169">emailAddresses</span></span>|<span data-ttu-id="161d3-170">[EmailAddress](../resources/emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="161d3-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="161d3-171">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="161d3-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="161d3-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="161d3-172">fileAs</span></span>|<span data-ttu-id="161d3-173">String</span><span class="sxs-lookup"><span data-stu-id="161d3-173">String</span></span>|<span data-ttu-id="161d3-174">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="161d3-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="161d3-175">generation</span><span class="sxs-lookup"><span data-stu-id="161d3-175">generation</span></span>|<span data-ttu-id="161d3-176">String</span><span class="sxs-lookup"><span data-stu-id="161d3-176">String</span></span>|<span data-ttu-id="161d3-177">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="161d3-177">The contact's generation.</span></span>|
|<span data-ttu-id="161d3-178">givenName</span><span class="sxs-lookup"><span data-stu-id="161d3-178">givenName</span></span>|<span data-ttu-id="161d3-179">String</span><span class="sxs-lookup"><span data-stu-id="161d3-179">String</span></span>|<span data-ttu-id="161d3-180">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="161d3-180">The contact's given name.</span></span>|
|<span data-ttu-id="161d3-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="161d3-181">homeAddress</span></span>|[<span data-ttu-id="161d3-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="161d3-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="161d3-183">連絡先の自宅住所。</span><span class="sxs-lookup"><span data-stu-id="161d3-183">The contact's home address.</span></span>|
|<span data-ttu-id="161d3-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="161d3-184">homePhones</span></span>|<span data-ttu-id="161d3-185">String collection</span><span class="sxs-lookup"><span data-stu-id="161d3-185">String collection</span></span>|<span data-ttu-id="161d3-186">連絡先の自宅の電話番号。</span><span class="sxs-lookup"><span data-stu-id="161d3-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="161d3-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="161d3-187">imAddresses</span></span>|<span data-ttu-id="161d3-188">String</span><span class="sxs-lookup"><span data-stu-id="161d3-188">String</span></span>|<span data-ttu-id="161d3-189">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="161d3-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="161d3-190">initials</span><span class="sxs-lookup"><span data-stu-id="161d3-190">initials</span></span>|<span data-ttu-id="161d3-191">String</span><span class="sxs-lookup"><span data-stu-id="161d3-191">String</span></span>|<span data-ttu-id="161d3-192">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="161d3-192">The contact's initials.</span></span>|
|<span data-ttu-id="161d3-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="161d3-193">jobTitle</span></span>|<span data-ttu-id="161d3-194">String</span><span class="sxs-lookup"><span data-stu-id="161d3-194">String</span></span>|<span data-ttu-id="161d3-195">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="161d3-195">The contact’s job title.</span></span>|
|<span data-ttu-id="161d3-196">manager</span><span class="sxs-lookup"><span data-stu-id="161d3-196">manager</span></span>|<span data-ttu-id="161d3-197">String</span><span class="sxs-lookup"><span data-stu-id="161d3-197">String</span></span>|<span data-ttu-id="161d3-198">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="161d3-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="161d3-199">middleName</span><span class="sxs-lookup"><span data-stu-id="161d3-199">middleName</span></span>|<span data-ttu-id="161d3-200">String</span><span class="sxs-lookup"><span data-stu-id="161d3-200">String</span></span>|<span data-ttu-id="161d3-201">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="161d3-201">The contact's middle name.</span></span>|
|<span data-ttu-id="161d3-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="161d3-202">mobilePhone</span></span>|<span data-ttu-id="161d3-203">String</span><span class="sxs-lookup"><span data-stu-id="161d3-203">String</span></span>|<span data-ttu-id="161d3-204">連絡先の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="161d3-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="161d3-205">nickName</span><span class="sxs-lookup"><span data-stu-id="161d3-205">nickName</span></span>|<span data-ttu-id="161d3-206">String</span><span class="sxs-lookup"><span data-stu-id="161d3-206">String</span></span>|<span data-ttu-id="161d3-207">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="161d3-207">The contact's nickname.</span></span>|
|<span data-ttu-id="161d3-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="161d3-208">officeLocation</span></span>|<span data-ttu-id="161d3-209">String</span><span class="sxs-lookup"><span data-stu-id="161d3-209">String</span></span>|<span data-ttu-id="161d3-210">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="161d3-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="161d3-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="161d3-211">otherAddress</span></span>|[<span data-ttu-id="161d3-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="161d3-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="161d3-213">連絡先の別の住所。</span><span class="sxs-lookup"><span data-stu-id="161d3-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="161d3-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="161d3-214">parentFolderId</span></span>|<span data-ttu-id="161d3-215">String</span><span class="sxs-lookup"><span data-stu-id="161d3-215">String</span></span>|<span data-ttu-id="161d3-216">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="161d3-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="161d3-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="161d3-217">personalNotes</span></span>|<span data-ttu-id="161d3-218">String</span><span class="sxs-lookup"><span data-stu-id="161d3-218">String</span></span>|<span data-ttu-id="161d3-219">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="161d3-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="161d3-220">profession</span><span class="sxs-lookup"><span data-stu-id="161d3-220">profession</span></span>|<span data-ttu-id="161d3-221">String</span><span class="sxs-lookup"><span data-stu-id="161d3-221">String</span></span>|<span data-ttu-id="161d3-222">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="161d3-222">The contact's profession.</span></span>|
|<span data-ttu-id="161d3-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="161d3-223">spouseName</span></span>|<span data-ttu-id="161d3-224">String</span><span class="sxs-lookup"><span data-stu-id="161d3-224">String</span></span>|<span data-ttu-id="161d3-225">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="161d3-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="161d3-226">姓</span><span class="sxs-lookup"><span data-stu-id="161d3-226">surname</span></span>|<span data-ttu-id="161d3-227">文字列</span><span class="sxs-lookup"><span data-stu-id="161d3-227">String</span></span>|<span data-ttu-id="161d3-228">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="161d3-228">The contact's surname.</span></span>|
|<span data-ttu-id="161d3-229">title</span><span class="sxs-lookup"><span data-stu-id="161d3-229">title</span></span>|<span data-ttu-id="161d3-230">String</span><span class="sxs-lookup"><span data-stu-id="161d3-230">String</span></span>|<span data-ttu-id="161d3-231">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="161d3-231">The contact's title.</span></span>|
|<span data-ttu-id="161d3-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="161d3-232">yomiCompanyName</span></span>|<span data-ttu-id="161d3-233">String</span><span class="sxs-lookup"><span data-stu-id="161d3-233">String</span></span>|<span data-ttu-id="161d3-p107">連絡先の会社名の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="161d3-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="161d3-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="161d3-236">yomiGivenName</span></span>|<span data-ttu-id="161d3-237">文字列</span><span class="sxs-lookup"><span data-stu-id="161d3-237">String</span></span>|<span data-ttu-id="161d3-p108">連絡先の名 (ファースト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="161d3-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="161d3-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="161d3-240">yomiSurname</span></span>|<span data-ttu-id="161d3-241">String</span><span class="sxs-lookup"><span data-stu-id="161d3-241">String</span></span>|<span data-ttu-id="161d3-p109">連絡先の姓 (ラスト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="161d3-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="161d3-244">応答</span><span class="sxs-lookup"><span data-stu-id="161d3-244">Response</span></span>

<span data-ttu-id="161d3-245">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="161d3-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="161d3-246">例</span><span class="sxs-lookup"><span data-stu-id="161d3-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="161d3-247">要求</span><span class="sxs-lookup"><span data-stu-id="161d3-247">Request</span></span>
<span data-ttu-id="161d3-248">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="161d3-248">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="161d3-249">応答</span><span class="sxs-lookup"><span data-stu-id="161d3-249">Response</span></span>
<span data-ttu-id="161d3-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="161d3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="161d3-253">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="161d3-253">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="161d3-254">C#</span><span class="sxs-lookup"><span data-stu-id="161d3-254">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_contact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="161d3-255">Javascript</span><span class="sxs-lookup"><span data-stu-id="161d3-255">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_contact-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="161d3-256">目的-C</span><span class="sxs-lookup"><span data-stu-id="161d3-256">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_contact-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contact-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/contact-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contact-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
